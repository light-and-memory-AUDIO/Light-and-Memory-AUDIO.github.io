<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Light and Memory Audio</title>
  <meta name="description" content="Light and Memory Audio — Service fee $50 (materials/parts not included). Serving Simi Valley, Moorpark, Northridge, Thousand Oaks, Santa Clarita, Porter Ranch." />
  <style>
    :root{
      --bg:#0b0f14;
      --muted:#9fb0c3;
      --text:#eaf2ff;
      --accent:#6ee7ff;
      --accent2:#a78bfa;
      --border: rgba(255,255,255,.10);
      --shadow: 0 10px 30px rgba(0,0,0,.35);
      --radius: 18px;
      --max: 1100px;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, "Apple Color Emoji","Segoe UI Emoji";
      background: radial-gradient(1200px 600px at 10% 0%, rgba(110,231,255,.18), transparent 55%),
                  radial-gradient(900px 500px at 90% 10%, rgba(167,139,250,.18), transparent 55%),
                  var(--bg);
      color:var(--text);
      line-height:1.45;
    }
    a{color:inherit;text-decoration:none}
    .wrap{max-width:var(--max); margin:0 auto; padding:24px}
    header{
      position:sticky; top:0; z-index:50;
      backdrop-filter: blur(10px);
      background: rgba(11,15,20,.65);
      border-bottom:1px solid var(--border);
    }
    .nav{
      display:flex; align-items:center; justify-content:space-between;
      gap:16px;
    }
    .brand{
      display:flex; align-items:center; gap:12px;
      padding:12px 0;
    }

    /* ✅ Logo image */
    .logoImg{
      width:40px;
      height:40px;
      border-radius:14px;
      box-shadow: var(--shadow);
      border: 1px solid rgba(255,255,255,.18);
      background: rgba(255,255,255,.03);
      object-fit: cover;
      display:block;
    }

    .brand h1{font-size:16px;margin:0}
    .brand p{margin:0;color:var(--muted);font-size:12px}

    .links{display:flex; gap:14px; flex-wrap:wrap; justify-content:flex-end}
    .links a{
      padding:10px 12px;
      border-radius:999px;
      color:var(--muted);
      border:1px solid transparent;
    }
    .links a:hover{color:var(--text); border-color:var(--border); background: rgba(255,255,255,.04)}
    .cta{
      display:flex; gap:10px; align-items:center; flex-wrap:wrap; justify-content:flex-end;
    }
    .btn{
      display:inline-flex; align-items:center; justify-content:center;
      padding:10px 14px;
      border-radius:999px;
      border:1px solid var(--border);
      background: rgba(255,255,255,.04);
      color:var(--text);
      cursor:pointer;
      transition: transform .06s ease, background .15s ease, border-color .15s ease;
      user-select:none;
      gap:8px;
      font-weight:600;
      font-size:14px;
      white-space:nowrap;
    }
    .btn:hover{background: rgba(255,255,255,.07); border-color: rgba(255,255,255,.18)}
    .btn:active{transform: translateY(1px)}
    .btn.primary{
      background: linear-gradient(135deg, rgba(110,231,255,.20), rgba(167,139,250,.20));
      border-color: rgba(110,231,255,.35);
    }
    .btn.primary:hover{border-color: rgba(110,231,255,.6)}

    .hero{
      padding:54px 0 22px;
      display:grid;
      grid-template-columns: 1.2fr .8fr;
      gap:22px;
      align-items:stretch;
    }
    @media (max-width: 900px){
      .hero{grid-template-columns: 1fr; padding-top:32px}
      .links{display:none}
    }
    .panel{
      background: linear-gradient(180deg, rgba(255,255,255,.04), rgba(255,255,255,.02));
      border:1px solid var(--border);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      overflow:hidden;
    }
    .hero .left{padding:28px}
    .kicker{
      display:inline-flex; gap:8px; align-items:center;
      padding:6px 10px;
      border-radius:999px;
      background: rgba(255,255,255,.06);
      border:1px solid var(--border);
      color:var(--muted);
      font-size:13px;
    }
    .dot{
      width:8px;height:8px;border-radius:99px;
      background: var(--accent);
      box-shadow: 0 0 20px rgba(110,231,255,.5);
    }
    .hero h2{
      font-size:42px;
      line-height:1.05;
      margin:14px 0 10px;
      letter-spacing:-.02em;
    }
    .hero p{color:var(--muted); margin:0 0 16px; font-size:16px}
    .hero .pricePills{
      display:flex; gap:10px; flex-wrap:wrap; margin:18px 0 22px;
    }
    .pill{
      padding:10px 12px;
      border-radius: 14px;
      background: rgba(110,231,255,.08);
      border:1px solid rgba(110,231,255,.18);
      color:var(--text);
      font-weight:700;
      font-size:14px;
    }
    .pill.secondary{
      background: rgba(167,139,250,.08);
      border-color: rgba(167,139,250,.18);
    }
    .heroActions{display:flex; gap:10px; flex-wrap:wrap}
    .right{display:flex; flex-direction:column;}
    .stats{
      padding:22px;
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap:12px;
    }
    .stat{
      padding:14px;
      border-radius:14px;
      border:1px solid var(--border);
      background: rgba(255,255,255,.03);
    }
    .stat .num{font-size:22px; font-weight:800}
    .stat .lab{color:var(--muted); font-size:13px}
    .badgeRow{
      padding:0 22px 22px;
      display:flex; gap:10px; flex-wrap:wrap;
    }
    .badge{
      font-size:12px;
      color:var(--muted);
      border:1px solid var(--border);
      background: rgba(255,255,255,.03);
      padding:8px 10px;
      border-radius:999px;
    }
    section{padding:26px 0}
    .sectionTitle{
      display:flex; justify-content:space-between; align-items:flex-end; gap:16px; flex-wrap:wrap;
      margin-bottom:14px;
    }
    .sectionTitle h3{margin:0; font-size:22px}
    .sectionTitle p{margin:0; color:var(--muted)}
    .grid3{
      display:grid;
      grid-template-columns: repeat(3, 1fr);
      gap:14px;
    }
    @media (max-width: 900px){
      .grid3{grid-template-columns: 1fr}
    }
    .card{
      padding:18px;
      border-radius: var(--radius);
      border:1px solid var(--border);
      background: rgba(255,255,255,.03);
      box-shadow: 0 8px 18px rgba(0,0,0,.25);
    }
    .card h4{margin:0 0 8px; font-size:16px}
    .card p{margin:0; color:var(--muted)}
    .list{
      margin:10px 0 0;
      padding-left:18px;
      color:var(--muted);
    }
    .pricing{
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap:14px;
    }
    @media (max-width: 900px){
      .pricing{grid-template-columns:1fr}
    }
    .priceCard{
      padding:20px;
      border-radius: var(--radius);
      border:1px solid var(--border);
      background: linear-gradient(180deg, rgba(255,255,255,.05), rgba(255,255,255,.02));
      position:relative;
      overflow:hidden;
    }
    .priceCard:before{
      content:"";
      position:absolute;
      width:280px;height:280px;
      right:-140px; top:-160px;
      background: radial-gradient(circle at 30% 30%, rgba(110,231,255,.28), transparent 60%);
    }
    .priceCard.repair:before{
      background: radial-gradient(circle at 30% 30%, rgba(167,139,250,.28), transparent 60%);
    }
    .priceTop{display:flex; align-items:flex-start; justify-content:space-between; gap:12px}
    .tag{
      font-size:12px;
      color:var(--muted);
      padding:6px 10px;
      border-radius:999px;
      border:1px solid var(--border);
      background: rgba(255,255,255,.03);
      white-space:nowrap;
    }
    .bigPrice{
      font-size:34px;
      font-weight:900;
      letter-spacing:-.02em;
      margin:8px 0 6px;
    }
    .small{color:var(--muted); margin:0}
    .divider{height:1px; background:var(--border); margin:16px 0}
    .twoCol{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:14px;
    }
    @media (max-width: 900px){.twoCol{grid-template-columns:1fr}}
    form{
      display:grid;
      gap:12px;
      padding:18px;
      border-radius: var(--radius);
      border:1px solid var(--border);
      background: rgba(255,255,255,.03);
    }
    label{font-size:13px; color:var(--muted)}
    input, select, textarea{
      width:100%;
      padding:12px 12px;
      border-radius:14px;
      border:1px solid rgba(255,255,255,.14);
      background: rgba(11,15,20,.55);
      color:var(--text);
      outline:none;
      font-size:14px;
    }
    input:focus, select:focus, textarea:focus{
      border-color: rgba(110,231,255,.55);
      box-shadow: 0 0 0 4px rgba(110,231,255,.10);
    }
    textarea{min-height:110px; resize:vertical}
    .formRow{display:grid; grid-template-columns:1fr 1fr; gap:12px}
    @media (max-width: 650px){.formRow{grid-template-columns:1fr}}
    .notice{
      padding:12px 14px;
      border-radius:14px;
      border:1px dashed rgba(255,255,255,.18);
      background: rgba(255,255,255,.03);
      color:var(--muted);
      font-size:13px;
    }
    .success{
      border-style: solid;
      border-color: rgba(110,231,255,.35);
      color: var(--text);
      background: rgba(110,231,255,.08);
    }
    footer{
      padding:34px 0;
      border-top:1px solid var(--border);
      color:var(--muted);
    }
    .footerGrid{
      display:grid;
      grid-template-columns: 1.2fr .8fr;
      gap:14px;
    }
    @media (max-width: 900px){.footerGrid{grid-template-columns:1fr}}
    .miniLinks{display:flex; gap:10px; flex-wrap:wrap}

    /* ✅ mini links tighter pills */
    .miniLinks a{
      color:var(--muted);
      padding:6px 8px;
      border-radius:999px;
      border:1px solid transparent;
      font-size:13px;
      line-height:1.1;
    }
    .miniLinks a:hover{border-color:var(--border); color:var(--text); background: rgba(255,255,255,.04)}
    .tiny{font-size:12px}
    .highlight{
      background: linear-gradient(135deg, rgba(110,231,255,.28), rgba(167,139,250,.28));
      -webkit-background-clip: text;
      background-clip:text;
      color: transparent;
    }
  </style>
