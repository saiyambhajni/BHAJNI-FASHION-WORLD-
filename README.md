import React, { useState, useRef, useEffect } from 'react';
import { create } from 'zustand';
import { useForm } from 'react-hook-form';
import { useReactToPrint } from 'react-to-print';
import { motion, AnimatePresence } from 'framer-motion';
import { ChevronDown, Download } from 'lucide-react';

// --- 1. GLOBAL STATE (Zustand) ---
const useResumeStore = create((set) => ({
  resumeData: {
    fullName: 'Jane Doe',
    role: 'Full Stack Developer',
    email: 'jane.doe@example.com',
    summary: 'Passionate developer building high-contrast UI tools.',
    experience: 'Built a live resume builder using React, Tailwind CSS, and Framer Motion. Engineered a split-screen architecture for real-time PDF generation.',
  },
  updateData: (newData) => 
    set((state) => ({ resumeData: { ...state.resumeData, ...newData } })),
}));

// --- 2. ANIMATED COMPONENT (Framer Motion) ---
function CollapsibleSection({ title, defaultOpen = false, children }) {
  const [isOpen, setIsOpen] = useState(defaultOpen);

  return (
    <div className="bg-slate-900 border border-slate-800 rounded-xl overflow-hidden shadow-lg transition-colors hover:border-slate-700">
      <button
        type="button"
        onClick={() => setIsOpen(!isOpen)}
        className="w-full p-5 flex items-center justify-between text-left focus:outline-none"
      >
        <span className="text-base font-semibold text-slate-200">{title}</span>
        <motion.div animate={{ rotate: isOpen ? 180 : 0 }} transition={{ duration: 0.25 }} className="text-slate-400">
          <ChevronDown size={18} />
        </motion.div>
      </button>
      <AnimatePresence initial={false}>
        {isOpen && (
          <motion.div
            initial={{ height: 0, opacity: 0 }}
            animate={{ height: 'auto', opacity: 1, transition: { height: { duration: 0.3 }, opacity: { duration: 0.25 } } }}
            exit={{ height: 0, opacity: 0, transition: { height: { duration: 0.25 }, opacity: { duration: 0.15 } } }}
            className="overflow-hidden"
          >
            <div className="px-5 pb-5 pt-1 border-t border-slate-800/60">
              {children}
            </div>
          </motion.div>
        )}
      </AnimatePresence>
    </div>
  );
}

// --- 3. MAIN UI (Split-Screen & PDF Generator) ---
export default function App() {
  const { resumeData, updateData } = useResumeStore();
  const resumeRef = useRef();
  
  const { register, watch } = useForm({ defaultValues: resumeData });
  const liveFormData = watch();
  
  useEffect(() => {
    updateData(liveFormData);
  }, [liveFormData, updateData]);

  const handlePrint = useReactToPrint({
    content: () => resumeRef.current,
    documentTitle: `${resumeData.fullName.replace(/\s+/g, '_')}_Resume`,
  });

  return (
    <div className="flex h-screen w-full bg-slate-950 text-slate-100 font-sans overflow-hidden">
      
      {/* LEFT PANEL: Editor */}
      <div className="w-2/5 h-full p-8 overflow-y-auto border-r border-slate-800 custom-scrollbar">
        <h1 className="text-2xl font-bold mb-6 text-emerald-400">Resume Editor</h1>
        
        <form className="space-y-4">
          <CollapsibleSection title="Personal Details" defaultOpen={true}>
            <div className="space-y-4 pt-2">
              <div>
                <label className="block text-sm text-slate-400 mb-1">Full Name</label>
                <input {...register("fullName")} className="w-full bg-slate-950 border border-slate-700 rounded-lg px-4 py-2 focus:outline-none focus:border-emerald-500" />
              </div>
              <div>
                <label className="block text-sm text-slate-400 mb-1">Role / Title</label>
                <input {...register("role")} className="w-full bg-slate-950 border border-slate-700 rounded-lg px-4 py-2 focus:outline-none focus:border-emerald-500" />
              </div>
              <div>
                <label className="block text-sm text-slate-400 mb-1">Email Address</label>
                <input {...register("email")} type="email" className="w-full bg-slate-950 border border-slate-700 rounded-lg px-4 py-2 focus:outline-none focus:border-emerald-500" />
              </div>
            </div>
          </CollapsibleSection>

          <CollapsibleSection title="Professional Summary" defaultOpen={false}>
            <div className="pt-2">
              <label className="block text-sm text-slate-400 mb-1">Summary</label>
              <textarea {...register("summary")} rows="4" className="w-full bg-slate-950 border border-slate-700 rounded-lg px-4 py-2 focus:outline-none focus:border-emerald-500" />
            </div>
          </CollapsibleSection>

          <CollapsibleSection title="Work Experience" defaultOpen={false}>
             <div className="pt-2">
              <label className="block text-sm text-slate-400 mb-1">Recent Achievements</label>
              <textarea {...register("experience")} rows="5" className="w-full bg-slate-950 border border-slate-700 rounded-lg px-4 py-2 focus:outline-none focus:border-emerald-500" />
            </div>
          </CollapsibleSection>
        </form>
      </div>

      {/* RIGHT PANEL: Live Preview */}
      <div className="w-3/5 h-full bg-slate-900 p-8 flex flex-col items-center overflow-y-auto relative custom-scrollbar">
        <button 
          onClick={handlePrint}
          className="absolute top-8 right-8 flex items-center gap-2 bg-emerald-500 hover:bg-emerald-400 text-slate-950 px-6 py-3 rounded-full font-bold shadow-lg transition-transform hover:scale-105"
        >
          <Download size={20} />
          Export PDF
        </button>

        {/* The Printable A4 Document */}
        <div ref={resumeRef} className="w-full max-w-[210mm] min-h-[297mm] bg-white text-slate-900 shadow-2xl p-12 mt-16">
          <header className="border-b-2 border-slate-200 pb-6 mb-6">
            <h1 className="text-4xl font-bold text-slate-900 tracking-tight">{resumeData.fullName || 'Your Name'}</h1>
            <p className="text-xl text-emerald-600 mt-2 font-medium">{resumeData.role || 'Your Role'}</p>
            <p className="text-sm text-slate-500 mt-2">{resumeData.email || 'email@example.com'}</p>
          </header>

          <section className="mb-8">
            <h3 className="text-lg font-bold text-slate-900 uppercase tracking-wider mb-3">Profile</h3>
            <p className="text-slate-700 leading-relaxed">{resumeData.summary || 'Write a brief professional summary...'}</p>
          </section>

          <section>
            <h3 className="text-lg font-bold text-slate-900 uppercase tracking-wider mb-3">Experience</h3>
            <p className="text-slate-700 leading-relaxed whitespace-pre-line">{resumeData.experience || 'Detail your recent work experience...'}</p>
          </section>
        </div>
      </div>
    </div>
  );
}
