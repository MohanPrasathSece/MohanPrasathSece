<!-- 🔥 EXTREME ARCADE MODE - RETRO 8-BIT ANIMATED HEADER (GitHub-safe) -->
<p align="center">
<svg width="100%" height="200" viewBox="0 0 900 200" xmlns="http://www.w3.org/2000/svg">

<!-- ===== BACKGROUND CRT SCANLINES =====-->
<defs>
  <pattern id="scan" width="4" height="4" patternUnits="userSpaceOnUse">
    <rect width="4" height="1" fill="rgba(255,255,255,0.08)"/>
  </pattern>
</defs>
<rect width="900" height="200" fill="black"/>
<rect width="900" height="200" fill="url(#scan)" opacity="0.5">
  <animate attributeName="opacity" values="0.3;0.5;0.3" dur="3s" repeatCount="indefinite"/>
</rect>

<!-- ===== PULSING ARCADE BORDER ===== -->
<rect x="5" y="5" width="890" height="190" fill="none" stroke="#39ff14" stroke-width="4"
      stroke-dasharray="10 5">
  <animate attributeName="stroke" values="#39ff14;#ff00ea;#00e5ff;#39ff14" dur="4s" repeatCount="indefinite"/>
  <animate attributeName="stroke-dashoffset" values="0;20" dur="1.2s" repeatCount="indefinite"/>
</rect>

<!-- ===== RANDOM PIXEL SPARKS ===== -->
<g id="sparkGroup">
  <!-- 15 Pixel Sparks -->
  <!-- (GitHub-safe animation: opacity + small transforms only) -->
  <!-- Spark template repeated with diff timings -->
  <circle cx="120" cy="60" r="2" fill="#ff004c">
    <animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite"/>
    <animate attributeName="cy" values="60;50;60" dur="1s" repeatCount="indefinite"/>
  </circle>

  <circle cx="350" cy="120" r="2" fill="#00eaff">
    <animate attributeName="opacity" values="1;0;1" dur="0.8s" repeatCount="indefinite"/>
    <animate attributeName="cy" values="120;110;120" dur="0.8s" repeatCount="indefinite"/>
  </circle>

  <circle cx="650" cy="80" r="2" fill="#ffe600">
    <animate attributeName="opacity" values="1;0;1" dur="1.3s" repeatCount="indefinite"/>
    <animate attributeName="cy" values="80;70;80" dur="1.3s" repeatCount="indefinite"/>
  </circle>

  <!-- More sparks -->
  <circle cx="250" cy="150" r="2" fill="#ff00ea">
    <animate attributeName="opacity" values="1;0;1" dur="0.9s" repeatCount="indefinite"/>
    <animate attributeName="cy" values="150;140;150" dur="0.9s" repeatCount="indefinite"/>
  </circle>

  <circle cx="760" cy="50" r="2" fill="#39ff14">
    <animate attributeName="opacity" values="1;0;1" dur="1.1s" repeatCount="indefinite"/>
    <animate attributeName="cy" values="50;40;50" dur="1.1s" repeatCount="indefinite"/>
  </circle>
</g>

<!-- ===== GLITCHY 8-BIT TITLE ===== -->
<text x="50%" y="50%" dominant-baseline="middle" text-anchor="middle"
      font-family="monospace" font-size="48px" fill="#39ff14" font-weight="bold">

  MOHAN — 8BIT MODE

  <!-- CRT glitch -->
  <animate attributeName="fill" values="#39ff14;#ff00ea;#00eaff;#39ff14"
           dur="3s" repeatCount="indefinite"/>

  <!-- Glitch jitter -->
  <animate attributeName="x" values="50%;49%;51%;50%" dur="0.35s" repeatCount="indefinite"/>
</text>

</svg>
</p>
