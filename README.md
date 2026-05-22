<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>RIIYAD — Profile</title>
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;600;700;800&family=Space+Mono:ital,wght@0,400;0,700;1,400&display=swap" rel="stylesheet">
<style>
  :root {
    --bg: #050508;
    --surface: #0d0d14;
    --border: #1e1e2e;
    --accent1: #ff2d6b;
    --accent2: #00f0ff;
    --accent3: #ffe44d;
    --text: #e8e8f0;
    --muted: #6666aa;
    --glow1: rgba(255,45,107,0.35);
    --glow2: rgba(0,240,255,0.25);
  }

  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  html { scroll-behavior: smooth; }

  body {
    background: var(--bg);
    color: var(--text);
    font-family: 'Space Mono', monospace;
    min-height: 100vh;
    overflow-x: hidden;
    cursor: none;
  }

  /* ── Custom Cursor ── */
  .cursor-dot {
    position: fixed; top: 0; left: 0; z-index: 9999;
    width: 8px; height: 8px; border-radius: 50%;
    background: var(--accent1);
    pointer-events: none;
    transform: translate(-50%,-50%);
    transition: width .15s, height .15s, background .15s;
    mix-blend-mode: screen;
  }
  .cursor-ring {
    position: fixed; top: 0; left: 0; z-index: 9998;
    width: 36px; height: 36px; border-radius: 50%;
    border: 1.5px solid var(--accent2);
    pointer-events: none;
    transform: translate(-50%,-50%);
    transition: transform .08s ease, width .2s, height .2s, border-color .2s;
    mix-blend-mode: screen;
  }
  body:hover .cursor-ring { opacity: 1; }

  /* ── Noise Overlay ── */
  body::before {
    content: '';
    position: fixed; inset: 0; z-index: 0;
    background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='0.04'/%3E%3C/svg%3E");
    pointer-events: none;
    opacity: 0.55;
  }

  /* ── Grid Lines ── */
  body::after {
    content: '';
    position: fixed; inset: 0; z-index: 0;
    background-image:
      linear-gradient(rgba(0,240,255,0.025) 1px, transparent 1px),
      linear-gradient(90deg, rgba(0,240,255,0.025) 1px, transparent 1px);
    background-size: 60px 60px;
    pointer-events: none;
  }

  /* ── Layout ── */
  .page {
    position: relative; z-index: 1;
    max-width: 780px;
    margin: 0 auto;
    padding: 60px 24px 80px;
  }

  /* ── Hero ── */
  .hero {
    position: relative;
    margin-bottom: 64px;
    animation: fadeUp .8s cubic-bezier(.16,1,.3,1) both;
  }

  .hero-tag {
    display: inline-block;
    font-size: 10px;
    letter-spacing: .25em;
    text-transform: uppercase;
    color: var(--accent2);
    border: 1px solid var(--accent2);
    padding: 4px 12px;
    margin-bottom: 24px;
    position: relative;
    overflow: hidden;
  }
  .hero-tag::after {
    content: '';
    position: absolute; top: 0; left: -100%;
    width: 100%; height: 100%;
    background: linear-gradient(90deg, transparent, rgba(0,240,255,.15), transparent);
    animation: shimmer 3s infinite;
  }

  .hero-name {
    font-family: 'Syne', sans-serif;
    font-size: clamp(42px, 10vw, 82px);
    font-weight: 800;
    line-height: .95;
    letter-spacing: -.02em;
    margin-bottom: 20px;
  }
  .hero-name .line1 { display: block; color: var(--text); }
  .hero-name .line2 {
    display: block;
    background: linear-gradient(90deg, var(--accent1) 0%, var(--accent2) 60%, var(--accent3) 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    animation: gradShift 5s ease infinite alternate;
    background-size: 200%;
  }

  .hero-emoji {
    display: inline-block;
    font-style: normal;
    -webkit-text-fill-color: initial;
    animation: bounce 2.5s ease-in-out infinite;
    margin-left: 8px;
  }

  .hero-desc {
    font-size: 13px;
    color: var(--muted);
    line-height: 1.9;
    max-width: 520px;
    border-left: 2px solid var(--accent1);
    padding-left: 18px;
    margin-top: 28px;
  }

  /* ── Status Badge ── */
  .status {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    font-size: 11px;
    color: var(--accent3);
    letter-spacing: .08em;
    margin-top: 22px;
  }
  .status-dot {
    width: 7px; height: 7px;
    border-radius: 50%;
    background: var(--accent3);
    animation: pulse 2s ease-in-out infinite;
  }

  /* ── Section ── */
  .section {
    margin-bottom: 52px;
    animation: fadeUp .8s cubic-bezier(.16,1,.3,1) both;
  }
  .section:nth-child(2) { animation-delay: .1s; }
  .section:nth-child(3) { animation-delay: .18s; }
  .section:nth-child(4) { animation-delay: .26s; }
  .section:nth-child(5) { animation-delay: .34s; }

  .section-label {
    font-size: 9px;
    letter-spacing: .3em;
    text-transform: uppercase;
    color: var(--accent1);
    margin-bottom: 18px;
    display: flex;
    align-items: center;
    gap: 12px;
  }
  .section-label::after {
    content: '';
    flex: 1;
    height: 1px;
    background: linear-gradient(90deg, var(--border), transparent);
  }

  /* ── Social Cards ── */
  .social-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
    gap: 12px;
  }

  .card {
    position: relative;
    background: var(--surface);
    border: 1px solid var(--border);
    padding: 18px 20px;
    text-decoration: none;
    color: var(--text);
    display: flex;
    align-items: center;
    gap: 14px;
    overflow: hidden;
    transition: border-color .25s, transform .25s;
    group: true;
  }
  .card::before {
    content: '';
    position: absolute; inset: 0;
    opacity: 0;
    transition: opacity .3s;
  }
  .card:hover { transform: translateY(-3px); }
  .card:hover::before { opacity: 1; }

  .card.tg::before  { background: linear-gradient(135deg, rgba(0,136,204,.12), transparent); }
  .card.tg:hover    { border-color: #08c; }
  .card.fb::before  { background: linear-gradient(135deg, rgba(24,119,242,.12), transparent); }
  .card.fb:hover    { border-color: #1877f2; }
  .card.mail::before { background: linear-gradient(135deg, rgba(255,45,107,.12), transparent); }
  .card.mail:hover  { border-color: var(--accent1); }
  .card.lock::before { background: linear-gradient(135deg, rgba(255,228,77,.1), transparent); }
  .card.lock:hover  { border-color: var(--accent3); }

  .card-icon {
    font-size: 24px;
    flex-shrink: 0;
    filter: drop-shadow(0 0 6px currentColor);
  }
  .card-body { overflow: hidden; }
  .card-title {
    font-family: 'Syne', sans-serif;
    font-size: 13px;
    font-weight: 700;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
  }
  .card-sub {
    font-size: 10px;
    color: var(--muted);
    margin-top: 2px;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
  }
  .card-arrow {
    margin-left: auto;
    font-size: 14px;
    color: var(--muted);
    transition: transform .2s, color .2s;
    flex-shrink: 0;
  }
  .card:hover .card-arrow { transform: translateX(4px); color: var(--accent2); }

  /* Restricted Badge */
  .badge-restricted {
    display: inline-block;
    font-size: 8px;
    letter-spacing: .12em;
    text-transform: uppercase;
    background: rgba(255,228,77,.12);
    color: var(--accent3);
    border: 1px solid var(--accent3);
    padding: 2px 7px;
    margin-top: 4px;
  }

  /* ── Email Cards ── */
  .email-grid {
    display: grid;
    gap: 10px;
  }

  /* ── Divider ── */
  .divider {
    display: flex;
    align-items: center;
    gap: 16px;
    margin: 48px 0;
    color: var(--muted);
    font-size: 10px;
    letter-spacing: .2em;
  }
  .divider::before, .divider::after {
    content: '';
    flex: 1;
    height: 1px;
    background: var(--border);
  }

  /* ── Footer ── */
  .footer {
    text-align: center;
    font-size: 10px;
    color: var(--muted);
    letter-spacing: .15em;
    padding-top: 40px;
    border-top: 1px solid var(--border);
    animation: fadeUp .8s .4s both;
  }
  .footer span {
    background: linear-gradient(90deg, var(--accent1), var(--accent2));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }

  /* ── Scanline ── */
  .scanline {
    position: fixed;
    top: -100%;
    left: 0;
    width: 100%;
    height: 4px;
    background: linear-gradient(transparent, rgba(0,240,255,.08), transparent);
    animation: scan 6s linear infinite;
    z-index: 2;
    pointer-events: none;
  }

  /* ── Glowing Orbs ── */
  .orb {
    position: fixed;
    border-radius: 50%;
    filter: blur(100px);
    pointer-events: none;
    z-index: 0;
    animation: orbFloat 12s ease-in-out infinite;
  }
  .orb1 {
    width: 400px; height: 400px;
    background: var(--glow1);
    top: -100px; right: -120px;
  }
  .orb2 {
    width: 350px; height: 350px;
    background: var(--glow2);
    bottom: 80px; left: -120px;
    animation-delay: -6s;
  }

  /* ── Keyframes ── */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(30px); }
    to   { opacity: 1; transform: translateY(0); }
  }
  @keyframes gradShift {
    0%   { background-position: 0% 50%; }
    100% { background-position: 100% 50%; }
  }
  @keyframes shimmer {
    0%   { left: -100%; }
    100% { left: 200%; }
  }
  @keyframes pulse {
    0%, 100% { transform: scale(1); opacity: 1; }
    50%       { transform: scale(1.6); opacity: .5; }
  }
  @keyframes bounce {
    0%, 100% { transform: translateY(0); }
    50%       { transform: translateY(-8px); }
  }
  @keyframes scan {
    0%   { top: -4px; }
    100% { top: 100vh; }
  }
  @keyframes orbFloat {
    0%, 100% { transform: translate(0, 0) scale(1); }
    33%       { transform: translate(30px, -20px) scale(1.05); }
    66%       { transform: translate(-20px, 30px) scale(.95); }
  }

  /* ── Typing effect ── */
  .typed-text::after {
    content: '|';
    animation: blink 1s step-end infinite;
    color: var(--accent2);
  }
  @keyframes blink {
    0%, 100% { opacity: 1; } 50% { opacity: 0; }
  }

  /* ── Scrollbar ── */
  ::-webkit-scrollbar { width: 4px; }
  ::-webkit-scrollbar-track { background: var(--bg); }
  ::-webkit-scrollbar-thumb {
    background: linear-gradient(var(--accent1), var(--accent2));
    border-radius: 2px;
  }
