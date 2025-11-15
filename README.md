<!-- ===========================
     MOHAN PRASATH S ─ 8-BIT LOBBY
     Pure SVG + Markdown. NO external images.
     Theme: 8-Bit Arcade (NES/SNES/Atari) + CRT overlay
   =========================== -->

<!-- ================= HEADER: 8-bit animated logo (SVG) ================= -->
<p align="center">
  <!-- big pixel title with neon animation -->
  <svg width="760" height="120" viewBox="0 0 760 120" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Mohan Prasath">
    <style>
      .bg { fill:#071017; }
      .px { font-family: "Courier New", monospace; font-weight:700; font-size:28px; letter-spacing:2px; }
      .neon { fill: #9B59FF; filter: url(#glow); }
      .neon2 { fill: #70D6FF; filter: url(#glow2); }
      .blink { animation: blink 1.6s infinite; }
      @keyframes blink { 0%{opacity:1}50%{opacity:0.35}100%{opacity:1} }
    </style>

    <defs>
      <filter id="glow"><feGaussianBlur stdDeviation="3.2" result="coloredBlur"/><feMerge><feMergeNode in="coloredBlur"/><feMergeNode in="SourceGraphic"/></feMerge></filter>
      <filter id="glow2"><feGaussianBlur stdDeviation="2.6" result="c"/><feMerge><feMergeNode in="c"/><feMergeNode in="SourceGraphic"/></feMerge></filter>
    </defs>

    <rect class="bg" width="760" height="120" rx="8" />
    <!-- Pixel border blocks -->
    <g>
      <!-- left pixel column -->
      <rect x="12" y="12" width="16" height="16" fill="#8A2BE2"/>
      <rect x="12" y="32" width="16" height="16" fill="#70D6FF"/>
      <rect x="12" y="52" width="16" height="16" fill="#8A2BE2"/>
      <rect x="32" y="12" width="16" height="16" fill="#70D6FF"/>
      <rect x="32" y="52" width="16" height="16" fill="#8A2BE2"/>
    </g>

    <!-- Title lines (pixel-style text using monospaced glyphs) -->
    <text x="120" y="52" class="px neon">👾 MOHAN PRASATH S 👾</text>
    <text x="120" y="86" class="px neon2 blink">FULL STACK DEVELOPER • MERN • ZYRA DIGITALS</text>

    <!-- moving 8-bit scanline (SMIL animation) -->
    <rect x="0" y="-40" width="760" height="6" fill="rgba(255,255,255,0.03)">
      <animate attributeName="y" from="-40" to="160" dur="2.8s" repeatCount="indefinite"/>
    </rect>
  </svg>
</p>

---

<!-- ================= PIXEL MOVING BORDER (SVG) ================= -->
<div align="center">
<svg width="100%" height="26" viewBox="0 0 760 26" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
  <style>
    .p { fill:#07070A; }
    .pxb { fill:#8A2BE2; }
    .pxb2 { fill:#70D6FF; }
  </style>
  <rect width="760" height="26" class="p" rx="6"/>
  <!-- animated row of pixels -->
  <g>
    <!-- repeat pattern with sliding animation -->
    <g id="stripe">
      <rect x="10" y="6" width="8" height="8" class="pxb"/>
      <rect x="24" y="6" width="8" height="8" class="pxb2"/>
      <rect x="38" y="6" width="8" height="8" class="pxb"/>
      <rect x="52" y="6" width="8" height="8" class="pxb2"/>
    </g>
    <use href="#stripe" x="0">
      <animateTransform attributeName="transform" type="translate" from="0 0" to="520 0" dur="3s" repeatCount="indefinite"/>
    </use>
    <use href="#stripe" x="260">
      <animateTransform attributeName="transform" type="translate" from="0 0" to="-520 0" dur="3s" repeatCount="indefinite"/>
    </use>
  </g>
</svg>
</div>

---

## 🕹️ WELCOME TO THE ARCADE LOBBY (8-BIT HUD)

<pre style="background:#071017;color:#8ef7ff;padding:12px;border-radius:6px;line-height:1.1;font-family: 'Courier New', monospace;">
 ███ PLAYER: MOHAN PRASATH S         CLASS: MERN WIZARD
 ███ LOCATION: Coimbatore, Tamil Nadu   GUILD: Zyra Digitals (Founder)
 ███ XP: 7+ Live Projects | 700+ SkillRack | 350+ LeetCode (1610)
</pre>

---

<!-- ================= JUMPING PIXEL BUTTONS (SVG) ================= -->
<p align="center">
  <svg width="760" height="84" viewBox="0 0 760 84" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="links">
    <style>
      .btnbg { fill:#04060a; stroke:#1b1f2b; stroke-width:2; rx:6 }
      .label { font-family: "Courier New", monospace; font-size:14px; fill:#bfefff }
      .pix { fill:#8A2BE2 }
      .pix2 { fill:#70D6FF }
      /* jump animation applied via SMIL to group transform */
    </style>

    <rect class="btnbg" x="20" y="12" width="220" height="56" rx="8" />
    <g transform="translate(20,12)">
      <g>
        <!-- pixel icon -->
        <rect x="12" y="12" width="8" height="8" class="pix"/>
        <rect x="22" y="12" width="8" height="8" class="pix2"/>
        <rect x="12" y="22" width="8" height="8" class="pix2"/>
      </g>
      <text x="64" y="38" class="label">Portfolio</text>
      <a href="https://mohanprasath.vercel.app/" target="_blank">
        <rect x="0" y="0" width="220" height="56" fill="transparent">
          <animate attributeName="y" values="0; -6; 0" dur="1.6s" repeatCount="indefinite"/>
        </rect>
      </a>
    </g>

    <!-- second -->
    <rect class="btnbg" x="270" y="12" width="220" height="56" rx="8" />
    <g transform="translate(270,12)">
      <g>
        <rect x="12" y="12" width="8" height="8" class="pix2"/>
        <rect x="22" y="12" width="8" height="8" class="pix"/>
      </g>
      <text x="64" y="38" class="label">GitHub</text>
      <a href="https://github.com/MohanPrasathSece" target="_blank">
        <rect x="0" y="0" width="220" height="56" fill="transparent">
          <animate attributeName="y" values="0; -8; 0" dur="1.9s" repeatCount="indefinite"/>
        </rect>
      </a>
    </g>

    <!-- third -->
    <rect class="btnbg" x="520" y="12" width="220" height="56" rx="8" />
    <g transform="translate(520,12)">
      <g>
        <rect x="12" y="12" width="8" height="8" class="pix"/>
        <rect x="22" y="22" width="8" height="8" class="pix2"/>
      </g>
      <text x="64" y="38" class="label">Contact</text>
      <a href="mailto:mohanprasath563@gmail.com">
        <rect x="0" y="0" width="220" height="56" fill="transparent">
          <animate attributeName="y" values="0; -5; 0" dur="1.7s" repeatCount="indefinite"/>
        </rect>
      </a>
    </g>
  </svg>
</p>

---

## 💾 ZYRA DIGITALS — RETRO STUDIO (Animated SVG card)

<svg width="760" height="160" viewBox="0 0 760 160" xmlns="http://www.w3.org/2000/svg" aria-label="Zyra Digitals">
  <style>
    .card { fill:#040511; stroke:#2a2233; stroke-width:2; rx:10 }
    .title { font-family: "Courier New", monospace; font-size:16px; fill:#ffd9ff }
    .desc { font-family: "Courier New", monospace; font-size:12px; fill:#9fe6ff }
    .tag { font-family: "Courier New", monospace; font-size:11px; fill:#112 }
    .chip { rx:4 }
  </style>

  <rect class="card" x="6" y="6" width="748" height="148" rx="10"/>
  <text x="28" y="36" class="title">⚙️ Zyra Digitals — Indie Web Studio (Founder)</text>
  <text x="28" y="60" class="desc">We build fast, conversion-focused websites & MERN apps with performance, SEO, and UX as core pillars.</text>

  <!-- animated service chips (SMIL translate) -->
  <g transform="translate(28,86)">
    <rect x="0" y="0" width="160" height="24" fill="#8A2BE2" class="chip"/>
    <text x="10" y="16" font-family="Courier New" font-size="12" fill="#071017">Business Sites</text>

    <g transform="translate(180,0)">
      <rect x="0" y="0" width="160" height="24" fill="#70D6FF" class="chip"/>
      <text x="10" y="16" font-family="Courier New" font-size="12" fill="#071017">E-commerce & Shops</text>
    </g>

    <g transform="translate(360,0)">
      <rect x="0" y="0" width="160" height="24" fill="#B07BFF" class="chip"/>
      <text x="10" y="16" font-family="Courier New" font-size="12" fill="#071017">MERN Web Apps</text>
    </g>

    <!-- looped subtle float -->
    <animateTransform attributeName="transform" type="translate" from="28,86" to="28,92" dur="2.6s" repeatCount="indefinite" additive="sum"/>
  </g>

  <text x="28" y="124" class="desc">Portfolio: https://www.zyradigitals.info • Affordable, quick turnarounds • Performance tuning</text>
</svg>

---

## 🕹 PROJECT CARTRIDGES (PIXEL ROW)
<p align="center">
<svg width="760" height="140" viewBox="0 0 760 140" xmlns="http://www.w3.org/2000/svg" aria-label="projects">
  <style>
    .cart { fill:#070912; stroke:#1d1f2b; stroke-width:2; rx:8 }
    .name { font-family: "Courier New", monospace; font-size:12px; fill:#bfefff }
    .meta { font-family: "Courier New", monospace; font-size:10px; fill:#9fe6ff }
    .pixel { fill:#8A2BE2 }
    .pixel2 { fill:#70D6FF }
  </style>

  <!-- Food Rescue -->
  <g transform="translate(12,8)">
    <rect class="cart" width="232" height="56" rx="6"/>
    <text x="12" y="22" class="name">🌍 Food Rescue Network</text>
    <text x="12" y="38" class="meta">MERN • Real-time donor-volunteer tracking • 50+ rescues</text>
    <!-- subtle pulse -->
    <rect x="190" y="14" width="18" height="18" rx="3" fill="#ff6ec7">
      <animate attributeName="opacity" values="1;0.35;1" dur="1.6s" repeatCount="indefinite"/>
    </rect>
  </g>

  <!-- MediSmart -->
  <g transform="translate(256,8)">
    <rect class="cart" width="232" height="56" rx="6"/>
    <text x="12" y="22" class="name">💊 MediSmart-AI</text>
    <text x="12" y="38" class="meta">OCR + NLP • Pharmacy matching • Socket.io</text>
    <rect x="190" y="14" width="18" height="18" rx="3" fill="#70D6FF">
      <animate attributeName="transform" type="translate" values="0 0;0 -4;0 0" dur="1.8s" repeatCount="indefinite"/>
    </rect>
  </g>

  <!-- Inventory -->
  <g transform="translate(500,8)">
    <rect class="cart" width="232" height="56" rx="6"/>
    <text x="12" y="22" class="name">📦 Inventory Tracker</text>
    <text x="12" y="38" class="meta">MERN • Suppliers • Stock logs • Analytics</text>
    <rect x="190" y="14" width="18" height="18" rx="3" fill="#8A2BE2">
      <animate attributeName="opacity" values="1;0.5;1" dur="2.1s" repeatCount="indefinite"/>
    </rect>
  </g>
</svg>
</p>

---

## ✨ SKILL BUBBLES (PIXEL SWELL ANIMATION)
<svg width="760" height="120" viewBox="0 0 760 120" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
  <style>
    .bubble { fill:#07070a; stroke:#1f1526; stroke-width:2; }
    .txt { font-family: "Courier New", monospace; font-size:12px; fill:#bfefff }
  </style>

  <!-- repeated chips with swell animation -->
  <g transform="translate(18,18)">
    <g>
      <rect class="bubble" x="0" y="0" rx="6" width="140" height="28"/>
      <text class="txt" x="12" y="18">React • Next • Vercel</text>
      <animateTransform attributeName="transform" type="scale" values="1;1.05;1" dur="3s" repeatCount="indefinite"/>
    </g>
  </g>

  <g transform="translate(172,18)">
    <g>
      <rect class="bubble" x="0" y="0" rx="6" width="140" height="28"/>
      <text class="txt" x="12" y="18">Node • Express • REST</text>
      <animateTransform attributeName="transform" type="scale" values="1;1.04;1" dur="3.2s" repeatCount="indefinite"/>
    </g>
  </g>

  <g transform="translate(326,18)">
    <g>
      <rect class="bubble" x="0" y="0" rx="6" width="140" height="28"/>
      <text class="txt" x="12" y="18">MongoDB • MySQL</text>
      <animateTransform attributeName="transform" type="scale" values="1;1.06;1" dur="2.9s" repeatCount="indefinite"/>
    </g>
  </g>

  <g transform="translate(480,18)">
    <g>
      <rect class="bubble" x="0" y="0" rx="6" width="140" height="28"/>
      <text class="txt" x="12" y="18">DSA • OOP • System Design</text>
      <animateTransform attributeName="transform" type="scale" values="1;1.03;1" dur="3.4s" repeatCount="indefinite"/>
    </g>
  </g>

  <g transform="translate(18,64)">
    <g>
      <rect class="bubble" x="0" y="0" rx="6" width="140" height="28"/>
      <text class="txt" x="12" y="18">Java • Python • C</text>
      <animateTransform attributeName="transform" type="scale" values="1;1.05;1" dur="3.1s" repeatCount="indefinite"/>
    </g>
  </g>

  <g transform="translate(172,64)">
    <g>
      <rect class="bubble" x="0" y="0" rx="6" width="308" height="28"/>
      <text class="txt" x="12" y="18">Tools: Git • GitHub • Postman • Figma • Unity3D • VSCode</text>
      <animateTransform attributeName="transform" type="scale" values="1;1.02;1" dur="3.3s" repeatCount="indefinite"/>
    </g>
  </g>
</svg>

---

## 🎵 8-BIT SOUND WAVE (SVG)
<svg width="760" height="120" viewBox="0 0 760 120" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
  <style>
    .bar { fill:#70D6FF; }
  </style>
  <!-- 16 vertical bars with animated heights -->
  <g transform="translate(20,20)">
    <!-- create 16 bars -->
    <!-- we'll add animate to each bar with slightly different durations/phases -->
    <g>
      <!-- bar template at x=0 -->
      <rect class="bar" x="0" y="40" width="12" height="40" rx="2">
        <animate attributeName="height" values="12;48;12" dur="1.2s" repeatCount="indefinite"/>
        <animate attributeName="y" values="68;32;68" dur="1.2s" repeatCount="indefinite"/>
      </rect>
    </g>
    <!-- replicate with offsets -->
    <!-- using <use> is not allowed with SMIL in some cases; just copy multiple -->
    <rect class="bar" x="18" y="40" width="12" height="40" rx="2">
      <animate attributeName="height" values="16;52;16" dur="1.4s" repeatCount="indefinite"/>
      <animate attributeName="y" values="64;28;64" dur="1.4s" repeatCount="indefinite"/>
    </rect>
    <rect class="bar" x="36" y="40" width="12" height="40" rx="2">
      <animate attributeName="height" values="20;60;20" dur="1.0s" repeatCount="indefinite"/>
      <animate attributeName="y" values="60;20;60" dur="1.0s" repeatCount="indefinite"/>
    </rect>
    <rect class="bar" x="54" y="40" width="12" height="40" rx="2">
      <animate attributeName="height" values="12;48;12" dur="1.6s" repeatCount="indefinite"/>
      <animate attributeName="y" values="68;32;68" dur="1.6s" repeatCount="indefinite"/>
    </rect>

    <rect class="bar" x="72" y="40" width="12" height="40" rx="2">
      <animate attributeName="height" values="22;56;22" dur="1.2s" repeatCount="indefinite"/>
      <animate attributeName="y" values="58;24;58" dur="1.2s" repeatCount="indefinite"/>
    </rect>

    <rect class="bar" x="90" y="40" width="12" height="40" rx="2">
      <animate attributeName="height" values="10;46;10" dur="1.3s" repeatCount="indefinite"/>
      <animate attributeName="y" values="70;34;70" dur="1.3s" repeatCount="indefinite"/>
    </rect>

    <rect class="bar" x="108" y="40" width="12" height="40" rx="2">
      <animate attributeName="height" values="18;54;18" dur="1.05s" repeatCount="indefinite"/>
      <animate attributeName="y" values="62;26;62" dur="1.05s" repeatCount="indefinite"/>
    </rect>

    <rect class="bar" x="126" y="40" width="12" height="40" rx="2">
      <animate attributeName="height" values="14;50;14" dur="1.35s" repeatCount="indefinite"/>
      <animate attributeName="y" values="66;30;66" dur="1.35s" repeatCount="indefinite"/>
    </rect>

    <rect class="bar" x="144" y="40" width="12" height="40" rx="2">
      <animate attributeName="height" values="24;60;24" dur="0.95s" repeatCount="indefinite"/>
      <animate attributeName="y" values="56;20;56" dur="0.95s" repeatCount="indefinite"/>
    </rect>

    <rect class="bar" x="162" y="40" width="12" height="40" rx="2">
      <animate attributeName="height" values="12;48;12" dur="1.2s" repeatCount="indefinite"/>
      <animate attributeName="y" values="68;32;68" dur="1.2s" repeatCount="indefinite"/>
    </rect>

    <rect class="bar" x="180" y="40" width="12" height="40" rx="2">
      <animate attributeName="height" values="16;52;16" dur="1.4s" repeatCount="indefinite"/>
      <animate attributeName="y" values="64;28;64" dur="1.4s" repeatCount="indefinite"/>
    </rect>

    <rect class="bar" x="198" y="40" width="12" height="40" rx="2">
      <animate attributeName="height" values="20;60;20" dur="1.0s" repeatCount="indefinite"/>
      <animate attributeName="y" values="60;20;60" dur="1.0s" repeatCount="indefinite"/>
    </rect>

    <rect class="bar" x="216" y="40" width="12" height="40" rx="2">
      <animate attributeName="height" values="12;48;12" dur="1.6s" repeatCount="indefinite"/>
      <animate attributeName="y" values="68;32;68" dur="1.6s" repeatCount="indefinite"/>
    </rect>

    <rect class="bar" x="234" y="40" width="12" height="40" rx="2">
      <animate attributeName="height" values="22;56;22" dur="1.2s" repeatCount="indefinite"/>
      <animate attributeName="y" values="58;24;58" dur="1.2s" repeatCount="indefinite"/>
    </rect>

    <rect class="bar" x="252" y="40" width="12" height="40" rx="2">
      <animate attributeName="height" values="10;46;10" dur="1.3s" repeatCount="indefinite"/>
      <animate attributeName="y" values="70;34;70" dur="1.3s" repeatCount="indefinite"/>
    </rect>

  </g>
</svg>

---

## 🐍 PIXEL SNAKE HEATMAP (SIMULATED SVG ANIMATION)
<p>
  <!-- 14x7 small grid contribution-snake style with a moving snake -->
  <svg width="760" height="160" viewBox="0 0 700 140" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
    <style>
      .cell { stroke:#0b0f12; stroke-width:2 }
      .low { fill:#0f1b1d }
      .mid { fill:#0b6e64 }
      .high { fill:#00ff9d }
      .snake { fill:#8affc8; }
    </style>

    <!-- grid -->
    <g id="grid" transform="translate(10,10)">
      <!-- 14 columns x 6 rows -->
      <!-- draw grid cells -->
      <!-- we'll animate a snake rect traversing a path -->
      <rect x="0" y="0" width="640" height="120" fill="#04060a" rx="6"/>
      <!-- sample heat cells (static low/mid/high) -->
      <!-- row major loop (we'll manually place a few) -->
      <!-- row 0 -->
      <rect x="8" y="8" width="40" height="20" class="cell low"/>
      <rect x="56" y="8" width="40" height="20" class="cell mid"/>
      <rect x="104" y="8" width="40" height="20" class="cell high"/>
      <rect x="152" y="8" width="40" height="20" class="cell low"/>
      <rect x="200" y="8" width="40" height="20" class="cell mid"/>
      <rect x="248" y="8" width="40" height="20" class="cell high"/>

      <!-- row 1 -->
      <rect x="8" y="36" width="40" height="20" class="cell mid"/>
      <rect x="56" y="36" width="40" height="20" class="cell high"/>
      <rect x="104" y="36" width="40" height="20" class="cell low"/>
      <rect x="152" y="36" width="40" height="20" class="cell mid"/>
      <rect x="200" y="36" width="40" height="20" class="cell high"/>
      <rect x="248" y="36" width="40" height="20" class="cell low"/>

      <!-- row 2 -->
      <rect x="8" y="64" width="40" height="20" class="cell high"/>
      <rect x="56" y="64" width="40" height="20" class="cell mid"/>
      <rect x="104" y="64" width="40" height="20" class="cell mid"/>
      <rect x="152" y="64" width="40" height="20" class="cell low"/>
      <rect x="200" y="64" width="40" height="20" class="cell high"/>
      <rect x="248" y="64" width="40" height="20" class="cell mid"/>
    </g>

    <!-- snake path: a small pixel square moving along a predefined path -->
    <rect id="snake" x="8" y="8" width="40" height="20" class="snake" rx="2">
      <animate attributeName="x" values="8;56;104;152;200;248;200;152;104;56;8;56;104;152;200" dur="9s" repeatCount="indefinite"/>
      <animate attributeName="y" values="8;8;8;8;8;8;36;36;36;36;36;64;64;64;64" dur="9s" repeatCount="indefinite"/>
    </rect>
  </svg>
</p>

---

## 🏅 HACKTOBERFEST BADGES (SVG ROW) — SIX BADGES
<p align="center">
<svg width="760" height="88" viewBox="0 0 760 88" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
  <style>
    .b { fill:#07090b; stroke:#1b1320; stroke-width:2; rx:6 }
    .label { font-family:"Courier New", monospace; font-size:12px; fill:#bfefff }
    .accent { fill:#ff7ab6 }
  </style>

  <!-- badge 1 -->
  <g transform="translate(28,12)">
    <rect class="b" width="104" height="64" rx="6"/>
    <text x="12" y="36" class="label">Hacktoberfest</text>
    <text x="12" y="52" class="label" font-size="10">Contributor</text>
  </g>

  <!-- badge 2 -->
  <g transform="translate(148,12)">
    <rect class="b" width="104" height="64" rx="6"/>
    <text x="12" y="36" class="label">PRs</text>
    <text x="12" y="52" class="label" font-size="10">06+</text>
  </g>

  <!-- badge 3 -->
  <g transform="translate(268,12)">
    <rect class="b" width="104" height="64" rx="6"/>
    <text x="12" y="36" class="label">OpenSource</text>
    <text x="12" y="52" class="label" font-size="10">Warrior</text>
  </g>

  <!-- badge 4 -->
  <g transform="translate(388,12)">
    <rect class="b" width="104" height="64" rx="6"/>
    <text x="12" y="36" class="label">LeetCode</text>
    <text x="12" y="52" class="label" font-size="10">1610</text>
  </g>

  <!-- badge 5 -->
  <g transform="translate(508,12)">
    <rect class="b" width="104" height="64" rx="6"/>
    <text x="12" y="36" class="label">SkillRack</text>
    <text x="12" y="52" class="label" font-size="10">700+</text>
  </g>

  <!-- badge 6 -->
  <g transform="translate(628,12)">
    <rect class="b" width="104" height="64" rx="6"/>
    <text x="12" y="36" class="label">Hacktoberfest</text>
    <text x="12" y="52" class="label" font-size="10">2025</text>
  </g>
</svg>
</p>

---

## 🏆 ACHIEVEMENTS (RETRO LIST)
<pre style="background:#04060a;color:#c3f7ff;padding:12px;border-radius:8px;font-family:'Courier New', monospace;">
 • 1st Prize — VR Escape Room Game (Unity3D)
 • Top 10 — Gen-AI Hackathon (133 teams)
 • SkillRack: 700+ problems solved
 • LeetCode: 350+ problems (Max Rating: 1610)
 • Hacktoberfest Super Contributor — 2025
</pre>

---

## 📬 CONTACT & PORTFOLIO
<pre style="background:#071017;color:#9ee6b9;padding:12px;border-radius:8px;font-family:'Courier New', monospace;">
 Portfolio : https://mohanprasath.vercel.app/
 Zyra     : https://www.zyradigitals.info
 Email    : mohanprasath563@gmail.com
 Phone    : +91 90254 21149
 GitHub   : https://github.com/MohanPrasathSece
</pre>

---

<!-- ================= CRT SCANLINES (SVG overlay) ================= -->
<div align="center">
<svg width="760" height="36" viewBox="0 0 760 36" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
  <defs>
    <linearGradient id="g" x1="0" x2="1">
      <stop offset="0" stop-color="#000" stop-opacity="0.0"/>
      <stop offset="0.5" stop-color="#000" stop-opacity="0.08"/>
      <stop offset="1" stop-color="#000" stop-opacity="0.0"/>
    </linearGradient>
  </defs>
  <!-- moving scanlines -->
  <rect width="760" height="36" fill="url(#g)">
    <animate attributeName="x" from="-760" to="760" dur="6s" repeatCount="indefinite"/>
  </rect>
</svg>
</div>

---

<p align="center" style="font-family: 'Courier New', monospace; color:#bfefff;">
  ✦ Built with pure SVG pixels • 8-Bit Arcade Style • Zyra Digitals • © 2025 Mohan Prasath S ✦
</p>

