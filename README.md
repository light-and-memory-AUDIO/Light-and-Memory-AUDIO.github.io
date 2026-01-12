<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Light and Memory Audio</title>

  <meta name="description" content="Light and Memory Audio — $30 service fee for guitar setups and select repairs. Serving Simi Valley and surrounding areas." />

  <!-- Social preview -->
  <meta property="og:title" content="Light and Memory Audio" />
  <meta property="og:description" content="$30 service fee • Transparent pricing • By appointment" />
  <meta property="og:type" content="website" />
  <meta property="og:image" content="assets/lama.jpeg" />

  <style>
    :root{
      --bg:#F2EEE9;
      --surface:#E8DED3;
      --ink:#1D1B18;
      --muted:#5E564D;
      --line:rgba(29,27,24,.10);
      --line2:rgba(29,27,24,.16);
      --radius:18px;
      --max:980px;
      --focus:rgba(29,27,24,.10);
    }

    *{box-sizing:border-box}
    body{
      margin:0;
      font-family:system-ui,-apple-system,Segoe UI,Roboto,Helvetica,Arial;
      background:var(--bg);
      color:var(--ink);
      font-size:16.5px;
      line-height:1.65;
      letter-spacing:.015em;
    }

    a{color:inherit;text-decoration:none}
    img{display:block}
    .wrap{max-width:var(--max);margin:0 auto;padding:26px 20px}
    .divider{height:1px;background:var(--line);margin:18px 0}
    .muted{color:var(--muted)}
    .tiny{font-size:13px;color:var(--muted)}
    .small{font-size:14px;color:var(--muted)}

    /* ===== Header ===== */
    header{
      position:sticky;
      top:0;
      z-index:20;
      background:rgba(242,238,233,.9);
      backdrop-filter:blur(10px);
      border-bottom:1px solid var(--line);
    }
    .nav{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:16px;
    }
    .brand{
      display:flex;
      gap:12px;
      align-items:center;
    }
    .logoImg{
      width:40px;
      height:40px;
      border-radius:14px;
      border:1px solid var(--line2);
      object-fit:cover;
      background:var(--surface);
    }
    .brandTitle{
      font-size:14px;
      letter-spacing:.08em;
      text-transform:uppercase;
      font-weight:800;
    }
    .brandSub{
      font-size:12px;
      color:var(--muted);
    }

    nav.links{
      display:flex;
      gap:14px;
    }
    nav.links a{
      font-size:13px;
      color:var(--muted);
      padding:8px 10px;
      border-radius:999px;
      font-weight:600;
    }
    nav.links a:hover{
      background:rgba(29,27,24,.05);
      color:var(--ink);
    }

    .cta{
      display:flex;
      gap:10px;
      align-items:center;
    }
    .ctaDesktop{
      display:flex;
      gap:10px;
      flex-wrap:nowrap;
    }

    .btn{
      padding:10px 12px;
      border-radius:999px;
      border:1px solid var(--line2);
      background:rgba(29,27,24,.02);
      font-size:13px;
      font-weight:700;
      cursor:pointer;
    }
    .btn.primary{
      background:var(--ink);
      color:var(--bg);
      border-color:var(--ink);
    }

    /* Hamburger */
    .menuBtn{display:none}
    .hamburger{
      width:18px;height:2px;background:var(--ink);
      position:relative;border-radius:99px;
    }
    .hamburger::before,.hamburger::after{
      content:"";position:absolute;left:0;width:18px;height:2px;
      background:var(--ink);border-radius:99px;
    }
    .hamburger::before{top:-6px}
    .hamburger::after{top:6px}

    /* Mobile menu */
    .menuOverlay{
      position:fixed;inset:0;
      background:rgba(29,27,24,.35);
      z-index:50;
    }
    .mobileMenu{
      position:fixed;top:0;right:0;
      width:min(84vw,360px);
      height:100vh;
      background:var(--bg);
      border-left:1px solid var(--line);
      padding:18px;
      transform:translateX(105%);
      transition:.2s ease;
      z-index:60;
      display:grid;
      gap:14px;
    }
    .mobileMenu.open{transform:translateX(0)}

    .mobileMenuNav a{
      display:block;
      padding:10px 12px;
      border:1px solid var(--line);
      border-radius:14px;
      font-weight:700;
      color:var(--muted);
    }

    @media(max-width:920px){
      nav.links{display:none}
      .ctaDesktop{display:none}
      .menuBtn{display:inline-flex}
    }
    @media(min-width:921px){
      .menuOverlay,.mobileMenu{display:none!important}
    }

    /* ===== Sections ===== */
    section{padding:26px 0}
    h1{
      font-size:38px;
      font-weight:900;
      line-height:1.08;
      letter-spacing:-.03em;
    }
    h2{
      font-size:14px;
      letter-spacing:.1em;
      text-transform:uppercase;
      color:var(--muted);
      font-weight:800;
      margin-bottom:12px;
    }

    .hero{
      border:1px solid var(--line);
      border-radius:var(--radius);
      background:linear-gradient(180deg,var(--surface),rgba(242,238,233,.6));
      padding:24px;
    }

    .pill{
      display:inline-block;
      padding:8px 12px;
      border-radius:14px;
      border:1px solid var(--line2);
      font-size:13px;
      font-weight:800;
      margin-right:6px;
    }

    .grid{
      display:grid;
      grid-template-columns:repeat(3,1fr);
      gap:14px;
    }
    @media(max-width:900px){.grid{grid-template-columns:1fr}}

    .card{
      border:1px solid var(--line);
      border-radius:16px;
      padding:18px;
      background:var(--surface);
    }

    footer{
      border-top:1px solid var(--line);
      padding:28px 0;
      font-size:14px;
      color:var(--muted);
    }
  </style>