</head>
<body>

<header>
  <div class="wrap">
    <div class="nav">
      <a class="brand" href="#top" aria-label="Light and Memory Audio Home">
        <img class="logoImg" alt="Light and Memory Audio logo"
             src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAASABIAAD/4QCMRXhpZgAATU0AKgAAAAgABQESAAMAAAABAAEAAAEaAAUAAAABAAAASgEbAAUAAAABAAAAUgEoAAMAAAABAAIAAAExAAIAAAAQAAAAWgEyAAIAAAAUAAAAagITAAMAAAABAAEAAIdpAAQAAAABAAAAfgAAAAAAAAAASAAAAAEAAABIAAAAAf/bAEMABQYFBQYGBQYGBggHBwYIChAKCgkJChQODwwQFxQYGBcUFhYaHSUfGhsjHBYWICwgIyYnKSopGR8tMC0oMCUoKSj/2wBDAQYGBgoIChMKChMoGhYaKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCj/wAARCADIAyADASIAAhEBAxEB/8QAHwAAAQUBAQEBAQEAAAAAAAAAAAECAwQFBgcICQoL/8QAtRAAAgEDAwIEAwUFBAQAAAF9AQIDAAQRBRIhMUEGE1FhByJxFDKBkaEII0KxwRVS0fAkM2JyggkKFhcYGRolJicoKSo0NTY3ODk6Q0RFRkdISUpTVFVWV1hZWmNkZWZnaGlqc3R1dnd4eXqDhIWGh4iJipKTlJWWl5iZmqKjpKWmp6ipqrKztLW2t7i5usLDxMXGx8jJytLT1NXW19jZ2uHi4+Tl5ufo6erx8vP09fb3+Pn6/8QAHwEAAwEBAQEBAQEBAQAAAAAAAAECAwQFBgcICQoL/8QAtREAAgECBAQDBAcFBAQAAQJ3AAECAxEEBSExBhJBUQdhcRMiMoEIFEKRobHBCSMzUvAVYnLRChYkNOEl8RcYGRomJygpKjU2Nzg5OkNERUZHSElKU1RVVldYWVpjZGVmZ2hpanN0dXZ3eHl6goOEhYaHiImKkpOUlZaXmJmaoqOkpaanqKmqsrO0tba3uLm6wsPExcbHyMnK0tPU1dbX2Nna4uPk5ebn6Onq8vP09fb3+Pn6/9oADAMBAAIRAxEAPwD5qooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooor/9k=" />
        <div>
          <h1>Light and Memory Audio</h1>
          <p>Setups. Repairs. Pro feel.</p>
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
        <a class="btn" id="callBtn" href="tel:+18055551234" title="Call">📞 Call</a>
        <a class="btn" id="textBtn" href="sms:+18055551234" title="Text">💬 Text</a>
        <a class="btn" id="igBtn" href="https://www.instagram.com/light_and_memory_audio?igsh=NTc4MTIwNjQ2YQ%3D%3D&utm_source=qr" target="_blank" rel="noopener noreferrer" title="Instagram">📷 Instagram</a>
        <a class="btn primary" href="#booking">Book Now</a>
      </div>
    </div>
  </div>
