
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
  <li><a onclick="showPage('blog')">Blog & FAQ</a></li>
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
    <div class="reviews-mini-grid" id="home-reviews-grid">
      <div style="grid-column:1/-1;text-align:center;color:#9CA3AF;padding:2rem;font-size:0.95rem;">
        <div style="font-size:2rem;margin-bottom:0.5rem">🍯</div>
        No reviews yet — be the first to share your experience!
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

    <!-- REVIEWS LIST -->
    <div class="reviews-list" id="reviews-list">
      <div style="text-align:center;color:#9CA3AF;padding:2rem;font-size:0.95rem;" id="no-reviews-msg">
        <div style="font-size:2.5rem;margin-bottom:0.75rem">🍯</div>
        No reviews yet. Be the first to share your experience!
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

<!-- ========== BLOG & FAQ PAGE ========== -->
<div class="page" id="page-blog">
<style>
  .blog-page { padding: 100px 6vw 5rem; min-height: 100vh; background: var(--cream); }
  .blog-hero { background: linear-gradient(135deg, var(--brown-deep), var(--brown)); padding: 3rem 2rem; border-radius: 20px; text-align: center; margin-bottom: 3rem; }
  .blog-hero h1 { font-family: 'Playfair Display', serif; color: var(--amber-glow); font-size: clamp(1.8rem,4vw,2.8rem); margin-bottom: 0.75rem; }
  .blog-hero p { color: #D6B89A; font-weight: 300; font-size: 1rem; }
  .blog-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 2rem; max-width: 1000px; margin: 0 auto 4rem; }
  .blog-card { background: white; border-radius: 20px; overflow: hidden; border: 1.5px solid #FDE68A; box-shadow: 0 8px 30px rgba(180,83,9,0.08); transition: transform 0.25s, box-shadow 0.25s; }
  .blog-card:hover { transform: translateY(-4px); box-shadow: 0 20px 50px rgba(180,83,9,0.15); }
  .blog-card-img { width: 100%; height: 160px; display: flex; align-items: center; justify-content: center; font-size: 4rem; }
  .blog-card-body { padding: 1.25rem; }
  .blog-tag { font-size: 0.7rem; font-weight: 700; text-transform: uppercase; letter-spacing: 0.1em; color: var(--amber); margin-bottom: 0.4rem; }
  .blog-card-title { font-family: 'Playfair Display', serif; font-size: 1.1rem; font-weight: 700; color: var(--brown-deep); margin-bottom: 0.6rem; line-height: 1.3; }
  .blog-card-excerpt { font-size: 0.85rem; color: #7C3B1E; font-weight: 300; line-height: 1.6; margin-bottom: 1rem; }
  .read-more-btn { font-size: 0.82rem; font-weight: 700; color: var(--amber); cursor: pointer; background: none; border: none; font-family: 'Inter', sans-serif; padding: 0; transition: color 0.2s; }
  .read-more-btn:hover { color: var(--brown); }

  /* FULL ARTICLE */
  .article-view { display: none; max-width: 800px; margin: 0 auto; }
  .article-view.show { display: block; }
  .blog-grid-view { display: block; }
  .blog-grid-view.hide { display: none; }
  .article-back { display: inline-flex; align-items: center; gap: 0.5rem; background: var(--cream-dark); color: var(--brown); padding: 0.5rem 1.25rem; border-radius: 100px; font-size: 0.85rem; font-weight: 600; border: 1px solid #FDE68A; cursor: pointer; margin-bottom: 2rem; transition: all 0.2s; font-family: 'Inter', sans-serif; }
  .article-back:hover { background: var(--amber); color: white; }
  .article-header { margin-bottom: 2rem; }
  .article-header h1 { font-family: 'Playfair Display', serif; font-size: clamp(1.6rem,4vw,2.2rem); color: var(--brown-deep); margin-bottom: 0.75rem; line-height: 1.2; }
  .article-meta { font-size: 0.82rem; color: #9CA3AF; margin-bottom: 1rem; }
  .article-body { color: #4A2000; font-weight: 300; line-height: 1.9; font-size: 0.95rem; }
  .article-body h2 { font-family: 'Playfair Display', serif; color: var(--brown-deep); font-size: 1.3rem; margin: 2rem 0 0.75rem; }
  .article-body h3 { font-family: 'Playfair Display', serif; color: var(--amber); font-size: 1.1rem; margin: 1.5rem 0 0.5rem; }
  .article-body p { margin-bottom: 1rem; }
  .article-body ul { margin: 0.75rem 0 1rem 1.5rem; }
  .article-body ul li { margin-bottom: 0.4rem; }
  .article-body .highlight { background: var(--cream-dark); border-left: 4px solid var(--amber); padding: 1rem 1.25rem; border-radius: 0 12px 12px 0; margin: 1.5rem 0; font-style: italic; }
  .article-cta { background: linear-gradient(135deg, var(--brown-deep), var(--brown)); border-radius: 16px; padding: 1.75rem; text-align: center; margin-top: 2.5rem; }
  .article-cta h3 { font-family: 'Playfair Display', serif; color: var(--amber-glow); margin-bottom: 0.5rem; }
  .article-cta p { color: #D6B89A; font-size: 0.9rem; margin-bottom: 1rem; font-weight: 300; }

  /* FAQ */
  .faq-section { max-width: 800px; margin: 0 auto; }
  .faq-section h2 { font-family: 'Playfair Display', serif; font-size: clamp(1.6rem,3vw,2rem); color: var(--brown-deep); text-align: center; margin-bottom: 2rem; }
  .faq-item { background: white; border-radius: 16px; border: 1.5px solid #FDE68A; margin-bottom: 1rem; overflow: hidden; }
  .faq-question { padding: 1.25rem 1.5rem; display: flex; justify-content: space-between; align-items: center; cursor: pointer; font-weight: 600; color: var(--brown-deep); font-size: 0.95rem; transition: background 0.2s; }
  .faq-question:hover { background: var(--cream-dark); }
  .faq-icon { font-size: 1.2rem; color: var(--amber); transition: transform 0.3s; flex-shrink: 0; margin-left: 1rem; }
  .faq-icon.open { transform: rotate(45deg); }
  .faq-answer { display: none; padding: 0 1.5rem 1.25rem; color: #7C3B1E; font-weight: 300; line-height: 1.8; font-size: 0.9rem; }
  .faq-answer.open { display: block; }

  @media (max-width: 768px) { .blog-grid { grid-template-columns: 1fr; } }
</style>

<section class="blog-page">
  <button class="back-btn" onclick="showPage('home')">← Back to Home</button>

  <!-- BLOG GRID VIEW -->
  <div class="blog-grid-view" id="blog-grid-view">
    <div class="blog-hero">
      <h1>🍯 Honey Knowledge Hub</h1>
      <p>Everything you need to know about pure African honey — health benefits, tips, and more.</p>
    </div>

    <div style="text-align:center;margin-bottom:2rem">
      <div class="section-label">Our Blog</div>
      <h2 class="section-title">Latest Articles</h2>
    </div>

    <div class="blog-grid">
      <div class="blog-card">
        <div class="blog-card-img" style="background:linear-gradient(135deg,#FDE68A,#F59E0B)">🍯</div>
        <div class="blog-card-body">
          <div class="blog-tag">Health & Wellness</div>
          <div class="blog-card-title">10 Proven Health Benefits of Raw African Honey</div>
          <div class="blog-card-excerpt">Raw African honey is more than a sweetener — it's a powerful natural remedy used for centuries. Discover the top 10 science-backed benefits...</div>
          <button class="read-more-btn" onclick="showArticle('article1')">Read More →</button>
        </div>
      </div>
      <div class="blog-card">
        <div class="blog-card-img" style="background:linear-gradient(135deg,#D97706,#92400E)">🌿</div>
        <div class="blog-card-body">
          <div class="blog-tag">Nutrition</div>
          <div class="blog-card-title">Raw Honey vs Processed Honey: What's the Difference?</div>
          <div class="blog-card-excerpt">Not all honey is created equal. Learn why raw, unfiltered African honey is far superior to the processed honey sold in supermarkets...</div>
          <button class="read-more-btn" onclick="showArticle('article2')">Read More →</button>
        </div>
      </div>
      <div class="blog-card">
        <div class="blog-card-img" style="background:linear-gradient(135deg,#166534,#14532D)">💊</div>
        <div class="blog-card-body">
          <div class="blog-tag">Natural Remedies</div>
          <div class="blog-card-title">How to Use Honey as a Natural Medicine at Home</div>
          <div class="blog-card-excerpt">From sore throats to skin care, honey has incredible medicinal properties. Here are practical ways to use raw honey as medicine...</div>
          <button class="read-more-btn" onclick="showArticle('article3')">Read More →</button>
        </div>
      </div>
      <div class="blog-card">
        <div class="blog-card-img" style="background:linear-gradient(135deg,#B45309,#451A03)">🇳🇬</div>
        <div class="blog-card-body">
          <div class="blog-tag">African Honey</div>
          <div class="blog-card-title">Why Nigerian Honey is Among the Best in the World</div>
          <div class="blog-card-excerpt">Nigeria's diverse flora gives its honey a unique richness and potency. Discover what makes Nigerian beekeeping special and why our honey stands out...</div>
          <button class="read-more-btn" onclick="showArticle('article4')">Read More →</button>
        </div>
      </div>
    </div>

    <!-- FAQ SECTION -->
    <div class="faq-section">
      <div style="text-align:center;margin-bottom:0.5rem"><div class="section-label">Got Questions?</div></div>
      <h2>Frequently Asked Questions</h2>

      <div class="faq-item">
        <div class="faq-question" onclick="toggleFaq(this)">Is Tribe Hive Honey 100% pure and natural? <span class="faq-icon">+</span></div>
        <div class="faq-answer">Yes! Tribe Hive Honey is 100% pure, raw, and unfiltered. We source directly from trusted Nigerian beekeepers and do not add any sugar, preservatives, or artificial ingredients. What you get is exactly what the bees made — nothing more, nothing less.</div>
      </div>
      <div class="faq-item">
        <div class="faq-question" onclick="toggleFaq(this)">Why does my honey look dark or crystallized? <span class="faq-icon">+</span></div>
        <div class="faq-answer">Dark color and crystallization are actually signs of REAL, high-quality raw honey! Crystallization happens naturally when glucose in the honey separates — it does NOT mean the honey has gone bad. To return it to liquid form, simply place the bottle in warm water for a few minutes. Never microwave honey as this destroys its nutrients.</div>
      </div>
      <div class="faq-item">
        <div class="faq-question" onclick="toggleFaq(this)">How long does Tribe Hive Honey last? <span class="faq-icon">+</span></div>
        <div class="faq-answer">Pure raw honey never expires! Archaeologists have found honey in ancient Egyptian tombs that was still perfectly edible after thousands of years. Tribe Hive Honey, when stored properly in a cool, dry place with the lid tightly sealed, will last indefinitely. Always use a clean, dry spoon to avoid introducing moisture.</div>
      </div>
      <div class="faq-item">
        <div class="faq-question" onclick="toggleFaq(this)">Do you deliver to my state in Nigeria? <span class="faq-icon">+</span></div>
        <div class="faq-answer">Yes! We deliver to ALL states across Nigeria. Delivery is already included in the price — there are no hidden charges. For Enugu State, delivery is faster (usually same day or next day). For other states, delivery typically takes 2–4 business days via our trusted courier partners.</div>
      </div>
      <div class="faq-item">
        <div class="faq-question" onclick="toggleFaq(this)">Can babies eat Tribe Hive Honey? <span class="faq-icon">+</span></div>
        <div class="faq-answer">Honey should NOT be given to babies under 12 months of age. This is because raw honey can contain Clostridium botulinum spores which, while harmless to older children and adults, can cause infant botulism in babies under one year. For children above 12 months and adults, Tribe Hive Honey is completely safe and very beneficial.</div>
      </div>
      <div class="faq-item">
        <div class="faq-question" onclick="toggleFaq(this)">How do I pay for my order? <span class="faq-icon">+</span></div>
        <div class="faq-answer">We accept payment via Opay. Simply send payment to our Opay business account number 6572638060 (Chinyere Breath Ihegazie), then send your payment receipt and delivery address to our WhatsApp number 07034529060 for order confirmation and dispatch.</div>
      </div>
      <div class="faq-item">
        <div class="faq-question" onclick="toggleFaq(this)">What are the health benefits of raw honey? <span class="faq-icon">+</span></div>
        <div class="faq-answer">Raw honey has numerous health benefits including: boosting immunity, soothing sore throats and coughs, aiding digestion, promoting wound healing, improving sleep, providing natural energy, supporting heart health, acting as an antioxidant, helping with ulcers, and nourishing the skin. It contains vitamins, minerals, enzymes, and antioxidants that are destroyed in processed honey.</div>
      </div>
      <div class="faq-item">
        <div class="faq-question" onclick="toggleFaq(this)">How should I store my honey? <span class="faq-icon">+</span></div>
        <div class="faq-answer">Store your Tribe Hive Honey at room temperature, away from direct sunlight and heat. Keep the lid tightly closed and always use a clean, dry spoon. Do not refrigerate honey as this speeds up crystallization. Avoid storing near the stove or in hot areas. A kitchen cupboard or pantry is ideal.</div>
      </div>
    </div>
  </div>

  <!-- ARTICLE VIEWS -->
  <div class="article-view" id="article1">
    <button class="article-back" onclick="showBlogGrid()">← Back to Blog</button>
    <div class="article-header">
      <div class="blog-tag">Health & Wellness</div>
      <h1>10 Proven Health Benefits of Raw African Honey</h1>
      <div class="article-meta">By Tribe Hive · Natural Health · 5 min read</div>
    </div>
    <div class="article-body">
      <p>Raw African honey has been used as food and medicine for thousands of years. Unlike processed honey found in supermarkets, raw honey retains all its natural enzymes, antioxidants, vitamins, and minerals — making it one of nature's most powerful superfoods.</p>
      <div class="highlight">"Let food be thy medicine and medicine be thy food." — Hippocrates, who frequently used honey in his treatments.</div>
      <h2>1. Boosts Your Immune System</h2>
      <p>Raw honey is rich in antioxidants including phenolic acids and flavonoids. These compounds help protect your body against free radicals and strengthen your immune system. Regular consumption of raw honey has been linked to fewer colds, flu, and infections.</p>
      <h2>2. Soothes Sore Throats and Coughs</h2>
      <p>Raw honey is one of the most effective natural remedies for sore throats and coughs. Its thick consistency coats the throat, while its antimicrobial properties fight infection. A tablespoon of raw honey with warm water and lemon is a time-tested remedy used across Nigeria and Africa.</p>
      <h2>3. Heals Wounds and Burns</h2>
      <p>Honey has powerful antibacterial properties. When applied to wounds, cuts, or burns, it creates a moist healing environment, prevents bacterial growth, and reduces inflammation. Medical-grade honey (Manuka) is even used in hospitals worldwide.</p>
      <h2>4. Aids Digestion</h2>
      <p>The enzymes in raw honey help break down food and improve digestion. It is particularly effective against H. pylori bacteria, which causes stomach ulcers. Many Nigerians take a spoonful of raw honey first thing in the morning to support their digestive health.</p>
      <h2>5. Provides Natural Energy</h2>
      <p>Honey contains natural sugars — glucose and fructose — that are easily absorbed by the body, providing a quick and sustained energy boost. It is an excellent pre-workout food and is used by athletes worldwide as a natural energy source.</p>
      <h2>6. Improves Sleep Quality</h2>
      <p>Taking a tablespoon of raw honey before bed helps stimulate the release of melatonin in the brain — the hormone responsible for sleep. It also helps replenish liver glycogen, preventing the brain from triggering stress hormones that can wake you up at night.</p>
      <h2>7. Supports Heart Health</h2>
      <p>Studies have shown that antioxidants in raw honey may help lower blood pressure, improve cholesterol levels, regulate heartbeat, and prevent cell death in the heart. Regular consumption as part of a balanced diet supports overall cardiovascular health.</p>
      <h2>8. Natural Skin Care</h2>
      <p>Honey's antimicrobial and moisturizing properties make it excellent for skin care. It can be used as a face mask to treat acne, dry skin, and eczema. Many people apply raw honey directly to their skin for a natural glow.</p>
      <h2>9. Rich in Antioxidants</h2>
      <p>Raw honey contains a wide range of antioxidants — organic acids and phenolic compounds like flavonoids. These antioxidants have been linked to reduced risk of heart attacks, strokes, and certain types of cancer.</p>
      <h2>10. Helps Manage Ulcers</h2>
      <p>One of the most celebrated uses of raw honey in Nigeria is for managing stomach and peptic ulcers. The antibacterial properties of raw honey inhibit the growth of H. pylori — the main cause of stomach ulcers — and help soothe the stomach lining.</p>
      <div class="highlight">Important: While honey has many health benefits, it is not a substitute for medical treatment. Always consult your doctor for serious health conditions.</div>
      <div class="article-cta">
        <h3>🍯 Get Pure Raw Honey Today</h3>
        <p>Experience all these benefits with Tribe Hive Honey — 100% pure, raw, and delivered to your door.</p>
        <button class="btn-primary" onclick="showPage('home'); setTimeout(()=>document.getElementById('products').scrollIntoView({behavior:'smooth'}),100)">Shop Now →</button>
      </div>
    </div>
  </div>

  <div class="article-view" id="article2">
    <button class="article-back" onclick="showBlogGrid()">← Back to Blog</button>
    <div class="article-header">
      <div class="blog-tag">Nutrition</div>
      <h1>Raw Honey vs Processed Honey: What's the Difference?</h1>
      <div class="article-meta">By Tribe Hive · Nutrition · 4 min read</div>
    </div>
    <div class="article-body">
      <p>Walk into any supermarket in Nigeria and you'll find shelves full of honey. But is all honey the same? Absolutely not. The difference between raw honey and processed honey is enormous — and it matters for your health.</p>
      <h2>What is Raw Honey?</h2>
      <p>Raw honey is honey exactly as it exists in the beehive. It is extracted from the hive, strained to remove large particles like beeswax and dead bees, and bottled — nothing else added or removed. Tribe Hive Honey is raw honey.</p>
      <h2>What is Processed Honey?</h2>
      <p>Processed honey goes through pasteurization — it is heated to high temperatures (around 70°C or higher) to destroy yeast, improve appearance, and extend shelf life. It also goes through ultrafiltration which removes pollen, propolis, and other beneficial particles.</p>
      <h2>Key Differences</h2>
      <h3>🔬 Nutrients</h3>
      <p>Raw honey retains all its natural enzymes, vitamins, minerals, antioxidants, and pollen. Processing destroys most of these — studies show that heating honey destroys up to 50% of its antioxidants and all of its enzymes.</p>
      <h3>🌸 Pollen Content</h3>
      <p>Raw honey contains natural pollen which has been linked to allergy relief, anti-inflammatory effects, and liver protection. Processed honey has virtually zero pollen — which also makes it impossible to trace its geographic origin.</p>
      <h3>🎨 Appearance</h3>
      <p>Raw honey is typically darker, cloudier, and may crystallize over time. Processed honey is clear, golden, and stays liquid for longer — but this comes at the cost of its nutritional value.</p>
      <h3>⚠️ Adulteration</h3>
      <p>Much of the "honey" sold in Nigerian markets is adulterated with sugar syrup, water, or artificial flavors. True raw honey like Tribe Hive is never mixed with anything — what you buy is pure, traceable honey from Nigerian beekeepers.</p>
      <div class="highlight">A simple test: place a drop of honey on your thumb. If it spreads immediately, it may be diluted. Pure raw honey stays in place and is thick and sticky.</div>
      <div class="article-cta">
        <h3>🍯 Choose Real Honey</h3>
        <p>Tribe Hive Honey is 100% raw, pure, and unprocessed — sourced directly from trusted Nigerian beekeepers.</p>
        <button class="btn-primary" onclick="showPage('home'); setTimeout(()=>document.getElementById('products').scrollIntoView({behavior:'smooth'}),100)">Shop Now →</button>
      </div>
    </div>
  </div>

  <div class="article-view" id="article3">
    <button class="article-back" onclick="showBlogGrid()">← Back to Blog</button>
    <div class="article-header">
      <div class="blog-tag">Natural Remedies</div>
      <h1>How to Use Honey as a Natural Medicine at Home</h1>
      <div class="article-meta">By Tribe Hive · Natural Remedies · 5 min read</div>
    </div>
    <div class="article-body">
      <p>For thousands of years, honey has been one of humanity's most trusted medicines. Ancient Egyptians, Greeks, and traditional African healers all used honey to treat a wide range of conditions. Here are practical ways you can use Tribe Hive raw honey at home.</p>
      <h2>For Sore Throat and Cough</h2>
      <p>Mix 1–2 tablespoons of raw honey with the juice of half a lemon in a cup of warm (not boiling) water. Drink slowly 2–3 times a day. The honey coats and soothes the throat while fighting infection, and the lemon provides vitamin C to boost immunity.</p>
      <h2>For Stomach Ulcers</h2>
      <p>Take 1 tablespoon of raw honey on an empty stomach first thing in the morning, 30 minutes before breakfast. Do this consistently for several weeks. Many Nigerians have reported significant improvement in ulcer symptoms using this method.</p>
      <h2>For Wounds and Cuts</h2>
      <p>Clean the wound with clean water, then apply a thin layer of raw honey directly to the wound. Cover with a clean bandage. Change the dressing daily. Honey's antibacterial properties prevent infection and its moisturizing effect promotes faster healing.</p>
      <h2>For Better Sleep</h2>
      <p>Take 1 tablespoon of raw honey in warm milk or warm water about 30 minutes before bed. This helps the brain release melatonin and promotes deeper, more restful sleep.</p>
      <h2>For Energy Before Exercise</h2>
      <p>Take 1–2 tablespoons of raw honey about 30 minutes before exercise. The natural glucose and fructose provide immediate and sustained energy without the crash that comes from processed sugar or energy drinks.</p>
      <h2>For Skin Care</h2>
      <ul>
        <li><strong>Face mask:</strong> Apply raw honey to clean face, leave for 15–20 minutes, rinse with warm water</li>
        <li><strong>Acne treatment:</strong> Apply a small amount of honey directly to pimples overnight</li>
        <li><strong>Moisturizer:</strong> Mix honey with a few drops of coconut oil for a natural body moisturizer</li>
        <li><strong>Lip balm:</strong> Apply a tiny amount of honey to dry, chapped lips</li>
      </ul>
      <h2>For Immunity Boost</h2>
      <p>Make a daily immunity tonic: mix 1 tablespoon raw honey + 1 teaspoon ginger juice + 1 teaspoon lemon juice + a pinch of turmeric in warm water. Drink every morning. This powerful combination supports your immune system, reduces inflammation, and improves overall health.</p>
      <div class="highlight">Always use raw, unprocessed honey for medicinal purposes. Processed honey has been stripped of the enzymes and antioxidants that give honey its healing properties.</div>
      <div class="article-cta">
        <h3>🍯 Get Your Tribe Hive Honey</h3>
        <p>Pure, raw, and ready to heal. Order today with delivery inclusive to anywhere in Nigeria.</p>
        <button class="btn-primary" onclick="showPage('home'); setTimeout(()=>document.getElementById('products').scrollIntoView({behavior:'smooth'}),100)">Shop Now →</button>
      </div>
    </div>
  </div>

  <div class="article-view" id="article4">
    <button class="article-back" onclick="showBlogGrid()">← Back to Blog</button>
    <div class="article-header">
      <div class="blog-tag">African Honey</div>
      <h1>Why Nigerian Honey is Among the Best in the World</h1>
      <div class="article-meta">By Tribe Hive · African Honey · 4 min read</div>
    </div>
    <div class="article-body">
      <p>Nigeria is one of Africa's leading honey producers, and for good reason. The country's rich and diverse vegetation — from the savannah of the north to the rainforests of the south — provides bees with an extraordinary variety of nectar sources, resulting in honey that is uniquely rich, complex, and potent.</p>
      <h2>Nigeria's Rich Floral Diversity</h2>
      <p>Nigerian honey bees have access to thousands of plant species across the country's diverse ecological zones. From shea trees in the north to mangrove forests in the south, the variety of nectar sources gives Nigerian honey a distinctive flavor profile and exceptional nutritional richness that is hard to match.</p>
      <h2>African Honey Bees Are Special</h2>
      <p>African honey bees (Apis mellifera scutellata) are known to be more industrious and produce honey with higher concentrations of beneficial compounds compared to European honey bee species. Nigerian beekeepers work with these native bees, resulting in honey that is naturally more potent.</p>
      <h2>Minimal Processing</h2>
      <p>Traditional Nigerian beekeeping methods involve minimal interference with the honey. Unlike industrial honey production in some countries that involves excessive heating and filtering, Nigerian raw honey is typically extracted and bottled with minimal processing, preserving its natural goodness.</p>
      <h2>Rich Dark Color = High Antioxidants</h2>
      <p>You may notice that Tribe Hive Honey is darker than the light golden honey you see in some stores. This dark color is a sign of high antioxidant content. Studies consistently show that darker honeys contain more polyphenols and antioxidants than lighter varieties.</p>
      <h2>Tribe Hive — Bringing Nigerian Honey to Your Door</h2>
      <p>At Tribe Hive, we work directly with trusted Nigerian beekeepers to bring you the finest raw African honey. Our honey is harvested sustainably, bottled with care, and delivered fresh to your doorstep anywhere in Nigeria — with delivery already included in the price.</p>
      <div class="highlight">When you buy Tribe Hive Honey, you are not just buying honey — you are supporting Nigerian beekeepers and choosing a healthier, more natural lifestyle.</div>
      <div class="article-cta">
        <h3>🍯 Taste the Difference</h3>
        <p>Order your Tribe Hive Honey today. Pure Nigerian honey, delivered to your door.</p>
        <button class="btn-primary" onclick="showPage('home'); setTimeout(()=>document.getElementById('products').scrollIntoView({behavior:'smooth'}),100)">Shop Now →</button>
      </div>
    </div>
  </div>

</section>
</div><!-- END BLOG PAGE -->

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
  // BLOG
  function showArticle(id) {
    document.getElementById('blog-grid-view').classList.add('hide');
    document.querySelectorAll('.article-view').forEach(a => a.classList.remove('show'));
    document.getElementById(id).classList.add('show');
    window.scrollTo(0,0);
  }
  function showBlogGrid() {
    document.getElementById('blog-grid-view').classList.remove('hide');
    document.querySelectorAll('.article-view').forEach(a => a.classList.remove('show'));
    window.scrollTo(0,0);
  }
  function toggleFaq(el) {
    const answer = el.nextElementSibling;
    const icon = el.querySelector('.faq-icon');
    answer.classList.toggle('open');
    icon.classList.toggle('open');
  }

  // PAGE NAV
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

  // SUPABASE CONFIG
  const SUPABASE_URL = 'https://bjxweknvekkmqzixwgns.supabase.co';
  const SUPABASE_KEY = 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6ImJqeHdla252ZWtrbXF6aXh3Z25zIiwicm9sZSI6ImFub24iLCJpYXQiOjE3OTE4NTIxOTAsImV4cCI6MjEwNzQyODE5MH0.44jqR3vA935r5jGru-Sx0K3nn7U31KtAco0wE2IyFfo';

  async function dbFetch(path, options = {}) {
    const res = await fetch(`${SUPABASE_URL}/rest/v1/${path}`, {
      headers: {
        'apikey': SUPABASE_KEY,
        'Authorization': `Bearer ${SUPABASE_KEY}`,
        'Content-Type': 'application/json',
        'Prefer': options.prefer || ''
      },
      ...options
    });
    if (!res.ok) throw new Error(await res.text());
    return options.method === 'POST' ? res : res.json();
  }  let userReviews = [];

  async function loadReviews() {
    try {
      const data = await dbFetch('reviews?order=created_at.desc');
      userReviews = data;
    } catch(e) {
      console.log('Error loading reviews:', e);
      userReviews = [];
    }
    renderAllReviews();
    updateRatingSummary();
    renderHomeReviews();
  }

  async function saveReviews(review) {
    try {
      await dbFetch('reviews', {
        method: 'POST',
        prefer: 'return=minimal',
        body: JSON.stringify(review)
      });
    } catch(e) {
      console.log('Error saving review:', e);
      throw e;
    }
  }

  function renderAllReviews() {
    const list = document.getElementById('reviews-list');
    const noMsg = document.getElementById('no-reviews-msg');
    if (!userReviews.length) {
      if (noMsg) noMsg.style.display = 'block';
      return;
    }
    if (noMsg) noMsg.style.display = 'none';
    // Show all reviews, newest first
    const visibleReviews = userReviews.slice().reverse();
    list.innerHTML = visibleReviews.map((r, i) => `
      <div class="review-card" id="review-${i}">
        <div class="review-card-header">
          <div class="reviewer-info">
            <div class="reviewer-avatar" style="background:var(--amber-glow)">${r.initials}</div>
            <div class="reviewer-details">
              <div class="name">${r.name}</div>
              <div class="date">${r.loc} · ${r.date}</div>
            </div>
          </div>
          <div class="review-stars" style="color:var(--amber-light)">${'★'.repeat(r.rating)}${'☆'.repeat(5-r.rating)}</div>
        </div>
        <div class="review-text">"${r.review_text || r.text}"</div>
        <span class="review-product-tag">🍯 ${r.product}</span>
      </div>`).join('');
  }

  function renderHomeReviews() {
    const grid = document.getElementById('home-reviews-grid');
    if (!userReviews.length) {
      grid.innerHTML = `<div style="grid-column:1/-1;text-align:center;color:#9CA3AF;padding:2rem;font-size:0.95rem;"><div style="font-size:2rem;margin-bottom:0.5rem">🍯</div>No reviews yet — be the first to share your experience!</div>`;
      return;
    }
    const latest = userReviews.slice(0, 3);
    grid.innerHTML = latest.map(r => `
      <div class="review-mini-card">
        <div class="stars">${'★'.repeat(r.rating)}</div>
        <p>"${(r.review_text || r.text || '').slice(0,100)}${(r.review_text || r.text || '').length > 100 ? '...' : ''}"</p>
        <div class="reviewer">
          <div class="avatar" style="background:var(--amber-glow);font-size:0.75rem;font-weight:700;color:var(--brown-deep)">${r.initials}</div>
          <div><div class="reviewer-name">${r.name}</div><div class="reviewer-loc">${r.location || r.loc}</div></div>
        </div>
      </div>`).join('');
  }

  function updateRatingSummary() {
    const total = userReviews.length;
    if (!total) return;
    const avg = (userReviews.reduce((s,r) => s + r.rating, 0) / total).toFixed(1);
    document.getElementById('avg-rating').textContent = avg;
    document.getElementById('review-count').textContent = `${total} review${total !== 1 ? 's' : ''}`;
    // Update bars
    const counts = [5,4,3,2,1].map(n => userReviews.filter(r => r.rating === n).length);
    const bars = document.querySelectorAll('.bar-fill');
    const barCounts = document.querySelectorAll('.rating-bar-row span:last-child');
    counts.forEach((c, i) => {
      if (bars[i]) bars[i].style.width = total ? (c/total*100)+'%' : '0%';
      if (barCounts[i]) barCounts[i].textContent = c;
    });
    // Update stars display
    const starEl = document.querySelector('.rating-big .stars');
    if (starEl) {
      const rounded = Math.round(avg);
      starEl.textContent = '★'.repeat(rounded) + '☆'.repeat(5-rounded);
    }
  }

  let selectedRating = 0;

  function setRating(n) {
    selectedRating = n;
    document.querySelectorAll('#star-rating span').forEach((s, i) => {
      s.classList.toggle('active', i < n);
    });
  }

  async function submitReview() {
    const name = document.getElementById('r-name').value.trim();
    const loc = document.getElementById('r-loc').value.trim();
    const product = document.getElementById('r-product').value;
    const text = document.getElementById('r-text').value.trim();
    if (!name || !text || !selectedRating) {
      alert('Please fill in your name, review, and select a star rating!');
      return;
    }
    const initials = name.split(' ').map(w => w[0]).join('').toUpperCase().slice(0,2);
    const now = new Date();
    const date = now.toLocaleDateString('en-GB', { day:'numeric', month:'short', year:'numeric' });
    const review = { name, location: loc || 'Nigeria', product, review_text: text, rating: selectedRating, initials, date };
    const btn = document.querySelector('.submit-review-btn');
    btn.textContent = 'Submitting...';
    btn.disabled = true;
    try {
      await saveReviews(review);
      userReviews.unshift({...review, text: review.review_text});
      renderAllReviews();
      updateRatingSummary();
      renderHomeReviews();
      document.getElementById('r-name').value = '';
      document.getElementById('r-loc').value = '';
      document.getElementById('r-text').value = '';
      selectedRating = 0;
      document.querySelectorAll('#star-rating span').forEach(s => s.classList.remove('active'));
      const success = document.getElementById('review-success');
      success.style.display = 'block';
      setTimeout(() => success.style.display = 'none', 4000);
      setTimeout(() => document.getElementById('reviews-list').scrollIntoView({behavior:'smooth'}), 300);
    } catch(e) {
      alert('Error submitting review. Please try again!');
    }
    btn.textContent = 'Submit Review ⭐';
    btn.disabled = false;
  }

  function showToast(msg) {
    const t = document.getElementById('toast');
    t.textContent = msg; t.classList.add('show');
    setTimeout(() => t.classList.remove('show'), 2500);
  }

  renderProducts();
  loadReviews();
</script>
</body>
</html>
