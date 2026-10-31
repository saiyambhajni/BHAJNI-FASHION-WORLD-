<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <meta name="description" content="BHAJNI FASHION WORLD - premium ladies winter wear, night wear and everyday fashion in Sector 9, Panchkula.">
        <title>BHAJNI FASHION WORLD | Premium Winter Edit</title>
        <style>
            :root {
                --bg: #07080b;
                --bg2: #0d0f14;
                --card: #12151b;
                --card2: #181b22;
                --gold: #d8b46a;
                --gold2: #f2d99a;
                --rose: #c56d84;
                --text: #f7f1e8;
                --muted: #aaa7a1;
                --line: rgba(216,180,106,.18);
                --whiteLine: rgba(255,255,255,.08);
                --shadow: 0 28px 90px rgba(0,0,0,.5);
                --r: 24px
            }

            * {
                box-sizing: border-box
            }

            html {
                scroll-behavior: smooth
            }

            body {
                margin: 0;
                color: var(--text);
                font-family: Inter,system-ui,-apple-system,Segoe UI,Roboto,Arial,sans-serif;
                background: radial-gradient(circle at 10% 0%,rgba(197,109,132,.13),transparent 28%), radial-gradient(circle at 90% 20%,rgba(216,180,106,.10),transparent 25%),var(--bg)
            }

            body:before {
                content: "";
                position: fixed;
                inset: 0;
                pointer-events: none;
                opacity: .07;
                background-image: linear-gradient(rgba(255,255,255,.5) 1px,transparent 1px),linear-gradient(90deg,rgba(255,255,255,.5) 1px,transparent 1px);
                background-size: 72px 72px
            }

            a {
                text-decoration: none;
                color: inherit
            }

            button {
                font: inherit
            }

            .container {
                width: min(1180px,92%);
                margin: auto
            }

            .topbar {
                border-bottom: 1px solid var(--line);
                color: #bbb5ab;
                font-size: 11px;
                letter-spacing: .06em;
                padding: 9px 0
            }

            .topbar .container {
                display: flex;
                justify-content: space-between;
                gap: 15px;
                flex-wrap: wrap
            }

            .nav {
                position: sticky;
                top: 0;
                z-index: 50;
                background: rgba(7,8,11,.84);
                backdrop-filter: blur(18px);
                border-bottom: 1px solid var(--whiteLine)
            }

            .navin {
                height: 78px;
                display: flex;
                align-items: center;
                justify-content: space-between;
                gap: 20px
            }

            .logo {
                font: 800 21px Georgia,serif;
                letter-spacing: .07em
            }

            .logo span {
                color: var(--gold2)
            }

            .links {
                display: flex;
                gap: 25px;
                color: #bbb6ae;
                font-size: 13px;
                font-weight: 800
            }

            .links a:hover {
                color: var(--gold2)
            }

            .cart {
                cursor: pointer;
                background: transparent;
                border: 1px solid var(--gold);
                color: var(--gold2);
                border-radius: 999px;
                padding: 10px 16px;
                font-weight: 900
            }

            .hero {
                padding: 75px 0 55px
            }

            .heroGrid {
                display: grid;
                grid-template-columns: 1.06fr .94fr;
                gap: 50px;
                align-items: center
            }

            .kicker {
                display: inline-flex;
                border: 1px solid var(--line);
                background: rgba(216,180,106,.05);
                color: var(--gold2);
                border-radius: 999px;
                padding: 8px 13px;
                font-size: 10px;
                font-weight: 900;
                letter-spacing: .16em;
                text-transform: uppercase
            }

            h1 {
                font: 500 clamp(56px,8vw,100px)/.86 Georgia,serif;
                letter-spacing: -.06em;
                margin: 24px 0
            }

            h1 em {
                color: var(--gold2);
                font-style: italic
            }

            .hero p {
                max-width: 650px;
                color: var(--muted);
                font-size: 17px;
                line-height: 1.8
            }

            .actions {
                display: flex;
                gap: 11px;
                flex-wrap: wrap;
                margin-top: 28px
            }

            .btn {
                display: inline-flex;
                align-items: center;
                justify-content: center;
                padding: 14px 19px;
                border-radius: 13px;
                font-weight: 900;
                border: 0;
                cursor: pointer
            }

            .primary {
                color: #17120a;
                background: linear-gradient(135deg,#f0d18d,#a87932);
                box-shadow: 0 12px 35px rgba(216,180,106,.16)
            }

            .secondary {
                color: var(--text);
                background: #101217;
                border: 1px solid var(--line)
            }

            .heroArt {
                height: 490px;
                border: 1px solid var(--line);
                border-radius: 34px;
                overflow: hidden;
                position: relative;
                box-shadow: var(--shadow);
                background: radial-gradient(circle at 50% 28%,rgba(242,217,154,.3),transparent 15%), radial-gradient(circle at 50% 50%,#6d414b 0,transparent 30%), linear-gradient(145deg,#272027,#0b0d11 70%)
            }

            .heroArt:before {
                content: "BHAJNI";
                position: absolute;
                left: 50%;
                top: 48%;
                transform: translate(-50%,-50%);
                font: 500 75px Georgia,serif;
                letter-spacing: .08em;
                color: rgba(255,255,255,.045)
            }

            .dress {
                position: absolute;
                left: 50%;
                top: 48%;
                transform: translate(-50%,-50%);
                width: 145px;
                height: 280px;
                border-radius: 75px 75px 35px 35px;
                background: linear-gradient(145deg,#d8b46a,#9a5d68 48%,#302229);
                box-shadow: 25px 35px 75px rgba(0,0,0,.6)
            }

            .heroTag {
                position: absolute;
                left: 24px;
                right: 24px;
                bottom: 24px;
                padding: 17px 19px;
                border-radius: 18px;
                background: rgba(7,8,11,.78);
                border: 1px solid var(--line);
                backdrop-filter: blur(12px)
            }

            .heroTag strong {
                font: 500 24px Georgia,serif
            }

            .heroTag small {
                display: block;
                color: var(--muted);
                margin-top: 5px
            }

            .section {
                padding: 62px 0
            }

            .head {
                display: flex;
                justify-content: space-between;
                align-items: end;
                gap: 25px;
                margin-bottom: 27px
            }

            .head h2 {
                font: 500 43px Georgia,serif;
                margin: 8px 0
            }

            .head p {
                max-width: 520px;
                color: var(--muted);
                line-height: 1.7
            }

            .offer {
                border: 1px solid rgba(216,180,106,.38);
                background: linear-gradient(110deg,rgba(216,180,106,.12),rgba(197,109,132,.07));
                border-radius: 24px;
                padding: 22px 25px;
                display: flex;
                align-items: center;
                justify-content: space-between;
                gap: 20px;
                margin-bottom: 27px
            }

            .offer b {
                font-size: 21px;
                color: var(--gold2)
            }

            .offer small {
                display: block;
                color: var(--muted);
                margin-top: 5px
            }

            .filters {
                display: flex;
                gap: 8px;
                flex-wrap: wrap;
                margin-bottom: 25px
            }

            .filter {
                cursor: pointer;
                border: 1px solid var(--line);
                background: #0d0f13;
                color: #bdb7ae;
                border-radius: 999px;
                padding: 10px 14px;
                font-size: 11px;
                font-weight: 900
            }

            .filter.active,.filter:hover {
                background: var(--gold);
                color: #17120a;
                border-color: var(--gold)
            }

            .products {
                display: grid;
                grid-template-columns: repeat(3,1fr);
                gap: 18px
            }

            .product {
                background: linear-gradient(145deg,#15181f,#0e1014);
                border: 1px solid var(--line);
                border-radius: var(--r);
                overflow: hidden;
                box-shadow: 0 12px 45px rgba(0,0,0,.25);
                transition: .25s
            }

            .product:hover {
                transform: translateY(-6px);
                border-color: rgba(216,180,106,.4);
                box-shadow: var(--shadow)
            }

            .productArt {
                height: 210px;
                display: flex;
                align-items: center;
                justify-content: center;
                position: relative;
                background: radial-gradient(circle at 50% 40%,rgba(216,180,106,.17),transparent 27%),#101218
            }

            .cloth {
                width: 132px;
                height: 154px;
                border-radius: 58px 58px 24px 24px;
                background: linear-gradient(145deg,#c87d91,#d8b46a 50%,#4a3039);
                box-shadow: 18px 24px 45px rgba(0,0,0,.55)
            }

            .badge {
                position: absolute;
                top: 15px;
                left: 15px;
                color: var(--gold2);
                border: 1px solid var(--line);
                background: #090a0d;
                padding: 7px 10px;
                border-radius: 999px;
                font-size: 9px;
                font-weight: 900;
                letter-spacing: .1em
            }

            .productBody {
                padding: 19px
            }

            .productBody h3 {
                font: 600 22px Georgia,serif;
                margin: 0 0 7px
            }

            .productBody p {
                color: var(--muted);
                font-size: 13px;
                line-height: 1.55;
                min-height: 41px;
                margin: 0
            }

            .price {
                color: var(--gold2);
                font-size: 23px;
                font-weight: 950;
                margin: 14px 0
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
                cursor: pointer;
                border: 1px solid var(--line);
                background: #0a0b0e;
                color: #ddd6cb;
                border-radius: 8px;
                padding: 7px 8px;
                font-size: 10px;
                font-weight: 850
            }

            .size:hover {
                border-color: var(--gold);
                color: var(--gold2)
            }

            .add {
                cursor: pointer;
                width: 100%;
                border: 0;
                border-radius: 11px;
                padding: 12px;
                font-weight: 950;
                background: linear-gradient(135deg,#f0d18d,#a87932);
                color: #17120a
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
                margin: 0 0 14px
            }

            .info p,.info li {
                color: var(--muted);
                line-height: 1.75
            }

            .info ul {
                padding-left: 19px
            }

            .footer {
                border-top: 1px solid var(--line);
                padding: 34px 0;
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
                color: var(--text)
            }

            .modal {
                display: none;
                position: fixed;
                inset: 0;
                z-index: 100;
                background: rgba(0,0,0,.74);
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
                background: #12151b;
                border: 1px solid var(--line);
                border-radius: 28px 28px 0 0;
                padding: 25px;
                box-shadow: var(--shadow)
            }

            .sheetTop {
                display: flex;
                align-items: center;
                justify-content: space-between
            }

            .sheetTop h2 {
                font: 500 31px Georgia,serif
            }

            .close {
                width: 38px;
                height: 38px;
                border-radius: 50%;
                border: 1px solid var(--line);
                background: #0a0b0e;
                color: #fff;
                cursor: pointer
            }

            .cartItem {
                display: flex;
                justify-content: space-between;
                gap: 15px;
                border-bottom: 1px solid var(--line);
                padding: 14px 0
            }

            .cartItem small {
                color: var(--muted)
            }

            .total {
                text-align: right;
                color: var(--gold2);
                font-size: 20px;
                font-weight: 950;
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

                .products {
                    grid-template-columns: repeat(2,1fr)
                }

                .links {
                    display: none
                }

                .heroArt {
                    height: 380px
                }
            }

            @media(max-width: 560px) {
                .products {
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
        <div class="topbar">
            <div class="container">
                <span>✦ PREMIUM WINTER EDIT • BHAJNI FASHION WORLD</span>
                <span>📍 SECTOR 9, PANCHKULA • BOOTH NO. 14</span>
            </div>
        </div>
        <nav class="nav">
            <div class="container navin">
                <a class="logo" href="#home">
                    BHAJNI <span>FASHION WORLD</span>
                </a>
                <div class="links">
                    <a href="#collection">Collection</a>
                    <a href="#offer">20% Offer</a>
                    <a href="#visit">Visit Us</a>
                </div>
                <button class="cart" onclick="openCart()">
                    BAG • <span id="count">0</span>
                </button>
            </div>
        </nav>
        <section class="hero" id="home">
            <div class="container heroGrid">
                <div>
                    <span class="kicker">Winter collection • now available</span>
                    <h1>
                        Warm looks.<br>
                        <em>Premium comfort.</em>
                    </h1>
                    <p>
                        Welcome to <b>BHAJNI FASHION WORLD</b>
                        — your destination for ladies' night wear and winter fashion. Shop winter lowers, night suits, nighties, cardigans and Kidley winter inner with a refined, comfortable feel.
                    </p>
                    <div class="actions">
                        <a class="btn primary" href="#collection">Explore Collection</a>
                        <a class="btn secondary" href="https://wa.me/919815395390?text=Hello%20BHAJNI%20FASHION%20WORLD%2C%20I%20want%20to%20see%20the%20winter%20collection." target="_blank">WhatsApp Us</a>
                    </div>
                </div>
                <div class="heroArt">
                    <div class="dress"></div>
                    <div class="heroTag">
                        <strong>Winter, beautifully worn.</strong>
                        <small>Cozy layers • everyday style • comfort you can feel</small>
                    </div>
                </div>
            </div>
        </section>
        <section class="section" id="collection">
            <div class="container">
                <div class="head">
                    <div>
                        <span class="kicker">Curated for the season</span>
                        <h2>The Winter Edit</h2>
                    </div>
                    <p>Choose a category and tap a size to add the item to your bag. Every listed price is shown clearly.</p>
                </div>
                <div class="offer" id="offer">
                    <div>
                        <b>BUY MORE, SAVE MORE — 20% OFF</b>
                        <small>
                            Purchase more than 2 items and receive a direct <strong>20% OFF</strong>
                            on the total amount.
                        </small>
                    </div>
                    <span style="font-size:34px;color:var(--gold2);font-weight:950">20%</span>
                </div>
                <div class="filters">
                    <button class="filter active" data-filter="all">ALL</button>
                    <button class="filter" data-filter="lower">WINTER LOWERS</button>
                    <button class="filter" data-filter="suit">NIGHT SUITS</button>
                    <button class="filter" data-filter="nightie">NIGHTIES</button>
                    <button class="filter" data-filter="cardigan">CARDIGANS</button>
                    <button class="filter" data-filter="inner">KIDLEY INNER</button>
                </div>
                <div class="products" id="products"></div>
            </div>
        </section>
        <section class="section" id="visit">
            <div class="container">
                <div class="head">
                    <div>
                        <span class="kicker">BHAJNI FASHION WORLD</span>
                        <h2>Visit The Store</h2>
                    </div>
                </div>
                <div class="infoGrid">
                    <div class="info">
                        <h3>Find Us</h3>
                        <ul>
                            <li>
                                <b>Shop:</b>
                                Sector 9, Panchkula
                            </li>
                            <li>
                                <b>Booth No.:</b>
                                14
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
                        <h3>Let's find your fit.</h3>
                        <p>Send us the product and size you want on WhatsApp. We can help you confirm availability, colour and the final price before you visit.</p>
                        <a class="btn primary" style="width:100%" href="https://wa.me/919815395390?text=Hello%20BHAJNI%20FASHION%20WORLD%2C%20please%20help%20me%20with%20product%20availability%20and%20sizes." target="_blank">Chat On WhatsApp</a>
                    </div>
                </div>
            </div>
        </section>
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
                <div class="total" id="total">Total: ₹0</div>
                <a id="wa" class="btn primary" style="width:100%" target="_blank">Send Order Enquiry On WhatsApp</a>
                <p class="note">When more than 2 items are purchased, the website calculates 20% OFF on the listed priced items. Kidley Inner is listed as 15% OFF MRP, so its exact amount depends on the MRP. Please confirm availability, colour and final bill with the shop.</p>
            </div>
        </div>
        <script>
            const products = [{
                cat: "lower",
                name: "Winter Lower",
                desc: "Warm and comfortable everyday winter lower.",
                sizes: [["SMALL", 250], ["MEDIUM", 250], ["LARGE", 300], ["XL", 300], ["XXL", 350], ["XXXL", 350]]
            }, {
                cat: "suit",
                name: "Winter Night Suit",
                desc: "Cozy winter night suit for relaxed evenings.",
                sizes: [["MEDIUM", 500], ["LARGE", 500], ["XL", 550], ["XXL", 550], ["XXL", 600]]
            }, {
                cat: "nightie",
                name: "Winter Blanket Nightie",
                desc: "Extra-cozy blanket winter nightie.",
                sizes: [["REGULAR", 650]]
            }, {
                cat: "nightie",
                name: "Winter Velvet Nightie",
                desc: "Soft velvet winter nightie with a premium feel.",
                sizes: [["REGULAR", 890], ["XXXL", 1190]]
            }, {
                cat: "cardigan",
                name: "Winter Cardigan",
                desc: "A warm and easy-to-style winter layer.",
                sizes: [["MEDIUM", 500], ["XL", 550], ["XXL", 600], ["XXXL", 600]]
            }, {
                cat: "inner",
                name: "Kidley Winter Inner",
                desc: "Winter inner available at 15% OFF MRP.",
                sizes: [["MRP − 15%", null]]
            }];
            let filter = "all"
              , bag = [];
            function render() {
                const box = document.getElementById("products");
                box.innerHTML = products.filter(p => filter === "all" || p.cat === filter).map(p => {
                    const idx = products.indexOf(p)
                      , nums = p.sizes.filter(s => s[1] != null).map(s => s[1]);
                    const price = nums.length ? `₹${Math.min(...nums)} <small>onwards</small>` : `15% OFF <small>MRP</small>`;
                    return `<article class="product"><div class="productArt"><span class="badge">${p.cat === "inner" ? "SPECIAL OFFER" : "WINTER EDIT"}</span><div class="cloth"></div></div><div class="productBody"><h3>${p.name}</h3><p>${p.desc}</p><div class="price">${price}</div><div class="sizes">${p.sizes.map( (s, j) => `<button class="size" onclick="add(${idx},${j})">${s[0]}${s[1] != null ? " • ₹" + s[1] : ""}</button>`).join("")}</div><button class="add" onclick="add(${idx},0)">ADD TO BAG</button></div></article>`;
                }
                ).join("");
            }
            document.querySelectorAll(".filter").forEach(b => b.onclick = () => {
                document.querySelectorAll(".filter").forEach(x => x.classList.remove("active"));
                b.classList.add("active");
                filter = b.dataset.filter;
                render()
            }
            );
            function add(pi, si) {
                const s = products[pi].sizes[si];
                bag.push({
                    name: products[pi].name,
                    size: s[0],
                    price: s[1]
                });
                document.getElementById("count").textContent = bag.length;
                openCart()
            }
            function openCart() {
                document.getElementById("modal").classList.add("open");
                document.getElementById("cart").innerHTML = bag.length ? bag.map(x => `<div class="cartItem"><span><b>${x.name}</b><br><small>Size: ${x.size}</small></span><b>${x.price == null ? "15% OFF MRP" : "₹" + x.price}</b></div>`).join("") : "<p class='note'>Your bag is empty. Choose a product size from the collection.</p>";
                const priced = bag.filter(x => x.price != null)
                  , subtotal = priced.reduce( (a, x) => a + x.price, 0)
                  , discount = bag.length > 2 ? subtotal * .2 : 0
                  , total = subtotal - discount;
                document.getElementById("total").innerHTML = bag.length ? `Subtotal: ₹${subtotal.toFixed(0)}${bag.length > 2 ? `<br><span style="color:#d8b46a">20% OFF: −₹${discount.toFixed(0)}</span><br>Total: ₹${total.toFixed(0)}` : `<br>Total: ₹${subtotal.toFixed(0)}`}${bag.some(x => x.price == null) ? '<br><small style="color:#aaa">+ Kidley Inner at 15% OFF MRP</small>' : ''}` : "Total: ₹0";
                let msg = "Hello BHAJNI FASHION WORLD! I would like to enquire about:%0A" + bag.map(x => `• ${x.name} — ${x.size}${x.price != null ? " — ₹" + x.price : " — 15% OFF MRP"}`).join("%0A");
                if (bag.length > 2)
                    msg += "%0A%0A20%25 OFF applies because more than 2 items are selected.";
                msg += "%0A%0APlease confirm availability, colour and final bill.";
                document.getElementById("wa").href = "https://wa.me/919815395390?text=" + msg;
            }
            function closeCart() {
                document.getElementById("modal").classList.remove("open")
            }
            render();
        </script>
    </body>
</html>
