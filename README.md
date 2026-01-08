<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Light and Memory Audio</title>
  <meta name="description" content="Light and Memory Audio — Service fee $30 (materials/parts not included). Serving Simi Valley, Moorpark, Northridge, Thousand Oaks, Santa Clarita, Porter Ranch." />

  <!-- Optional: social preview image (add assets/preview.jpg if you want link previews) -->
  <meta property="og:title" content="Light and Memory Audio" />
  <meta property="og:description" content="Service fee $30 (materials/parts not included). Setups & select repairs." />
  <meta property="og:type" content="website" />
  <meta property="og:image" content="assets/preview.jpg" />

  <style>
    /* ===== Creamy Poetry palette (logo-friendly, warm, premium) ===== */
    :root{
      /* Core palette */
      --bg: #F2EEE9;        /* Isabelline (paper) */
      --surface: #E8DED3;   /* warm cream / light brown */
      --surface2:#E1D6C9;   /* slightly deeper warm brown */
      --ink: #1D1B18;       /* near-black ink */
      --muted: #5E564D;     /* warm gray text */
      --line: rgba(29,27,24,.10);
      --line2: rgba(29,27,24,.16);

      /* Accents (subtle) */
      --almond: #C9BBAA;
      --timberwolf: #D8D3CB;
      --linen: #E9DDCC;
      --paledogwood: #E2C6BD;

      --radius: 18px;
      --max: 980px;
      --focus: rgba(29,27,24,.10);
    }

    *{box-sizing:border-box}

    html{background:var(--bg)}
    body{
      margin:0;
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial;
      background: var(--bg);
      color: var(--ink);

      /* ✅ readability boost */
      font-size: 16.5px;
      font-weight: 500;
      line-height: 1.65;
      letter-spacing: .015em;
    }

    a{color:inherit;text-decoration:none}
    .wrap{max-width:var(--max); margin:0 auto; padding:28px 20px}
    @media (max-width:600px){ .wrap{padding:22px 16px} }

    p, li{font-weight:500}

    .muted{color:var(--muted); font-weight:500}
    .tiny{font-size:13px; font-weight:500; color:var(--muted)}
    .small{font-size:14px; font-weight:500; color:var(--muted)}
    .divider{height:1px; background:var(--line); margin:18px 0}

    /* ===== Header ===== */
    header{
      position:sticky;
      top:0;
      z-index:10;
      background: rgba(242,238,233,.88);
      backdrop-filter: blur(10px);
      border-bottom:1px solid var(--line);
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
      min-width:240px;
    }
    .logoImg{
      width:40px;
      height:40px;
      border-radius:14px;
      border:1px solid var(--line2);
      object-fit:cover;
      background: var(--surface);
    }
    .brandTitle{
      margin:0;
      font-size:14px;
      letter-spacing:.08em;
      text-transform:uppercase;
      font-weight:800;
      line-height:1.1;
    }
    .brandSub{
      margin:3px 0 0;
      font-size:12px;
      color:var(--muted);
      line-height:1.1;
      font-weight:500;
    }

    nav.links{display:flex; gap:14px; flex-wrap:wrap; justify-content:flex-end}
    nav.links a{
      font-size:13px;
      color:var(--muted);
      padding:8px 10px;
      border-radius:999px;
      border:1px solid transparent;
      font-weight:600;
    }
    nav.links a:hover{
      color:var(--ink);
      border-color: var(--line);
      background: rgba(29,27,24,.03);
    }
    @media (max-width:920px){
      nav.links{display:none}
    }

    .cta{
      display:flex;
      gap:10px;
      align-items:center;
      flex-wrap:wrap;
      justify-content:flex-end;
    }
    .btn{
      display:inline-flex;
      align-items:center;
      justify-content:center;
      gap:8px;
      padding:10px 12px;
      border-radius:999px;
      border:1px solid var(--line2);
      background: rgba(29,27,24,.02);
      color:var(--ink);
      font-size:13px;
      font-weight:700;
      cursor:pointer;
      transition: background .15s ease, transform .06s ease;
      white-space:nowrap;
    }
    .btn:hover{background: rgba(29,27,24,.05)}
    .btn:active{transform: translateY(1px)}
    .btn.primary{
      background: var(--ink);
      color: var(--bg);
      border-color: var(--ink);
    }
    .btn.primary:hover{background: #11100e}

    /* ===== Hero ===== */
    .hero{
      margin-top:22px;
      border:1px solid var(--line);
      border-radius: var(--radius);
      background: linear-gradient(180deg, var(--surface), rgba(242,238,233,.55));
      padding:24px;
    }
    .kicker{
      display:inline-flex;
      align-items:center;
      gap:8px;
      padding:6px 10px;
      border-radius:999px;
      border:1px solid var(--line);
      background: rgba(29,27,24,.02);
      color:var(--muted);
      font-size:12px;
      letter-spacing:.06em;
      text-transform:uppercase;
      font-weight:650;
    }
    .dot{
      width:8px;height:8px;border-radius:99px;
      background: var(--paledogwood);
      border:1px solid rgba(29,27,24,.10);
    }
    .hero h1{
      margin:14px 0 10px;
      font-size:38px;
      line-height:1.07;
      letter-spacing:-.03em;
      font-weight:900;
    }
    .hero p{
      margin:0 0 14px;
      color:var(--muted);
      font-size:16px;
      max-width:62ch;
      font-weight:500;
    }
     a:focus-visible, button:focus-visible{
     outline: none;
     box-shadow: 0 0 0 4px var(--focus);
    }
    .pillRow{
      display:flex;
      gap:10px;
      flex-wrap:wrap;
      margin:16px 0 18px;
    }
    .pill{
      padding:8px 12px;
      border-radius:14px;
      border:1px solid var(--line2);
      background: rgba(29,27,24,.02);
      font-size:13px;
      font-weight:800;
    }
    .pill.soft{
      background: rgba(226,198,189,.30); /* pale dogwood tint */
      border-color: rgba(29,27,24,.12);
      color: var(--ink);
    }

    /* ===== Sections ===== */
    section{padding:26px 0}
    h2{
      margin:0 0 12px;
      font-size:14px;
      letter-spacing:.10em;
      text-transform:uppercase;
      color:var(--muted);
      font-weight:800;
    }
    .grid{
      display:grid;
      grid-template-columns: repeat(3, 1fr);
      gap:14px;
    }
    @media (max-width:900px){
      .grid{grid-template-columns:1fr}
    }
    .card{
      border:1px solid var(--line);
      border-radius:16px;
      padding:18px;
      background: var(--surface);
    }
    .card h3{
      margin:0 0 8px;
      font-size:16px;
      font-weight:700;
      letter-spacing:.02em;
      color: var(--ink);
    }
    .card p{
      margin:0;
      color:var(--muted);
      font-size:14.5px;
      font-weight:500;
    }
    .card ul{
      margin:10px 0 0;
      padding-left:18px;
      color:var(--muted);
      font-size:14.5px;
      display:grid;
      gap:6px;
      font-weight:500;
    }

    .notice{
      margin-top:16px;
      padding:14px;
      border:1px dashed rgba(29,27,24,.18);
      border-radius:14px;
      background: rgba(233,221,204,.40); /* linen tint */
      color: var(--muted);
      font-size:14px;
      font-weight:500;
    }

    /* ===== Pricing blocks ===== */
    .pricing{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:14px;
    }
    @media (max-width:900px){
      .pricing{grid-template-columns:1fr}
    }
    .priceCard{
      border:1px solid var(--line);
      border-radius:16px;
      padding:18px;
      background: var(--surface);
    }
    .priceTop{
      display:flex;
      justify-content:space-between;
      align-items:flex-start;
      gap:12px;
    }
    .tag{
      font-size:12px;
      color:var(--muted);
      padding:6px 10px;
      border-radius:999px;
      border:1px solid var(--line);
      background: rgba(29,27,24,.02);
      white-space:nowrap;
      font-weight:650;
    }
    .bigPrice{
      margin:8px 0 6px;
      font-size:34px;
      font-weight:900;
      letter-spacing:-.02em;
      color:var(--ink);
    }

    /* ===== Booking ===== */
    .twoCol{display:grid; grid-template-columns:1fr 1fr; gap:14px}
    @media (max-width:900px){ .twoCol{grid-template-columns:1fr} }

    form{
      border:1px solid var(--line);
      border-radius:16px;
      padding:18px;
      background: var(--surface);
      display:grid;
      gap:12px;
    }
    label{
      font-size:12px;
      letter-spacing:.08em;
      text-transform:uppercase;
      color:var(--muted);
      font-weight:800;
    }
    input, select, textarea{
      width:100%;
      padding:12px 12px;
      border-radius:14px;
      border:1px solid rgba(29,27,24,.16);
      background: rgba(242,238,233,.85);
      color: var(--ink);
      outline:none;
      font-size:15px;
      font-weight:500;
    }
    input:focus, select:focus, textarea:focus{
      border-color: rgba(29,27,24,.25);
      box-shadow: 0 0 0 4px var(--focus);
    }
    textarea{min-height:110px; resize:vertical}
    .formRow{display:grid; grid-template-columns:1fr 1fr; gap:12px}
    @media (max-width:650px){ .formRow{grid-template-columns:1fr} }

    /* ===== Footer ===== */
    footer{
      border-top:1px solid var(--line);
      padding:28px 0;
      color:var(--muted);
      font-size:14px;
      font-weight:500;
    }
    .footerGrid{
      display:grid;
      grid-template-columns:1.2fr .8fr;
      gap:14px;
      align-items:start;
    }
    @media (max-width:900px){ .footerGrid{grid-template-columns:1fr} }
    .miniLinks{display:flex; gap:10px; flex-wrap:wrap; justify-content:flex-end}
    .miniLinks a{
      color:var(--muted);
      padding:6px 8px;
      border-radius:999px;
      border:1px solid transparent;
      font-size:13px;
      font-weight:650;
    }
    .miniLinks a:hover{
      border-color: var(--line);
      color: var(--ink);
      background: rgba(29,27,24,.03);
    }
  </style>
</head>

<body>
<header>
  <div class="wrap">
    <div class="nav">
      <a class="brand" href="#top" aria-label="Light and Memory Audio Home">
        <img class="logoImg" src="assets/lama.jpg" alt="Light and Memory Audio logo" />
        <div>
          <div class="brandTitle">Light and Memory Audio</div>
          <div class="brandSub">Setups. Repairs. Pro feel.</div>
        </div>
      </a>

      <nav class="links" aria-label="Site navigation">
        <a href="#services">Services</a>
        <a href="#pricing">Pricing</a>
        <a href="#booking">Booking</a>
        <a href="#faq">FAQ</a>
      </nav>

      <div class="cta">
        <!-- UPDATE THESE -->
        <a class="btn" id="callBtn" href="tel:+18055551234">Call</a>
        <a class="btn" id="textBtn" href="sms:+18055551234">Text</a>
        <a class="btn" href="https://www.instagram.com/light_and_memory_audio?igsh=NTc4MTIwNjQ2YQ%3D%3D&utm_source=qr" target="_blank" rel="noopener noreferrer">Instagram</a>
        <a class="btn primary" href="#booking">Book</a>
      </div>
    </div>
  </div>
</header>

<main id="top" class="wrap">

  <section class="hero" aria-label="Hero">
    <span class="kicker"><span class="dot" aria-hidden="true"></span> Clean feel • Stable tuning • Honest work</span>

    <h1>Make your guitar feel right again.</h1>

    <p>
      Playability-first setups and select repairs for musicians who care about
      tuning stability, feel, and reliability.
    </p>

    <div class="pillRow" aria-label="Pricing highlights">
      <div class="pill soft">Service Fee: $30</div>
      <div class="pill">Materials / parts not included</div>
    </div>

    <div class="cta" style="justify-content:flex-start; margin-top:4px">
      <a class="btn primary" href="#booking">Book an appointment</a>
      <a class="btn" href="#pricing">See pricing</a>
    </div>

    <div class="divider"></div>

    <p class="small" style="margin:0">
      <strong class="muted">Service area:</strong>
      <span id="locationText">Simi Valley / Moorpark / Northridge / Thousand Oaks / Santa Clarita / Porter Ranch</span>
      &nbsp;•&nbsp;
      <strong class="muted">Hours:</strong>
      <span id="hoursText">By appointment</span>
    </p>
  </section>

  <section id="services" aria-label="Services">
    <h2>Services</h2>

    <div class="grid">
      <div class="card">
        <h3>Setups</h3>
        <p>Comfort + clarity for live players and daily practice.</p>
        <ul>
          <li>Neck relief adjustment</li>
          <li>Action / saddle height</li>
          <li>Intonation</li>
          <li>Basic cleaning + inspection</li>
        </ul>
      </div>

      <div class="card">
        <h3>Select repairs</h3>
        <p>Common issues fixed cleanly and reliably (within scope).</p>
        <ul>
          <li>Electronics troubleshooting</li>
          <li>Output jack / pot / switch</li>
          <li>Pickup swaps (standard installs)</li>
          <li>Hardware fixes</li>
        </ul>
      </div>

      <div class="card">
        <h3>Not sure?</h3>
        <p>Describe the issue and I’ll tell you if it’s in scope.</p>
        <ul>
          <li>Tuning instability</li>
          <li>Buzzing / dead notes</li>
          <li>Bridge / trem issues</li>
          <li>String gauge changes</li>
        </ul>
      </div>
    </div>

    <div class="notice">
      <strong style="color:var(--ink); font-weight:800;">Current limitations:</strong><br>
      I’m limited to certain repairs and setups due to available tools, supplies, and hardware. This will expand as I continue investing in my shop.<br><br>
      <strong style="color:var(--ink); font-weight:800;">Not currently offered:</strong>
      <ul style="margin:10px 0 0; padding-left:18px;">
        <li>Fret repair / fretwork</li>
        <li>Structural repairs (neck breaks, cracks, major body damage)</li>
      </ul>
    </div>
  </section>

  <section id="pricing" aria-label="Pricing">
    <h2>Pricing</h2>

    <div class="pricing">
      <div class="priceCard">
        <div class="priceTop">
          <div>
            <div class="muted" style="letter-spacing:.08em;text-transform:uppercase;font-size:12px;font-weight:800;">Service fee</div>
            <div class="bigPrice">$30</div>
            <div class="small">Labor/service for setups and in-scope repair work (confirmed before starting).</div>
          </div>
          <div class="tag">Upfront</div>
        </div>

        <div class="divider"></div>

        <ul style="margin:0; padding-left:18px; color:var(--muted); display:grid; gap:6px;">
          <li>Relief, action, intonation</li>
          <li>Basic troubleshooting + fixes</li>
          <li>Electronics/hardware labor (within scope)</li>
        </ul>

        <p class="small" style="margin-top:12px">
          <strong style="color:var(--ink); font-weight:800;">Materials/parts not included.</strong> You approve any parts cost before purchase.
        </p>
      </div>

      <div class="priceCard">
        <div class="priceTop">
          <div>
            <div class="muted" style="letter-spacing:.08em;text-transform:uppercase;font-size:12px;font-weight:800;">Parts &amp; materials</div>
            <div class="bigPrice">Not included</div>
            <div class="small">Strings, pickups, pots, switches, jacks, hardware, etc. billed separately.</div>
          </div>
          <div class="tag">Approved first</div>
        </div>

        <div class="divider"></div>

        <ul style="margin:0; padding-left:18px; color:var(--muted); display:grid; gap:6px;">
          <li>Strings / consumables</li>
          <li>Electronics parts</li>
          <li>Hardware replacements</li>
        </ul>

        <p class="small" style="margin-top:12px">
          Customer-supplied parts are fine — compatibility confirmed before install.
        </p>
      </div>
    </div>
  </section>

  <section id="booking" aria-label="Booking">
    <h2>Booking</h2>

    <div class="twoCol">
      <form id="bookingForm">
        <div class="formRow">
          <div>
            <label for="name">Name</label>
            <input id="name" name="name" autocomplete="name" required />
          </div>
          <div>
            <label for="phone">Phone</label>
            <input
              id="phone"
              name="phone"
              type="tel"
              inputmode="tel"
              placeholder="(805) 555-5555"
              autocomplete="tel"
              required
             />

          </div>
        </div>

        <div class="formRow">
          <div>
            <label for="instrument">Instrument</label>
            <select id="instrument" name="instrument" required>
              <option value="" selected disabled>Select one</option>
              <option>Electric Guitar</option>
              <option>Acoustic Guitar</option>
              <option>Bass</option>
              <option>Other</option>
            </select>
          </div>
          <div>
            <label for="service">Service</label>
            <select id="service" name="service" required>
              <option value="" selected disabled>Select one</option>
              <option value="Service Fee ($30) — Setup">Service Fee ($30) — Setup</option>
              <option value="Service Fee ($30) — Repair / Install">Service Fee ($30) — Repair / Install</option>
              <option value="Not sure — help me decide">Not sure — help me decide</option>
            </select>
          </div>
        </div>

        <div class="formRow">
          <div>
            <label for="timing">Preferred timing</label>
            <select id="timing" name="timing" required>
              <option value="" selected disabled>Select one</option>
              <option>ASAP</option>
              <option>This week</option>
              <option>Next week</option>
              <option>Flexible</option>
            </select>
          </div>
          <div>
            <label for="location">Drop-off area</label>
            <select id="location" name="location" required>
              <option value="" selected disabled>Select one</option>
              <option>Simi Valley</option>
              <option>Moorpark</option>
              <option>Northridge</option>
              <option>Thousand Oaks</option>
              <option>Santa Clarita</option>
              <option>Porter Ranch</option>
              <option>Other (describe below)</option>
            </select>
          </div>
        </div>

        <div>
          <label for="details">Details</label>
          <textarea id="details" name="details" placeholder="What’s happening? Include tuning + string gauge if you know it." required></textarea>
        </div>

        <div class="notice" id="formNotice" style="margin-top:0">
          Service fee: <strong style="color:var(--ink); font-weight:800;">$30</strong> (materials/parts not included).<br>
          Not offered currently: fretwork and structural repairs.
        </div>

        <div style="display:flex; gap:10px; flex-wrap:wrap; align-items:center">
          <button class="btn primary" type="submit">Send booking email</button>
          <button class="btn" type="button" id="copyBtn">Copy message</button>
        </div>

        <div id="fallbackWrap" style="display:none; margin-top:10px">
          <label for="fallbackText">Copy/paste this message</label>
          <textarea id="fallbackText" readonly></textarea>
        </div>

        <p class="tiny" style="margin:0">
          This form opens your email app (no data stored on the website).
        </p>
      </form>

      <div class="card">
        <h3>Contact</h3>
        <p class="muted" style="margin:0 0 12px">Update your email/phone in the script near the bottom.</p>

        <div class="notice" style="margin-top:0">
          <div><strong style="color:var(--ink); font-weight:800;">Email:</strong> <span id="emailText">youremail@example.com</span></div>
          <div style="margin-top:8px"><strong style="color:var(--ink); font-weight:800;">Phone:</strong> <span id="phoneText">(805) 424-7735</span></div>
          <div style="margin-top:8px">
            <strong style="color:var(--ink); font-weight:800;">Instagram:</strong>
            <a href="https://www.instagram.com/light_and_memory_audio?igsh=NTc4MTIwNjQ2YQ%3D%3D&utm_source=qr"
               target="_blank" rel="noopener noreferrer"
               style="text-decoration:underline; text-underline-offset:3px;">
              @light_and_memory_audio
            </a>
          </div>
          <div style="margin-top:8px">
            <strong style="color:var(--ink); font-weight:800;">Service area:</strong>
            <span id="areaText">Simi Valley / Moorpark / Northridge / Thousand Oaks / Santa Clarita / Porter Ranch</span>
          </div>
        </div>

        <div class="divider"></div>

        <h3 style="margin-top:0">What to bring</h3>
        <ul style="margin:0; padding-left:18px; color:var(--muted); display:grid; gap:6px;">
          <li>Your guitar + case/bag</li>
          <li>Preferred strings (or ask me to supply)</li>
          <li>Notes on tuning + gauge</li>
        </ul>
      </div>
    </div>
  </section>

  <section id="faq" aria-label="FAQ">
    <h2>FAQ</h2>

    <div class="grid">
      <div class="card">
        <h3>Do you work on acoustics?</h3>
        <p>Yes — acoustics, electrics, and bass. If it’s unusual, tell me what it is and I’ll confirm.</p>
      </div>
      <div class="card">
        <h3>Do I need new strings for a setup?</h3>
        <p>Highly recommended. Setups are best with the strings you’ll actually play.</p>
      </div>
      <div class="card">
        <h3>Do you do fretwork or structural repairs?</h3>
        <p>Not currently — limited by tools/supplies for now. This will expand as the shop grows.</p>
      </div>
    </div>
  </section>

</main>

<footer>
  <div class="wrap">
    <div class="footerGrid">
      <div style="display:flex; gap:10px; align-items:center">
        <img class="logoImg" src="assets/lama.jpg" alt="Light and Memory Audio logo" />
        <div>
          <div style="font-weight:900; letter-spacing:.08em; text-transform:uppercase; color:var(--ink);">Light and Memory Audio</div>
          <div class="tiny">Service fee: $30 • Materials/parts not included</div>
        </div>
      </div>

      <div class="miniLinks">
        <a href="#services">Services</a>
        <a href="#pricing">Pricing</a>
        <a href="#booking">Booking</a>
        <a href="https://www.instagram.com/light_and_memory_audio?igsh=NTc4MTIwNjQ2YQ%3D%3D&utm_source=qr" target="_blank" rel="noopener noreferrer">Instagram</a>
        <a href="#top">Top</a>
      </div>
    </div>

    <div class="tiny" style="margin-top:16px">
      © <span id="year"></span> Light and Memory Audio — Simi Valley / Moorpark / Northridge / Thousand Oaks / Santa Clarita / Porter Ranch
    </div>
  </div>
</footer>

<script>
  // ========= UPDATE THESE =========
  const BUSINESS_EMAIL = "lightandmemoryaudio26@gmail.com";     // <-- your real email
  const BUSINESS_PHONE = "+18054247735";              // <-- your real phone (E.164 format works best)
  const SERVICE_AREA   = "Simi Valley / Moorpark / Northridge / Thousand Oaks / Santa Clarita / Porter Ranch";
  const HOURS_TEXT     = "By appointment";

  document.getElementById("year").textContent = new Date().getFullYear();

  document.getElementById("emailText").textContent = BUSINESS_EMAIL;
  document.getElementById("phoneText").textContent = formatPhoneForDisplay(BUSINESS_PHONE) || BUSINESS_PHONE;
  document.getElementById("areaText").textContent = SERVICE_AREA;
  document.getElementById("locationText").textContent = SERVICE_AREA;
  document.getElementById("hoursText").textContent = HOURS_TEXT;

  document.getElementById("callBtn").href = `tel:${BUSINESS_PHONE}`;
  document.getElementById("textBtn").href = `sms:${BUSINESS_PHONE}`;

  const form = document.getElementById("bookingForm");
  const notice = document.getElementById("formNotice");
  const copyBtn = document.getElementById("copyBtn");
  const fallbackWrap = document.getElementById("fallbackWrap");
  const fallbackText = document.getElementById("fallbackText");

  function buildMessage(data){
    const subject = `Booking Request — ${data.service} — ${data.name}`;
    const body =
`Booking Request (Light and Memory Audio)

Name: ${data.name}
Phone: ${data.phone}
Instrument: ${data.instrument}
Service: ${data.service}
Preferred timing: ${data.timing}
Drop-off area: ${data.location}

Details:
${data.details}

Notes:
- Service fee: $30
- Materials/parts not included (approved before purchase)
- Not currently offered: fret repair/fretwork, structural repairs

— Sent from the website`;

    return { subject, body };
  }

  function getFormData(){
    return {
      name: form.name.value.trim(),
      phone: form.phone.value.trim(),
      instrument: form.instrument.value,
      service: form.service.value,
      timing: form.timing.value,
      location: form.location.value,
      details: form.details.value.trim()
    };
  }

  function validate(data){
    if(!data.name || data.name.length < 2) return "Please enter your name.";
    if(!data.phone || data.phone.length < 7) return "Please enter a valid phone number.";
    if(!data.instrument) return "Please choose an instrument.";
    if(!data.service) return "Please choose a service.";
    if(!data.timing) return "Please choose preferred timing.";
    if(!data.location) return "Please choose a drop-off area.";
    if(!data.details || data.details.length < 10) return "Please add a bit more detail about the issue.";
    return null;
  }

  function setNotice(text, ok=false){
    notice.textContent = text;
    notice.style.borderStyle = ok ? "solid" : "dashed";
    notice.style.borderColor = ok ? "rgba(29,27,24,.20)" : "rgba(29,27,24,.18)";
    notice.style.background = ok ? "rgba(226,198,189,.35)" : "rgba(233,221,204,.40)";
    notice.style.color = ok ? "var(--ink)" : "var(--muted)";
  }

  form.addEventListener("submit", (e) => {
    e.preventDefault();
    const data = getFormData();
    const err = validate(data);
    if(err){ setNotice(err, false); return; }

      const msg = buildMessage(data);

  // show fallback text in case mailto doesn't open on someone's device
  fallbackWrap.style.display = "block";
  fallbackText.value = `Subject: ${msg.subject}\n\n${msg.body}`;

  const mailto = `mailto:${encodeURIComponent(BUSINESS_EMAIL)}?subject=${encodeURIComponent(msg.subject)}&body=${encodeURIComponent(msg.body)}`;
  setNotice("Opening your email app… If it doesn’t open, copy/paste the message below.", true);
  window.location.href = mailto;
  });

  copyBtn.addEventListener("click", async () => {
    const data = getFormData();
    const err = validate(data);
    if(err){ setNotice(err, false); return; }

    const msg = buildMessage(data);
    try{
      await navigator.clipboard.writeText(`Subject: ${msg.subject}\n\n${msg.body}`);
      setNotice("Copied. Paste into a text or email and send it over.", true);
    }catch{
      setNotice("Couldn’t copy automatically on this device. Copy manually from the email that opens.", false);
    }
  });

  function formatPhoneForDisplay(e164){
    const m = (e164 || "").match(/^\+1(\d{10})$/);
    if(!m) return "";
    const d = m[1];
    return `(${d.slice(0,3)}) ${d.slice(3,6)}-${d.slice(6)}`;
  }
</script>
</body>
</html>
