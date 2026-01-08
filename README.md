<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Light and Memory Audio</title>
  <meta name="description" content="Light and Memory Audio — Service fee $50 (materials/parts not included)." />

  <style>
    :root{
  /* Logo-based palette */
  --bg: #f4efe9;          /* logo cream background */
  --surface: #eee7df;     /* card surface (slightly darker cream) */
  --text: #1f1f1f;        /* logo charcoal */
  --muted: #6b6b6b;       /* soft gray */
  --line: rgba(0,0,0,.08);
  --line2: rgba(0,0,0,.14);

  --radius: 18px;
  --focus: rgba(0,0,0,.08);
}

    *{box-sizing:border-box}
    html{background:var(--bg)}
    body{
      margin:0;
      font-family: system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial;
      background:var(--bg);
      color:var(--text);
      line-height:1.55;
    }

    a{color:inherit;text-decoration:none}
    .wrap{max-width:980px;margin:0 auto;padding:28px 20px}
    .muted{color:var(--muted)}
    .divider{height:1px;background:var(--line);margin:18px 0}

    /* Header */
    header{
      position:sticky;
      top:0;
      background:var(--bg);
      border-bottom:1px solid var(--line);
      z-index:10;
    }
    .nav{
      display:flex;
      justify-content:space-between;
      align-items:center;
      gap:16px;
    }
    .brand{
      display:flex;
      align-items:center;
      gap:12px;
    }
    .logoImg{
      width:40px;
      height:40px;
      border-radius:12px;
      border:1px solid var(--line2);
      object-fit:cover;
    }
    nav a{
      margin-left:16px;
      color:var(--muted);
      font-size:14px;
    }
    nav a:hover{color:var(--text)}

    .btn{
      padding:9px 14px;
      border-radius:999px;
      border:1px solid var(--line);
      background:transparent;
      color:var(--text);
      font-size:13px;
      cursor:pointer;
    }
    .btn.primary{
      border-color:var(--line2);
      background:rgba(214,194,167,.12);
    }

    /* Hero */
    .hero{
      margin-top:28px;
      border:1px solid var(--line);
      border-radius:var(--radius);
      padding:26px;
    }
    .hero h1{
      font-size:38px;
      letter-spacing:-0.03em;
      margin:0 0 12px;
    }
    .hero p{
      max-width:60ch;
      color:var(--muted);
      font-size:15.5px;
    }

    .pillRow{
      display:flex;
      gap:10px;
      flex-wrap:wrap;
      margin:16px 0;
    }
    .pill{
      padding:8px 12px;
      border-radius:14px;
      border:1px solid var(--line2);
      font-size:13px;
    }

    section{padding:32px 0}

    .grid{
      display:grid;
      grid-template-columns:repeat(3,1fr);
      gap:14px;
    }
    @media(max-width:900px){
      .grid{grid-template-columns:1fr}
    }

    .card{
      border:1px solid var(--line);
      border-radius:16px;
      padding:18px;
      background:rgba(243,234,223,.015);
    }
    .card h3{
      margin:0 0 8px;
      font-size:15px;
    }
    .card ul{
      margin:8px 0 0;
      padding-left:18px;
      color:var(--muted);
      font-size:14px;
    }

    .notice{
      margin-top:16px;
      padding:14px;
      border:1px dashed var(--line2);
      border-radius:14px;
      color:var(--muted);
      font-size:13px;
    }

    /* Footer */
    footer{
      border-top:1px solid var(--line);
      padding:32px 0;
      color:var(--muted);
      font-size:13px;
    }
  </style>
</head>

<body>

<header>
  <div class="wrap nav">
    <div class="brand">
      <img src="assets/lama.jpg" class="logoImg" alt="Light and Memory Audio logo">
      <div>
        <strong>Light and Memory Audio</strong><br>
        <span class="muted" style="font-size:12px">Setups. Repairs. Pro feel.</span>
      </div>
    </div>
    <nav>
      <a href="#services">Services</a>
      <a href="#pricing">Pricing</a>
      <a href="#booking">Booking</a>
    </nav>
  </div>
</header>

<main class="wrap">

  <section class="hero">
    <h1>Make your guitar feel right again.</h1>
    <p>
      Playability-first setups and select repairs for musicians who care about
      tuning stability, feel, and reliability.
    </p>

    <div class="pillRow">
      <div class="pill">Service Fee: $50</div>
      <div class="pill">Materials / parts not included</div>
    </div>

    <a class="btn primary" href="#booking">Book an appointment</a>
  </section>

  <section id="services">
    <h2>Services</h2>

    <div class="grid">
      <div class="card">
        <h3>Setups</h3>
        <ul>
          <li>Neck relief</li>
          <li>Action & saddle height</li>
          <li>Intonation</li>
          <li>Basic cleaning & inspection</li>
        </ul>
      </div>

      <div class="card">
        <h3>Select Repairs</h3>
        <ul>
          <li>Electronics troubleshooting</li>
          <li>Jack / pot / switch repair</li>
          <li>Pickup swaps</li>
          <li>Hardware fixes</li>
        </ul>
      </div>

      <div class="card">
        <h3>Not sure?</h3>
        <ul>
          <li>Tuning instability</li>
          <li>Buzzing / dead notes</li>
          <li>Bridge / trem issues</li>
          <li>String gauge changes</li>
        </ul>
      </div>
    </div>

    <div class="notice">
      <strong>Service limitations:</strong><br>
      Fret repair/fretwork and structural repairs are not currently offered.
      Services will expand as tools and shop capabilities grow.
    </div>
  </section>

  <section id="pricing">
    <h2>Pricing</h2>
    <p class="muted">
      $50 service fee for setups and in-scope repairs.  
      Parts and materials billed separately with approval.
    </p>
  </section>

  <section id="booking">
    <h2>Booking</h2>
    <p class="muted">
      Contact via Instagram or text to schedule.
    </p>
    <a class="btn" href="https://www.instagram.com/light_and_memory_audio" target="_blank">
      Instagram
    </a>
  </section>

</main>

<footer>
  <div class="wrap">
    © <span id="year"></span> Light and Memory Audio — Simi Valley / Moorpark / Northridge /
    Thousand Oaks / Santa Clarita / Porter Ranch
  </div>
</footer>

<script>
  document.getElementById("year").textContent = new Date().getFullYear();
</script>

</body>
</html>
