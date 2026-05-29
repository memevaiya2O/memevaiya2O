<!-- ============================================================
       RIIYAD / memevaiya2O — GitHub Profile README
       Full SVG animations (GitHub-safe)
       ============================================================ -->

  <div align="center">

  <!-- ══════════════════════════════════════════
       MAIN HEADER BANNER
  ══════════════════════════════════════════ -->

  <svg width="800" height="220" xmlns="http://www.w3.org/2000/svg">
    <defs>
      <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" style="stop-color:#020408"/>
        <stop offset="100%" style="stop-color:#050916"/>
      </linearGradient>
      <linearGradient id="nameGrad" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%"   style="stop-color:#ff1f5a;stop-opacity:1"/>
        <stop offset="40%"  style="stop-color:#0df5e3;stop-opacity:1"/>
        <stop offset="70%"  style="stop-color:#0df5e3;stop-opacity:1"/>
        <stop offset="100%" style="stop-color:#f5d800;stop-opacity:1"/>
        <animateTransform attributeName="gradientTransform" type="translate"
          values="-0.5 0; 0.5 0; -0.5 0" dur="5s" repeatCount="indefinite"/>
      </linearGradient>
      <linearGradient id="nxtGrad" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%"  style="stop-color:#0df5e3"/>
        <stop offset="100%" style="stop-color:#0088cc"/>
      </linearGradient>
      <filter id="glow"><feGaussianBlur stdDeviation="3" result="b"/><feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge></filter>
      <filter id="glow2"><feGaussianBlur stdDeviation="6" result="b"/><feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge></filter>
      <filter id="softglow"><feGaussianBlur stdDeviation="10" result="b"/><feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge></filter>
    </defs>

    <!-- Background -->
    <rect width="800" height="220" fill="url(#bgGrad)" rx="14"/>

    <!-- Grid lines -->
    <g stroke="#0df5e3" stroke-width="0.25" opacity="0.06">
      <line x1="0" y1="44" x2="800" y2="44"/><line x1="0" y1="88" x2="800" y2="88"/>
      <line x1="0" y1="132" x2="800" y2="132"/><line x1="0" y1="176" x2="800" y2="176"/>
      <line x1="160" y1="0" x2="160" y2="220"/><line x1="320" y1="0" x2="320" y2="220"/>
      <line x1="480" y1="0" x2="480" y2="220"/><line x1="640" y1="0" x2="640" y2="220"/>
    </g>

    <!-- Big glow orbs -->
    <circle cx="660" cy="40" r="100" fill="#ff1f5a" opacity="0.06" filter="url(#softglow)">
      <animate attributeName="r" values="100;120;100" dur="6s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.06;0.10;0.06" dur="6s" repeatCount="indefinite"/>
    </circle>
    <circle cx="100" cy="180" r="85" fill="#0df5e3" opacity="0.05" filter="url(#softglow)">
      <animate attributeName="r" values="85;105;85" dur="7s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.05;0.09;0.05" dur="7s" repeatCount="indefinite"/>
    </circle>
    <circle cx="400" cy="110" r="60" fill="#f5d800" opacity="0.04" filter="url(#softglow)">
      <animate attributeName="r" values="60;75;60" dur="9s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.04;0.07;0.04" dur="9s" repeatCount="indefinite"/>
    </circle>

    <!-- Corner brackets -->
    <g stroke="#0df5e3" stroke-width="1.2" opacity="0.5" fill="none">
      <path d="M8,24 L8,8 L24,8"/>
      <path d="M776,8 L792,8 L792,24"/>
      <path d="M8,196 L8,212 L24,212"/>
      <path d="M776,212 L792,212 L792,196"/>
    </g>

    <!-- Flying particles -->
    <circle cx="200" cy="15" r="1.2" fill="#f5d800" opacity="0.5">
      <animate attributeName="cx" values="200;240;200;160;200" dur="9s" repeatCount="indefinite"/>
      <animate attributeName="cy" values="15;30;15;25;15" dur="9s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.5;1;0.5;0.8;0.5" dur="9s" repeatCount="indefinite"/>
    </circle>
    <circle cx="600" cy="200" r="1.5" fill="#0df5e3" opacity="0.6">
      <animate attributeName="cx" values="600;640;600;560;600" dur="7s" repeatCount="indefinite"/>
      <animate attributeName="cy" values="200;185;200;195;200" dur="7s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.6;1;0.6;0.9;0.6" dur="7s" repeatCount="indefinite"/>
    </circle>
    <circle cx="750" cy="110" r="1" fill="#ff1f5a" opacity="0.6">
      <animate attributeName="cy" values="110;90;110;130;110" dur="8s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.6;1;0.6;1;0.6" dur="8s" repeatCount="indefinite"/>
    </circle>
    <circle cx="50" cy="80" r="1.2" fill="#f5d800" opacity="0.5">
      <animate attributeName="cx" values="50;65;50;38;50" dur="10s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.5;1;0.5;0.8;0.5" dur="10s" repeatCount="indefinite"/>
    </circle>
    <circle cx="400" cy="20" r="1" fill="#ff1f5a" opacity="0.4">
      <animate attributeName="cx" values="400;420;400;380;400" dur="11s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.4;0.9;0.4;0.7;0.4" dur="11s" repeatCount="indefinite"/>
    </circle>

    <!-- "It's Me" subtle label -->
    <text x="30" y="80" fill="#2a2a4a" font-family="monospace" font-size="17" letter-spacing="4" font-weight="300" opacity="0.9">It's Me</text>

    <!-- RIIYAD main name -->
    <text x="28" y="170" fill="url(#nameGrad)" font-family="monospace" font-size="80" font-weight="900"
          letter-spacing="-3" filter="url(#glow)">RIIYAD</text>
    <!-- Echo shadow -->
    <text x="30" y="172" fill="#ff1f5a" font-family="monospace" font-size="80" font-weight="900"
          letter-spacing="-3" opacity="0.05">RIIYAD</text>
    <text x="26" y="168" fill="#0df5e3" font-family="monospace" font-size="80" font-weight="900"
          letter-spacing="-3" opacity="0.05">RIIYAD</text>

    <!-- Emojis -->
    <text x="535" y="168" font-size="58">🤡💋</text>

    <!-- Tag label top-right -->
    <rect x="22" y="22" width="140" height="18" rx="2" fill="none" stroke="#0df5e3" stroke-width="0.7" opacity="0.45"/>
    <text x="92" y="35" fill="#0df5e3" font-family="monospace" font-size="8.5" text-anchor="middle" letter-spacing="3" opacity="0.65">// GITHUB PROFILE</text>

    <!-- Scanline sweep -->
    <rect x="0" y="0" width="800" height="3" fill="#0df5e3" opacity="0.05" rx="1">
      <animateTransform attributeName="transform" type="translate"
        values="0,-3; 0,223; 0,-3" dur="5s" repeatCount="indefinite"/>
    </rect>

    <!-- Glitch lines -->
    <rect x="0" y="70" width="800" height="1" fill="#ff1f5a" opacity="0">
      <animate attributeName="opacity" values="0;0;0;0.18;0;0;0;0.10;0;0" dur="7s" repeatCount="indefinite"/>
      <animate attributeName="y" values="70;70;70;72;70;70;70;68;70;70" dur="7s" repeatCount="indefinite"/>
    </rect>
    <rect x="0" y="140" width="800" height="1" fill="#0df5e3" opacity="0">
      <animate attributeName="opacity" values="0;0;0.14;0;0;0;0.07;0;0;0" dur="9s" repeatCount="indefinite"/>
    </rect>
    <rect x="0" y="100" width="800" height="1.5" fill="#f5d800" opacity="0">
      <animate attributeName="opacity" values="0;0;0;0;0;0.12;0;0;0;0" dur="11s" repeatCount="indefinite"/>
    </rect>

    <!-- Status dots bottom-right -->
    <circle cx="726" cy="192" r="4" fill="#ff1f5a">
      <animate attributeName="opacity" values="1;0.15;1" dur="1.8s" repeatCount="indefinite"/>
    </circle>
    <text x="737" y="196" fill="#3a3a60" font-family="monospace" font-size="8.5" letter-spacing="1.5">ACTIVE</text>
  </svg>

  <!-- ══════════════════════════════════════════
       ANIMATED TYPING TAGLINE
  ══════════════════════════════════════════ -->

  <svg width="800" height="68" xmlns="http://www.w3.org/2000/svg">
    <rect width="800" height="68" fill="#020408"/>
    <line x1="0" y1="0" x2="800" y2="0" stroke="#0d1526" stroke-width="1"/>
    <line x1="0" y1="67" x2="800" y2="67" stroke="#0d1526" stroke-width="1"/>
    <!-- Animated line expanders -->
    <line x1="30" y1="18" x2="30" y2="18" stroke="#0df5e3" stroke-width="0.5" opacity="0.3">
      <animate attributeName="x2" values="30;780;780" dur="1.2s" fill="freeze"/>
    </line>
    <text x="400" y="32" fill="#40406a" font-family="monospace" font-size="11"
          text-anchor="middle" letter-spacing="2">
      Just existing on the internet — everywhere yet nowhere.
      <animate attributeName="opacity" values="0;0;1;1" dur="1.5s" fill="freeze"/>
    </text>
    <text x="400" y="52" fill="#272740" font-family="monospace" font-size="10"
          text-anchor="middle" letter-spacing="2">
      Don't search too hard, you might find me.
      <animate attributeName="opacity" values="0;0;0;1" dur="2.5s" fill="freeze"/>
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
  &nbsp;
  ![](https://img.shields.io/badge/⚡%20NxT-Coder-00c6ff?style=flat-square&labelColor=06080e&color=00c6ff)

  <br><br>

  </div>

  ---

  <!-- ══════════════════════════════════════════
       TYPING SVG ANIMATION
  ══════════════════════════════════════════ -->

  <div align="center">

  <svg width="780" height="55" xmlns="http://www.w3.org/2000/svg">
    <rect width="780" height="55" fill="#020408"/>
    <rect x="0" y="12" width="780" height="31" fill="#080d1c" rx="4" opacity="0.5"/>
    <text x="20" y="33" fill="#0df5e3" font-family="monospace" font-size="13" letter-spacing="1" opacity="0.7">▶</text>
    <text x="40" y="33" fill="#50507a" font-family="monospace" font-size="12" letter-spacing="1">~$</text>
    <text x="60" y="33" fill="#0df5e3" font-family="monospace" font-size="12" letter-spacing=".5" opacity="0.9">whoami</text>
    <text x="130" y="33" fill="#6060a0" font-family="monospace" font-size="12" letter-spacing=".5">→</text>
    <text x="155" y="33" fill="#d8d8ee" font-family="monospace" font-size="12" letter-spacing=".5">riiyad</text>
    <text x="205" y="33" fill="#6060a0" font-family="monospace" font-size="12" letter-spacing=".5">·</text>
    <text x="220" y="33" fill="#f5d800" font-family="monospace" font-size="12" letter-spacing=".5" opacity="0.8">dev</text>
    <text x="250" y="33" fill="#6060a0" font-family="monospace" font-size="12">·</text>
    <text x="265" y="33" fill="#ff1f5a" font-family="monospace" font-size="12" letter-spacing=".5" opacity="0.8">ghost</text>
    <text x="313" y="33" fill="#6060a0" font-family="monospace" font-size="12">·</text>
    <text x="328" y="33" fill="#0df5e3" font-family="monospace" font-size="12" letter-spacing=".5" opacity="0.8">untraceable</text>
    <!-- Blinking cursor -->
    <rect x="452" y="21" width="8" height="15" fill="#0df5e3" opacity="0.8">
      <animate attributeName="opacity" values="0.8;0;0.8" dur="1s" repeatCount="indefinite"/>
    </rect>
  </svg>

  <br>

  <!-- ══════════════════════════════════════════
       TELEGRAM SECTION
  ══════════════════════════════════════════ -->

  <svg width="760" height="44" xmlns="http://www.w3.org/2000/svg">
    <rect width="760" height="44" fill="#020408"/>
    <text x="0" y="16" fill="#ff1f5a" font-family="monospace" font-size="8" letter-spacing="5" font-weight="bold">TELEGRAM</text>
    <line x1="88" y1="12" x2="760" y2="12" stroke="#12122a" stroke-width="1">
      <animate attributeName="x2" values="88;760;760" dur="1.5s" fill="freeze"/>
    </line>
    <rect x="92" y="5" width="6" height="14" fill="#ff1f5a" opacity="0.7">
      <animate attributeName="opacity" values="0.7;0;0.7" dur="1s" repeatCount="indefinite"/>
    </rect>
  </svg>

  <br>

  <table>
  <tr>
  <td align="center" width="360">

  <svg width="320" height="80" xmlns="http://www.w3.org/2000/svg">
    <defs>
      <linearGradient id="card1bg" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" style="stop-color:#07080f"/>
        <stop offset="100%" style="stop-color:#0a0b18"/>
      </linearGradient>
    </defs>
    <rect width="320" height="80" fill="url(#card1bg)" rx="8" stroke="#14142a" stroke-width="1"/>
    <!-- Animated border pulse -->
    <rect width="320" height="80" rx="8" fill="none" stroke="#0088cc" stroke-width="0">
      <animate attributeName="stroke-width" values="0;2;0" dur="3s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;0.5;0" dur="3s" repeatCount="indefinite"/>
    </rect>
    <rect x="8" y="1" width="304" height="1.5" rx="1" fill="#0088cc" opacity="0.25"/>
    <circle cx="38" cy="40" r="20" fill="#0088cc" opacity="0.12"/>
    <circle cx="38" cy="40" r="20" fill="none" stroke="#0088cc" stroke-width="0.5" opacity="0.3">
      <animate attributeName="r" values="20;25;20" dur="3s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.3;0;0.3" dur="3s" repeatCount="indefinite"/>
    </circle>
    <text x="38" y="46" font-size="20" text-anchor="middle">✈️</text>
    <text x="68" y="30" fill="#d8d8ee" font-family="monospace" font-size="14" font-weight="bold">@zerox6t9</text>
    <text x="68" y="48" fill="#404068" font-family="monospace" font-size="9" letter-spacing="2">PRIMARY ACCOUNT</text>
    <rect x="68" y="57" width="68" height="13" rx="3" fill="#0088cc" opacity="0.12"/>
    <text x="102" y="67" fill="#0088cc" font-family="monospace" font-size="7.5" text-anchor="middle" letter-spacing="1">TELEGRAM</text>
    <text x="296" y="44" fill="#0df5e3" font-family="monospace" font-size="16" opacity="0.55">→</text>
  </svg>

  **[→ @zerox6t9](https://t.me/zerox6t9)**

  </td>
  <td align="center" width="360">

  <svg width="320" height="80" xmlns="http://www.w3.org/2000/svg">
    <rect width="320" height="80" fill="#07080f" rx="8" stroke="#14142a" stroke-width="1"/>
    <rect width="320" height="80" rx="8" fill="none" stroke="#0088cc" stroke-width="0">
      <animate attributeName="stroke-width" values="0;2;0" dur="3s" begin="1.5s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;0.5;0" dur="3s" begin="1.5s" repeatCount="indefinite"/>
    </rect>
    <rect x="8" y="1" width="304" height="1.5" rx="1" fill="#0088cc" opacity="0.25"/>
    <circle cx="38" cy="40" r="20" fill="#0088cc" opacity="0.10"/>
    <circle cx="38" cy="40" r="20" fill="none" stroke="#0088cc" stroke-width="0.5" opacity="0.3">
      <animate attributeName="r" values="20;25;20" dur="3s" begin="1.5s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.3;0;0.3" dur="3s" begin="1.5s" repeatCount="indefinite"/>
    </circle>
    <text x="38" y="46" font-size="20" text-anchor="middle">✈️</text>
    <text x="68" y="30" fill="#d8d8ee" font-family="monospace" font-size="14" font-weight="bold">@o0oeveo0o</text>
    <text x="68" y="48" fill="#404068" font-family="monospace" font-size="9" letter-spacing="2">SECONDARY ACCOUNT</text>
    <rect x="68" y="57" width="68" height="13" rx="3" fill="#0088cc" opacity="0.12"/>
    <text x="102" y="67" fill="#0088cc" font-family="monospace" font-size="7.5" text-anchor="middle" letter-spacing="1">TELEGRAM</text>
    <text x="296" y="44" fill="#0df5e3" font-family="monospace" font-size="16" opacity="0.55">→</text>
  </svg>

  **[→ @o0oeveo0o](https://t.me/o0oeveo0o)**

  </td>
  </tr>
  </table>

  </div>

  <br>

  ---

  <!-- ══════════════════════════════════════════
       NxT CODER PROJECT SECTION
  ══════════════════════════════════════════ -->

  <div align="center">

  <svg width="760" height="44" xmlns="http://www.w3.org/2000/svg">
    <rect width="760" height="44" fill="#020408"/>
    <text x="0" y="16" fill="#00c6ff" font-family="monospace" font-size="8" letter-spacing="5" font-weight="bold">NxT CODER</text>
    <line x1="100" y1="12" x2="760" y2="12" stroke="#12122a" stroke-width="1">
      <animate attributeName="x2" values="100;760;760" dur="1.5s" fill="freeze"/>
    </line>
    <rect x="104" y="5" width="6" height="14" fill="#00c6ff" opacity="0.7">
      <animate attributeName="opacity" values="0.7;0;0.7" dur="1.2s" repeatCount="indefinite"/>
    </rect>
  </svg>

  <br>

  <table>
  <tr>
  <td align="center" width="360">

  <svg width="320" height="95" xmlns="http://www.w3.org/2000/svg">
    <defs>
      <linearGradient id="nxtbg" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" style="stop-color:#06080f"/>
        <stop offset="100%" style="stop-color:#080e1c"/>
      </linearGradient>
    </defs>
    <rect width="320" height="95" fill="url(#nxtbg)" rx="8" stroke="#0d1f30" stroke-width="1"/>
    <rect width="320" height="95" rx="8" fill="none" stroke="#00c6ff" stroke-width="0">
      <animate attributeName="stroke-width" values="0;1.5;0" dur="4s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;0.4;0" dur="4s" repeatCount="indefinite"/>
    </rect>
    <!-- Glow top bar -->
    <rect x="0" y="0" width="320" height="3" rx="2" fill="#00c6ff" opacity="0.4"/>
    <!-- NxT logo -->
    <circle cx="38" cy="42" r="22" fill="rgba(0,198,255,0.10)"/>
    <circle cx="38" cy="42" r="22" fill="none" stroke="#00c6ff" stroke-width="0.7" opacity="0.3">
      <animate attributeName="r" values="22;27;22" dur="4s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.3;0;0.3" dur="4s" repeatCount="indefinite"/>
    </circle>
    <text x="38" y="48" font-size="16" text-anchor="middle" fill="#00c6ff" font-family="monospace" font-weight="bold">N×T</text>
    <!-- Text -->
    <text x="70" y="28" fill="#edf0fb" font-family="monospace" font-size="14" font-weight="bold">NxT Coder</text>
    <text x="70" y="46" fill="#304a60" font-family="monospace" font-size="9" letter-spacing="2">PROGRAMMING · BOTS · TOOLS</text>
    <!-- Tag -->
    <rect x="70" y="55" width="90" height="14" rx="3" fill="rgba(0,198,255,0.10)"/>
    <text x="115" y="65" fill="#00c6ff" font-family="monospace" font-size="7.5" text-anchor="middle" letter-spacing="1">t.me/nxt_coder</text>
    <!-- Members badge -->
    <rect x="170" y="55" width="60" height="14" rx="3" fill="rgba(245,216,0,0.10)"/>
    <text x="200" y="65" fill="#f5d800" font-family="monospace" font-size="7.5" text-anchor="middle" letter-spacing="1">CHANNEL</text>
    <!-- Bottom description -->
    <text x="70" y="83" fill="#252540" font-family="monospace" font-size="8.5" letter-spacing=".5">Code · Bots · API tools &amp; more</text>
    <!-- Arrow -->
    <text x="296" y="52" fill="#00c6ff" font-family="monospace" font-size="16" opacity="0.6">→</text>
  </svg>

  **[→ @nxt_coder](https://t.me/nxt_coder)**

  </td>
  <td align="center" width="360">

  <svg width="320" height="95" xmlns="http://www.w3.org/2000/svg">
    <rect width="320" height="95" fill="#06080f" rx="8" stroke="#0d1f30" stroke-width="1"/>
    <rect width="320" height="95" rx="8" fill="none" stroke="#00c6ff" stroke-width="0">
      <animate attributeName="stroke-width" values="0;1.5;0" dur="4s" begin="2s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;0.4;0" dur="4s" begin="2s" repeatCount="indefinite"/>
    </rect>
    <rect x="0" y="0" width="320" height="3" rx="2" fill="#00c6ff" opacity="0.3"/>
    <circle cx="38" cy="42" r="22" fill="rgba(0,198,255,0.08)"/>
    <circle cx="38" cy="42" r="22" fill="none" stroke="#00c6ff" stroke-width="0.7" opacity="0.3">
      <animate attributeName="r" values="22;27;22" dur="4s" begin="2s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.3;0;0.3" dur="4s" begin="2s" repeatCount="indefinite"/>
    </circle>
    <text x="38" y="48" font-size="16" text-anchor="middle" fill="#00c6ff" font-family="monospace" font-weight="bold">CX</text>
    <text x="70" y="28" fill="#edf0fb" font-family="monospace" font-size="14" font-weight="bold">Code Xen</text>
    <text x="70" y="46" fill="#304a60" font-family="monospace" font-size="9" letter-spacing="2">PROJECTS · UPDATES · RELEASES</text>
    <rect x="70" y="55" width="90" height="14" rx="3" fill="rgba(0,198,255,0.10)"/>
    <text x="115" y="65" fill="#00c6ff" font-family="monospace" font-size="7.5" text-anchor="middle" letter-spacing="1">t.me/code_xen</text>
    <rect x="170" y="55" width="60" height="14" rx="3" fill="rgba(245,216,0,0.10)"/>
    <text x="200" y="65" fill="#f5d800" font-family="monospace" font-size="7.5" text-anchor="middle" letter-spacing="1">CHANNEL</text>
    <text x="70" y="83" fill="#252540" font-family="monospace" font-size="8.5" letter-spacing=".5">Project drops &amp; dev content</text>
    <text x="296" y="52" fill="#00c6ff" font-family="monospace" font-size="16" opacity="0.6">→</text>
  </svg>

  **[→ @code_xen](https://t.me/code_xen)**

  </td>
  </tr>
  </table>

  </div>

  <br>

  ---

  <!-- ══════════════════════════════════════════
       OTHER SOCIALS
  ══════════════════════════════════════════ -->

  <div align="center">

  <svg width="760" height="44" xmlns="http://www.w3.org/2000/svg">
    <rect width="760" height="44" fill="#020408"/>
    <text x="0" y="16" fill="#f5d800" font-family="monospace" font-size="8" letter-spacing="5" font-weight="bold">OTHER SOCIALS</text>
    <line x1="126" y1="12" x2="760" y2="12" stroke="#12122a" stroke-width="1">
      <animate attributeName="x2" values="126;760;760" dur="1.5s" fill="freeze"/>
    </line>
    <rect x="130" y="5" width="6" height="14" fill="#f5d800" opacity="0.7">
      <animate attributeName="opacity" values="0.7;0;0.7" dur="1s" repeatCount="indefinite"/>
    </rect>
  </svg>

  <br>

  <table>
  <tr>
  <td align="center" width="240">

  <svg width="200" height="72" xmlns="http://www.w3.org/2000/svg">
    <rect width="200" height="72" fill="#07080f" rx="8" stroke="#14142a" stroke-width="1"/>
    <rect width="200" height="72" rx="8" fill="none" stroke="#f5d800" stroke-width="0">
      <animate attributeName="stroke-width" values="0;1;0" dur="5s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;0.2;0" dur="5s" repeatCount="indefinite"/>
    </rect>
    <circle cx="32" cy="36" r="18" fill="#1877f2" opacity="0.12"/>
    <text x="32" y="43" font-size="22" text-anchor="middle" font-family="serif" font-weight="bold" fill="#1877f2">𝒇</text>
    <text x="58" y="28" fill="#d8d8ee" font-family="monospace" font-size="12" font-weight="bold">Facebook</text>
    <rect x="58" y="36" width="78" height="17" rx="2" fill="rgba(245,216,0,0.08)" stroke="#f5d800" stroke-width="0.5"/>
    <text x="97" y="48" fill="#f5d800" font-family="monospace" font-size="7.5" text-anchor="middle">RESTRICTED</text>
    <text x="58" y="64" fill="#25253a" font-family="monospace" font-size="7.5" letter-spacing=".5">Access limited</text>
  </svg>

  </td>
  <td align="center" width="240">

  <svg width="200" height="72" xmlns="http://www.w3.org/2000/svg">
    <rect width="200" height="72" fill="#07080f" rx="8" stroke="#14142a" stroke-width="1"/>
    <rect width="200" height="72" rx="8" fill="none" stroke="#ff1f5a" stroke-width="0">
      <animate attributeName="stroke-width" values="0;1;0" dur="4s" begin="1s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;0.2;0" dur="4s" begin="1s" repeatCount="indefinite"/>
    </rect>
    <circle cx="32" cy="36" r="18" fill="#e1306c" opacity="0.12"/>
    <text x="32" y="42" font-size="20" text-anchor="middle">📸</text>
    <text x="58" y="28" fill="#d8d8ee" font-family="monospace" font-size="12" font-weight="bold">Instagram</text>
    <rect x="58" y="36" width="78" height="17" rx="2" fill="rgba(255,31,90,0.08)" stroke="#ff1f5a" stroke-width="0.5"/>
    <text x="97" y="48" fill="#ff1f5a" font-family="monospace" font-size="7.5" text-anchor="middle">RESTRICTED</text>
    <text x="58" y="64" fill="#25253a" font-family="monospace" font-size="7.5" letter-spacing=".5">Private account</text>
  </svg>

  </td>
  <td align="center" width="240">

  <svg width="200" height="72" xmlns="http://www.w3.org/2000/svg">
    <rect width="200" height="72" fill="#07080f" rx="8" stroke="#14142a" stroke-width="1"/>
    <rect width="200" height="72" rx="8" fill="none" stroke="#0df5e3" stroke-width="0">
      <animate attributeName="stroke-width" values="0;1;0" dur="6s" begin="0.5s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;0.2;0" dur="6s" begin="0.5s" repeatCount="indefinite"/>
    </rect>
    <circle cx="32" cy="36" r="18" fill="#1da1f2" opacity="0.12"/>
    <text x="32" y="43" font-size="20" text-anchor="middle">🐦</text>
    <text x="58" y="28" fill="#d8d8ee" font-family="monospace" font-size="12" font-weight="bold">Twitter / X</text>
    <rect x="58" y="36" width="78" height="17" rx="2" fill="rgba(13,245,227,0.08)" stroke="#0df5e3" stroke-width="0.5"/>
    <text x="97" y="48" fill="#0df5e3" font-family="monospace" font-size="7.5" text-anchor="middle">RESTRICTED</text>
    <text x="58" y="64" fill="#25253a" font-family="monospace" font-size="7.5" letter-spacing=".5">Limited activity</text>
  </svg>

  </td>
  </tr>
  </table>

  </div>

  <br>

  ---

  <!-- ══════════════════════════════════════════
       ANIMATED STATS WAVE FOOTER
  ══════════════════════════════════════════ -->

  <div align="center">

  <svg width="800" height="120" xmlns="http://www.w3.org/2000/svg">
    <rect width="800" height="120" fill="#020408" rx="12"/>
    <!-- Animated wave paths -->
    <path d="" stroke="#0df5e3" stroke-width="1" fill="none" opacity="0.15">
      <animate attributeName="d"
        values="M0,60 Q100,30 200,60 Q300,90 400,60 Q500,30 600,60 Q700,90 800,60;
                M0,60 Q100,90 200,60 Q300,30 400,60 Q500,90 600,60 Q700,30 800,60;
                M0,60 Q100,30 200,60 Q300,90 400,60 Q500,30 600,60 Q700,90 800,60"
        dur="8s" repeatCount="indefinite"/>
    </path>
    <path d="" stroke="#ff1f5a" stroke-width="0.8" fill="none" opacity="0.10">
      <animate attributeName="d"
        values="M0,70 Q120,40 240,70 Q360,100 480,70 Q600,40 720,70 Q760,80 800,70;
                M0,70 Q120,100 240,70 Q360,40 480,70 Q600,100 720,70 Q760,60 800,70;
                M0,70 Q120,40 240,70 Q360,100 480,70 Q600,40 720,70 Q760,80 800,70"
        dur="10s" repeatCount="indefinite"/>
    </path>
    <!-- Center text -->
    <text x="400" y="40" fill="#1e1e3a" font-family="monospace" font-size="9" text-anchor="middle" letter-spacing="5">RIIYAD · MEMEVAIYA2O</text>
    <text x="400" y="62" fill="#2a2a4a" font-family="monospace" font-size="11" text-anchor="middle" letter-spacing="3">Just existing on the internet.</text>
    <text x="400" y="83" fill="#0df5e3" font-family="monospace" font-size="9" text-anchor="middle" letter-spacing="4" opacity="0.4">t.me/nxt_coder  ·  t.me/code_xen</text>
    <!-- Bottom pulse bar -->
    <rect x="200" y="98" width="400" height="1.5" rx="1" fill="#0df5e3" opacity="0.08">
      <animate attributeName="width" values="400;340;400;460;400" dur="6s" repeatCount="indefinite"/>
      <animate attributeName="x" values="200;230;200;170;200" dur="6s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.08;0.15;0.08" dur="3s" repeatCount="indefinite"/>
    </rect>
  </svg>

  </div>