</header>

<main id="top" class="wrap">

  <section class="hero" aria-label="Hero">
    <div class="panel left">
      <span class="kicker"><span class="dot" aria-hidden="true"></span> Fast turnaround • Detailed work • Honest pricing</span>
      <h2>Make your guitar feel <span class="highlight">effortless</span> again.</h2>
      <p>
        Setups and repairs focused on playability, tuning stability, and a clean professional finish.
        Bring in your electric, acoustic, or bass — leave with a guitar that feels brand new.
      </p>

      <div class="pricePills" aria-label="Pricing highlights">
        <div class="pill">Service Fee: $50</div>
        <div class="pill secondary">Materials/Parts: Not Included</div>
      </div>

      <div class="heroActions">
        <a class="btn primary" href="#booking">📅 Book an appointment</a>
        <a class="btn" href="#pricing">View pricing</a>
      </div>

      <div class="divider"></div>

      <p class="small">
        <strong>Service area:</strong> <span id="locationText">Simi Valley / Moorpark / Northridge / Thousand Oaks / Santa Clarita / Porter Ranch</span> •
        <strong>Hours:</strong> <span id="hoursText">By appointment (update this)</span>
      </p>
    </div>

    <aside class="panel right" aria-label="Quick info">
      <div class="stats">
        <div class="stat">
          <div class="num">Setup-first</div>
          <div class="lab">Playability & tuning stability</div>
        </div>
        <div class="stat">
          <div class="num">Clean work</div>
          <div class="lab">No shortcuts • No guesswork</div>
        </div>
        <div class="stat">
          <div class="num">Transparent</div>
          <div class="lab">You’ll know the cost before we proceed</div>
        </div>
        <div class="stat">
          <div class="num">All styles</div>
          <div class="lab">Electric • Acoustic • Bass</div>
        </div>
      </div>
      <div class="badgeRow" aria-label="Highlights">
        <span class="badge">Intonation + action</span>
        <span class="badge">Nut + saddle tweaks</span>
        <span class="badge">Electronics repairs</span>
        <span class="badge">Pickup swaps</span>
        <span class="badge">String changes</span>
      </div>
    </aside>
  </section>

  <section id="services" aria-label="Services">
    <div class="sectionTitle">
      <div>
        <h3>Services</h3>
        <p>Focused, practical work that makes a difference the moment you play.</p>
      </div>
    </div>

    <div class="grid3">
      <div class="card">
        <h4>Setups</h4>
        <p>Dialed action, intonation, and feel. Perfect for gigging, studio, or worship rigs.</p>
        <ul class="list">
          <li>Neck relief adjustment</li>
          <li>Action + saddle height</li>
          <li>Intonation</li>
          <li>Basic cleaning + inspection</li>
        </ul>
      </div>

      <div class="card">
        <h4>Repairs</h4>
        <p>Fix common issues quickly with clean, reliable results.</p>
        <ul class="list">
          <li>Electronics troubleshooting</li>
          <li>Jack/pot/switch repair</li>
          <li>Pickup swaps</li>
          <li>Hardware fixes</li>
        </ul>
      </div>

      <div class="card">
        <h4>Ask About</h4>
        <p>Not sure what you need? Describe the problem and I’ll point you to the right service.</p>
        <ul class="list">
          <li>Tuning instability</li>
          <li>Buzzing / dead notes</li>
          <li>Bridge / trem issues</li>
          <li>String gauge changes</li>
        </ul>
      </div>
    </div>

    <div class="notice" style="margin-top:14px">
      <strong>Service limitations:</strong><br>
      At this time, I am limited to certain repairs and setups due to available tools, supplies, and hardware.
      <br><br>
      <strong>Not currently offered:</strong>
      <ul class="list" style="margin-top:8px">
        <li>Fret repair or fretwork</li>
        <li>Structural repairs (neck breaks, cracks, major body damage)</li>
      </ul>
      These services may become available in the future as I continue investing in my own shop and equipment.
    </div>
  </section>

  <section id="pricing" aria-label="Pricing">
    <div class="sectionTitle">
      <div>
        <h3>Pricing</h3>
        <p>Simple and upfront. Materials/parts are not included in the service fee.</p>
      </div>
    </div>

    <div class="pricing">
      <div class="priceCard">
        <div class="priceTop">
          <div>
            <h4 style="margin:0">Service Fee</h4>
            <div class="bigPrice">$50</div>
            <p class="small">Labor/service fee for setups and common repair work (quote confirmed before work).</p>
          </div>
          <div class="tag">Upfront</div>
        </div>
        <div class="divider"></div>
        <ul class="list">
          <li>Setups: relief, action, intonation</li>
          <li>Basic troubleshooting + fixes</li>
          <li>Hardware/electronics labor</li>
        </ul>
        <p class="small" style="margin-top:12px"><strong>Materials/parts not included.</strong> You’ll approve any parts cost before purchase.</p>
        <p class="small" style="margin-top:10px">Note: Fretwork and structural repairs are not currently offered.</p>
      </div>

      <div class="priceCard repair">
        <div class="priceTop">
          <div>
            <h4 style="margin:0">Parts & Materials</h4>
            <div class="bigPrice">Not Included</div>
            <p class="small">Strings, pickups, pots, switches, jacks, hardware, etc. are billed separately.</p>
          </div>
          <div class="tag">Approved First</div>
        </div>
        <div class="divider"></div>
        <ul class="list">
          <li>Strings / consumables</li>
          <li>Pickups + electronics parts</li>
          <li>Hardware replacements</li>
        </ul>
        <p class="small" style="margin-top:12px">If you bring your own parts, I’ll confirm compatibility before install.</p>
      </div>
    </div>
  </section>

  <section id="booking" aria-label="Booking">
    <div class="sectionTitle">
      <div>
        <h3>Book an appointment</h3>
        <p>Fill this out and it’ll open an email with everything formatted. Easy.</p>
      </div>
      <div class="tag">Reply time: same day (update if needed)</div>
    </div>

    <div class="twoCol">
      <form id="bookingForm">
        <div class="formRow">
          <div>
            <label for="name">Name</label>
            <input id="name" name="name" placeholder="Your name" autocomplete="name" required />
          </div>
          <div>
            <label for="phone">Phone</label>
            <input id="phone" name="phone" placeholder="(555) 555-5555" autocomplete="tel" required />
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
              <option value="Service Fee ($50) — Setup">Service Fee ($50) — Setup</option>
              <option value="Service Fee ($50) — Repair / Install">Service Fee ($50) — Repair / Install</option>
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
          <label for="details">What’s going on?</label>
          <textarea id="details" name="details" placeholder="Buzzing on frets 1–5, tuning issues, pickup swap request, preferred string gauge, tuning, etc." required></textarea>
        </div>

        <div class="notice" id="formNotice">
          Tip: Include your string gauge (e.g., 10–46), tuning, and preferences.<br><br>
          <strong>Service fee:</strong> $50 (materials/parts not included).<br>
          <strong>Please note:</strong> Fret repair/fretwork and structural repairs are not currently offered.
        </div>

        <button class="btn primary" type="submit">✉️ Send booking request</button>
        <button class="btn" type="button" id="copyBtn">📋 Copy message</button>

        <p class="tiny" style="margin:0;color:var(--muted)">
          This form uses your email app to send the request (no data stored on the site).
        </p>
      </form>

      <div class="card">
        <h4>Contact</h4>
        <p style="margin-bottom:12px">Update these details in the HTML so customers can reach you.</p>
        <div class="notice">
          <div><strong>Email:</strong> <span id="emailText">youremail@example.com</span></div>
          <div style="margin-top:8px"><strong>Phone:</strong> <span id="phoneText">(805) 555-1234</span></div>
          <div style="margin-top:8px"><strong>Instagram:</strong>
            <a href="https://www.instagram.com/light_and_memory_audio?igsh=NTc4MTIwNjQ2YQ%3D%3D&utm_source=qr" target="_blank" rel="noopener noreferrer" style="text-decoration:underline; text-underline-offset:3px;">
              @light_and_memory_audio
            </a>
          </div>
          <div style="margin-top:8px"><strong>Service area:</strong> <span id="areaText">Simi Valley / Moorpark / Northridge / Thousand Oaks / Santa Clarita / Porter Ranch</span></div>
        </div>

        <div class="divider"></div>

        <h4>What to bring</h4>
        <ul class="list">
          <li>Your guitar + case/bag</li>
          <li>Preferred strings (or ask me to supply)</li>
          <li>Notes on tuning + string gauge</li>
        </ul>

        <div class="divider"></div>

        <h4>Turnaround</h4>
        <p class="small">Setups and common repairs can be quick depending on schedule. Parts availability may affect timing.</p>
      </div>
    </div>
  </section>

  <section id="faq" aria-label="FAQ">
    <div class="sectionTitle">
      <div>
        <h3>FAQ</h3>
        <p>Quick answers to common questions.</p>
      </div>
    </div>

    <div class="grid3">
      <div class="card">
        <h4>Do you work on acoustics?</h4>
        <p>Yes — acoustics, electrics, and bass. If it’s unusual, tell me what it is and I’ll confirm.</p>
      </div>
      <div class="card">
        <h4>Do I need new strings for a setup?</h4>
        <p>Highly recommended. Setups are best when done on the strings you’ll actually play.</p>
      </div>
      <div class="card">
        <h4>Do you do fretwork or structural repairs?</h4>
        <p>Not at this time. Due to current tooling and shop limitations, fret repair/fretwork and structural repairs are not offered. This may change as I continue investing in my own shop.</p>
      </div>
    </div>
  </section>