</head>

<body>

<header>
  <div class="wrap">
    <div class="nav">
      <a class="brand" href="#top">
        <img class="logoImg" src="assets/lama.jpeg" alt="Light and Memory Audio logo">
        <div>
          <div class="brandTitle">Light and Memory Audio</div>
          <div class="brandSub">Setups. Repairs. Pro feel.</div>
        </div>
      </a>

      <nav class="links">
        <a href="#services">Services</a>
        <a href="#pricing">Pricing</a>
        <a href="#booking">Booking</a>
      </nav>

      <div class="cta">
        <div class="ctaDesktop">
          <a class="btn" href="tel:+18054247735">Call</a>
          <a class="btn" href="sms:+18054247735">Text</a>
          <a class="btn primary" href="#booking">Book</a>
        </div>

        <button class="btn menuBtn" id="menuBtn">
          <span class="hamburger"></span>
        </button>
      </div>
    </div>
  </div>
</header>

<div class="menuOverlay" id="menuOverlay" hidden></div>
<aside class="mobileMenu" id="mobileMenu">
  <a class="btn" href="tel:+18054247735">Call</a>
  <a class="btn" href="sms:+18054247735">Text</a>
  <a class="btn primary" href="#booking">Book</a>
  <div class="divider"></div>
  <nav class="mobileMenuNav">
    <a href="#services">Services</a>
    <a href="#pricing">Pricing</a>
    <a href="#booking">Booking</a>
  </nav>
</aside>

<main id="top" class="wrap">

<section class="hero">
  <h1>Make your guitar feel right again.</h1>
  <p class="muted">Playability-first setups and select repairs focused on tuning stability and feel.</p>
  <span class="pill">$30 Service Fee</span>
  <span class="pill">Parts not included</span>
</section>

<section id="services">
  <h2>Services</h2>
  <div class="grid">
    <div class="card">
      <strong>Setups</strong>
      <p class="small">Relief, action, intonation, inspection</p>
    </div>
    <div class="card">
      <strong>Select repairs</strong>
      <p class="small">Electronics, jacks, pots, pickup swaps</p>
    </div>
    <div class="card">
      <strong>Not sure?</strong>
      <p class="small">Describe the issue and I’ll confirm scope</p>
    </div>
  </div>
</section>

<section id="pricing">
  <h2>Pricing</h2>
  <div class="card">
    <strong>$30 Service Fee</strong>
    <p class="small">Labor for setups and in-scope work. Parts approved separately.</p>
  </div>
</section>

<section>
  <h2>Why it’s a better value</h2>
  <div class="card">
    <ul class="small">
      <li>Low overhead, appointment-based shop</li>
      <li>No upsells or surprise charges</li>
      <li>Customer-approved parts only</li>
      <li>Play-tested before pickup</li>
    </ul>
  </div>
</section>

<section id="booking">
  <h2>Booking</h2>
  <div class="card">
    <p class="small">
      Text or call to book.  
      <br><strong>Payment:</strong> Cash or Zelle only.
    </p>
  </div>
</section>

</main>

<footer>
  <div class="wrap">
    <strong>Light and Memory Audio</strong><br>
    Simi Valley & surrounding areas<br>
    Cash • Zelle • By appointment
  </div>
</footer>

<script>
  const menuBtn = document.getElementById("menuBtn");
  const mobileMenu = document.getElementById("mobileMenu");
  const overlay = document.getElementById("menuOverlay");

  if(menuBtn){
    menuBtn.onclick = () => {
      mobileMenu.classList.add("open");
      overlay.hidden = false;
      document.body.style.overflow = "hidden";
    };
    overlay.onclick = () => {
      mobileMenu.classList.remove("open");
      overlay.hidden = true;
      document.body.style.overflow = "";
    };
  }
</script>

</body>