</style>
</head>
<body>

<!-- Cursor -->
<div class="cursor-dot" id="dot"></div>
<div class="cursor-ring" id="ring"></div>

<!-- Scan + Orbs -->
<div class="scanline"></div>
<div class="orb orb1"></div>
<div class="orb orb2"></div>

<div class="page">

  <!-- ──────── HERO ──────── -->
  <header class="hero">
    <div class="hero-tag">// GitHub Profile</div>
    <h1 class="hero-name">
      <span class="line1">It's Me</span>
      <span class="line2">RIIYAD<span class="hero-emoji">🤡💋</span></span>
    </h1>
    <p class="hero-desc typed-text">
      Just existing on the internet — everywhere yet nowhere.<br>
      Don't search too hard, you might find me.
    </p>
    <div class="status">
      <span class="status-dot"></span>
      Active · Restricted · Untraceable
    </div>
  </header>

  <!-- ──────── TELEGRAM ──────── -->
  <section class="section">
    <div class="section-label">Telegram</div>
    <div class="social-grid">

      <a class="card tg" href="https://t.me/zerox6t9" target="_blank" rel="noopener">
        <span class="card-icon" style="color:#08c">✈️</span>
        <div class="card-body">
          <div class="card-title">@zerox6t9</div>
          <div class="card-sub">Primary Account</div>
        </div>
        <span class="card-arrow">→</span>
      </a>

      <a class="card tg" href="https://t.me/o0oeveo0o" target="_blank" rel="noopener">
        <span class="card-icon" style="color:#08c">✈️</span>
        <div class="card-body">
          <div class="card-title">@o0oeveo0o</div>
          <div class="card-sub">Secondary Account</div>
        </div>
        <span class="card-arrow">→</span>
      </a>

    </div>
  </section>

  <!-- ──────── FACEBOOK ──────── -->
  <section class="section">
    <div class="section-label">Facebook</div>
    <div class="social-grid">

      <div class="card lock" style="cursor:default;">
        <span class="card-icon" style="color:#1877f2">𝒇</span>
        <div class="card-body">
          <div class="card-title">Facebook</div>
          <div>
            <span class="badge-restricted">🔒 Restricted</span>
          </div>
        </div>
      </div>

      <div class="card lock" style="cursor:default;">
        <span class="card-icon" style="color:#e1306c">📷</span>
        <div class="card-body">
          <div class="card-title">Other Socials</div>
          <div>
            <span class="badge-restricted">🔒 Restricted</span>
          </div>
        </div>
      </div>

    </div>
  </section>

  <div class="divider">// reach me via</div>

  <!-- ──────── EMAIL ──────── -->
  <section class="section">
    <div class="section-label">Email</div>
    <div class="email-grid">

      <a class="card mail" href="mailto:riadalhasan91@gmail.com">
        <span class="card-icon" style="color:var(--accent1)">✉</span>
        <div class="card-body">
          <div class="card-title">riadalhasan91@gmail.com</div>
          <div class="card-sub">Gmail · Primary</div>
        </div>
        <span class="card-arrow">→</span>
      </a>

      <a class="card mail" href="mailto:riadalhasan9t5@outlook.com">
        <span class="card-icon" style="color:var(--accent2)">✉</span>
        <div class="card-body">
          <div class="card-title">riadalhasan9t5@outlook.com</div>
          <div class="card-sub">Outlook · Backup</div>
        </div>
        <span class="card-arrow">→</span>
      </a>

    </div>
  </section>

  <!-- ──────── FOOTER ──────── -->
  <footer class="footer">
    <p>Crafted with chaos by <span>RIIYAD</span> &nbsp;·&nbsp; 🤡💋</p>
    <p style="margin-top:8px; font-size:9px; opacity:.5;">© All rights restricted.</p>
  </footer>