</main>

<footer>
  <div class="wrap">
    <div class="footerGrid">
      <div>
        <div style="display:flex;align-items:center;gap:10px">
          <img class="logoImg" alt="Light and Memory Audio logo"
               src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAASABIAAD/4QCMRXhpZgAATU0AKgAAAAgABQESAAMAAAABAAEAAAEaAAUAAAABAAAASgEbAAUAAAABAAAAUgEoAAMAAAABAAIAAAExAAIAAAAQAAAAWgEyAAIAAAAUAAAAagITAAMAAAABAAEAAIdpAAQAAAABAAAAfgAAAAAAAAAASAAAAAEAAABIAAAAAf/bAEMABQYFBQYGBQYGBggHBwYIChAKCgkJChQODwwQFxQYGBcUFhYaHSUfGhsjHBYWICwgIyYnKSopGR8tMC0oMCUoKSj/2wBDAQYGBgoIChMKChMoGhYaKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCj/wAARCADIAyADASIAAhEBAxEB/8QAHwAAAQUBAQEBAQEAAAAAAAAAAAECAwQFBgcICQoL/8QAtRAAAgEDAwIEAwUFBAQAAAF9AQIDAAQRBRIhMUEGE1FhByJxFDKBkaEII0KxwRVS0fAkM2JyggkKFhcYGRolJicoKSo0NTY3ODk6Q0RFRkdISUpTVFVWV1hZWmNkZWZnaGlqc3R1dnd4eXqDhIWGh4iJipKTlJWWl5iZmqKjpKWmp6ipqrKztLW2t7i5usLDxMXGx8jJytLT1NXW19jZ2uHi4+Tl5ufo6erx8vP09fb3+Pn6/8QAHwEAAwEBAQEBAQEBAQAAAAAAAAECAwQFBgcICQoL/8QAtREAAgECBAQDBAcFBAQAAQJ3AAECAxEEBSExBhJBUQdhcRMiMoEIFEKRobHBCSMzUvAVYnLRChYkNOEl8RcYGRomJygpKjU2Nzg5OkNERUZHSElKU1RVVldYWVpjZGVmZ2hpanN0dXZ3eHl6goOEhYaHiImKkpOUlZaXmJmaoqOkpaanqKmqsrO0tba3uLm6wsPExcbHyMnK0tPU1dbX2Nna4uPk5ebn6Onq8vP09fb3+Pn6/9oADAMBAAIRAxEAPwD5qooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooor/9k=" />
          <div>
            <strong>Light and Memory Audio</strong>
            <div class="tiny">Service fee: $50 • Materials/parts not included</div>
          </div>
        </div>
        <p class="tiny" style="margin-top:14px">
          © <span id="year"></span> Light and Memory Audio. All rights reserved.
        </p>
      </div>
      <div class="miniLinks">
        <a href="#services">Services</a>
        <a href="#pricing">Pricing</a>
        <a href="#booking">Booking</a>
        <a href="https://www.instagram.com/light_and_memory_audio?igsh=NTc4MTIwNjQ2YQ%3D%3D&utm_source=qr" target="_blank" rel="noopener noreferrer">Instagram</a>
        <a href="#top">Back to top</a>
      </div>
    </div>
  </div>
