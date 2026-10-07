
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Tribe Hive — Pure African Honey</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,700;0,900;1,700&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">
<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-8745527260470621" crossorigin="anonymous"></script>
<style>
  :root {
    --amber: #B45309; --amber-light: #F59E0B; --amber-glow: #FCD34D;
    --cream: #FFFBEB; --cream-dark: #FEF3C7; --brown: #78350F;
    --brown-deep: #451A03; --green: #166534; --text: #1C0A00;
  }
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: 'Inter', sans-serif; background: var(--cream); color: var(--text); overflow-x: hidden; }

  /* PAGE SYSTEM */
  .page { display: none; }
  .page.active { display: block; }

  nav {
    position: fixed; top: 0; left: 0; right: 0; z-index: 100;
    background: rgba(255,251,235,0.95); backdrop-filter: blur(12px);
    border-bottom: 1px solid #FDE68A; padding: 0 6vw;
    display: flex; align-items: center; justify-content: space-between; height: 64px;
  }
  .logo { font-family: 'Playfair Display', serif; font-size: 1.5rem; font-weight: 900; color: var(--brown); cursor: pointer; }
  .logo span { color: var(--amber-light); }
  nav ul { list-style: none; display: flex; gap: 1.5rem; align-items: center; }
  nav ul a { text-decoration: none; color: var(--brown); font-size: 0.85rem; font-weight: 500; transition: color 0.2s; cursor: pointer; }
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

  /* MEDIA PREVIEW SECTION */
  .media-preview { padding: 5rem 6vw; background: var(--cream-dark); text-align: center; }
  .media-preview-grid { display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 1.5rem; max-width: 960px; margin: 2rem auto; }
  .media-thumb { border-radius: 16px; overflow: hidden; box-shadow: 0 12px 30px rgba(180,83,9,0.12); border: 1.5px solid #FDE68A; height: 200px; }
  .media-thumb img { width: 100%; height: 100%; object-fit: cover; }
  .media-thumb-video { background: var(--brown-deep); display: flex; flex-direction: column; align-items: center; justify-content: center; color: var(--amber-glow); font-size: 3rem; }
  .media-thumb-video span { font-size: 0.85rem; margin-top: 0.5rem; color: var(--cream); font-weight: 500; }
  .view-media-btn {
    display: inline-flex; align-items: center; gap: 0.5rem;
    background: var(--amber); color: white;
    padding: 0.85rem 2rem; border-radius: 100px;
    font-weight: 700; font-size: 1rem; border: none; cursor: pointer;
    font-family: 'Inter', sans-serif; transition: all 0.2s;
    margin-top: 1rem; text-decoration: none;
  }
  .view-media-btn:hover { background: var(--brown); transform: translateY(-2px); }

  /* REVIEWS PREVIEW */
  .reviews-preview { padding: 5rem 6vw; background: white; text-align: center; }
  .reviews-mini-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(260px, 1fr)); gap: 1.25rem; max-width: 960px; margin: 2rem auto; }
  .review-mini-card { background: var(--cream); border-radius: 16px; padding: 1.25rem; border: 1px solid #FDE68A; text-align: left; }
  .review-mini-card .stars { margin-bottom: 0.5rem; }
  .review-mini-card p { color: #4A2000; font-size: 0.88rem; line-height: 1.6; font-style: italic; margin-bottom: 0.75rem; font-weight: 300; }
  .reviewer { display: flex; align-items: center; gap: 0.6rem; }
  .avatar { width: 36px; height: 36px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 1rem; background: var(--cream-dark); }
  .reviewer-name { font-weight: 600; font-size: 0.85rem; color: var(--brown-deep); }
  .reviewer-loc { font-size: 0.75rem; color: #9CA3AF; }
  .view-reviews-btn {
    display: inline-flex; align-items: center; gap: 0.5rem;
    background: transparent; color: var(--amber);
    padding: 0.85rem 2rem; border-radius: 100px;
    font-weight: 700; font-size: 1rem;
    border: 2px solid var(--amber); cursor: pointer;
    font-family: 'Inter', sans-serif; transition: all 0.2s;
    margin-top: 1rem;
  }
  .view-reviews-btn:hover { background: var(--amber); color: white; transform: translateY(-2px); }

  .why-section { background: var(--brown-deep); padding: 6rem 6vw; color: var(--cream); }
  .why-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 5rem; align-items: center; max-width: 1100px; margin: 0 auto; }
  .why-text .section-title { color: var(--cream-dark); }
  .why-text p { color: #D6B89A; font-weight: 300; line-height: 1.8; margin: 1.25rem 0 2rem; }
  .why-items { display: flex; flex-direction: column; gap: 1.5rem; }
  .why-item { display: flex; gap: 1rem; align-items: flex-start; }
  .why-icon { width: 44px; height: 44px; flex-shrink: 0; background: rgba(245,158,11,0.15); border-radius: 12px; display: flex; align-items: center; justify-content: center; font-size: 1.3rem; }
  .why-item h4 { font-size: 1rem; font-weight: 600; color: var(--amber-glow); margin-bottom: 0.25rem; }
  .why-item p { color: #C4986E; font-size: 0.9rem; margin: 0; }

  .order-section { padding: 6rem 6vw; text-align: center; }
  .steps { display: flex; gap: 2rem; margin-top: 3rem; justify-content: center; flex-wrap: wrap; }
  .step { max-width: 240px; display: flex; flex-direction: column; align-items: center; }
  .step-num { width: 56px; height: 56px; background: var(--amber); color: white; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-family: 'Playfair Display', serif; font-size: 1.3rem; font-weight: 700; margin-bottom: 1rem; }
  .step h4 { font-weight: 600; color: var(--brown-deep); margin-bottom: 0.5rem; }
  .step p { font-size: 0.875rem; color: #7C3B1E; font-weight: 300; line-height: 1.6; }
  .opay-btn { display: inline-flex; align-items: center; gap: 0.5rem; background: #00A859; color: white; padding: 0.6rem 1.4rem; border-radius: 100px; font-weight: 700; font-size: 0.9rem; text-decoration: none; margin-top: 0.75rem; transition: background 0.2s, transform 0.15s; }
  .opay-btn:hover { background: #007a3d; transform: scale(1.04); }
  .wa-step-link { display: inline-flex; align-items: center; gap: 0.4rem; color: #25D366; font-weight: 600; font-size: 0.9rem; text-decoration: none; margin-top: 0.75rem; }

  footer { background: var(--brown-deep); padding: 3rem 6vw; text-align: center; color: #C4986E; font-size: 0.875rem; }
  footer .logo { margin-bottom: 0.75rem; display: block; font-family: 'Playfair Display', serif; font-size: 1.5rem; font-weight: 900; color: var(--brown); cursor: pointer; }
  footer p { font-weight: 300; line-height: 1.8; }
  footer a { color: var(--amber-light); text-decoration: none; }
  .wa-footer { display: inline-flex; align-items: center; gap: 0.4rem; color: var(--amber-light); }

  /* MEDIA PAGE */
  .inner-page { padding: 100px 6vw 5rem; min-height: 100vh; }
  .back-btn {
    display: inline-flex; align-items: center; gap: 0.5rem;
    background: var(--cream-dark); color: var(--brown);
    padding: 0.5rem 1.25rem; border-radius: 100px;
    font-size: 0.85rem; font-weight: 600; border: 1px solid #FDE68A;
    cursor: pointer; margin-bottom: 2rem; transition: all 0.2s;
    font-family: 'Inter', sans-serif;
  }
  .back-btn:hover { background: var(--amber); color: white; }
  .media-full-grid { display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 1.5rem; max-width: 1100px; margin: 2rem auto 0; }
  .media-card { border-radius: 20px; overflow: hidden; box-shadow: 0 20px 50px rgba(180,83,9,0.15); border: 1.5px solid #FDE68A; background: white; }
  .media-card img { width: 100%; height: 280px; object-fit: cover; display: block; }
  .media-card iframe { width: 100%; height: 280px; border: none; display: block; }
  .media-card-body { padding: 1rem 1.25rem 1.25rem; display: flex; align-items: center; justify-content: space-between; }
  .media-card-title { font-family: 'Playfair Display', serif; font-size: 0.95rem; font-weight: 700; color: var(--brown-deep); }
  .yt-btn { display: inline-flex; align-items: center; gap: 0.5rem; background: #FF0000; color: white; padding: 0.5rem 1.1rem; border-radius: 100px; font-weight: 700; font-size: 0.82rem; text-decoration: none; transition: background 0.2s, transform 0.15s; }
  .yt-btn:hover { background: #cc0000; transform: scale(1.04); }

  /* REVIEWS PAGE */
  .reviews-page { padding: 100px 6vw 5rem; min-height: 100vh; background: var(--cream); }
  .reviews-list { max-width: 800px; margin: 2rem auto 0; display: flex; flex-direction: column; gap: 1.25rem; }
  .review-card { background: white; border-radius: 16px; padding: 1.5rem; border: 1px solid #FDE68A; box-shadow: 0 4px 16px rgba(180,83,9,0.07); }
  .review-card-header { display: flex; align-items: center; justify-content: space-between; margin-bottom: 0.75rem; }
  .reviewer-info { display: flex; align-items: center; gap: 0.75rem; }
  .reviewer-avatar { width: 44px; height: 44px; border-radius: 50%; background: var(--amber-glow); display: flex; align-items: center; justify-content: center; font-size: 1.2rem; font-weight: 700; color: var(--brown-deep); }
  .reviewer-details .name { font-weight: 700; font-size: 0.95rem; color: var(--brown-deep); }
  .reviewer-details .date { font-size: 0.75rem; color: #9CA3AF; }
  .review-stars { color: var(--amber-light); font-size: 1rem; }
  .review-text { color: #4A2000; font-size: 0.92rem; line-height: 1.7; font-weight: 300; }
  .review-product-tag { display: inline-block; background: var(--cream-dark); color: var(--brown); font-size: 0.72rem; font-weight: 600; padding: 0.2rem 0.65rem; border-radius: 100px; margin-top: 0.75rem; }

  /* REVIEW FORM */
  .review-form-card { background: white; border-radius: 20px; padding: 2rem; border: 1.5px solid #FDE68A; max-width: 800px; margin: 2.5rem auto 0; box-shadow: 0 8px 30px rgba(180,83,9,0.1); }
  .review-form-card h3 { font-family: 'Playfair Display', serif; color: var(--brown-deep); font-size: 1.3rem; margin-bottom: 1.5rem; }
  .form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 1rem; margin-bottom: 1rem; }
  .form-group { display: flex; flex-direction: column; gap: 0.4rem; margin-bottom: 1rem; }
  .form-group label { font-size: 0.82rem; font-weight: 600; color: var(--brown); text-transform: uppercase; letter-spacing: 0.06em; }
  .form-group input, .form-group select, .form-group textarea {
    padding: 0.75rem 1rem; border: 1.5px solid #FDE68A; border-radius: 12px;
    font-family: 'Inter', sans-serif; font-size: 0.9rem; color: var(--text);
    background: var(--cream); outline: none; transition: border 0.2s;
  }
  .form-group input:focus, .form-group select:focus, .form-group textarea:focus { border-color: var(--amber); }
  .form-group textarea { min-height: 100px; resize: vertical; }
  .star-rating { display: flex; gap: 0.4rem; margin-top: 0.25rem; }
  .star-rating span { font-size: 1.8rem; cursor: pointer; color: #D1D5DB; transition: color 0.15s; }
  .star-rating span.active { color: var(--amber-light); }
  .submit-review-btn {
    width: 100%; background: var(--amber); color: white; border: none; cursor: pointer;
    padding: 1rem; border-radius: 100px; font-size: 1rem; font-weight: 700;
    font-family: 'Inter', sans-serif; transition: background 0.2s; margin-top: 0.5rem;
  }
  .submit-review-btn:hover { background: var(--brown); }
  .review-success { display: none; text-align: center; padding: 1.5rem; background: #DCFCE7; border-radius: 12px; color: var(--green); font-weight: 600; margin-top: 1rem; }

  /* RATING SUMMARY */
  .rating-summary { max-width: 800px; margin: 0 auto 2rem; background: white; border-radius: 20px; padding: 1.5rem 2rem; border: 1.5px solid #FDE68A; display: flex; align-items: center; gap: 2rem; flex-wrap: wrap; }
  .rating-big { text-align: center; }
  .rating-big .num { font-family: 'Playfair Display', serif; font-size: 3.5rem; font-weight: 900; color: var(--amber); line-height: 1; }
  .rating-big .stars { font-size: 1.2rem; color: var(--amber-light); }
  .rating-big .count { font-size: 0.8rem; color: #9CA3AF; margin-top: 0.25rem; }
  .rating-bars { flex: 1; display: flex; flex-direction: column; gap: 0.4rem; }
  .rating-bar-row { display: flex; align-items: center; gap: 0.75rem; font-size: 0.82rem; }
  .rating-bar-row span:first-child { width: 30px; color: var(--brown); font-weight: 600; }
  .bar-bg { flex: 1; height: 8px; background: var(--cream-dark); border-radius: 100px; overflow: hidden; }
  .bar-fill { height: 100%; background: var(--amber-light); border-radius: 100px; }
  .rating-bar-row span:last-child { width: 24px; color: #9CA3AF; font-size: 0.78rem; }

  .cart-overlay { visibility: hidden; opacity: 0; position: fixed; inset: 0; z-index: 200; background: rgba(0,0,0,0.5); pointer-events: none; }
  .cart-overlay.open { visibility: visible; opacity: 1; display: flex; justify-content: flex-end; pointer-events: all; }
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

  @media (max-width: 900px) {
    .hero-visual { display: none; }
    .why-grid { grid-template-columns: 1fr; gap: 2rem; }
    nav ul { display: none; }
    .media-preview-grid, .media-full-grid { grid-template-columns: 1fr; }
    .form-row { grid-template-columns: 1fr; }
    .rating-summary { flex-direction: column; }
  }
</style>
</head>
<body>

<!-- NAV -->
<nav>
  <div class="logo" onclick="showPage('home')">Tribe <span>Hive</span></div>
  <ul>
    <li><a onclick="showPage('home')">Home</a></li>
    <li><a onclick="showPage('home'); setTimeout(()=>document.getElementById('products').scrollIntoView({behavior:'smooth'}),100)">Shop</a></li>
    <li><a onclick="showPage('media')">Gallery</a></li>
    <li><a onclick="showPage('reviews')">Reviews</a></li>
  </ul>
  <button class="cart-btn" onclick="openCart()">🛒 Cart <span id="cart-count">0</span></button>
</nav>

<!-- ========== HOME PAGE ========== -->
<div class="page active" id="page-home">

  <section class="hero">
    <div class="hero-content">
      <div class="hero-badge">🍯 100% Pure & Natural · African Honey</div>
      <h1>Pure African Honey,<br>Straight from the <em>Source</em></h1>
      <p>Sourced directly from trusted Nigerian beekeepers. Every bottle is raw, unfiltered, and naturally rich — the real thing, nothing else.</p>
      <div class="hero-cta">
        <a onclick="showPage('home'); setTimeout(()=>document.getElementById('products').scrollIntoView({behavior:'smooth'}),100)" class="btn-primary" style="cursor:pointer">Shop Honey</a>
        <a onclick="showPage('home'); setTimeout(()=>document.getElementById('why').scrollIntoView({behavior:'smooth'}),100)" class="btn-outline" style="cursor:pointer">Our Promise</a>
      </div>
    </div>
    <div class="hero-visual">
      <img src="https://i.ibb.co/7JwHjr1F/file-00000000002871f48bbfde27c0381cac.png" onerror="this.style.display='none'" alt="Tribe Hive Honey">
    </div>
  </section>

  <div class="trust-bar">
    <div class="trust-item">✅ No Sugar Added</div>
    <div class="trust-item">🚚 Delivery Inclusive Nationwide</div>
    <div class="trust-item">🐝 Direct from Nigerian Beekeepers</div>
    <div class="trust-item">🌿 100% Pure & Natural</div>
  </div>

  <section class="products-section" id="products">
    <div class="products-header">
      <div class="section-label">Our Collection</div>
      <h2 class="section-title">Tribe Hive Honey</h2>
      <p>100% Pure & Natural — raw, unprocessed, freshly harvested. <strong>All prices include delivery anywhere in Nigeria.</strong></p>
    </div>
    <div class="honey-grid" id="product-grid"></div>
  </section>

  <!-- MEDIA PREVIEW -->
  <section class="media-preview">
    <div class="section-label">Photos & Videos</div>
    <h2 class="section-title">See Our Honey in Action</h2>
    <p style="color:#6B3B1A;font-weight:300;margin-top:0.5rem">Real photos, real quality — see Tribe Hive Honey for yourself.</p>
    <div class="media-preview-grid">
      <div class="media-thumb"><img src="https://i.ibb.co/gbDLMSJt/IMG-20260720-WA0011.jpg" alt="Tribe Hive Honey"></div>
      <div class="media-thumb"><img src="https://i.ibb.co/pvqTLbNP/file-00000000045881f4b5fd891a547fc512.png" alt="Tribe Hive Family"></div>
      <div class="media-thumb media-thumb-video">
        <span>▶</span>
        <span>Watch Video</span>
      </div>
    </div>
    <button class="view-media-btn" onclick="showPage('media')">📸 View Full Gallery & Videos →</button>
  </section>

  <!-- REVIEWS PREVIEW -->
  <section class="reviews-preview">
    <div class="section-label">Happy Customers</div>
    <h2 class="section-title">What People Are Saying</h2>
    <div class="reviews-mini-grid">
      <div class="review-mini-card">
        <div class="stars">★★★★★</div>
        <p>"This honey from Tribe Hive blew my mind — thick, dark, and incredibly aromatic. The genuine article!"</p>
        <div class="reviewer"><div class="avatar">👩🏾</div><div><div class="reviewer-name">Amaka O.</div><div class="reviewer-loc">Enugu, Nigeria</div></div></div>
      </div>
      <div class="review-mini-card">
        <div class="stars">★★★★★</div>
        <p>"Within weeks I noticed real improvement. Delivery was fast and there were no extra charges!"</p>
        <div class="reviewer"><div class="avatar">👨🏾</div><div><div class="reviewer-name">Emeka A.</div><div class="reviewer-loc">Anambra, Nigeria</div></div></div>
      </div>
      <div class="review-mini-card">
        <div class="stars">★★★★★</div>
        <p>"I ordered multiple bottles as gifts. Everyone loved it. You can taste the purity!"</p>
        <div class="reviewer"><div class="avatar">👩🏿</div><div><div class="reviewer-name">Fatima B.</div><div class="reviewer-loc">Abuja, Nigeria</div></div></div>
      </div>
    </div>
    <button class="view-reviews-btn" onclick="showPage('reviews')">⭐ Read All Reviews & Leave Yours →</button>
  </section>

  <!-- WHY US -->
  <section class="why-section" id="why">
    <div class="why-grid">
      <div class="why-text">
        <div class="section-label" style="color:var(--amber-glow)">Our Promise</div>
        <h2 class="section-title" style="color:var(--cream-dark)">We Don't Compromise<br>on Purity</h2>
        <p style="color:#D6B89A;font-weight:300;line-height:1.8;margin:1.25rem 0 2rem">Tribe Hive was born from frustration — too much fake honey in the market. We went to the source: trusted Nigerian beekeepers, delivering pure, uncut honey straight to your door.</p>
        <button class="btn-primary" onclick="showPage('home'); setTimeout(()=>document.getElementById('products').scrollIntoView({behavior:'smooth'}),100)">Shop Now</button>
      </div>
      <div class="why-items">
        <div class="why-item"><div class="why-icon">🐝</div><div><h4>Ethically Harvested</h4><p>We partner only with beekeepers who use sustainable practices and treat their bees well.</p></div></div>
        <div class="why-item"><div class="why-icon">🌿</div><div><h4>100% Natural</h4><p>No additives, no preservatives, no sugar. Just pure honey the way nature intended.</p></div></div>
        <div class="why-item"><div class="why-icon">🚚</div><div><h4>Delivery Inclusive</h4><p>All prices include delivery to anywhere in Nigeria. No hidden charges — ever.</p></div></div>
        <div class="why-item"><div class="why-icon">✅</div><div><h4>100% Satisfaction</h4><p>If your honey isn't authentic and delicious, we'll replace it or refund you. Full stop.</p></div></div>
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
        <p>Pick from 75cl, 1 Litre, or 1.5 Litres. All prices include delivery anywhere in Nigeria.</p>
      </div>
      <div class="step">
        <div class="step-num">2</div>
        <h4>Pay via Opay</h4>
        <p>Send payment to <strong>6572638060</strong><br>Chinyere Breath Ihegazie</p>
        <a class="opay-btn" href="https://opayweb.com" target="_blank">
          <img src="https://i.ibb.co/rSf9Gfm/a53b3bcfe00067e98812f7a247b67cfc.png" style="width:24px;height:24px;object-fit:contain;background:white;border-radius:50%;padding:2px;" alt="Opay">
          Pay with Opay
        </a>
        <div style="margin-top:0.75rem;background:#f0fff8;border:1px solid #00A859;border-radius:12px;padding:0.75rem;text-align:left;">
          <p style="font-size:0.78rem;font-weight:700;color:#00A859;margin-bottom:0.25rem">Opay Business Account:</p>
          <p style="font-size:0.85rem;font-weight:700;color:var(--brown-deep)">Account No: <strong>6572638060</strong></p>
          <p style="font-size:0.82rem;color:var(--brown-deep)">Name: <strong>Chinyere Breath Ihegazie</strong></p>
          <p style="font-size:0.78rem;color:#7C3B1E;margin-top:0.25rem">After payment, send receipt to WhatsApp for confirmation.</p>
        </div>
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

  <footer>
    <div class="logo" onclick="showPage('home')">Tribe <span style="color:var(--amber-light)">Hive</span></div>
    <p>Pure. Original. Nigerian.<br>
      <a href="https://wa.me/2347034529060" target="_blank" class="wa-footer">
        <svg width="16" height="16" viewBox="0 0 24 24" fill="#25D366"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/></svg>
        07034529060
      </a>
      &nbsp;|&nbsp; 📧 <a href="mailto:orders@tribehive.com.ng">orders@tribehive.com.ng</a>
      &nbsp;|&nbsp; 📍 Enugu State, Nigeria
    </p>
    <p style="margin-top:1rem;font-size:0.78rem;opacity:0.5;">© 2026 Tribe Hive. All rights reserved.</p>
  </footer>

</div><!-- END HOME PAGE -->

<!-- ========== MEDIA PAGE ========== -->
<div class="page" id="page-media">
  <section class="inner-page" style="background:var(--cream-dark)">
    <button class="back-btn" onclick="showPage('home')">← Back to Home</button>
    <div style="text-align:center">
      <div class="section-label">Our Gallery</div>
      <h2 class="section-title">Photos & Videos</h2>
      <p style="color:#6B3B1A;font-weight:300;margin-top:0.5rem;margin-bottom:0">Experience the purity and quality of Tribe Hive Honey.</p>
    </div>
    <div class="media-full-grid">
      <div class="media-card">
        <img src="https://i.ibb.co/gbDLMSJt/IMG-20260720-WA0011.jpg" alt="Tribe Hive Honey">
        <div class="media-card-body">
          <div class="media-card-title">🍯 Pure Tribe Hive Honey</div>
        </div>
      </div>
      <div class="media-card">
        <img src="https://i.ibb.co/pvqTLbNP/file-00000000045881f4b5fd891a547fc512.png" alt="Tribe Hive Family">
        <div class="media-card-body">
          <div class="media-card-title">🏡 Your Right Choice for Healthy Family</div>
        </div>
      </div>
      <div class="media-card">
        <iframe src="https://www.youtube.com/embed/0yXHVXmSsaQ" title="Tribe Hive Honey Video" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        <div class="media-card-body">
          <div class="media-card-title">▶ Watch Our Video</div>
          <a class="yt-btn" href="https://youtube.com/shorts/0yXHVXmSsaQ" target="_blank">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="white"><path d="M23.498 6.186a3.016 3.016 0 00-2.122-2.136C19.505 3.545 12 3.545 12 3.545s-7.505 0-9.377.505A3.017 3.017 0 00.502 6.186C0 8.07 0 12 0 12s0 3.93.502 5.814a3.016 3.016 0 002.122 2.136c1.871.505 9.376.505 9.376.505s7.505 0 9.377-.505a3.015 3.015 0 002.122-2.136C24 15.93 24 12 24 12s0-3.93-.502-5.814zM9.545 15.568V8.432L15.818 12l-6.273 3.568z"/></svg>
            Visit Our Channel
          </a>
        </div>
      </div>
    </div>
  </section>
</div><!-- END MEDIA PAGE -->

<!-- ========== REVIEWS PAGE ========== -->
<div class="page" id="page-reviews">
  <section class="reviews-page">
    <button class="back-btn" onclick="showPage('home')">← Back to Home</button>
    <div style="text-align:center;margin-bottom:2rem">
      <div class="section-label">Customer Reviews</div>
      <h2 class="section-title">What Our Customers Say</h2>
      <p style="color:#6B3B1A;font-weight:300;margin-top:0.5rem">Real reviews from real customers. Rate and share your experience!</p>
    </div>

    <!-- RATING SUMMARY -->
    <div class="rating-summary">
      <div class="rating-big">
        <div class="num" id="avg-rating">5.0</div>
        <div class="stars">★★★★★</div>
        <div class="count" id="review-count">3 reviews</div>
      </div>
      <div class="rating-bars">
        <div class="rating-bar-row"><span>5★</span><div class="bar-bg"><div class="bar-fill" style="width:100%"></div></div><span>3</span></div>
        <div class="rating-bar-row"><span>4★</span><div class="bar-bg"><div class="bar-fill" style="width:0%"></div></div><span>0</span></div>
        <div class="rating-bar-row"><span>3★</span><div class="bar-bg"><div class="bar-fill" style="width:0%"></div></div><span>0</span></div>
        <div class="rating-bar-row"><span>2★</span><div class="bar-bg"><div class="bar-fill" style="width:0%"></div></div><span>0</span></div>
        <div class="rating-bar-row"><span>1★</span><div class="bar-bg"><div class="bar-fill" style="width:0%"></div></div><span>0</span></div>
      </div>
    </div>

    <!-- EXISTING REVIEWS -->
    <div class="reviews-list" id="reviews-list">
      <div class="review-card">
        <div class="review-card-header">
          <div class="reviewer-info"><div class="reviewer-avatar">AO</div><div class="reviewer-details"><div class="name">Amaka O.</div><div class="date">Enugu, Nigeria</div></div></div>
          <div class="review-stars">★★★★★</div>
        </div>
        <div class="review-text">"I have been searching for real honey for years. This honey from Tribe Hive blew my mind — thick, dark, and incredibly aromatic. This is the genuine article."</div>
        <span class="review-product-tag">🍯 Tribe Hive Honey — 1 Litre</span>
      </div>
      <div class="review-card">
        <div class="review-card-header">
          <div class="reviewer-info"><div class="reviewer-avatar">EA</div><div class="reviewer-details"><div class="name">Emeka A.</div><div class="date">Anambra, Nigeria</div></div></div>
          <div class="review-stars">★★★★★</div>
        </div>
        <div class="review-text">"My doctor recommended raw honey. I tried Tribe Hive — within weeks I noticed real improvement. Delivery was fast and there were no extra charges!"</div>
        <span class="review-product-tag">🍯 Tribe Hive Honey — 75cl</span>
      </div>
      <div class="review-card">
        <div class="review-card-header">
          <div class="reviewer-info"><div class="reviewer-avatar">FB</div><div class="reviewer-details"><div class="name">Fatima B.</div><div class="date">Abuja, Nigeria</div></div></div>
          <div class="review-stars">★★★★★</div>
        </div>
        <div class="review-text">"I ordered multiple bottles as gifts. Everyone loved it and several have reordered. You can taste the purity — absolutely wonderful honey."</div>
        <span class="review-product-tag">🍯 Tribe Hive Honey — 1.5 Litres</span>
      </div>
    </div>

    <!-- REVIEW FORM -->
    <div class="review-form-card">
      <h3>✍ Leave Your Review</h3>
      <div class="form-row">
        <div class="form-group">
          <label>Your Name</label>
          <input type="text" id="r-name" placeholder="e.g. Chidi Okafor">
        </div>
        <div class="form-group">
          <label>Your Location</label>
          <input type="text" id="r-loc" placeholder="e.g. Lagos, Nigeria">
        </div>
      </div>
      <div class="form-group">
        <label>Product Purchased</label>
        <select id="r-product">
          <option value="Tribe Hive Honey — 75cl">Tribe Hive Honey — 75cl</option>
          <option value="Tribe Hive Honey — 1 Litre" selected>Tribe Hive Honey — 1 Litre</option>
          <option value="Tribe Hive Honey — 1.5 Litres">Tribe Hive Honey — 1.5 Litres</option>
        </select>
      </div>
      <div class="form-group">
        <label>Your Rating</label>
        <div class="star-rating" id="star-rating">
          <span onclick="setRating(1)">★</span>
          <span onclick="setRating(2)">★</span>
          <span onclick="setRating(3)">★</span>
          <span onclick="setRating(4)">★</span>
          <span onclick="setRating(5)">★</span>
        </div>
      </div>
      <div class="form-group">
        <label>Your Review</label>
        <textarea id="r-text" placeholder="Tell others about your experience with Tribe Hive Honey..."></textarea>
      </div>
      <button class="submit-review-btn" onclick="submitReview()">Submit Review ⭐</button>
      <div class="review-success" id="review-success">🎉 Thank you! Your review has been submitted successfully!</div>
    </div>
  </section>
</div><!-- END REVIEWS PAGE -->

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
  // PAGE NAVIGATION
  function showPage(page) {
    document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
    document.getElementById('page-' + page).classList.add('active');
    window.scrollTo(0, 0);
  }

  // PRODUCTS
  const products = [
    { id:1, name:"Tribe Hive Honey", size:"75cl", tag:"Starter Size", emoji:"🍯",
      bg:"linear-gradient(135deg,#D97706 0%,#B45309 60%,#92400E 100%)",
      desc:"Perfect starter size. Raw, unfiltered African honey from trusted Nigerian beekeepers. Rich, thick and naturally sweet.", price:16000, stars:5 },
    { id:2, name:"Tribe Hive Honey", size:"1 Litre", tag:"Most Popular", emoji:"🍯",
      bg:"linear-gradient(135deg,#F59E0B 0%,#B45309 60%,#78350F 100%)",
      desc:"Our best-selling size. Pure African honey for daily use — for health, cooking, or as a natural sweetener.", price:23000, stars:5 },
    { id:3, name:"Tribe Hive Honey", size:"1.5 Litres", tag:"Best Value", emoji:"🍯",
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

  // CART
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
    const msg = `Hello Tribe Hive! I'd like to order:\n\n${items}\n\nTotal: ₦${total.toLocaleString()} (Delivery Inclusive)\n\nI will send my payment receipt after paying via Opay to 6572638060 (Chinyere Breath Ihegazie).\n\nMy delivery address: `;
    window.open(`https://wa.me/2347034529060?text=${encodeURIComponent(msg)}`, '_blank');
  }

  // REVIEWS
  let selectedRating = 0;
  let userReviews = [];

  function setRating(n) {
    selectedRating = n;
    document.querySelectorAll('#star-rating span').forEach((s, i) => {
      s.classList.toggle('active', i < n);
    });
  }

  function submitReview() {
    const name = document.getElementById('r-name').value.trim();
    const loc = document.getElementById('r-loc').value.trim();
    const product = document.getElementById('r-product').value;
    const text = document.getElementById('r-text').value.trim();
    if (!name || !text || !selectedRating) {
      alert('Please fill in your name, review, and select a rating!');
      return;
    }
    const initials = name.split(' ').map(w => w[0]).join('').toUpperCase().slice(0,2);
    const review = { name, loc: loc || 'Nigeria', product, text, rating: selectedRating, initials };
    userReviews.unshift(review);
    renderNewReview(review);
    document.getElementById('r-name').value = '';
    document.getElementById('r-loc').value = '';
    document.getElementById('r-text').value = '';
    selectedRating = 0;
    document.querySelectorAll('#star-rating span').forEach(s => s.classList.remove('active'));
    const success = document.getElementById('review-success');
    success.style.display = 'block';
    setTimeout(() => success.style.display = 'none', 4000);
  }

  function renderNewReview(r) {
    const stars = '★'.repeat(r.rating) + '☆'.repeat(5 - r.rating);
    const card = document.createElement('div');
    card.className = 'review-card';
    card.style.border = '2px solid var(--amber-light)';
    card.innerHTML = `
      <div class="review-card-header">
        <div class="reviewer-info"><div class="reviewer-avatar" style="background:var(--amber-glow)">${r.initials}</div><div class="reviewer-details"><div class="name">${r.name}</div><div class="date">${r.loc}</div></div></div>
        <div class="review-stars" style="color:var(--amber-light)">${stars}</div>
      </div>
      <div class="review-text">"${r.text}"</div>
      <span class="review-product-tag">🍯 ${r.product}</span>`;
    const list = document.getElementById('reviews-list');
    list.insertBefore(card, list.firstChild);
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
