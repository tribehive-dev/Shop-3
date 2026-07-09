<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-8745527260470621"
     crossorigin="anonymous"></script>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Tribe Hive — Pure African Honey</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,700;0,900;1,700&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">
<style>
  :root {
    --amber: #B45309; --amber-light: #F59E0B; --amber-glow: #FCD34D;
    --cream: #FFFBEB; --cream-dark: #FEF3C7; --brown: #78350F;
    --brown-deep: #451A03; --green: #166534; --text: #1C0A00;
  }
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: 'Inter', sans-serif; background: var(--cream); color: var(--text); overflow-x: hidden; }

  nav {
    position: fixed; top: 0; left: 0; right: 0; z-index: 100;
    background: rgba(255,251,235,0.95); backdrop-filter: blur(12px);
    border-bottom: 1px solid #FDE68A; padding: 0 6vw;
    display: flex; align-items: center; justify-content: space-between; height: 64px;
  }
  .logo { font-family: 'Playfair Display', serif; font-size: 1.5rem; font-weight: 900; color: var(--brown); }
  .logo span { color: var(--amber-light); }
  nav ul { list-style: none; display: flex; gap: 2rem; }
  nav ul a { text-decoration: none; color: var(--brown); font-size: 0.875rem; font-weight: 500; transition: color 0.2s; }
  nav ul a:hover { color: var(--amber); }
  .cart-btn {
    background: var(--amber); color: white; border: none; cursor: pointer;
    padding: 0.5rem 1.25rem; border-radius: 100px; font-size: 0.875rem; font-weight: 600;
    font-family: 'Inter', sans-serif; display: flex; align-items: center; gap: 0.4rem;
    transition: background 0.2s, transform 0.15s;
  }
  .cart-btn:hover { background: var(--brown); transform: scale(1.04); }
  #cart-count {
    background: var(--amber-glow); color: var(--brown-deep); border-radius: 50%;
    width: 20px; height: 20px; display: flex; align-items: center; justify-content: center;
    font-size: 0.75rem; font-weight: 700;
  }

  .hero {
    min-height: 100vh; display: flex; align-items: center;
    padding: 80px 6vw 60px;
    background: linear-gradient(135deg, #FFFBEB 60%, #FEF3C7 100%);
    position: relative; overflow: hidden;
  }
  .hero::before {
    content: ''; position: absolute; top: -60px; right: -60px;
    width: 520px; height: 520px;
    background: radial-gradient(circle, #FCD34D33 0%, transparent 70%);
    border-radius: 50%; animation: pulse 4s ease-in-out infinite;
  }
  @keyframes pulse { 0%,100%{transform:scale(1);opacity:.7} 50%{transform:scale(1.1);opacity:1} }
  .hero-content { max-width: 520px; position: relative; z-index: 2; }
  .hero-badge {
    display: inline-flex; align-items: center; gap: 0.4rem;
    background: #FDE68A; color: var(--brown); padding: 0.3rem 1rem; border-radius: 100px;
    font-size: 0.8rem; font-weight: 600; text-transform: uppercase; letter-spacing: 0.08em; margin-bottom: 1.5rem;
  }
  .hero h1 { font-family: 'Playfair Display', serif; font-size: clamp(2.4rem, 5vw, 4rem); font-weight: 900; line-height: 1.05; color: var(--brown-deep); margin-bottom: 1.25rem; }
  .hero h1 em { font-style: italic; color: var(--amber); }
  .hero p { font-size: 1.05rem; font-weight: 300; color: #6B3B1A; line-height: 1.7; margin-bottom: 2rem; max-width: 440px; }
  .hero-cta { display: flex; gap: 1rem; flex-wrap: wrap; }
  .btn-primary { background: var(--amber); color: white; text-decoration: none; padding: 0.85rem 2rem; border-radius: 100px; font-weight: 600; font-size: 1rem; transition: background 0.2s, transform 0.15s; border: none; cursor: pointer; font-family: 'Inter', sans-serif; }
  .btn-primary:hover { background: var(--brown); transform: translateY(-2px); }
  .btn-outline { background: transparent; color: var(--amber); text-decoration: none; padding: 0.85rem 2rem; border-radius: 100px; font-weight: 600; font-size: 1rem; border: 2px solid var(--amber); transition: all 0.2s; cursor: pointer; font-family: 'Inter', sans-serif; }
  .btn-outline:hover { background: var(--amber); color: white; transform: translateY(-2px); }

  .hero-visual {
    position: absolute; right: 5vw; top: 50%; transform: translateY(-50%);
    z-index: 1; width: 420px; max-width: 38vw;
  }
  .hero-visual img { width: 100%; border-radius: 20px; box-shadow: 0 24px 60px rgba(180,83,9,0.25); animation: floatImg 4s ease-in-out infinite; }
  @keyframes floatImg { 0%,100%{transform:translateY(0)} 50%{transform:translateY(-12px)} }

  .trust-bar { background: var(--brown); padding: 1.5rem 6vw; display: flex; justify-content: center; gap: 3rem; flex-wrap: wrap; }
  .trust-item { display: flex; align-items: center; gap: 0.6rem; color: var(--cream); font-size: 0.9rem; font-weight: 500; }

  .section-label { font-size: 0.75rem; font-weight: 600; text-transform: uppercase; letter-spacing: 0.12em; color: var(--amber); margin-bottom: 0.5rem; }
  .section-title { font-family: 'Playfair Display', serif; font-size: clamp(1.8rem, 4vw, 2.8rem); font-weight: 700; color: var(--brown-deep); line-height: 1.15; }

  .products-section { padding: 6rem 6vw; }
  .products-header { text-align: center; margin-bottom: 3.5rem; }
  .products-header p { color: #6B3B1A; font-size: 1rem; margin-top: 0.75rem; font-weight: 300; }
  .honey-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(280px, 1fr)); gap: 1.5rem; max-width: 960px; margin: 0 auto; }
  .product-card { background: white; border-radius: 20px; overflow: hidden; border: 1.5px solid #FDE68A; transition: transform 0.25s, box-shadow 0.25s; }
  .product-card:hover { transform: translateY(-6px); box-shadow: 0 20px 50px rgba(180,83,9,0.15); }
  .card-img { width: 100%; height: 210px; display: flex; align-items: center; justify-content: center; overflow: hidden; }
  .card-img img { width: 100%; height: 100%; object-fit: cover; }
  .card-body { padding: 1.25rem; }
  .card-tag { font-size: 0.7rem; font-weight: 600; text-transform: uppercase; letter-spacing: 0.1em; color: var(--green); margin-bottom: 0.4rem; }
  .card-name { font-family: 'Playfair Display', serif; font-size: 1.2rem; font-weight: 700; color: var(--brown-deep); margin-bottom: 0.4rem; }
  .card-desc { font-size: 0.85rem; color: #7C3B1E; font-weight: 300; line-height: 1.5; margin-bottom: 1rem; }
  .card-footer { display: flex; align-items: center; justify-content: space-between; }
  .card-price { font-size: 1.1rem; font-weight: 700; color: var(--amber); }
  .card-price small { font-size: 0.75rem; color: #9CA3AF; font-weight: 400; }
  .add-btn { background: var(--amber-light); color: var(--brown-deep); border: none; cursor: pointer; padding: 0.5rem 1.1rem; border-radius: 100px; font-size: 0.85rem; font-weight: 600; font-family: 'Inter', sans-serif; transition: background 0.2s, transform 0.15s; }
  .add-btn:hover { background: var(--amber); color: white; transform: scale(1.05); }
  .add-btn.added { background: var(--green); color: white; }
  .stars { color: var(--amber-light); font-size: 0.85rem; margin-bottom: 0.5rem; }
  .delivery-badge { display: inline-block; background: #DCFCE7; color: var(--green); font-size: 0.7rem; font-weight: 600; padding: 0.2rem 0.65rem; border-radius: 100px; margin-bottom: 0.75rem; }

  .why-section { background: var(--brown-deep); padding: 6rem 6vw; color: var(--cream); }
  .why-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 5rem; align-items: center; max-width: 1100px; margin: 0 auto; }
  .why-text .section-title { color: var(--cream-dark); }
  .why-text p { color: #D6B89A; font-weight: 300; line-height: 1.8; margin: 1.25rem 0 2rem; }
  .why-items { display: flex; flex-direction: column; gap: 1.5rem; }
  .why-item { display: flex; gap: 1rem; align-items: flex-start; }
  .why-icon { width: 44px; height: 44px; flex-shrink: 0; background: rgba(245,158,11,0.15); border-radius: 12px; display: flex; align-items: center; justify-content: center; font-size: 1.3rem; }
  .why-item h4 { font-size: 1rem; font-weight: 600; color: var(--amber-glow); margin-bottom: 0.25rem; }
  .why-item p { color: #C4986E; font-size: 0.9rem; margin: 0; }

  .testimonials { padding: 6rem 6vw; background: var(--cream-dark); }
  .testimonials-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(280px, 1fr)); gap: 1.5rem; margin-top: 3rem; }
  .testimonial-card { background: white; border-radius: 16px; padding: 1.75rem; border: 1px solid #FDE68A; }
  .testimonial-card p { color: #4A2000; font-size: 0.95rem; line-height: 1.7; font-style: italic; margin-bottom: 1.25rem; font-weight: 300; }
  .reviewer { display: flex; align-items: center; gap: 0.75rem; }
  .avatar { width: 42px; height: 42px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 1.2rem; background: var(--cream-dark); }
  .reviewer-name { font-weight: 600; font-size: 0.9rem; color: var(--brown-deep); }
  .reviewer-loc { font-size: 0.78rem; color: #9CA3AF; }

  .order-section { padding: 6rem 6vw; text-align: center; }
  .steps { display: flex; gap: 2rem; margin-top: 3rem; justify-content: center; flex-wrap: wrap; }
  .step { max-width: 240px; display: flex; flex-direction: column; align-items: center; }
  .step-num { width: 56px; height: 56px; background: var(--amber); color: white; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-family: 'Playfair Display', serif; font-size: 1.3rem; font-weight: 700; margin-bottom: 1rem; }
  .step h4 { font-weight: 600; color: var(--brown-deep); margin-bottom: 0.5rem; }
  .step p { font-size: 0.875rem; color: #7C3B1E; font-weight: 300; line-height: 1.6; }
  .opay-btn { display: inline-flex; align-items: center; gap: 0.5rem; background: #FF6600; color: white; padding: 0.6rem 1.4rem; border-radius: 100px; font-weight: 700; font-size: 0.9rem; text-decoration: none; margin-top: 0.75rem; transition: background 0.2s, transform 0.15s; }
  .opay-btn:hover { background: #e05a00; transform: scale(1.04); }
  .opay-circle { width: 22px; height: 22px; background: white; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 0.65rem; font-weight: 900; color: #FF6600; }
  .wa-step-link { display: inline-flex; align-items: center; gap: 0.4rem; color: #25D366; font-weight: 600; font-size: 0.9rem; text-decoration: none; margin-top: 0.75rem; }

  footer { background: var(--brown-deep); padding: 3rem 6vw; text-align: center; color: #C4986E; font-size: 0.875rem; }
  footer .logo { margin-bottom: 0.75rem; display: block; }
  footer p { font-weight: 300; line-height: 1.8; }
  footer a { color: var(--amber-light); text-decoration: none; }
  .wa-footer { display: inline-flex; align-items: center; gap: 0.4rem; color: var(--amber-light); }

  .cart-overlay { display: none; position: fixed; inset: 0; z-index: 200; background: rgba(0,0,0,0.5); }
  .cart-overlay.open { display: flex; justify-content: flex-end; }
  .cart-panel { background: var(--cream); width: min(420px,100vw); height: 100vh; overflow-y: auto; padding: 2rem; animation: slideIn 0.3s ease; }
  @keyframes slideIn { from{transform:translateX(100%)} to{transform:translateX(0)} }
  .cart-header { display: flex; justify-content: space-between; align-items: center; margin-bottom: 2rem; }
  .cart-header h2 { font-family: 'Playfair Display', serif; font-size: 1.5rem; color: var(--brown-deep); }
  .close-btn { background: none; border: none; cursor: pointer; font-size: 1.5rem; color: var(--brown); }
  .cart-items { display: flex; flex-direction: column; gap: 1rem; margin-bottom: 2rem; }
  .cart-item { background: white; border-radius: 12px; padding: 1rem; display: flex; align-items: center; gap: 1rem; border: 1px solid #FDE68A; }
  .cart-item-emoji { font-size: 2rem; }
  .cart-item-info { flex: 1; }
  .cart-item-name { font-weight: 600; font-size: 0.9rem; color: var(--brown-deep); }
  .cart-item-price { font-size: 0.85rem; color: var(--amber); font-weight: 600; }
  .remove-btn { background: none; border: none; cursor: pointer; color: #EF4444; font-size: 1rem; }
  .cart-total { background: var(--brown-deep); color: white; padding: 1.5rem; border-radius: 16px; margin-bottom: 1rem; display: flex; justify-content: space-between; align-items: center; }
  .cart-total span { font-weight: 300; font-size: 0.85rem; }
  .cart-total strong { font-size: 1.25rem; color: var(--amber-glow); }
  .checkout-btn { width: 100%; background: #25D366; color: white; border: none; cursor: pointer; padding: 1rem; border-radius: 100px; font-size: 1rem; font-weight: 600; font-family: 'Inter', sans-serif; transition: background 0.2s; display: flex; align-items: center; justify-content: center; gap: 0.5rem; }
  .checkout-btn:hover { background: #1ebe5d; }
  .empty-cart { text-align: center; color: #9CA3AF; padding: 3rem 0; font-size: 0.95rem; }
  .empty-cart div { font-size: 3rem; margin-bottom: 1rem; }
  .toast { position: fixed; bottom: 2rem; left: 50%; transform: translateX(-50%) translateY(100px); background: var(--green); color: white; padding: 0.75rem 1.5rem; border-radius: 100px; font-size: 0.9rem; font-weight: 500; z-index: 300; transition: transform 0.4s ease; pointer-events: none; }
  .toast.show { transform: translateX(-50%) translateY(0); }

  @media (max-width: 900px) { .hero-visual { display: none; } .why-grid { grid-template-columns: 1fr; gap: 2rem; } nav ul { display: none; } }
</style>
</head>
<body>

<nav>
  <div class="logo">Tribe <span>Hive</span></div>
  <ul>
    <li><a href="#products">Shop</a></li>
    <li><a href="#why">Our Story</a></li>
    <li><a href="#order">How to Order</a></li>
  </ul>
  <button class="cart-btn" onclick="openCart()">🛒 Cart <span id="cart-count">0</span></button>
</nav>

<!-- HERO -->
<section class="hero">
  <div class="hero-content">
    <div class="hero-badge">🍯 100% Pure & Natural · African Honey</div>
    <h1>Pure African Honey,<br>Straight from the <em>Source</em></h1>
    <p>Sourced directly from trusted Nigerian beekeepers. Every bottle is raw, unfiltered, and naturally rich — the real thing, nothing else.</p>
    <div class="hero-cta">
      <a href="#products" class="btn-primary">Shop Honey</a>
      <a href="#why" class="btn-outline">Our Promise</a>
    </div>
  </div>
  <div class="hero-visual">
    <!-- YOUR TRIBE HIVE PHOTO — upload to imgbb.com and replace this src -->
    <img src="https://i.ibb.co/7JwHjr1F/file-00000000002871f48bbfde27c0381cac.png"
      onerror="this.style.display='none'"
      alt="Tribe Hive — 2 Litres, 1 Litre, 75cl">
  </div>
</section>

<!-- TRUST BAR -->
<div class="trust-bar">
  <div class="trust-item">✅ No Sugar Added</div>
  <div class="trust-item">🚚 Delivery Inclusive Nationwide</div>
  <div class="trust-item">🐝 Direct from Nigerian Beekeepers</div>
  <div class="trust-item">🌿 100% Pure & Natural</div>
</div>

<!-- PRODUCTS -->
<section class="products-section" id="products">
  <div class="products-header">
    <div class="section-label">Our Collection</div>
    <h2 class="section-title">Tribe Hive Honey</h2>
    <p>100% Pure & Natural — raw, unprocessed, freshly harvested. <strong>All prices include delivery anywhere in Nigeria.</strong></p>
  </div>
  <div class="honey-grid" id="product-grid"></div>
</section>

<!-- WHY US -->
<section class="why-section" id="why">
  <div class="why-grid">
    <div class="why-text">
      <div class="section-label" style="color:var(--amber-glow)">Our Promise</div>
      <h2 class="section-title">We Don't Compromise<br>on Purity</h2>
      <p>Tribe Hive was born from frustration — too much fake honey in the market. We went to the source: trusted Nigerian beekeepers, delivering pure, uncut honey straight to your door.</p>
      <a href="#products" class="btn-primary">Shop Now</a>
    </div>
    <div class="why-items">
      <div class="why-item"><div class="why-icon">🐝</div><div><h4>Ethically Harvested</h4><p>We partner only with beekeepers who use sustainable practices and treat their bees well.</p></div></div>
      <div class="why-item"><div class="why-icon">🌿</div><div><h4>100% Natural</h4><p>No additives, no preservatives, no sugar. Just pure honey the way nature intended.</p></div></div>
      <div class="why-item"><div class="why-icon">🚚</div><div><h4>Delivery Inclusive</h4><p>All prices include delivery to anywhere in Nigeria. No hidden charges — ever.</p></div></div>
      <div class="why-item"><div class="why-icon">✅</div><div><h4>100% Satisfaction</h4><p>If your honey isn't authentic and delicious, we'll replace it or refund you. Full stop.</p></div></div>
    </div>
  </div>
</section>

<!-- TESTIMONIALS -->
<section class="testimonials">
  <div style="text-align:center">
    <div class="section-label">Happy Customers</div>
    <h2 class="section-title">What People Are Saying</h2>
  </div>
  <div class="testimonials-grid">
    <div class="testimonial-card">
      <div class="stars">★★★★★</div>
      <p>"I have been searching for real honey for years. This honey from Tribe Hive blew my mind — thick, dark, and incredibly aromatic. This is the genuine article."</p>
      <div class="reviewer"><div class="avatar">👩🏾</div><div><div class="reviewer-name">Amaka O.</div><div class="reviewer-loc">Enugu, Nigeria</div></div></div>
    </div>
    <div class="testimonial-card">
      <div class="stars">★★★★★</div>
      <p>"My doctor recommended raw honey. I tried Tribe Hive — within weeks I noticed real improvement. Delivery was fast and there were no extra charges!"</p>
      <div class="reviewer"><div class="avatar">👨🏾</div><div><div class="reviewer-name">Emeka A.</div><div class="reviewer-loc">Anambra, Nigeria</div></div></div>
    </div>
    <div class="testimonial-card">
      <div class="stars">★★★★★</div>
      <p>"I ordered multiple bottles as gifts. Everyone loved it and several have reordered. You can taste the purity — absolutely wonderful honey."</p>
      <div class="reviewer"><div class="avatar">👩🏿</div><div><div class="reviewer-name">Fatima B.</div><div class="reviewer-loc">Abuja, Nigeria</div></div></div>
    </div>
  </div>
</section>

<!-- HOW TO ORDER -->
<section class="order-section" id="order">
  <div class="section-label">Simple Process</div>
  <h2 class="section-title">How to Order</h2>
  <div class="steps">
    <div class="step">
      <div class="step-num">1</div>
      <h4>Choose Your Size</h4>
      <p>Pick from 75cl, 1 Litre, or 2 Litres. All prices include delivery anywhere in Nigeria.</p>
    </div>
    <div class="step">
      <div class="step-num">2</div>
      <h4>Pay via Opay</h4>
      <p>Send payment to <strong>7034529060</strong><br>Chinyere Breath Ihegazie</p>
      <a class="opay-btn" href="https://opayweb.com" target="_blank">
        <span class="opay-circle">O</span> Pay on Opay
      </a>
    </div>
    <div class="step">
      <div class="step-num">3</div>
      <h4>Send Receipt on WhatsApp</h4>
      <p>After payment, send your receipt to our WhatsApp for order confirmation and your delivery address.</p>
      <a class="wa-step-link" href="https://wa.me/2347034529060" target="_blank">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="#25D366"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/></svg>
        Send Receipt: 07034529060
      </a>
    </div>
    <div class="step">
      <div class="step-num">4</div>
      <h4>Enjoy Pure Honey</h4>
      <p>We confirm your order and dispatch immediately. Your honey arrives sealed and fresh.</p>
    </div>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <div class="logo">Tribe <span style="color:var(--amber-light)">Hive</span></div>
  <p>Pure. Original. Nigerian.<br>
    <a href="https://wa.me/2347034529060" target="_blank" class="wa-footer">
      <svg width="16" height="16" viewBox="0 0 24 24" fill="#25D366"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/></svg>
      07034529060
    </a>
    &nbsp;|&nbsp; 📍 Enugu State, Nigeria
  </p>
  <p style="margin-top:1rem;font-size:0.78rem;opacity:0.5;">© 2026 Tribe Hive. All rights reserved.</p>
</footer>

<!-- CART -->
<div class="cart-overlay" id="cart-overlay" onclick="closeCartOnOverlay(event)">
  <div class="cart-panel">
    <div class="cart-header">
      <h2>🛒 Your Cart</h2>
      <button class="close-btn" onclick="closeCart()">✕</button>
    </div>
    <div class="cart-items" id="cart-items-list"></div>
    <div id="cart-summary"></div>
  </div>
</div>
<div class="toast" id="toast"></div>

<script>
  const products = [
    { id:1, name:"Tribe Hive Honey", size:"75cl", tag:"Starter Size", emoji:"🍯",
      bg:"linear-gradient(135deg,#D97706 0%,#B45309 60%,#92400E 100%)",
      desc:"Perfect starter size. Raw, unfiltered African honey from trusted Nigerian beekeepers. Rich, thick and naturally sweet.", price:11500, stars:5 },
    { id:2, name:"Tribe Hive Honey", size:"1 Litre", tag:"Most Popular", emoji:"🍯",
      bg:"linear-gradient(135deg,#F59E0B 0%,#B45309 60%,#78350F 100%)",
      desc:"Our best-selling size. Pure African honey for daily use — for health, cooking, or as a natural sweetener.", price:23000, stars:5 },
    { id:3, name:"Tribe Hive Honey", size:"2 Litres", tag:"Best Value", emoji:"🍯",
      bg:"linear-gradient(135deg,#B45309 0%,#78350F 50%,#451A03 100%)",
      desc:"Family size. Stock up on the purest African honey — ideal for families, gifting, or daily health routines.", price:35000, stars:5 }
  ];

  let cart = [];

  function renderProducts() {
    document.getElementById('product-grid').innerHTML = products.map(p => `
      <div class="product-card">
        <div class="card-img" style="background:${p.bg}">
          <span style="font-size:5.5rem;filter:drop-shadow(0 4px 16px rgba(0,0,0,0.3))">${p.emoji}</span>
        </div>
        <div class="card-body">
          <div class="card-tag">${p.tag}</div>
          <div class="card-name">${p.name} <span style="color:var(--amber)">(${p.size})</span></div>
          <div class="stars">${'★'.repeat(p.stars)}</div>
          <div class="delivery-badge">🚚 Delivery Inclusive — Anywhere in Nigeria</div>
          <div class="card-desc">${p.desc}</div>
          <div class="card-footer">
            <div class="card-price">₦${p.price.toLocaleString()} <small>/ ${p.size}</small></div>
            <button class="add-btn" id="btn-${p.id}" onclick="addToCart(${p.id})">Add to Cart</button>
          </div>
        </div>
      </div>`).join('');
  }

  function addToCart(id) {
    const p = products.find(x => x.id === id);
    const ex = cart.find(c => c.id === id);
    if (ex) ex.qty++; else cart.push({...p, qty:1});
    updateCartCount();
    showToast(`${p.emoji} ${p.name} (${p.size}) added!`);
    const btn = document.getElementById(`btn-${id}`);
    btn.textContent = '✓ Added'; btn.classList.add('added');
    setTimeout(() => { btn.textContent = 'Add to Cart'; btn.classList.remove('added'); }, 1500);
  }

  function removeFromCart(id) { cart = cart.filter(c => c.id !== id); updateCartCount(); renderCart(); }
  function updateCartCount() { document.getElementById('cart-count').textContent = cart.reduce((s,c) => s+c.qty, 0); }
  function openCart() { document.getElementById('cart-overlay').classList.add('open'); renderCart(); }
  function closeCart() { document.getElementById('cart-overlay').classList.remove('open'); }
  function closeCartOnOverlay(e) { if (e.target === document.getElementById('cart-overlay')) closeCart(); }

  function renderCart() {
    const list = document.getElementById('cart-items-list');
    const summary = document.getElementById('cart-summary');
    if (!cart.length) {
      list.innerHTML = `<div class="empty-cart"><div>🍯</div>Your cart is empty.<br><small>Add some honey!</small></div>`;
      summary.innerHTML = ''; return;
    }
    list.innerHTML = cart.map(item => `
      <div class="cart-item">
        <div class="cart-item-emoji">${item.emoji}</div>
        <div class="cart-item-info">
          <div class="cart-item-name">${item.name} (${item.size}) × ${item.qty}</div>
          <div class="cart-item-price">₦${(item.price*item.qty).toLocaleString()}</div>
        </div>
        <button class="remove-btn" onclick="removeFromCart(${item.id})">✕</button>
      </div>`).join('');
    const total = cart.reduce((s,c) => s+c.price*c.qty, 0);
    summary.innerHTML = `
      <div class="cart-total"><span>Total (Delivery Inclusive)</span><strong>₦${total.toLocaleString()}</strong></div>
      <button class="checkout-btn" onclick="checkout()">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="white"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/></svg>
        Send Order via WhatsApp
      </button>`;
  }

  function checkout() {
    if (!cart.length) return;
    const total = cart.reduce((s,c) => s+c.price*c.qty, 0);
    const items = cart.map(c => `${c.name} (${c.size}) x${c.qty} — ₦${(c.price*c.qty).toLocaleString()}`).join('\n');
    const msg = `Hello Tribe Hive! I'd like to order:\n\n${items}\n\nTotal: ₦${total.toLocaleString()} (Delivery Inclusive)\n\nI will send my payment receipt after paying via Opay to 7034529060 (Chinyere Breath Ihegazie).\n\nMy delivery address: `;
    window.open(`https://wa.me/2347034529060?text=${encodeURIComponent(msg)}`, '_blank');
  }

  function showToast(msg) {
    const t = document.getElementById('toast');
    t.textContent = msg; t.classList.add('show');
    setTimeout(() => t.classList.remove('show'), 2500);
  }

  renderProducts();
</script>
</body>
</html>