</footer>

<script>
  // ========= UPDATE THESE DEFAULTS =========
  const BUSINESS_EMAIL = "youremail@example.com";     // <-- put your real email
  const BUSINESS_PHONE = "+18055551234";              // <-- put your real phone (E.164 format works best)
  const SERVICE_AREA   = "Simi Valley / Moorpark / Northridge / Thousand Oaks / Santa Clarita / Porter Ranch";
  const HOURS_TEXT     = "By appointment";            // <-- update

  // ========= Populate contact UI =========
  document.getElementById("year").textContent = new Date().getFullYear();
  document.getElementById("emailText").textContent = BUSINESS_EMAIL;
  document.getElementById("phoneText").textContent = formatPhoneForDisplay(BUSINESS_PHONE) || BUSINESS_PHONE;
  document.getElementById("areaText").textContent = SERVICE_AREA;
  document.getElementById("locationText").textContent = SERVICE_AREA;
  document.getElementById("hoursText").textContent = HOURS_TEXT;

  // update call/text buttons
  const callBtn = document.getElementById("callBtn");
  const textBtn = document.getElementById("textBtn");
  callBtn.href = `tel:${BUSINESS_PHONE}`;
  textBtn.href = `sms:${BUSINESS_PHONE}`;

  // ========= Form handling =========
  const form = document.getElementById("bookingForm");
  const notice = document.getElementById("formNotice");
  const copyBtn = document.getElementById("copyBtn");

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
- Service fee: $50
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
    if(!data.details || data.details.length < 10) return "Please add a little more detail about the issue.";
    return null;
  }

  function setNotice(text, ok=false){
    notice.textContent = text;
    notice.classList.toggle("success", ok);
  }

  form.addEventListener("submit", (e) => {
    e.preventDefault();
    const data = getFormData();
    const err = validate(data);
    if(err){
      setNotice(err, false);
      return;
    }
    const msg = buildMessage(data);

    const mailto = `mailto:${encodeURIComponent(BUSINESS_EMAIL)}?subject=${encodeURIComponent(msg.subject)}&body=${encodeURIComponent(msg.body)}`;
    setNotice("Opening your email app now… If it doesn’t open, click “Copy message” and text/email it to me.", true);
    window.location.href = mailto;
  });

  copyBtn.addEventListener("click", async () => {
    const data = getFormData();
    const err = validate(data);
    if(err){
      setNotice(err, false);
      return;
    }
    const msg = buildMessage(data);
    try{
      await navigator.clipboard.writeText(`Subject: ${msg.subject}\n\n${msg.body}`);
      setNotice("Copied! Paste it into a text or email and send it over.", true);
    }catch{
      setNotice("Couldn’t copy automatically on this device. Select the text in the form and copy manually.", false);
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