</div><!-- /page -->

<script>
  // ── Custom Cursor ──
  const dot  = document.getElementById('dot');
  const ring = document.getElementById('ring');
  let mx = 0, my = 0, rx = 0, ry = 0;

  document.addEventListener('mousemove', e => { mx = e.clientX; my = e.clientY; });

  function animCursor() {
    dot.style.left  = mx + 'px';
    dot.style.top   = my + 'px';
    rx += (mx - rx) * .12;
    ry += (my - ry) * .12;
    ring.style.left = rx + 'px';
    ring.style.top  = ry + 'px';
    requestAnimationFrame(animCursor);
  }
  animCursor();

  document.querySelectorAll('a, .card').forEach(el => {
    el.addEventListener('mouseenter', () => {
      dot.style.width  = '14px';
      dot.style.height = '14px';
      dot.style.background = 'var(--accent2)';
      ring.style.width  = '50px';
      ring.style.height = '50px';
      ring.style.borderColor = 'var(--accent1)';
    });
    el.addEventListener('mouseleave', () => {
      dot.style.width  = '8px';
      dot.style.height = '8px';
      dot.style.background = 'var(--accent1)';
      ring.style.width  = '36px';
      ring.style.height = '36px';
      ring.style.borderColor = 'var(--accent2)';
    });
  });

  // ── Typing Effect ──
  const target = document.querySelector('.typed-text');
  const fullHTML = target.innerHTML;
  target.innerHTML = '';
  let i = 0, plain = target.closest('.hero').querySelector('.hero-desc');

  // Simple char-by-char for plain text only
  const rawText = `Just existing on the internet — everywhere yet nowhere.\nDon't search too hard, you might find me.`;
  let idx = 0;
  function typeChar() {
    if (idx < rawText.length) {
      if (rawText[idx] === '\n') {
        target.innerHTML += '<br>';
      } else {
        target.innerHTML += rawText[idx];
      }
      idx++;
      setTimeout(typeChar, 28);
    }
  }
  setTimeout(typeChar, 900);

  // ── Card hover glow trace ──
  document.querySelectorAll('.card').forEach(card => {
    card.addEventListener('mousemove', e => {
      const rect = card.getBoundingClientRect();
      const x = e.clientX - rect.left;
      const y = e.clientY - rect.top;
      card.style.setProperty('--mx', x + 'px');
      card.style.setProperty('--my', y + 'px');
    });
  });
</script>
</body>
</html>
