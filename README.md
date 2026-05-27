<!-- ============================================================
     RIIYAD — GitHub Profile README
     Animated SVG + HTML layout (GitHub-safe)
     ============================================================ -->

<div align="center">

<!-- ══════════════════════════════════════════
     ANIMATED HEADER BANNER (SVG)
══════════════════════════════════════════ -->

<svg width="800" height="200" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#030305;stop-opacity:1"/>
      <stop offset="100%" style="stop-color:#0d0d1a;stop-opacity:1"/>
    </linearGradient>
    <linearGradient id="nameGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#ff1f5a"/>
      <stop offset="50%" style="stop-color:#0df5e3"/>
      <stop offset="100%" style="stop-color:#f5d800"/>
      <animateTransform attributeName="gradientTransform" type="translate"
        values="-1 0; 1 0; -1 0" dur="4s" repeatCount="indefinite"/>
    </linearGradient>
    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <filter id="softglow">
      <feGaussianBlur stdDeviation="8" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>

  <rect width="800" height="200" fill="url(#bgGrad)" rx="12"/>

  <!-- Grid lines -->
  <g stroke="#0df5e3" stroke-width="0.3" opacity="0.08">
    <line x1="0" y1="40" x2="800" y2="40"/>
    <line x1="0" y1="80" x2="800" y2="80"/>
    <line x1="0" y1="120" x2="800" y2="120"/>
    <line x1="0" y1="160" x2="800" y2="160"/>
    <line x1="160" y1="0" x2="160" y2="200"/>
    <line x1="320" y1="0" x2="320" y2="200"/>
    <line x1="480" y1="0" x2="480" y2="200"/>
    <line x1="640" y1="0" x2="640" y2="200"/>
  </g>

  <!-- Glow orbs -->
  <circle cx="680" cy="40" r="80" fill="#ff1f5a" opacity="0.07" filter="url(#softglow)">
    <animate attributeName="r" values="80;95;80" dur="5s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.07;0.12;0.07" dur="5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="120" cy="160" r="70" fill="#0df5e3" opacity="0.06" filter="url(#softglow)">
    <animate attributeName="r" values="70;85;70" dur="6s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.06;0.10;0.06" dur="6s" repeatCount="indefinite"/>
  </circle>

  <!-- Corner particles -->
  <circle cx="400" cy="10" r="1.5" fill="#f5d800" opacity="0.4">
    <animate attributeName="cx" values="400;420;400;380;400" dur="8s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.4;0.8;0.4;0.8;0.4" dur="8s" repeatCount="indefinite"/>
  </circle>
  <circle cx="700" cy="100" r="1" fill="#0df5e3" opacity="0.5">
    <animate attributeName="cy" values="100;80;100;120;100" dur="6s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.5;1;0.5;1;0.5" dur="6s" repeatCount="indefinite"/>
  </circle>
  <circle cx="50" cy="100" r="1" fill="#ff1f5a" opacity="0.5">
    <animate attributeName="cy" values="100;120;100;80;100" dur="7s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.5;1;0.5;1;0.5" dur="7s" repeatCount="indefinite"/>
  </circle>

  <!-- Tag label -->
  <rect x="24" y="20" width="130" height="20" rx="2" fill="none" stroke="#0df5e3" stroke-width="0.8" opacity="0.5"/>
  <text x="89" y="34" fill="#0df5e3" font-family="monospace" font-size="9" text-anchor="middle" letter-spacing="3" opacity="0.7">// GITHUB PROFILE</text>

  <!-- "It's Me" -->
  <text x="30" y="90" fill="#50507a" font-family="monospace" font-size="16" letter-spacing="4" font-weight="300">It's Me</text>

  <!-- RIIYAD name -->
  <text x="28" y="155" fill="url(#nameGrad)" font-family="monospace" font-size="72" font-weight="900"
        letter-spacing="-2" filter="url(#glow)">RIIYAD</text>

  <!-- Shadow/echo text -->
  <text x="30" y="157" fill="#ff1f5a" font-family="monospace" font-size="72" font-weight="900"
        letter-spacing="-2" opacity="0.07">RIIYAD</text>

  <!-- Emojis -->
  <text x="530" y="155" font-size="52">🤡💋</text>

  <!-- Scanline sweep -->
  <rect x="0" y="0" width="800" height="3" fill="#0df5e3" opacity="0.06" rx="1">
    <animateTransform attributeName="transform" type="translate"
      values="0,-3; 0,203; 0,-3" dur="5s" repeatCount="indefinite"/>
  </rect>

  <!-- Horizontal glitch lines -->
  <rect x="0" y="60" width="800" height="1" fill="#ff1f5a" opacity="0">
    <animate attributeName="opacity" values="0;0;0;0.15;0;0;0;0.08;0;0" dur="7s" repeatCount="indefinite"/>
    <animate attributeName="y" values="60;60;60;62;60;60;60;58;60;60" dur="7s" repeatCount="indefinite"/>
  </rect>
  <rect x="0" y="130" width="800" height="1" fill="#0df5e3" opacity="0">
    <animate attributeName="opacity" values="0;0;0.12;0;0;0;0.06;0;0;0" dur="9s" repeatCount="indefinite"/>
  </rect>

  <!-- Status dots bottom right -->
  <circle cx="730" cy="175" r="4" fill="#ff1f5a">
    <animate attributeName="opacity" values="1;0.2;1" dur="2s" repeatCount="indefinite"/>
  </circle>
  <text x="742" y="179" fill="#50507a" font-family="monospace" font-size="9" letter-spacing="1">ACTIVE</text>

  <!-- Bottom right corner decoration -->
  <rect x="770" y="10" width="20" height="1" fill="#f5d800" opacity="0.3"/>
  <rect x="789" y="10" width="1" height="20" fill="#f5d800" opacity="0.3"/>
  <rect x="10" y="185" width="20" height="1" fill="#0df5e3" opacity="0.3"/>
  <rect x="10" y="165" width="1" height="20" fill="#0df5e3" opacity="0.3"/>
