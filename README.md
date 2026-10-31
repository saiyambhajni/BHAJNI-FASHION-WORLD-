<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <meta name="description" content="BHAJNI FASHION WORLD — Premium ladies winter wear, night suits, lowers, nighties, cardigans and Kidley inner. Sector 9, Panchkula, SCO No. 14.">
        <title>BHAJNI FASHION WORLD — Winter Collection</title>
        <style>
            :root {
                --bg: #08090c;
                --panel: #111319;
                --panel2: #171920;
                --gold: #d9b36c;
                --gold2: #f0d08c;
                --cream: #f7f1e7;
                --muted: #aaa7a1;
                --line: rgba(217,179,108,.18);
                --pink: #d47a91;
                --shadow: 0 25px 80px rgba(0,0,0,.45);
                --radius: 24px
            }

            * {
                box-sizing: border-box
            }

            html {
                scroll-behavior: smooth
            }

            body {
                margin: 0;
                background: radial-gradient(circle at 15% 0%,#211a15 0,#08090c 32%),#08090c;
                color: var(--cream);
                font-family: Inter,system-ui,-apple-system,Segoe UI,Roboto,Arial,sans-serif
            }

            body:before {
                content: "";
                position: fixed;
                inset: 0;
                pointer-events: none;
                opacity: .12;
                background-image: linear-gradient(rgba(255,255,255,.05) 1px,transparent 1px),linear-gradient(90deg,rgba(255,255,255,.05) 1px,transparent 1px);
                background-size: 70px 70px
            }

            a {
                text-decoration: none;
                color: inherit
            }

            button,input,select {
                font: inherit
            }

            .container {
                width: min(1180px,92%);
                margin: auto
            }

            .top {
                border-bottom: 1px solid var(--line);
                font-size: 12px;
                color: var(--muted);
                padding: 9px 0
            }

            .top .container {
                display: flex;
                justify-content: space-between;
                gap: 12px;
                flex-wrap: wrap
            }

            .nav {
                position: sticky;
                top: 0;
                z-index: 30;
                background: rgba(8,9,12,.86);
                backdrop-filter: blur(18px);
                border-bottom: 1px solid var(--line)
            }

            .navin {
                height: 78px;
                display: flex;
                align-items: center;
                justify-content: space-between;
                gap: 20px
            }

            .logo {
                font-family: Georgia,serif;
                font-size: 22px;
                letter-spacing: .08em;
                font-weight: 900
            }

            .logo b {
                color: var(--gold)
            }

            .links {
                display: flex;
                gap: 25px;
                color: #c8c3ba;
                font-size: 13px;
                font-weight: 750
            }

            .links a:hover {
                color: var(--gold)
            }

            .bag {
                border: 1px solid var(--gold);
                background: transparent;
                color: var(--gold2);
                padding: 10px 15px;
                border-radius: 999px;
                font-weight: 850;
                cursor: pointer
            }

            .hero {
                padding: 72px 0 55px
            }

            .heroGrid {
                display: grid;
                grid-template-columns: 1.05fr .95fr;
                gap: 48px;
                align-items: center
            }

            .kicker {
                display: inline-block;
                color: var(--gold2);
                border: 1px solid var(--line);
                padding: 8px 13px;
                border-radius: 999px;
                font-size: 11px;
                letter-spacing: .13em;
                text-transform: uppercase;
                font-weight: 900;
                background: rgba(217,179,108,.05)
            }

            h1 {
                font-family: Georgia,serif;
                font-weight: 500;
                font-size: clamp(55px,8vw,100px);
                line-height: .88;
                letter-spacing: -.055em;
                margin: 23px 0
            }

            h1 span {
                color: var(--gold2);
                font-style: italic
            }

            .hero p {
                color: var(--muted);
                font-size: 17px;
                line-height: 1.8;
                max-width: 650px
            }

            .actions {
                display: flex;
                gap: 12px;
                flex-wrap: wrap;
                margin-top: 28px
            }

            .btn {
                border: 0;
                border-radius: 12px;
                padding: 14px 19px;
                font-weight: 900;
                cursor: pointer;
                display: inline-flex;
                justify-content: center;
                align-items: center
            }

            .primary {
                background: linear-gradient(135deg,#e4c17a,#a97830);
                color: #17120b;
                box-shadow: 0 12px 35px rgba(217,179,108,.18)
            }

            .outline {
                border: 1px solid var(--line);
                color: var(--cream);
                background: #101116
            }

            .heroVisual {
                height: 490px;
                border: 1px solid var(--line);
                border-radius: 34px;
                position: relative;
                overflow: hidden;
                background: radial-gradient(circle at 50% 34%,rgba(240,208,140,.32),transparent 20%), radial-gradient(circle at 50% 45%,#6c3e45 0,#24191d 34%,#0b0c0f 72%);
                box-shadow: var(--shadow)
            }

            .heroVisual:before {
                content: "BHAJNI";
                position: absolute;
                left: 50%;
                top: 50%;
                transform: translate(-50%,-50%);
                font-family: Georgia,serif;
                font-size: 78px;
                letter-spacing: .08em;
                color: rgba(255,255,255,.055);
                white-space: nowrap
            }

            .heroVisual:after {
                content: "WINTER  •  2026";
                position: absolute;
                top: 28px;
                right: 28px;
                color: var(--gold2);
                font-size: 10px;
                letter-spacing: .2em
            }

            .orb {
                position: absolute;
                width: 210px;
                height: 290px;
                border-radius: 55% 45% 42% 58%;
                left: 50%;
                top: 48%;
                transform: translate(-50%,-50%);
                background: linear-gradient(145deg,#ead6c0,#9a5d63 50%,#38262c);
                box-shadow: 0 35px 70px rgba(0,0,0,.55);
                opacity: .9
            }

            .visualTag {
                position: absolute;
                bottom: 25px;
                left: 25px;
                right: 25px;
                background: rgba(8,9,12,.78);
                border: 1px solid var(--line);
                padding: 17px;
                border-radius: 18px;
                backdrop-filter: blur(12px)
            }

            .visualTag strong {
                font-family: Georgia,serif;
                font-size: 24px
            }

            .visualTag small {
                display: block;
                color: var(--muted);
                margin-top: 5px
            }

            .section {
                padding: 60px 0
            }

            .head {
                display: flex;
                justify-content: space-between;
                align-items: end;
                gap: 20px;
                margin-bottom: 25px
            }

            .head h2 {
                font: 500 43px Georgia,serif;
                margin: 8px 0
            }

            .head p {
                color: var(--muted);
                max-width: 520px;
                line-height: 1.6
            }

            .offer {
                border: 1px solid rgba(217,179,108,.35);
                background: linear-gradient(135deg,rgba(217,179,108,.12),rgba(212,122,145,.07));
                border-radius: 24px;
                padding: 22px;
                display: flex;
                align-items: center;
                justify-content: space-between;
                gap: 20px;
                margin-bottom: 30px
            }

            .offer strong {
                font-size: 22px;
                color: var(--gold2)
            }

            .offer span {
                display: block;
                color: var(--muted);
                font-size: 13px;
                margin-top: 5px
            }

            .filters {
                display: flex;
                gap: 8px;
                flex-wrap: wrap;
                margin-bottom: 25px
            }

            .filter {
                border: 1px solid var(--line);
                background: #0d0f13;
                color: #bcb7ae;
                padding: 10px 14px;
                border-radius: 999px;
                cursor: pointer;
                font-weight: 800;
                font-size: 12px
            }

            .filter.active,.filter:hover {
                background: var(--gold);
                color: #17120b;
                border-color: var(--gold)
            }

            .grid {
                display: grid;
                grid-template-columns: repeat(3,1fr);
                gap: 18px
            }

            .card {
                background: linear-gradient(145deg,#14161c,#0e1014);
                border: 1px solid var(--line);
                border-radius: var(--radius);
                overflow: hidden;
                transition: .25s;
                box-shadow: 0 10px 40px rgba(0,0,0,.22)
            }

            .card:hover {
                transform: translateY(-5px);
                border-color: rgba(217,179,108,.4);
                box-shadow: var(--shadow)
            }

            .art {
                height: 205px;
                background: radial-gradient(circle at 50% 35%,rgba(217,179,108,.18),transparent 28%),linear-gradient(145deg,#202027,#0d0f13);
                position: relative;
                display: flex;
                align-items: center;
                justify-content: center
            }

            .cloth {
                width: 130px;
                height: 150px;
                border-radius: 55px 55px 22px 22px;
                background: linear-gradient(145deg,#9b6872,#d9b36c 52%,#432c35);
                box-shadow: 18px 20px 45px rgba(0,0,0,.5)
            }

            .badge {
                position: absolute;
                left: 15px;
                top: 15px;
                background: #0b0c0f;
                border: 1px solid var(--line);
                color: var(--gold2);
                padding: 7px 10px;
                border-radius: 999px;
                font-size: 10px;
                font-weight: 900;
                letter-spacing: .08em
            }

            .body {
                padding: 19px
            }

            .body h3 {
                margin: 0 0 7px;
                font: 600 22px Georgia,serif
            }

            .body p {
                margin: 0;
                color: var(--muted);
                font-size: 13px;
                line-height: 1.55;
                min-height: 41px
            }

            .price {
                font-size: 23px;
                font-weight: 950;
                color: var(--gold2);
                margin: 13px 0
            }

            .price small {
                font-size: 11px;
                color: var(--muted)
            }

            .sizes {
                display: flex;
                gap: 6px;
                flex-wrap: wrap;
                margin-bottom: 14px
            }

            .size {
                background: #0b0c0f;
                border: 1px solid var(--line);
                color: #ddd6cc;
                border-radius: 8px;
                padding: 7px 8px;
                font-size: 10px;
                font-weight: 850;
                cursor: pointer
            }

            .size:hover {
                border-color: var(--gold);
                color: var(--gold2)
            }

            .add {
                width: 100%;
                background: linear-gradient(135deg,#e4c17a,#a97830);
                border: 0;
                border-radius: 11px;
                padding: 12px;
                color: #17120b;
                font-weight: 950;
                cursor: pointer
            }

            .infoGrid {
                display: grid;
                grid-template-columns: 1fr 1fr;
                gap: 18px
            }

            .info {
                background: #111319;
                border: 1px solid var(--line);
                border-radius: 25px;
                padding: 28px
            }

            .info h3 {
                font: 500 29px Georgia,serif;
                margin: 0 0 15px
            }

            .info p,.info li {
                color: var(--muted);
                line-height: 1.7
            }

            .info ul {
                padding-left: 20px
            }

            .footer {
                border-top: 1px solid var(--line);
                padding: 35px 0;
                color: var(--muted);
                font-size: 12px
            }

            .foot {
                display: flex;
                justify-content: space-between;
                gap: 20px;
                flex-wrap: wrap
            }

            .foot b {
                color: var(--cream)
            }

            .modal {
                display: none;
                position: fixed;
                inset: 0;
                background: rgba(0,0,0,.72);
                z-index: 100;
                align-items: flex-end;
                justify-content: center
            }

            .modal.open {
                display: flex
            }

            .sheet {
                width: min(620px,100%);
                max-height: 88vh;
                overflow: auto;
                background: #12141a;
                border: 1px solid var(--line);
                border-radius: 27px 27px 0 0;
                padding: 25px;
                box-shadow: var(--shadow)
            }

            .sheetTop {
                display: flex;
                justify-content: space-between;
                align-items: center
            }

            .sheetTop h2 {
                font: 500 30px Georgia,serif
            }

            .close {
                border: 1px solid var(--line);
                background: #0b0c0f;
                color: #fff;
                border-radius: 50%;
                width: 38px;
                height: 38px;
                cursor: pointer
            }

            .cartItem {
                display: flex;
                justify-content: space-between;
                gap: 15px;
                padding: 14px 0;
                border-bottom: 1px solid var(--line)
            }

            .cartItem small {
                color: var(--muted)
            }

            .cartTotal {
                text-align: right;
                font-size: 21px;
                font-weight: 950;
                color: var(--gold2);
                margin: 18px 0
            }

            .note {
                color: var(--muted);
                font-size: 12px;
                line-height: 1.6
            }

            @media(max-width: 850px) {
                .heroGrid,.infoGrid {
                    grid-template-columns:1fr
                }

                .grid {
                    grid-template-columns: repeat(2,1fr)
                }

                .links {
                    display: none
                }

                .heroVisual {
                    height: 380px
                }
            }

            @media(max-width: 560px) {
                .grid {
                    grid-template-columns:1fr
                }

                .hero {
                    padding-top: 45px
                }

                h1 {
                    font-size: 58px
                }

                .offer {
                    align-items: flex-start;
                    flex-direction: column
                }

                .head {
                    align-items: flex-start;
                    flex-direction: column
                }
            }
        </style>
    </head>
    <body>
        <div class="top">
            <div class="container">
                <span>✦ PREMIUM WINTER COLLECTION • BHAJNI FASHION WORLD</span>
                <span>📍 SECTOR 9, PANCHKULA • SCO NO. 14</span>
            </div>
        </div>
        <nav class="nav">
            <div class="container navin">
                <a class="logo" href="#home">
                    BHAJNI <b>FASHION WORLD</b>
                </a>
                <div class="links">
                    <a href="#collection">Collection</a>
                    <a href="#offer">20% Offer</a>
                    <a href="#visit">Visit</a>
                </div>
                <button class="bag" onclick="openCart()">
                    BAG • <span id="count">0</span>
                </button>
            </div>
        </nav>
        <main id="home">
            <section class="hero">
                <div class="container heroGrid">
                    <div>
                        <span class="kicker">The winter edit • now in store</span>
                        <h1>
                            Luxury comfort.<br>
                            <span>Everyday warmth.</span>
                        </h1>
                        <p>
                            Step into <b>BHAJNI FASHION WORLD</b>
                            — a premium destination for ladies' winter wear and night wear. Discover cozy lowers, winter night suits, elegant nighties, cardigans and Kidley winter inner, all under one roof.
                        </p>
                        <div class="actions">
                            <a class="btn primary" href="#collection">Explore The Collection</a>
                            <a class="btn outline" href="https://wa.me/919815395390?text=Hello%20BHAJNI%20FASHION%20WORLD%2C%20I%20want%20to%20see%20the%20winter%20collection." target="_blank">WhatsApp Us</a>
                        </div>
                    </div>
                    <div class="heroVisual">
                        <div class="orb"></div>
                        <div class="visualTag">
                            <strong>Winter, but make it beautiful.</strong>
                            <small>Soft layers • flattering comfort • premium everyday feel</small>
                        </div>
                    </div>
                </div>
            </section>
            <section class="section" id="collection">
                <div class="container">
                    <div class="head">
                        <div>
                            <span class="kicker">Curated for winter</span>
                            <h2>Shop The Collection</h2>
                        </div>
                        <p>Choose a category, select your size and add your favourites to your bag. Prices shown below are the current listed prices.</p>
                    </div>
                    <div class="offer" id="offer">
                        <div>
                            <strong>BUY MORE • SAVE MORE — 20% OFF</strong>
                            <span>Purchase more than 2 items and get a direct 20% OFF on the total eligible amount.</span>
                        </div>
                        <span style="font-size:30px;color:var(--gold2)">20%</span>
                    </div>
                    <div class="filters">
                        <button class="filter active" data-filter="all">ALL</button>
                        <button class="filter" data-filter="lower">WINTER LOWERS</button>
                        <button class="filter" data-filter="suit">NIGHT SUITS</button>
                        <button class="filter" data-filter="nightie">NIGHTIES</button>
                        <button class="filter" data-filter="cardigan">CARDIGANS</button>
                        <button class="filter" data-filter="inner">KIDLEY INNER</button>
                    </div>
                    <div class="grid" id="products"></div>
                </div>
            </section>
            <section class="section" id="visit">
                <div class="container">
                    <div class="head">
                        <div>
                            <span class="kicker">BHAJNI FASHION WORLD</span>
                            <h2>Visit. Feel. Choose.</h2>
                        </div>
                    </div>
                    <div class="infoGrid">
                        <div class="info">
                            <h3>Our Store</h3>
                            <ul>
                                <li>
                                    <b>Address:</b>
                                    Sector 9, Panchkula, SCO No. 14
                                </li>
                                <li>
                                    <b>Mobile:</b>
                                    <a href="tel:9815395390">9815395390</a>
                                </li>
                                <li>
                                    <b>Alternative:</b>
                                    <a href="tel:7009247903">7009247903</a>
                                </li>
                                <li>
                                    <b>Email:</b>
                                    <a href="mailto:bhajnidashionworld@gmail.com">bhajnidashionworld@gmail.com</a>
                                </li>
                            </ul>
                        </div>
                        <div class="info">
                            <h3>Need help choosing?</h3>
                            <p>Message us with the product and size you want. We can help you confirm availability, colours and the final bill before you visit.</p>
                            <a class="btn primary" style="width:100%" href="https://wa.me/919815395390?text=Hello%20BHAJNI%20FASHION%20WORLD%2C%20please%20help%20me%20with%20sizes%20and%20availability." target="_blank">Chat on WhatsApp</a>
                        </div>
                    </div>
                </div>
            </section>
        </main>
        <footer class="footer">
            <div class="container foot">
                <div>
                    <b>BHAJNI FASHION WORLD</b>
                    <br>Premium winter comfort • Sector 9, Panchkula
                </div>
                <div>© 2026 BHAJNI FASHION WORLD</div>
            </div>
        </footer>
        <div class="modal" id="modal" onclick="if(event.target===this)closeCart()">
            <div class="sheet">
                <div class="sheetTop">
                    <h2>Your Bag</h2>
                    <button class="close" onclick="closeCart()">×</button>
                </div>
                <div id="cart"></div>
                <div class="cartTotal" id="total">Total: ₹0</div>
                <a id="wa" class="btn primary" style="width:100%" target="_blank">Send Order Enquiry on WhatsApp</a>
                <p class="note">Special offer: when your bag contains more than 2 items, a 20% discount is applied to the total. Kidley Inner is listed as 15% OFF MRP and its final amount depends on the MRP. Please confirm stock, colour and final price with the shop.</p>
            </div>
        </div>
        <script>
            const products = [{
                cat: 'lower',
                name: 'Winter Lower',
                desc: 'Warm, comfortable everyday winter lower.',
                sizes: [['SMALL', 250], ['MEDIUM', 250], ['LARGE', 300], ['XL', 300], ['XXL', 350], ['XXXL', 350]]
            }, {
                cat: 'suit',
                name: 'Winter Night Suit',
                desc: 'Cozy winter night suit for relaxed evenings.',
                sizes: [['MEDIUM', 500], ['LARGE', 500], ['XL', 550], ['XXL', 550], ['XXL', 600]]
            }, {
                cat: 'nightie',
                name: 'Winter Blanket Nightie',
                desc: 'Extra-cozy blanket winter nightie.',
                sizes: [['REGULAR', 650]]
            }, {
                cat: 'nightie',
                name: 'Winter Velvet Nightie',
                desc: 'Soft velvet winter nightie with a premium feel.',
                sizes: [['REGULAR', 890], ['XXXL', 1190]]
            }, {
                cat: 'cardigan',
                name: 'Winter Cardigan',
                desc: 'A warm, easy-to-style winter layer.',
                sizes: [['MEDIUM', 500], ['XL', 550], ['XXL', 600], ['XXXL', 600]]
            }, {
                cat: 'inner',
                name: 'Kidley Winter Inner',
                desc: 'Winter inner available at 15% OFF MRP.',
                sizes: [['MRP − 15%', null]]
            }];
            let filter = 'all'
              , bag = [];
            const money = n => n == null ? '15% OFF MRP' : '₹' + n;
            function render() {
                const box = document.getElementById('products');
                box.innerHTML = products.filter(p => filter === 'all' || p.cat === filter).map( (p, i) => {
                    const idx = products.indexOf(p)
                      , nums = p.sizes.filter(s => s[1] != null).map(s => s[1]);
                    const display = nums.length ? `₹${Math.min(...nums)} <small>onwards</small>` : '15% OFF <small>MRP</small>';
                    return `<article class="card"><div class="art"><span class="badge">${p.cat === 'inner' ? 'SPECIAL OFFER' : 'WINTER EDIT'}</span><div class="cloth"></div></div><div class="body"><h3>${p.name}</h3><p>${p.desc}</p><div class="price">${display}</div><div class="sizes">${p.sizes.map( (s, j) => `<button class="size" onclick="add(${idx},${j})">${s[0]}${s[1] != null ? ' • ₹' + s[1] : ''}</button>`).join('')}</div><button class="add" onclick="add(${idx},0)">ADD TO BAG</button></div></article>`;
                }
                ).join('');
            }
            document.querySelectorAll('.filter').forEach(b => b.onclick = () => {
                document.querySelectorAll('.filter').forEach(x => x.classList.remove('active'));
                b.classList.add('active');
                filter = b.dataset.filter;
                render()
            }
            );
            function add(pi, si) {
                bag.push({
                    name: products[pi].name,
                    size: products[pi].sizes[si][0],
                    price: products[pi].sizes[si][1]
                });
                document.getElementById('count').textContent = bag.length;
                openCart()
            }
            function openCart() {
                document.getElementById('modal').classList.add('open');
                const list = document.getElementById('cart');
                list.innerHTML = bag.length ? bag.map(x => `<div class="cartItem"><span><b>${x.name}</b><br><small>Size: ${x.size}</small></span><b>${money(x.price)}</b></div>`).join('') : '<p class="note">Your bag is empty. Select a product size to add it here.</p>';
                const known = bag.filter(x => x.price != null)
                  , subtotal = known.reduce( (a, x) => a + x.price, 0)
                  , discount = bag.length > 2 ? subtotal * .2 : 0
                  , final = subtotal - discount;
                document.getElementById('total').innerHTML = bag.length ? `Subtotal: ₹${subtotal.toFixed(0)}${bag.length > 2 ? `<br><span style="color:#d9b36c">20% OFF: −₹${discount.toFixed(0)}</span><br>Total: ₹${final.toFixed(0)}` : `<br>Total: ₹${subtotal.toFixed(0)}`}${bag.some(x => x.price == null) ? '<br><small style="color:#aaa">+ Kidley Inner at 15% OFF MRP</small>' : ''}` : 'Total: ₹0';
                let msg = 'Hello BHAJNI FASHION WORLD! I would like to enquire about:%0A' + bag.map(x => `• ${x.name} — ${x.size}${x.price != null ? ' — ₹' + x.price : ' — 15% OFF MRP'}`).join('%0A');
                if (bag.length > 2)
                    msg += `%0A%0A20%20OFF%20applies%20to%20more%20than%202%20items.`;
                msg += '%0A%0APlease confirm availability, colour and final bill.';
                document.getElementById('wa').href = 'https://wa.me/919815395390?text=' + msg;
            }
            function closeCart() {
                document.getElementById('modal').classList.remove('open')
            }
            render();
        </script>
    </body>
</html>