</svg>

<!-- ══════════════════════════════════════════
     ANIMATED TAGLINE SVG
══════════════════════════════════════════ -->

<svg width="800" height="60" xmlns="http://www.w3.org/2000/svg">
  <rect width="800" height="60" fill="#030305"/>
  <!-- typing cursor line -->
  <rect x="30" y="14" width="740" height="1" fill="#0df5e3" opacity="0.04"/>
  <text x="400" y="28" fill="#50507a" font-family="monospace" font-size="11"
        text-anchor="middle" letter-spacing="2">
    Just existing on the internet — everywhere yet nowhere.
    <animate attributeName="opacity" values="0;1;1;1" dur="2s" fill="freeze"/>
  </text>
  <text x="400" y="48" fill="#2a2a4a" font-family="monospace" font-size="10"
        text-anchor="middle" letter-spacing="2">
    Don't search too hard, you might find me.
    <animate attributeName="opacity" values="0;0;1;1" dur="3s" fill="freeze"/>
  </text>
</svg>

<br>

<!-- ══════════════════════════════════════════
     STATUS BADGES
══════════════════════════════════════════ -->

![](https://img.shields.io/badge/●%20ACTIVE-online-ff1f5a?style=flat-square&labelColor=0d0d14&color=ff1f5a)
&nbsp;
![](https://img.shields.io/badge/◈%20RESTRICTED-access%20denied-f5d800?style=flat-square&labelColor=0d0d14&color=f5d800)
&nbsp;
![](https://img.shields.io/badge/◌%20UNTRACEABLE-ghost%20mode-0df5e3?style=flat-square&labelColor=0d0d14&color=0df5e3)

<br><br>

</div>

---

<!-- ══════════════════════════════════════════
     TELEGRAM SECTION
══════════════════════════════════════════ -->

<div align="center">

<svg width="760" height="44" xmlns="http://www.w3.org/2000/svg">
  <rect width="760" height="44" fill="#030305"/>
  <line x1="0" y1="43" x2="760" y2="43" stroke="#161628" stroke-width="1"/>
  <text x="0" y="16" fill="#ff1f5a" font-family="monospace" font-size="8" letter-spacing="5" font-weight="bold">TELEGRAM</text>
  <line x1="88" y1="12" x2="760" y2="12" stroke="#161628" stroke-width="1">
    <animate attributeName="x2" values="88;760;760" dur="1.5s" fill="freeze"/>
  </line>
  <rect x="92" y="6" width="6" height="12" fill="#ff1f5a" opacity="0.7">
    <animate attributeName="opacity" values="0.7;0;0.7" dur="1s" repeatCount="indefinite"/>
  </rect>
</svg>

<br>

<table>
<tr>
<td align="center" width="360">

<svg width="320" height="72" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="tgCard1" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#080810"/>
      <stop offset="100%" style="stop-color:#0a0a18"/>
    </linearGradient>
  </defs>
  <rect width="320" height="72" fill="url(#tgCard1)" rx="6" stroke="#161628" stroke-width="1"/>
  <!-- Animated border glow -->
  <rect width="320" height="72" rx="6" fill="none" stroke="#0088cc" stroke-width="0" opacity="0">
    <animate attributeName="stroke-width" values="0;1.5;0" dur="3s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0;0.4;0" dur="3s" repeatCount="indefinite"/>
  </rect>
  <!-- Top accent line -->
  <rect x="6" y="2" width="308" height="1" rx="1" fill="#0088cc" opacity="0.2"/>
  <!-- Icon bg -->
  <circle cx="36" cy="36" r="18" fill="#0088cc" opacity="0.15"/>
  <circle cx="36" cy="36" r="18" fill="none" stroke="#0088cc" stroke-width="0.5" opacity="0.3">
    <animate attributeName="r" values="18;22;18" dur="3s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.3;0;0.3" dur="3s" repeatCount="indefinite"/>
  </circle>
  <text x="36" y="42" font-size="18" text-anchor="middle">✈️</text>
  <!-- Text -->
  <text x="64" y="28" fill="#d8d8ee" font-family="monospace" font-size="13" font-weight="bold">@zerox6t9</text>
  <text x="64" y="46" fill="#50507a" font-family="monospace" font-size="9" letter-spacing="2">PRIMARY ACCOUNT</text>
  <!-- Badge -->
  <rect x="64" y="54" width="60" height="12" rx="2" fill="#0088cc" opacity="0.12"/>
  <text x="94" y="63" fill="#0088cc" font-family="monospace" font-size="7" text-anchor="middle" letter-spacing="1">TELEGRAM</text>
  <!-- Arrow -->
  <text x="290" y="40" fill="#0df5e3" font-family="monospace" font-size="14" opacity="0.6">→</text>
</svg>

**[→ Open @zerox6t9](https://t.me/zerox6t9)**

</td>
<td align="center" width="360">

<svg width="320" height="72" xmlns="http://www.w3.org/2000/svg">
  <rect width="320" height="72" fill="#080810" rx="6" stroke="#161628" stroke-width="1"/>
  <rect width="320" height="72" rx="6" fill="none" stroke="#0088cc" stroke-width="0" opacity="0">
    <animate attributeName="stroke-width" values="0;1.5;0" dur="3s" begin="1.5s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0;0.4;0" dur="3s" begin="1.5s" repeatCount="indefinite"/>
  </rect>
  <rect x="6" y="2" width="308" height="1" rx="1" fill="#0088cc" opacity="0.2"/>
  <circle cx="36" cy="36" r="18" fill="#0088cc" opacity="0.12"/>
  <circle cx="36" cy="36" r="18" fill="none" stroke="#0088cc" stroke-width="0.5" opacity="0.3">
    <animate attributeName="r" values="18;22;18" dur="3s" begin="1.5s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.3;0;0.3" dur="3s" begin="1.5s" repeatCount="indefinite"/>
  </circle>
  <text x="36" y="42" font-size="18" text-anchor="middle">✈️</text>
  <text x="64" y="28" fill="#d8d8ee" font-family="monospace" font-size="13" font-weight="bold">@o0oeveo0o</text>
  <text x="64" y="46" fill="#50507a" font-family="monospace" font-size="9" letter-spacing="2">SECONDARY ACCOUNT</text>
  <rect x="64" y="54" width="60" height="12" rx="2" fill="#0088cc" opacity="0.12"/>
  <text x="94" y="63" fill="#0088cc" font-family="monospace" font-size="7" text-anchor="middle" letter-spacing="1">TELEGRAM</text>
  <text x="290" y="40" fill="#0df5e3" font-family="monospace" font-size="14" opacity="0.6">→</text>
</svg>

**[→ Open @o0oeveo0o](https://t.me/o0oeveo0o)**

</td>
</tr>
</table>

</div>

<br>

---

<!-- ══════════════════════════════════════════
     RESTRICTED SOCIALS
══════════════════════════════════════════ -->

<div align="center">

<svg width="760" height="44" xmlns="http://www.w3.org/2000/svg">
  <rect width="760" height="44" fill="#030305"/>
  <text x="0" y="16" fill="#f5d800" font-family="monospace" font-size="8" letter-spacing="5" font-weight="bold">OTHER SOCIALS</text>
  <line x1="126" y1="12" x2="760" y2="12" stroke="#161628" stroke-width="1">
    <animate attributeName="x2" values="126;760;760" dur="1.5s" fill="freeze"/>
  </line>
  <!-- Blinking cursor -->
  <rect x="130" y="6" width="6" height="12" fill="#f5d800" opacity="0.7">
    <animate attributeName="opacity" values="0.7;0;0.7" dur="1s" repeatCount="indefinite"/>
  </rect>
</svg>

<br>

<table>
<tr>
<td align="center" width="360">

<svg width="320" height="72" xmlns="http://www.w3.org/2000/svg">
  <rect width="320" height="72" fill="#080810" rx="6" stroke="#161628" stroke-width="1"/>
  <rect width="320" height="72" rx="6" fill="none" stroke="#f5d800" stroke-width="0.5" opacity="0.15"/>
  <!-- Warning pulse -->
  <rect width="320" height="72" rx="6" fill="none" stroke="#f5d800" stroke-width="0" opacity="0">
    <animate attributeName="stroke-width" values="0;1;0" dur="4s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0;0.2;0" dur="4s" repeatCount="indefinite"/>
  </rect>
  <circle cx="36" cy="36" r="18" fill="#1877f2" opacity="0.12"/>
  <text x="36" y="43" font-size="20" text-anchor="middle" font-family="serif" font-weight="bold" fill="#1877f2">𝒇</text>
  <text x="64" y="28" fill="#d8d8ee" font-family="monospace" font-size="13" font-weight="bold">Facebook</text>
  <rect x="64" y="36" width="88" height="18" rx="2" fill="#f5d80015" stroke="#f5d800" stroke-width="0.6"/>
  <text x="108" y="49" fill="#f5d800" font-family="monospace" font-size="8" text-anchor="middle" letter-spacing="1">🔒 RESTRICTED</text>
  <!-- Lock blink -->
  <rect x="64" y="36" width="88" height="18" rx="2" fill="#f5d800" opacity="0">
    <animate attributeName="opacity" values="0;0;0;0.05;0;0;0" dur="5s" repeatCount="indefinite"/>
  </rect>
</svg>

</td>
<td align="center" width="360">

<svg width="320" height="72" xmlns="http://www.w3.org/2000/svg">
  <rect width="320" height="72" fill="#080810" rx="6" stroke="#161628" stroke-width="1"/>
  <rect width="320" height="72" rx="6" fill="none" stroke="#f5d800" stroke-width="0.5" opacity="0.15"/>
  <rect width="320" height="72" rx="6" fill="none" stroke="#f5d800" stroke-width="0" opacity="0">
    <animate attributeName="stroke-width" values="0;1;0" dur="4s" begin="2s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0;0.2;0" dur="4s" begin="2s" repeatCount="indefinite"/>
  </rect>
  <circle cx="36" cy="36" r="18" fill="#e1306c" opacity="0.12"/>
  <text x="36" y="43" font-size="20" text-anchor="middle">📷</text>
  <text x="64" y="28" fill="#d8d8ee" font-family="monospace" font-size="13" font-weight="bold">Other Socials</text>
  <rect x="64" y="36" width="88" height="18" rx="2" fill="#f5d80015" stroke="#f5d800" stroke-width="0.6"/>
  <text x="108" y="49" fill="#f5d800" font-family="monospace" font-size="8" text-anchor="middle" letter-spacing="1">🔒 RESTRICTED</text>
</svg>

</td>
</tr>
</table>

</div>

<br>

---

<!-- ══════════════════════════════════════════
     DIVIDER — reach me via
══════════════════════════════════════════ -->

<div align="center">

<svg width="760" height="30" xmlns="http://www.w3.org/2000/svg">
  <rect width="760" height="30" fill="#030305"/>
  <line x1="0" y1="15" x2="310" y2="15" stroke="#161628" stroke-width="1"/>
  <text x="380" y="19" fill="#2a2a4a" font-family="monospace" font-size="9" text-anchor="middle" letter-spacing="3">// reach me via</text>
  <line x1="450" y1="15" x2="760" y2="15" stroke="#161628" stroke-width="1"/>
  <!-- Animated dots on divider -->
  <circle cx="380" cy="15" r="2" fill="#0df5e3" opacity="0">
    <animate attributeName="cx" values="0;760" dur="6s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0;0.5;0" dur="6s" repeatCount="indefinite"/>
  </circle>
</svg>

</div>

---

<!-- ══════════════════════════════════════════
     EMAIL SECTION
══════════════════════════════════════════ -->

<div align="center">

<svg width="760" height="44" xmlns="http://www.w3.org/2000/svg">
  <rect width="760" height="44" fill="#030305"/>
  <text x="0" y="16" fill="#ff1f5a" font-family="monospace" font-size="8" letter-spacing="5" font-weight="bold">EMAIL</text>
  <line x1="55" y1="12" x2="760" y2="12" stroke="#161628" stroke-width="1">
    <animate attributeName="x2" values="55;760;760" dur="1.5s" fill="freeze"/>
  </line>
  <rect x="59" y="6" width="6" height="12" fill="#ff1f5a" opacity="0.7">
    <animate attributeName="opacity" values="0.7;0;0.7" dur="1s" repeatCount="indefinite"/>
  </rect>
</svg>

<br>

<table>
<tr>
<td align="center" width="360">

<svg width="320" height="80" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="mailGrad1" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0d0410"/>
      <stop offset="100%" style="stop-color:#080810"/>
    </linearGradient>
  </defs>
  <rect width="320" height="80" fill="url(#mailGrad1)" rx="6" stroke="#1e0a1a" stroke-width="1"/>
  <rect width="320" height="80" rx="6" fill="none" stroke="#ff1f5a" stroke-width="0" opacity="0">
    <animate attributeName="stroke-width" values="0;1;0" dur="4s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0;0.35;0" dur="4s" repeatCount="indefinite"/>
  </rect>
  <!-- Top accent -->
  <rect x="6" y="2" width="80" height="1" rx="1" fill="#ff1f5a" opacity="0.4"/>
  <!-- Icon -->
  <circle cx="36" cy="40" r="18" fill="#ff1f5a" opacity="0.1"/>
  <circle cx="36" cy="40" r="18" fill="none" stroke="#ff1f5a" stroke-width="0.5" opacity="0.2">
    <animate attributeName="r" values="18;23;18" dur="4s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.2;0;0.2" dur="4s" repeatCount="indefinite"/>
  </circle>
  <text x="36" y="46" font-size="18" text-anchor="middle">✉️</text>
  <!-- Text -->
  <text x="64" y="30" fill="#d8d8ee" font-family="monospace" font-size="11" font-weight="bold">riadalhasan91@gmail.com</text>
  <text x="64" y="46" fill="#50507a" font-family="monospace" font-size="9" letter-spacing="2">GMAIL · PRIMARY</text>
  <rect x="64" y="54" width="50" height="14" rx="2" fill="#ff1f5a" opacity="0.12"/>
  <text x="89" y="64" fill="#ff1f5a" font-family="monospace" font-size="7" text-anchor="middle" letter-spacing="1">PRIMARY</text>
  <text x="295" y="44" fill="#0df5e3" font-family="monospace" font-size="14" opacity="0.5">→</text>
</svg>

**[✉ riadalhasan91@gmail.com](mailto:riadalhasan91@gmail.com)**

</td>
<td align="center" width="360">

<svg width="320" height="80" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="mailGrad2" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#040d10"/>
      <stop offset="100%" style="stop-color:#080810"/>
    </linearGradient>
  </defs>
  <rect width="320" height="80" fill="url(#mailGrad2)" rx="6" stroke="#0a1e1e" stroke-width="1"/>
  <rect width="320" height="80" rx="6" fill="none" stroke="#0df5e3" stroke-width="0" opacity="0">
    <animate attributeName="stroke-width" values="0;1;0" dur="4s" begin="2s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0;0.3;0" dur="4s" begin="2s" repeatCount="indefinite"/>
  </rect>
  <rect x="234" y="2" width="80" height="1" rx="1" fill="#0df5e3" opacity="0.4"/>
  <circle cx="36" cy="40" r="18" fill="#0df5e3" opacity="0.08"/>
  <circle cx="36" cy="40" r="18" fill="none" stroke="#0df5e3" stroke-width="0.5" opacity="0.2">
    <animate attributeName="r" values="18;23;18" dur="4s" begin="2s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.2;0;0.2" dur="4s" begin="2s" repeatCount="indefinite"/>
  </circle>
  <text x="36" y="46" font-size="18" text-anchor="middle">📬</text>
  <text x="64" y="30" fill="#d8d8ee" font-family="monospace" font-size="11" font-weight="bold">riadalhasan9t5@outlook.com</text>
  <text x="64" y="46" fill="#50507a" font-family="monospace" font-size="9" letter-spacing="2">OUTLOOK · BACKUP</text>
  <rect x="64" y="54" width="50" height="14" rx="2" fill="#0df5e3" opacity="0.08"/>
  <text x="89" y="64" fill="#0df5e3" font-family="monospace" font-size="7" text-anchor="middle" letter-spacing="1">BACKUP</text>
  <text x="295" y="44" fill="#0df5e3" font-family="monospace" font-size="14" opacity="0.5">→</text>
</svg>

**[✉ riadalhasan9t5@outlook.com](mailto:riadalhasan9t5@outlook.com)**

</td>
</tr>
</table>

</div>

<br>

---

<!-- ══════════════════════════════════════════
     ANIMATED FOOTER BANNER
══════════════════════════════════════════ -->

<div align="center">

<svg width="760" height="80" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="footerBg" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#030305"/>
      <stop offset="50%" style="stop-color:#080810"/>
      <stop offset="100%" style="stop-color:#030305"/>
    </linearGradient>
    <linearGradient id="footerText" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#ff1f5a">
        <animate attributeName="stop-color" values="#ff1f5a;#0df5e3;#f5d800;#ff1f5a" dur="6s" repeatCount="indefinite"/>
      </stop>
      <stop offset="100%" style="stop-color:#0df5e3">
        <animate attributeName="stop-color" values="#0df5e3;#f5d800;#ff1f5a;#0df5e3" dur="6s" repeatCount="indefinite"/>
      </stop>
    </linearGradient>
  </defs>
  <rect width="760" height="80" fill="url(#footerBg)" rx="8"/>
  <line x1="0" y1="1" x2="760" y2="1" stroke="#ff1f5a" stroke-width="0.5" opacity="0.4"/>
  <line x1="0" y1="79" x2="760" y2="79" stroke="#0df5e3" stroke-width="0.5" opacity="0.2"/>

  <!-- Corner brackets -->
  <rect x="8" y="8" width="16" height="1" fill="#ff1f5a" opacity="0.4"/>
  <rect x="8" y="8" width="1" height="16" fill="#ff1f5a" opacity="0.4"/>
  <rect x="736" y="8" width="16" height="1" fill="#0df5e3" opacity="0.4"/>
  <rect x="751" y="8" width="1" height="16" fill="#0df5e3" opacity="0.4"/>
  <rect x="8" y="71" width="16" height="1" fill="#0df5e3" opacity="0.4"/>
  <rect x="8" y="55" width="1" height="16" fill="#0df5e3" opacity="0.4"/>
  <rect x="736" y="71" width="16" height="1" fill="#ff1f5a" opacity="0.4"/>
  <rect x="751" y="55" width="1" height="16" fill="#ff1f5a" opacity="0.4"/>

  <!-- Particles -->
  <circle cx="100" cy="40" r="1.5" fill="#ff1f5a" opacity="0.5">
    <animate attributeName="cy" values="40;20;40" dur="3s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.5;0;0.5" dur="3s" repeatCount="indefinite"/>
  </circle>
  <circle cx="660" cy="40" r="1.5" fill="#0df5e3" opacity="0.5">
    <animate attributeName="cy" values="40;60;40" dur="4s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.5;0;0.5" dur="4s" repeatCount="indefinite"/>
  </circle>
  <circle cx="380" cy="20" r="1" fill="#f5d800" opacity="0.4">
    <animate attributeName="cy" values="20;60;20" dur="5s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.4;0;0.4" dur="5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="200" cy="60" r="1" fill="#f5d800" opacity="0.3">
    <animate attributeName="cx" values="200;560;200" dur="8s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.3;0.6;0.3" dur="8s" repeatCount="indefinite"/>
  </circle>

  <text x="380" y="38" fill="url(#footerText)" font-family="monospace" font-size="16"
        font-weight="bold" text-anchor="middle" letter-spacing="3">
    Crafted with chaos by RIIYAD
  </text>
  <text x="380" y="58" fill="#2a2a4a" font-family="monospace" font-size="9"
        text-anchor="middle" letter-spacing="4">
    © All rights restricted. &nbsp; 🤡💋
  </text>
</svg>

</div>
