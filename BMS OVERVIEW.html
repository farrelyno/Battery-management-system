<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Battery Management System — Dasar Teori</title>
<style>
  :root {
    --bg: #0d1117; --bg2: #161b22; --bg3: #21262d;
    --border: #30363d; --border2: #484f58;
    --text: #e6edf3; --text2: #8b949e; --text3: #6e7681;
    --blue: #388bfd; --blue2: #1f6feb; --blue3: #0d419d;
    --green: #3fb950; --green2: #238636;
    --amber: #d29922; --amber2: #9e6a03;
    --red: #f85149; --red2: #da3633;
    --purple: #a371f7; --purple2: #6e40c9;
    --teal: #39d353; --cyan: #56d3ec;
    --font: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Noto Sans', Helvetica, Arial, sans-serif;
    --mono: 'SFMono-Regular', Consolas, 'Liberation Mono', Menlo, monospace;
  }
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body { background: var(--bg); color: var(--text); font-family: var(--font); font-size: 15px; line-height: 1.6; }

  .layout { display: flex; min-height: 100vh; }

  /* SIDEBAR */
  nav {
    width: 260px; min-width: 260px; background: var(--bg2);
    border-right: 1px solid var(--border); padding: 24px 0;
    position: sticky; top: 0; height: 100vh; overflow-y: auto;
    font-size: 13px;
  }
  .nav-logo { padding: 0 20px 20px; border-bottom: 1px solid var(--border); margin-bottom: 12px; }
  .nav-logo h1 { font-size: 14px; font-weight: 600; color: var(--text); }
  .nav-logo p { font-size: 11px; color: var(--text3); margin-top: 2px; }
  .nav-section { padding: 4px 20px 4px; font-size: 11px; font-weight: 600; color: var(--text3); text-transform: uppercase; letter-spacing: .6px; margin-top: 12px; }
  nav a { display: block; padding: 5px 20px; color: var(--text2); text-decoration: none; border-left: 2px solid transparent; transition: all .15s; }
  nav a:hover { color: var(--text); background: var(--bg3); }
  nav a.active { color: var(--blue); border-left-color: var(--blue); background: rgba(56,139,253,.08); }
  nav a.sub { padding-left: 32px; font-size: 12px; }

  /* MAIN */
  main { flex: 1; max-width: 900px; padding: 48px 40px; }

  /* SECTIONS */
  section { margin-bottom: 72px; scroll-margin-top: 24px; }
  h2 { font-size: 26px; font-weight: 600; border-bottom: 1px solid var(--border); padding-bottom: 12px; margin-bottom: 24px; color: var(--text); }
  h3 { font-size: 18px; font-weight: 600; margin: 32px 0 12px; color: var(--text); }
  h4 { font-size: 15px; font-weight: 600; margin: 20px 0 8px; color: var(--text2); }
  p { margin-bottom: 12px; color: var(--text2); line-height: 1.7; }
  p strong { color: var(--text); }
  code { font-family: var(--mono); font-size: 13px; background: var(--bg3); border: 1px solid var(--border); border-radius: 4px; padding: 1px 5px; color: #ffa657; }
  pre { background: var(--bg3); border: 1px solid var(--border); border-radius: 8px; padding: 20px; overflow-x: auto; margin: 16px 0; }
  pre code { background: none; border: none; padding: 0; color: #e6edf3; font-size: 13px; line-height: 1.6; }

  /* BADGES */
  .badge { display: inline-block; font-size: 11px; font-weight: 500; padding: 2px 8px; border-radius: 12px; }
  .badge-blue { background: rgba(56,139,253,.15); color: var(--blue); }
  .badge-green { background: rgba(63,185,80,.15); color: var(--green); }
  .badge-amber { background: rgba(210,153,34,.15); color: var(--amber); }
  .badge-red { background: rgba(248,81,73,.15); color: var(--red); }
  .badge-purple { background: rgba(163,113,247,.15); color: var(--purple); }

  /* CALLOUT */
  .callout { border-radius: 8px; padding: 14px 16px; margin: 16px 0; border-left: 3px solid; font-size: 14px; }
  .callout-info { background: rgba(56,139,253,.08); border-color: var(--blue); color: #b0caff; }
  .callout-warn { background: rgba(210,153,34,.08); border-color: var(--amber); color: #f0c060; }
  .callout-danger { background: rgba(248,81,73,.08); border-color: var(--red); color: #ffb3b0; }
  .callout-success { background: rgba(63,185,80,.08); border-color: var(--green); color: #80ff99; }
  .callout strong { color: inherit; }

  /* TABLES */
  .tbl-wrap { overflow-x: auto; margin: 16px 0; }
  table { width: 100%; border-collapse: collapse; font-size: 13px; }
  th { background: var(--bg3); color: var(--text2); font-weight: 600; padding: 10px 14px; text-align: left; border-bottom: 1px solid var(--border); }
  td { padding: 9px 14px; border-bottom: 1px solid var(--border); color: var(--text2); }
  tr:last-child td { border-bottom: none; }
  tr:hover td { background: rgba(255,255,255,.02); }
  td strong { color: var(--text); }

  /* CARDS */
  .card-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 14px; margin: 20px 0; }
  .card { background: var(--bg2); border: 1px solid var(--border); border-radius: 10px; padding: 18px; }
  .card-title { font-size: 13px; font-weight: 600; color: var(--text); margin-bottom: 6px; }
  .card-val { font-size: 24px; font-weight: 700; }
  .card-desc { font-size: 12px; color: var(--text3); margin-top: 4px; }
  .card-blue { border-color: var(--blue3); }
  .card-blue .card-val { color: var(--blue); }
  .card-green { border-color: var(--green2); }
  .card-green .card-val { color: var(--green); }
  .card-amber { border-color: var(--amber2); }
  .card-amber .card-val { color: var(--amber); }
  .card-red { border-color: var(--red2); }
  .card-red .card-val { color: var(--red); }

  /* SVG DIAGRAM WRAPPERS */
  .diagram-wrap { background: var(--bg2); border: 1px solid var(--border); border-radius: 10px; padding: 24px; margin: 20px 0; overflow-x: auto; }
  .diagram-caption { font-size: 12px; color: var(--text3); text-align: center; margin-top: 10px; }

  /* INTERACTIVE COMPONENTS */
  .interactive-box { background: var(--bg2); border: 1px solid var(--border); border-radius: 10px; padding: 24px; margin: 20px 0; }
  .ctrl-row { display: flex; align-items: center; gap: 12px; margin: 10px 0; flex-wrap: wrap; }
  .ctrl-label { font-size: 13px; color: var(--text2); min-width: 160px; }
  input[type=range] { flex: 1; min-width: 120px; accent-color: var(--blue); cursor: pointer; }
  .ctrl-val { font-size: 13px; font-weight: 600; color: var(--blue); min-width: 60px; }
  .readout-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(130px, 1fr)); gap: 10px; margin: 16px 0; }
  .readout { background: var(--bg3); border: 1px solid var(--border); border-radius: 6px; padding: 10px; text-align: center; }
  .readout-label { font-size: 11px; color: var(--text3); }
  .readout-val { font-size: 18px; font-weight: 600; margin-top: 2px; }
  .status-bar { display: flex; align-items: center; gap: 10px; padding: 10px 14px; border-radius: 6px; font-size: 13px; font-weight: 500; margin: 12px 0; }
  .status-ok { background: rgba(63,185,80,.1); color: var(--green); border: 1px solid rgba(63,185,80,.3); }
  .status-warn { background: rgba(210,153,34,.1); color: var(--amber); border: 1px solid rgba(210,153,34,.3); }
  .status-err { background: rgba(248,81,73,.1); color: var(--red); border: 1px solid rgba(248,81,73,.3); }
  .dot { width: 8px; height: 8px; border-radius: 50%; background: currentColor; }

  /* MOSFET ANIMATION */
  @keyframes pulse { 0%,100%{opacity:1} 50%{opacity:.4} }
  @keyframes flow { from{stroke-dashoffset:20} to{stroke-dashoffset:0} }
  .flow-on { stroke-dasharray: 6 3; animation: flow .6s linear infinite; }
  .flow-off { stroke-dasharray: 6 3; stroke: var(--red); opacity: .3; }

  /* STEP TABS */
  .tabs { display: flex; gap: 4px; margin-bottom: 16px; flex-wrap: wrap; }
  .tab { padding: 7px 16px; border-radius: 6px; border: 1px solid var(--border); background: var(--bg3); color: var(--text2); cursor: pointer; font-size: 13px; transition: all .15s; }
  .tab.active { background: var(--blue3); border-color: var(--blue2); color: #fff; }
  .tab-content { display: none; }
  .tab-content.active { display: block; }

  /* PROGRESS/BAR */
  .bar-wrap { margin: 8px 0; }
  .bar-label { display: flex; justify-content: space-between; font-size: 12px; color: var(--text3); margin-bottom: 4px; }
  .bar-track { height: 6px; background: var(--bg3); border-radius: 3px; overflow: hidden; }
  .bar-fill { height: 100%; border-radius: 3px; transition: width .4s; }

  /* EQUATION */
  .eq { background: var(--bg3); border: 1px solid var(--border); border-radius: 6px; padding: 12px 18px; font-family: var(--mono); font-size: 14px; color: #ffa657; margin: 12px 0; display: inline-block; }
  .eq-wrap { margin: 12px 0; }

  /* GRID 2-COL */
  .grid2 { display: grid; grid-template-columns: 1fr 1fr; gap: 20px; margin: 16px 0; }
  @media(max-width:640px){ .grid2 { grid-template-columns: 1fr; } }

  /* TOP BADGE ROW */
  .badge-row { display: flex; gap: 8px; flex-wrap: wrap; margin-bottom: 24px; }

  /* HERO */
  .hero { background: linear-gradient(135deg, rgba(56,139,253,.1) 0%, rgba(163,113,247,.1) 100%); border: 1px solid var(--border); border-radius: 12px; padding: 32px; margin-bottom: 48px; }
  .hero h1 { font-size: 32px; font-weight: 700; margin-bottom: 8px; background: linear-gradient(90deg, var(--blue), var(--purple)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text; }
  .hero p { color: var(--text2); font-size: 16px; line-height: 1.6; }
  .hero-meta { display: flex; gap: 16px; margin-top: 20px; flex-wrap: wrap; }
  .hero-meta span { font-size: 12px; color: var(--text3); }
  .hero-meta span strong { color: var(--text2); }
</style>
</head>
<body>
<div class="layout">

<!-- SIDEBAR -->
<nav>
  <div class="nav-logo">
    <h1>⚡ BMS Theory</h1>
    <p>Battery Management System</p>
  </div>
  <div class="nav-section">Pendahuluan</div>
  <a href="#intro">Mengapa BMS Penting?</a>
  <a href="#arsitektur">Arsitektur Sistem</a>
  <div class="nav-section">Sensing</div>
  <a href="#voltage">Voltage Sensing</a>
  <a href="#current">Current Sensing</a>
  <a href="#temperature">Temperature Sensing</a>
  <div class="nav-section">Proteksi</div>
  <a href="#threshold">Threshold & Hysteresis</a>
  <a href="#mosfet">Power Path MOSFET</a>
  <a href="#proteksi-sim">Simulasi Proteksi</a>
  <div class="nav-section">Fitur Lanjutan</div>
  <a href="#balancing">Cell Balancing</a>
  <a href="#soc">SOC Estimation</a>
  <div class="nav-section">Desain</div>
  <a href="#ic">Pemilihan IC BMS</a>
  <a href="#mosfet-select">Pemilihan MOSFET</a>
  <a href="#pcb">PCB Layout Tips</a>
  <div class="nav-section">Referensi</div>
  <a href="#troubleshoot">Troubleshooting</a>
  <a href="#formula">Kumpulan Formula</a>
</nav>

<!-- MAIN CONTENT -->
<main>

  <!-- HERO -->
  <div class="hero">
    <h1>Battery Management System</h1>
    <p>Dokumentasi teknis komprehensif: dari prinsip dasar hingga rekayasa BMS untuk berbagai kondisi operasi. Termasuk simulasi interaktif, panduan pemilihan komponen, dan troubleshooting guide.</p>
    <div class="hero-meta">
      <span><strong>Topik:</strong> BMS Engineering</span>
      <span><strong>Level:</strong> Intermediate → Advanced</span>
      <span><strong>Kimia sel:</strong> Li-Ion, LFP, NMC</span>
    </div>
  </div>

  <!-- ═══════════════════════════════════════════════════════ -->
  <!-- 1. MENGAPA BMS PENTING -->
  <!-- ═══════════════════════════════════════════════════════ -->
  <section id="intro">
    <h2>1. Mengapa BMS Itu Wajib Ada?</h2>
    <p>Baterai lithium menyimpan energi sangat tinggi dalam volume kecil — ini kelebihannya. Namun tanpa pengawasan, karakteristik elektrokimianya yang sensitif bisa berujung pada kerusakan permanen atau bahaya fisik.</p>

    <div class="card-grid">
      <div class="card card-red">
        <div class="card-title">🔥 Overcharge</div>
        <div class="card-val">&gt;4.2V</div>
        <div class="card-desc">Elektrolit terurai → panas → thermal runaway → terbakar</div>
      </div>
      <div class="card card-amber">
        <div class="card-title">⚡ Overdischarge</div>
        <div class="card-val">&lt;2.5V</div>
        <div class="card-desc">Struktur kristal anode rusak permanen, kapasitas turun drastis</div>
      </div>
      <div class="card card-amber">
        <div class="card-title">🌡️ Overtemperature</div>
        <div class="card-val">&gt;60°C</div>
        <div class="card-desc">Plating lithium metalik saat charge → short circuit internal</div>
      </div>
      <div class="card card-blue">
        <div class="card-title">⚡ Overcurrent</div>
        <div class="card-val">&gt;C-rate</div>
        <div class="card-desc">Panas berlebih, kenaikan resistansi internal, sel kembung</div>
      </div>
    </div>

    <div class="callout callout-danger">
      <strong>Thermal Runaway:</strong> Reaksi berantai eksotermik yang self-sustaining. Dimulai dari satu sel panas → memanas sel tetangga → pack terbakar total. BMS adalah pencegahan lini pertama.
    </div>

    <h3>Kurva Tegangan vs Kapasitas</h3>
    <p>Memahami kurva ini krusial untuk menentukan threshold yang tepat.</p>
    <div class="diagram-wrap">
      <svg width="100%" viewBox="0 0 700 300" role="img">
        <title>Kurva tegangan discharge baterai lithium</title>
        <defs>
          <marker id="arr" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse">
            <path d="M2 1L8 5L2 9" fill="none" stroke="context-stroke" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
          </marker>
        </defs>
        <!-- Grid -->
        <line x1="60" y1="20" x2="60" y2="240" stroke="#30363d" stroke-width="1"/>
        <line x1="60" y1="240" x2="660" y2="240" stroke="#30363d" stroke-width="1"/>
        <!-- Y axis labels -->
        <text x="50" y="45" fill="#8b949e" font-size="11" text-anchor="end">4.2V</text>
        <text x="50" y="90" fill="#8b949e" font-size="11" text-anchor="end">4.0V</text>
        <text x="50" y="140" fill="#8b949e" font-size="11" text-anchor="end">3.7V</text>
        <text x="50" y="190" fill="#8b949e" font-size="11" text-anchor="end">3.2V</text>
        <text x="50" y="225" fill="#8b949e" font-size="11" text-anchor="end">2.5V</text>
        <!-- Grid lines -->
        <line x1="60" y1="45" x2="660" y2="45" stroke="#21262d" stroke-width="0.5"/>
        <line x1="60" y1="90" x2="660" y2="90" stroke="#21262d" stroke-width="0.5"/>
        <line x1="60" y1="140" x2="660" y2="140" stroke="#21262d" stroke-width="0.5"/>
        <line x1="60" y1="190" x2="660" y2="190" stroke="#21262d" stroke-width="0.5"/>
        <line x1="60" y1="225" x2="660" y2="225" stroke="#21262d" stroke-width="0.5"/>
        <!-- Curve NMC (blue) -->
        <path d="M60,42 C100,45 150,60 200,100 C280,150 350,155 450,160 C520,163 570,175 610,195 C630,205 645,218 660,235"
              fill="none" stroke="#388bfd" stroke-width="2.5"/>
        <!-- Curve LFP (green) -->
        <path d="M60,55 C80,58 120,75 160,100 C200,120 240,135 350,138 C450,140 530,145 580,160 C620,172 645,200 660,235"
              fill="none" stroke="#3fb950" stroke-width="2.5" stroke-dasharray="6 3"/>
        <!-- Safe zone fill -->
        <rect x="60" y="45" width="560" height="180" fill="rgba(56,139,253,.04)" rx="2"/>
        <!-- OV line -->
        <line x1="60" y1="42" x2="660" y2="42" stroke="#f85149" stroke-width="1" stroke-dasharray="4 3"/>
        <text x="665" y="46" fill="#f85149" font-size="10">OV cutoff</text>
        <!-- UV line -->
        <line x1="60" y1="225" x2="660" y2="225" stroke="#f85149" stroke-width="1" stroke-dasharray="4 3"/>
        <text x="665" y="229" fill="#f85149" font-size="10">UV cutoff</text>
        <!-- Zone labels -->
        <text x="100" y="28" fill="#f85149" font-size="11" font-weight="500">OVERCHARGE ZONE</text>
        <text x="100" y="270" fill="#f85149" font-size="11" font-weight="500">OVERDISCHARGE ZONE</text>
        <text x="310" y="120" fill="#56d3ec" font-size="12" font-weight="500" text-anchor="middle">✓ SAFE OPERATING ZONE</text>
        <!-- X axis -->
        <text x="360" y="260" fill="#8b949e" font-size="11" text-anchor="middle">Kapasitas (0% → 100%)</text>
        <text x="60" y="260" fill="#8b949e" font-size="10">0%</text>
        <text x="655" y="260" fill="#8b949e" font-size="10">100%</text>
        <!-- Legend -->
        <line x1="400" y1="280" x2="430" y2="280" stroke="#388bfd" stroke-width="2.5"/>
        <text x="435" y="284" fill="#8b949e" font-size="11">NMC/LCO</text>
        <line x1="530" y1="280" x2="560" y2="280" stroke="#3fb950" stroke-width="2.5" stroke-dasharray="6 3"/>
        <text x="565" y="284" fill="#8b949e" font-size="11">LFP</text>
        <!-- Y label -->
        <text x="14" y="140" fill="#8b949e" font-size="11" text-anchor="middle" transform="rotate(-90,14,140)">Tegangan Sel (V)</text>
      </svg>
      <p class="diagram-caption">Gambar 1 — Kurva discharge NMC (solid) vs LFP (dashed). Zona merah = zona bahaya yang diproteksi BMS.</p>
    </div>
  </section>

  <!-- ═══════════════════════════════════════════════════════ -->
  <!-- 2. ARSITEKTUR -->
  <!-- ═══════════════════════════════════════════════════════ -->
  <section id="arsitektur">
    <h2>2. Arsitektur BMS</h2>
    <p>Setiap BMS — dari yang paling sederhana hingga automotive-grade — selalu memiliki tiga fungsi utama yang bekerja secara pipeline:</p>

    <div class="diagram-wrap">
      <svg width="100%" viewBox="0 0 700 200" role="img">
        <title>Arsitektur tiga fungsi utama BMS</title>
        <defs>
          <marker id="arr2" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse">
            <path d="M2 1L8 5L2 9" fill="none" stroke="context-stroke" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
          </marker>
        </defs>
        <!-- Input: Baterai -->
        <rect x="10" y="70" width="110" height="60" rx="8" fill="rgba(56,139,253,.12)" stroke="#388bfd" stroke-width="1.5"/>
        <text x="65" y="96" fill="#388bfd" font-size="13" font-weight="600" text-anchor="middle">Baterai</text>
        <text x="65" y="112" fill="#8b949e" font-size="11" text-anchor="middle">V, I, T signals</text>
        <!-- Arrow -->
        <line x1="122" y1="100" x2="155" y2="100" stroke="#484f58" stroke-width="1.5" marker-end="url(#arr2)"/>
        <!-- Box 1: Sensing -->
        <rect x="157" y="55" width="130" height="90" rx="8" fill="rgba(163,113,247,.12)" stroke="#a371f7" stroke-width="1.5"/>
        <text x="222" y="85" fill="#a371f7" font-size="14" font-weight="600" text-anchor="middle">SENSING</text>
        <text x="222" y="103" fill="#8b949e" font-size="11" text-anchor="middle">Voltage per sel</text>
        <text x="222" y="117" fill="#8b949e" font-size="11" text-anchor="middle">Arus (shunt)</text>
        <text x="222" y="131" fill="#8b949e" font-size="11" text-anchor="middle">Suhu (NTC)</text>
        <!-- Arrow -->
        <line x1="289" y1="100" x2="322" y2="100" stroke="#484f58" stroke-width="1.5" marker-end="url(#arr2)"/>
        <!-- Box 2: Processing -->
        <rect x="324" y="55" width="130" height="90" rx="8" fill="rgba(56,139,253,.12)" stroke="#388bfd" stroke-width="1.5"/>
        <text x="389" y="85" fill="#388bfd" font-size="14" font-weight="600" text-anchor="middle">PROCESSING</text>
        <text x="389" y="103" fill="#8b949e" font-size="11" text-anchor="middle">Compare threshold</text>
        <text x="389" y="117" fill="#8b949e" font-size="11" text-anchor="middle">SOC estimation</text>
        <text x="389" y="131" fill="#8b949e" font-size="11" text-anchor="middle">Cell balancing</text>
        <!-- Arrow -->
        <line x1="456" y1="100" x2="489" y2="100" stroke="#484f58" stroke-width="1.5" marker-end="url(#arr2)"/>
        <!-- Box 3: Acting -->
        <rect x="491" y="55" width="130" height="90" rx="8" fill="rgba(63,185,80,.12)" stroke="#3fb950" stroke-width="1.5"/>
        <text x="556" y="85" fill="#3fb950" font-size="14" font-weight="600" text-anchor="middle">ACTING</text>
        <text x="556" y="103" fill="#8b949e" font-size="11" text-anchor="middle">MOSFET control</text>
        <text x="556" y="117" fill="#8b949e" font-size="11" text-anchor="middle">Balancing switch</text>
        <text x="556" y="131" fill="#8b949e" font-size="11" text-anchor="middle">Alert / CAN bus</text>
        <!-- Output arrow -->
        <line x1="623" y1="100" x2="658" y2="100" stroke="#3fb950" stroke-width="1.5" marker-end="url(#arr2)"/>
        <text x="665" y="96" fill="#3fb950" font-size="11">Load/</text>
        <text x="665" y="108" fill="#3fb950" font-size="11">Charger</text>
        <!-- Labels -->
        <text x="222" y="160" fill="#484f58" font-size="10" text-anchor="middle">AFE / IC</text>
        <text x="389" y="160" fill="#484f58" font-size="10" text-anchor="middle">MCU / Logic</text>
        <text x="556" y="160" fill="#484f58" font-size="10" text-anchor="middle">Gate Driver / FET</text>
      </svg>
      <p class="diagram-caption">Gambar 2 — Pipeline tiga fungsi utama BMS: Sense → Process → Act</p>
    </div>

    <h3>Topologi Pack: Seri vs Paralel</h3>
    <div class="grid2">
      <div>
        <h4>Konfigurasi Seri (xS)</h4>
        <p>Tegangan bertambah, kapasitas tetap. Digunakan untuk meningkatkan tegangan sistem.</p>
        <div class="eq-wrap"><span class="eq">V_pack = n × V_sel</span></div>
        <p><strong>Contoh:</strong> 4S LFP = 4 × 3.2V = 12.8V nominal</p>
      </div>
      <div>
        <h4>Konfigurasi Paralel (xP)</h4>
        <p>Kapasitas bertambah, tegangan tetap. Digunakan untuk meningkatkan arus dan energi.</p>
        <div class="eq-wrap"><span class="eq">C_pack = n × C_sel</span></div>
        <p><strong>Contoh:</strong> 3P 3000mAh = 9000mAh pack</p>
      </div>
    </div>
    <div class="callout callout-info">
      <strong>Notasi xSyP:</strong> Pack disebut sebagai "4S3P" artinya 4 sel seri × 3 paralel = 12 sel total. BMS harus mampu memonitor semua grup seri (dalam contoh ini: 4 VC channels).
    </div>
  </section>

  <!-- ═══════════════════════════════════════════════════════ -->
  <!-- 3. VOLTAGE SENSING -->
  <!-- ═══════════════════════════════════════════════════════ -->
  <section id="voltage">
    <h2>3. Voltage Sensing</h2>
    <p>Setiap sel dalam pack harus diukur <strong>secara individual</strong>. Mengukur total tegangan pack saja tidak cukup — sel yang paling lemah menentukan performa seluruh pack.</p>

    <h3>Mengapa Individual Cell Monitoring Penting?</h3>
    <div class="diagram-wrap">
      <svg width="100%" viewBox="0 0 700 180" role="img">
        <title>Ilustrasi bahaya sel lemah dalam pack seri</title>
        <defs>
          <marker id="arr3" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse">
            <path d="M2 1L8 5L2 9" fill="none" stroke="context-stroke" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
          </marker>
        </defs>
        <!-- Pack label -->
        <text x="20" y="30" fill="#8b949e" font-size="12">Pack 4S — Tegangan Total: 13.7V (terlihat "normal")</text>
        <!-- Sel 1 -->
        <rect x="20" y="50" width="130" height="70" rx="6" fill="rgba(56,139,253,.15)" stroke="#388bfd" stroke-width="1.5"/>
        <text x="85" y="82" fill="#388bfd" font-size="16" font-weight="700" text-anchor="middle">3.8V</text>
        <text x="85" y="100" fill="#8b949e" font-size="11" text-anchor="middle">Sel 1 ✓</text>
        <!-- Sel 2 -->
        <rect x="170" y="50" width="130" height="70" rx="6" fill="rgba(56,139,253,.15)" stroke="#388bfd" stroke-width="1.5"/>
        <text x="235" y="82" fill="#388bfd" font-size="16" font-weight="700" text-anchor="middle">3.8V</text>
        <text x="235" y="100" fill="#8b949e" font-size="11" text-anchor="middle">Sel 2 ✓</text>
        <!-- Sel 3 -->
        <rect x="320" y="50" width="130" height="70" rx="6" fill="rgba(56,139,253,.15)" stroke="#388bfd" stroke-width="1.5"/>
        <text x="385" y="82" fill="#388bfd" font-size="16" font-weight="700" text-anchor="middle">3.7V</text>
        <text x="385" y="100" fill="#8b949e" font-size="11" text-anchor="middle">Sel 3 ✓</text>
        <!-- Sel 4 — KRITIS -->
        <rect x="470" y="50" width="130" height="70" rx="6" fill="rgba(248,81,73,.15)" stroke="#f85149" stroke-width="2.5"/>
        <text x="535" y="82" fill="#f85149" font-size="16" font-weight="700" text-anchor="middle">2.4V</text>
        <text x="535" y="100" fill="#f85149" font-size="12" font-weight="600" text-anchor="middle">⚠ SEL KRITIS!</text>
        <!-- Connectors -->
        <line x1="152" y1="85" x2="168" y2="85" stroke="#484f58" stroke-width="2"/>
        <line x1="302" y1="85" x2="318" y2="85" stroke="#484f58" stroke-width="2"/>
        <line x1="452" y1="85" x2="468" y2="85" stroke="#484f58" stroke-width="2"/>
        <!-- Warning text -->
        <text x="535" y="145" fill="#f85149" font-size="11" text-anchor="middle">Tanpa cell sensing,</text>
        <text x="535" y="160" fill="#f85149" font-size="11" text-anchor="middle">sel ini tidak terdeteksi!</text>
      </svg>
      <p class="diagram-caption">Gambar 3 — Sel keempat sudah di bawah UV threshold (2.4V), tapi tegangan pack total masih terlihat 13.7V (normal). BMS dengan individual cell monitoring akan mendeteksi ini.</p>
    </div>

    <h3>Topologi Pengukuran Tegangan IC BMS</h3>
    <p>IC BMS menggunakan <strong>flying capacitor multiplexer</strong> atau <strong>resistive divider bertingkat</strong> untuk mengukur tegangan setiap sel relatif terhadap VSS. Pin VC0–VC5 pada bq77915 masing-masing terhubung ke titik junction antar sel.</p>

    <div class="tbl-wrap">
      <table>
        <tr><th>Pin VC</th><th>Mengukur</th><th>Nilai (4S pack fully charged)</th></tr>
        <tr><td><code>VC0</code></td><td>Titik negatif pack (VSS)</td><td>0V (referensi)</td></tr>
        <tr><td><code>VC1</code></td><td>Junction Sel1–Sel2</td><td>4.2V</td></tr>
        <tr><td><code>VC2</code></td><td>Junction Sel2–Sel3</td><td>8.4V</td></tr>
        <tr><td><code>VC3</code></td><td>Junction Sel3–Sel4</td><td>12.6V</td></tr>
        <tr><td><code>VC4/VDD</code></td><td>Titik positif pack</td><td>16.8V</td></tr>
      </table>
    </div>
    <p>IC secara internal menghitung <strong>V_sel = VC[n] − VC[n−1]</strong> untuk mendapatkan tegangan masing-masing sel.</p>
  </section>

  <!-- ═══════════════════════════════════════════════════════ -->
  <!-- 4. CURRENT SENSING -->
  <!-- ═══════════════════════════════════════════════════════ -->
  <section id="current">
    <h2>4. Current Sensing</h2>
    <p>Pengukuran arus menggunakan <strong>shunt resistor</strong> yang dipasang secara seri di jalur PACK−. IC BMS mengukur tegangan diferensial pada pin <code>SRP</code> dan <code>SRN</code>.</p>

    <div class="eq-wrap" style="text-align:center">
      <span class="eq">I = V_shunt / R_SNS = (V_SRP − V_SRN) / R_SNS</span>
    </div>

    <h3>Simulasi Pemilihan Shunt Resistor</h3>
    <div class="interactive-box">
      <p style="font-size:13px; color: var(--text3); margin-bottom:16px">Geser untuk melihat trade-off antara akurasi sinyal dan rugi daya</p>
      <div class="ctrl-row">
        <span class="ctrl-label">Resistansi Shunt (R_SNS)</span>
        <input type="range" id="r-shunt" min="1" max="20" value="5" oninput="calcShunt()">
        <span class="ctrl-val" id="r-val">5 mΩ</span>
      </div>
      <div class="ctrl-row">
        <span class="ctrl-label">Arus Maksimum (I_max)</span>
        <input type="range" id="i-max" min="5" max="100" value="20" oninput="calcShunt()">
        <span class="ctrl-val" id="i-val">20 A</span>
      </div>
      <div class="readout-grid">
        <div class="readout">
          <div class="readout-label">Tegangan Shunt</div>
          <div class="readout-val" id="v-shunt" style="color:var(--blue)">100 mV</div>
        </div>
        <div class="readout">
          <div class="readout-label">Rugi Daya</div>
          <div class="readout-val" id="p-loss" style="color:var(--amber)">2.0 W</div>
        </div>
        <div class="readout">
          <div class="readout-label">Efisiensi (10A)</div>
          <div class="readout-val" id="eff" style="color:var(--green)">99.8%</div>
        </div>
        <div class="readout">
          <div class="readout-label">Rekomendasi ADC</div>
          <div class="readout-val" id="adc-rec" style="color:var(--purple); font-size:14px">12-bit</div>
        </div>
      </div>
      <div id="shunt-status" class="status-bar status-ok"><div class="dot"></div><span id="shunt-msg">Parameter optimal untuk aplikasi umum</span></div>
    </div>

    <h3>Tipe Current Sensing</h3>
    <div class="tbl-wrap">
      <table>
        <tr><th>Metode</th><th>Akurasi</th><th>Biaya</th><th>Isolasi</th><th>Cocok untuk</th></tr>
        <tr><td><strong>Shunt Resistor</strong></td><td>±0.5–1%</td><td>Rendah</td><td>Tidak</td><td>Sebagian besar aplikasi BMS</td></tr>
        <tr><td><strong>Hall Effect Sensor</strong></td><td>±1–3%</td><td>Menengah</td><td>Ya (galvanik)</td><td>Arus > 200A, EV</td></tr>
        <tr><td><strong>Current Transformer</strong></td><td>±0.2–1%</td><td>Menengah</td><td>Ya</td><td>Hanya AC, power grid</td></tr>
        <tr><td><strong>Rogowski Coil</strong></td><td>±0.5%</td><td>Tinggi</td><td>Ya</td><td>Arus sangat besar, transient</td></tr>
      </table>
    </div>
  </section>

  <!-- ═══════════════════════════════════════════════════════ -->
  <!-- 5. TEMPERATURE SENSING -->
  <!-- ═══════════════════════════════════════════════════════ -->
  <section id="temperature">
    <h2>5. Temperature Sensing</h2>
    <p>Sensor suhu menggunakan <strong>NTC thermistor</strong> (Negative Temperature Coefficient). Resistansinya turun secara eksponensial saat suhu naik, mengikuti persamaan Steinhart-Hart.</p>

    <div class="eq-wrap">
      <span class="eq">R_NTC = R₀ × exp[ B × (1/T − 1/T₀) ]</span>
    </div>
    <p>IC BMS mengukur tegangan pada voltage divider di pin <code>TS</code>. Makin panas → R_NTC turun → tegangan TS turun → IC mendeteksi suhu tinggi.</p>

    <div class="diagram-wrap">
      <svg width="100%" viewBox="0 0 700 180" role="img">
        <title>Voltage divider NTC thermistor untuk temperature sensing</title>
        <defs>
          <marker id="arr4" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse">
            <path d="M2 1L8 5L2 9" fill="none" stroke="context-stroke" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
          </marker>
        </defs>
        <!-- Circuit -->
        <!-- VDD -->
        <line x1="200" y1="20" x2="200" y2="50" stroke="#388bfd" stroke-width="2"/>
        <text x="200" y="15" fill="#388bfd" font-size="12" text-anchor="middle">VDD (3.3V)</text>
        <!-- R_pullup -->
        <rect x="175" y="50" width="50" height="30" rx="4" fill="rgba(56,139,253,.15)" stroke="#388bfd" stroke-width="1.5"/>
        <text x="200" y="70" fill="#388bfd" font-size="11" text-anchor="middle">R_pu</text>
        <!-- Line to junction -->
        <line x1="200" y1="80" x2="200" y2="110" stroke="#8b949e" stroke-width="1.5"/>
        <!-- Junction to TS pin -->
        <line x1="200" y1="110" x2="340" y2="110" stroke="#8b949e" stroke-width="1.5" marker-end="url(#arr4)"/>
        <!-- IC box -->
        <rect x="342" y="85" width="120" height="50" rx="6" fill="rgba(163,113,247,.15)" stroke="#a371f7" stroke-width="1.5"/>
        <text x="402" y="108" fill="#a371f7" font-size="12" text-anchor="middle" font-weight="600">BMS IC</text>
        <text x="402" y="124" fill="#8b949e" font-size="11" text-anchor="middle">pin TS (ADC)</text>
        <!-- NTC -->
        <line x1="200" y1="110" x2="200" y2="130" stroke="#8b949e" stroke-width="1.5"/>
        <rect x="175" y="130" width="50" height="30" rx="4" fill="rgba(248,81,73,.15)" stroke="#f85149" stroke-width="1.5"/>
        <text x="200" y="150" fill="#f85149" font-size="11" text-anchor="middle">NTC</text>
        <!-- GND -->
        <line x1="200" y1="160" x2="200" y2="175" stroke="#8b949e" stroke-width="1.5"/>
        <text x="200" y="172" fill="#8b949e" font-size="12" text-anchor="middle">⏚</text>
        <!-- Labels right -->
        <text x="480" y="50" fill="#8b949e" font-size="12">Formula:</text>
        <text x="480" y="70" fill="#56d3ec" font-size="12">V_TS = VDD × R_NTC / (R_pu + R_NTC)</text>
        <text x="480" y="95" fill="#8b949e" font-size="11">Suhu naik → R_NTC turun</text>
        <text x="480" y="112" fill="#8b949e" font-size="11">→ V_TS turun → IC deteksi panas</text>
        <text x="480" y="140" fill="#f85149" font-size="11">Pasang NTC sedekat mungkin</text>
        <text x="480" y="155" fill="#f85149" font-size="11">dengan sel yang paling panas!</text>
      </svg>
      <p class="diagram-caption">Gambar 4 — Rangkaian voltage divider NTC thermistor ke pin TS pada IC BMS</p>
    </div>

    <div class="tbl-wrap">
      <table>
        <tr><th>Suhu (°C)</th><th>R_NTC (10kΩ @ 25°C, B=3950)</th><th>V_TS (R_pu=10kΩ, VDD=3.3V)</th><th>Status</th></tr>
        <tr><td>−20°C</td><td>~98 kΩ</td><td>3.00V</td><td><span class="badge badge-blue">Dingin</span></td></tr>
        <tr><td>0°C</td><td>~32 kΩ</td><td>2.50V</td><td><span class="badge badge-blue">Normal</span></td></tr>
        <tr><td>25°C</td><td>10 kΩ</td><td>1.65V</td><td><span class="badge badge-green">Nominal</span></td></tr>
        <tr><td>45°C</td><td>~4.2 kΩ</td><td>0.97V</td><td><span class="badge badge-amber">Charge limit</span></td></tr>
        <tr><td>60°C</td><td>~2.2 kΩ</td><td>0.57V</td><td><span class="badge badge-red">OT cutoff</span></td></tr>
      </table>
    </div>
  </section>

  <!-- ═══════════════════════════════════════════════════════ -->
  <!-- 6. THRESHOLD & HYSTERESIS -->
  <!-- ═══════════════════════════════════════════════════════ -->
  <section id="threshold">
    <h2>6. Threshold &amp; Hysteresis</h2>
    <p>Threshold adalah batas parameter yang memicu proteksi. <strong>Hysteresis</strong> adalah perbedaan antara threshold trigger dan threshold recovery — sangat penting untuk mencegah "flapping" (ON-OFF-ON-OFF cepat yang merusak MOSFET).</p>

    <h3>Visualisasi Hysteresis OV</h3>
    <div class="diagram-wrap">
      <svg width="100%" viewBox="0 0 700 220" role="img">
        <title>Visualisasi hysteresis pada overvoltage protection</title>
        <!-- Time axis -->
        <line x1="40" y1="190" x2="660" y2="190" stroke="#30363d" stroke-width="1" marker-end="url(#arr)"/>
        <line x1="40" y1="20" x2="40" y2="190" stroke="#30363d" stroke-width="1"/>
        <defs>
          <marker id="arr" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse">
            <path d="M2 1L8 5L2 9" fill="none" stroke="context-stroke" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
          </marker>
        </defs>
        <!-- Y labels -->
        <text x="36" y="58" fill="#f85149" font-size="11" text-anchor="end">4.25V</text>
        <text x="36" y="90" fill="#3fb950" font-size="11" text-anchor="end">4.20V</text>
        <text x="36" y="130" fill="#8b949e" font-size="11" text-anchor="end">4.10V</text>
        <!-- Threshold lines -->
        <line x1="40" y1="58" x2="660" y2="58" stroke="#f85149" stroke-width="1" stroke-dasharray="5 3"/>
        <line x1="40" y1="90" x2="660" y2="90" stroke="#3fb950" stroke-width="1" stroke-dasharray="5 3"/>
        <!-- Labels for threshold lines -->
        <text x="665" y="62" fill="#f85149" font-size="10">OV Trigger</text>
        <text x="665" y="94" fill="#3fb950" font-size="10">OV Recovery</text>
        <!-- Voltage curve -->
        <path d="M50,160 C100,140 150,110 200,80 C220,62 240,52 260,52 C270,52 275,55 285,55"
              fill="none" stroke="#388bfd" stroke-width="2.5"/>
        <!-- OV triggered zone (red fill) -->
        <rect x="260" y="52" width="80" height="6" rx="2" fill="rgba(248,81,73,.3)"/>
        <path d="M285,55 C295,55 300,58 310,58 C330,58 340,52 350,42"
              fill="none" stroke="#388bfd" stroke-width="2.5"/>
        <line x1="260" y1="52" x2="260" y2="190" stroke="#f85149" stroke-width="1" stroke-dasharray="3 3" opacity=".5"/>
        <!-- MOSFET OFF indicator -->
        <rect x="260" y="160" width="90" height="20" rx="4" fill="rgba(248,81,73,.15)" stroke="#f85149" stroke-width="1"/>
        <text x="305" y="174" fill="#f85149" font-size="11" text-anchor="middle">MOSFET OFF</text>
        <!-- Recovery -->
        <path d="M350,42 C370,35 400,88 430,86 C450,85 470,88 500,90"
              fill="none" stroke="#388bfd" stroke-width="2.5" stroke-dasharray="6 3" opacity=".7"/>
        <line x1="430" y1="86" x2="430" y2="190" stroke="#3fb950" stroke-width="1" stroke-dasharray="3 3" opacity=".5"/>
        <rect x="430" y="160" width="90" height="20" rx="4" fill="rgba(63,185,80,.15)" stroke="#3fb950" stroke-width="1"/>
        <text x="475" y="174" fill="#3fb950" font-size="11" text-anchor="middle">MOSFET ON</text>
        <!-- Hysteresis brace -->
        <line x1="300" y1="58" x2="300" y2="90" stroke="#a371f7" stroke-width="1.5" marker-end="url(#arr)"/>
        <line x1="300" y1="90" x2="300" y2="58" stroke="#a371f7" stroke-width="1.5" marker-end="url(#arr)"/>
        <text x="308" y="78" fill="#a371f7" font-size="11">Hysteresis</text>
        <text x="308" y="90" fill="#a371f7" font-size="11">= 0.05V</text>
        <!-- Axis labels -->
        <text x="350" y="205" fill="#8b949e" font-size="11" text-anchor="middle">Waktu →</text>
        <text x="14" y="120" fill="#8b949e" font-size="11" text-anchor="middle" transform="rotate(-90,14,120)">Tegangan</text>
      </svg>
      <p class="diagram-caption">Gambar 5 — Hysteresis mencegah MOSFET toggle berulang kali ketika tegangan berada tepat di batas threshold</p>
    </div>

    <h3>Tabel Threshold Standar per Kimia Sel</h3>
    <div class="tbl-wrap">
      <table>
        <tr><th>Parameter</th><th>NMC/LCO</th><th>LFP</th><th>NCA</th><th>LTO</th></tr>
        <tr><td><strong>OV Cutoff</strong></td><td>4.20–4.25V</td><td>3.65V</td><td>4.20V</td><td>2.85V</td></tr>
        <tr><td><strong>OV Recovery</strong></td><td>4.15–4.18V</td><td>3.55V</td><td>4.15V</td><td>2.75V</td></tr>
        <tr><td><strong>UV Cutoff</strong></td><td>2.50–2.80V</td><td>2.50V</td><td>2.50V</td><td>1.50V</td></tr>
        <tr><td><strong>UV Recovery</strong></td><td>2.90–3.00V</td><td>2.80V</td><td>2.90V</td><td>1.80V</td></tr>
        <tr><td><strong>OT Charge</strong></td><td>45°C</td><td>45°C</td><td>45°C</td><td>55°C</td></tr>
        <tr><td><strong>OT Discharge</strong></td><td>60°C</td><td>60°C</td><td>60°C</td><td>70°C</td></tr>
        <tr><td><strong>Nominal Voltage</strong></td><td>3.60–3.70V</td><td>3.20–3.30V</td><td>3.65V</td><td>2.30V</td></tr>
      </table>
    </div>
    <div class="callout callout-warn">
      <strong>Penting:</strong> Threshold di atas adalah panduan umum. Selalu rujuk datasheet sel spesifik yang digunakan. Beberapa sel premium NMC dapat dicharge hingga 4.35V atau bahkan 4.45V.
    </div>
  </section>

  <!-- ═══════════════════════════════════════════════════════ -->
  <!-- 7. POWER PATH MOSFET -->
  <!-- ═══════════════════════════════════════════════════════ -->
  <section id="mosfet">
    <h2>7. Power Path MOSFET</h2>
    <p>Jantung dari proteksi hardware BMS adalah dua MOSFET yang dipasang back-to-back di jalur negatif. Konfigurasi ini memungkinkan BMS memblokir arus dari kedua arah secara independen.</p>

    <div class="diagram-wrap">
      <svg width="100%" viewBox="0 0 700 260" role="img" id="mosfet-svg">
        <title>Topologi back-to-back MOSFET pada power path BMS</title>
        <defs>
          <marker id="arr5" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse">
            <path d="M2 1L8 5L2 9" fill="none" stroke="context-stroke" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
          </marker>
        </defs>

        <!-- PACK+ line -->
        <line x1="20" y1="50" x2="680" y2="50" stroke="#3fb950" stroke-width="2.5"/>
        <text x="30" y="40" fill="#3fb950" font-size="12" font-weight="600">PACK+</text>

        <!-- Battery cells (left) -->
        <rect x="20" y="40" width="80" height="170" rx="6" fill="rgba(56,139,253,.1)" stroke="#388bfd" stroke-width="1.5"/>
        <text x="60" y="75" fill="#388bfd" font-size="11" text-anchor="middle">Sel 4</text>
        <text x="60" y="100" fill="#388bfd" font-size="11" text-anchor="middle">Sel 3</text>
        <text x="60" y="125" fill="#388bfd" font-size="11" text-anchor="middle">Sel 2</text>
        <text x="60" y="150" fill="#388bfd" font-size="11" text-anchor="middle">Sel 1</text>
        <text x="60" y="62" fill="#8b949e" font-size="9" text-anchor="middle">Battery</text>
        <text x="60" y="168" fill="#8b949e" font-size="9" text-anchor="middle">Pack</text>

        <!-- PACK- line -->
        <line x1="100" y1="210" x2="200" y2="210" stroke="#8b949e" stroke-width="2.5"/>
        <!-- R_SNS -->
        <rect x="200" y="198" width="50" height="24" rx="4" fill="rgba(163,113,247,.15)" stroke="#a371f7" stroke-width="1.5"/>
        <text x="225" y="214" fill="#a371f7" font-size="10" text-anchor="middle">R_SNS</text>
        <line x1="250" y1="210" x2="300" y2="210" stroke="#8b949e" stroke-width="2.5"/>

        <!-- MOSFET DSG -->
        <rect x="300" y="185" width="70" height="50" rx="6" fill="rgba(63,185,80,.15)" stroke="#3fb950" stroke-width="2" id="fet-dsg"/>
        <text x="335" y="208" fill="#3fb950" font-size="11" font-weight="600" text-anchor="middle">DSG</text>
        <text x="335" y="222" fill="#8b949e" font-size="10" text-anchor="middle">FET</text>
        <!-- Gate DSG -->
        <line x1="335" y1="185" x2="335" y2="155" stroke="#8b949e" stroke-width="1.5" stroke-dasharray="4 2"/>
        <text x="335" y="148" fill="#8b949e" font-size="10" text-anchor="middle">Gate DSG</text>

        <line x1="370" y1="210" x2="420" y2="210" stroke="#8b949e" stroke-width="2.5"/>

        <!-- MOSFET CHG -->
        <rect x="420" y="185" width="70" height="50" rx="6" fill="rgba(56,139,253,.15)" stroke="#388bfd" stroke-width="2" id="fet-chg"/>
        <text x="455" y="208" fill="#388bfd" font-size="11" font-weight="600" text-anchor="middle">CHG</text>
        <text x="455" y="222" fill="#8b949e" font-size="10" text-anchor="middle">FET</text>
        <!-- Gate CHG -->
        <line x1="455" y1="185" x2="455" y2="155" stroke="#8b949e" stroke-width="1.5" stroke-dasharray="4 2"/>
        <text x="455" y="148" fill="#8b949e" font-size="10" text-anchor="middle">Gate CHG</text>

        <line x1="490" y1="210" x2="560" y2="210" stroke="#8b949e" stroke-width="2.5"/>

        <!-- BMS IC -->
        <rect x="290" y="60" width="200" height="70" rx="8" fill="rgba(163,113,247,.15)" stroke="#a371f7" stroke-width="1.5"/>
        <text x="390" y="82" fill="#a371f7" font-size="13" font-weight="600" text-anchor="middle">BMS IC</text>
        <text x="390" y="98" fill="#8b949e" font-size="11" text-anchor="middle">(bq77915 / similar)</text>
        <text x="390" y="114" fill="#8b949e" font-size="10" text-anchor="middle">DSG pin → Gate driver → FET</text>
        <!-- IC to gate lines -->
        <line x1="355" y1="130" x2="335" y2="148" stroke="#a371f7" stroke-width="1" stroke-dasharray="3 2"/>
        <line x1="425" y1="130" x2="455" y2="148" stroke="#a371f7" stroke-width="1" stroke-dasharray="3 2"/>

        <!-- Load/Charger (right) -->
        <rect x="562" y="40" width="100" height="170" rx="6" fill="rgba(248,81,73,.08)" stroke="#f85149" stroke-width="1"/>
        <text x="612" y="115" fill="#f85149" font-size="12" text-anchor="middle">Load /</text>
        <text x="612" y="130" fill="#f85149" font-size="12" text-anchor="middle">Charger</text>
        <line x1="562" y1="50" x2="662" y2="50" stroke="#3fb950" stroke-width="2" opacity=".5"/>
        <line x1="560" y1="210" x2="562" y2="210" stroke="#8b949e" stroke-width="2.5"/>
        <line x1="562" y1="210" x2="662" y2="210" stroke="#8b949e" stroke-width="1.5" opacity=".5"/>
        <text x="30" y="225" fill="#8b949e" font-size="11">PACK−</text>

        <!-- Body diode symbols -->
        <text x="335" y="240" fill="#8b949e" font-size="9" text-anchor="middle">⊳ body diode</text>
        <text x="455" y="240" fill="#8b949e" font-size="9" text-anchor="middle">body diode ⊲</text>
        <text x="395" y="257" fill="#56d3ec" font-size="10" text-anchor="middle">← Saling berhadapan → blokir arus dua arah</text>
      </svg>
      <p class="diagram-caption">Gambar 6 — Konfigurasi back-to-back MOSFET. DSG FET mengontrol arus discharge, CHG FET mengontrol arus charge.</p>
    </div>

    <h3>Mengapa Harus Back-to-Back?</h3>
    <p>Setiap MOSFET N-channel memiliki <strong>body diode</strong> bawaan. Satu MOSFET saja tidak cukup memblokir arus dari kedua arah:</p>
    <div class="tbl-wrap">
      <table>
        <tr><th>Kondisi</th><th>MOSFET DSG saja</th><th>MOSFET CHG saja</th><th>Back-to-Back</th></tr>
        <tr><td>Blokir discharge (OV)</td><td>✓ FET OFF + body diode</td><td>✗ body diode lewatkan</td><td>✓ CHG OFF blokir</td></tr>
        <tr><td>Blokir charge (OC)</td><td>✗ body diode lewatkan</td><td>✓ FET OFF + body diode</td><td>✓ DSG OFF blokir</td></tr>
        <tr><td>Blokir keduanya</td><td>✗</td><td>✗</td><td>✓✓ keduanya OFF</td></tr>
      </table>
    </div>
  </section>

  <!-- ═══════════════════════════════════════════════════════ -->
  <!-- 8. SIMULASI PROTEKSI -->
  <!-- ═══════════════════════════════════════════════════════ -->
  <section id="proteksi-sim">
    <h2>8. Simulasi Proteksi BMS</h2>
    <p>Simulasikan kondisi operasi pack baterai dan lihat bagaimana BMS merespons secara real-time.</p>

    <div class="interactive-box">
      <div class="tabs">
        <div class="tab active" onclick="simTab('nmc')">NMC 4S Pack</div>
        <div class="tab" onclick="simTab('lfp')">LFP 4S Pack</div>
      </div>

      <div class="ctrl-row">
        <span class="ctrl-label">Tegangan Sel Tertinggi</span>
        <input type="range" id="sim-v" min="2.0" max="4.4" step="0.05" value="3.8" oninput="simUpdate()">
        <span class="ctrl-val" id="sim-v-val">3.80 V</span>
      </div>
      <div class="ctrl-row">
        <span class="ctrl-label">Arus (+ = discharge, − = charge)</span>
        <input type="range" id="sim-i" min="-60" max="60" value="10" oninput="simUpdate()">
        <span class="ctrl-val" id="sim-i-val">+10 A</span>
      </div>
      <div class="ctrl-row">
        <span class="ctrl-label">Suhu Sel</span>
        <input type="range" id="sim-t" min="-10" max="80" value="25" oninput="simUpdate()">
        <span class="ctrl-val" id="sim-t-val">25 °C</span>
      </div>

      <div class="readout-grid">
        <div class="readout">
          <div class="readout-label">MOSFET DSG</div>
          <div class="readout-val" id="dsg-state" style="color:var(--green)">ON</div>
        </div>
        <div class="readout">
          <div class="readout-label">MOSFET CHG</div>
          <div class="readout-val" id="chg-state" style="color:var(--green)">ON</div>
        </div>
        <div class="readout">
          <div class="readout-label">Daya ke Beban</div>
          <div class="readout-val" id="sim-power" style="color:var(--blue)">60.8 W</div>
        </div>
        <div class="readout">
          <div class="readout-label">Fault Code</div>
          <div class="readout-val" id="fault-code" style="color:var(--green); font-size:13px">NONE</div>
        </div>
      </div>

      <div id="sim-status" class="status-bar status-ok">
        <div class="dot"></div>
        <span id="sim-msg">Semua parameter dalam batas aman. MOSFET aktif.</span>
      </div>

      <div style="margin-top:16px">
        <div class="bar-wrap">
          <div class="bar-label"><span>Tegangan vs OV Threshold</span><span id="ov-pct">90%</span></div>
          <div class="bar-track"><div class="bar-fill" id="ov-bar" style="width:90%;background:var(--blue)"></div></div>
        </div>
        <div class="bar-wrap">
          <div class="bar-label"><span>Arus vs OC Threshold</span><span id="oc-pct">20%</span></div>
          <div class="bar-track"><div class="bar-fill" id="oc-bar" style="width:20%;background:var(--green)"></div></div>
        </div>
        <div class="bar-wrap">
          <div class="bar-label"><span>Suhu vs OT Threshold</span><span id="ot-pct">42%</span></div>
          <div class="bar-track"><div class="bar-fill" id="ot-bar" style="width:42%;background:var(--green)"></div></div>
        </div>
      </div>
    </div>
  </section>

  <!-- ═══════════════════════════════════════════════════════ -->
  <!-- 9. CELL BALANCING -->
  <!-- ═══════════════════════════════════════════════════════ -->
  <section id="balancing">
    <h2>9. Cell Balancing</h2>
    <p>Dalam pack multi-sel, ketidakseimbangan tegangan antar sel adalah masalah nyata yang mengurangi umur dan kapasitas efektif pack. Cell balancing adalah mekanisme untuk menyamakan tegangan semua sel.</p>

    <div class="tabs">
      <div class="tab active" onclick="balTab('passive')">Passive Balancing</div>
      <div class="tab" onclick="balTab('active')">Active Balancing</div>
    </div>

    <div id="bal-passive" class="tab-content active">
      <p>Sel yang sudah penuh (tegangan tertinggi) di-bypass melalui resistor — energi lebih dibuang sebagai panas sambil sel lain terus di-charge.</p>
      <div class="diagram-wrap">
        <svg width="100%" viewBox="0 0 700 200" role="img">
          <title>Skema passive cell balancing</title>
          <defs>
            <marker id="arr6" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse">
              <path d="M2 1L8 5L2 9" fill="none" stroke="context-stroke" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
            </marker>
          </defs>
          <!-- 4 cells -->
          <rect x="30" y="50" width="80" height="100" rx="6" fill="rgba(56,139,253,.15)" stroke="#388bfd" stroke-width="1.5"/>
          <text x="70" y="95" fill="#388bfd" font-size="12" text-anchor="middle" font-weight="600">3.80V</text>
          <text x="70" y="112" fill="#8b949e" font-size="10" text-anchor="middle">Sel 1 ✓</text>
          <rect x="140" y="50" width="80" height="100" rx="6" fill="rgba(56,139,253,.15)" stroke="#388bfd" stroke-width="1.5"/>
          <text x="180" y="95" fill="#388bfd" font-size="12" text-anchor="middle" font-weight="600">3.82V</text>
          <text x="180" y="112" fill="#8b949e" font-size="10" text-anchor="middle">Sel 2 ✓</text>
          <!-- Sel 3 — PENUH -->
          <rect x="250" y="30" width="80" height="140" rx="6" fill="rgba(248,81,73,.15)" stroke="#f85149" stroke-width="2.5"/>
          <text x="290" y="95" fill="#f85149" font-size="12" text-anchor="middle" font-weight="700">4.20V</text>
          <text x="290" y="112" fill="#f85149" font-size="10" text-anchor="middle">PENUH → bypass!</text>
          <!-- Bypass resistor -->
          <line x1="290" y1="30" x2="290" y2="10" stroke="#f85149" stroke-width="1.5"/>
          <rect x="260" y="5" width="60" height="16" rx="4" fill="rgba(248,81,73,.2)" stroke="#f85149" stroke-width="1"/>
          <text x="290" y="17" fill="#f85149" font-size="9" text-anchor="middle">R_bal (heat)</text>
          <!-- Sel 4 -->
          <rect x="360" y="50" width="80" height="100" rx="6" fill="rgba(56,139,253,.15)" stroke="#388bfd" stroke-width="1.5"/>
          <text x="400" y="95" fill="#388bfd" font-size="12" text-anchor="middle" font-weight="600">3.85V</text>
          <text x="400" y="112" fill="#8b949e" font-size="10" text-anchor="middle">Sel 4 ✓</text>
          <!-- Labels -->
          <text x="550" y="60" fill="#8b949e" font-size="12" font-weight="500">Trade-off:</text>
          <text x="550" y="80" fill="#3fb950" font-size="11">✓ Sederhana &amp; murah</text>
          <text x="550" y="98" fill="#3fb950" font-size="11">✓ Tidak perlu induktor</text>
          <text x="550" y="116" fill="#f85149" font-size="11">✗ Energi terbuang (panas)</text>
          <text x="550" y="134" fill="#f85149" font-size="11">✗ Perlu heat management</text>
          <text x="550" y="152" fill="#f85149" font-size="11">✗ Efisiensi rendah</text>
          <!-- Heat symbol -->
          <text x="290" y="185" fill="#f85149" font-size="18" text-anchor="middle">🌡</text>
          <text x="290" y="200" fill="#f85149" font-size="10" text-anchor="middle">Energi terbuang</text>
        </svg>
      </div>
      <div class="eq-wrap">
        <span class="eq">I_bal = (V_max − V_min) / R_bal</span>
      </div>
      <p><strong>Contoh:</strong> ΔV = 50mV, R_bal = 10Ω → I_bal = 5mA. Waktu balancing ≈ ΔCapacity / I_bal.</p>
    </div>

    <div id="bal-active" class="tab-content">
      <p>Energi dipindahkan dari sel yang lebih penuh ke sel yang kurang penuh menggunakan induktor atau kapasitor. Tidak ada energi yang dibuang sebagai panas.</p>
      <div class="callout callout-info">
        <strong>Active balancing</strong> menggunakan topologi seperti switched-capacitor, inductor-based (Cuk converter), atau transformer-based. Efisiensi hingga 90–95%, cocok untuk pack besar (EV, ESS) di mana energi yang dihemat signifikan. Namun kompleksitas dan biaya jauh lebih tinggi.
      </div>
      <div class="tbl-wrap">
        <table>
          <tr><th>Topologi</th><th>Efisiensi</th><th>Kompleksitas</th><th>Kelebihan</th></tr>
          <tr><td><strong>Switched Capacitor</strong></td><td>80–90%</td><td>Menengah</td><td>Tidak perlu induktor besar</td></tr>
          <tr><td><strong>Inductor-based (Cuk)</strong></td><td>90–95%</td><td>Tinggi</td><td>Efisiensi sangat tinggi</td></tr>
          <tr><td><strong>Flyback Transformer</strong></td><td>85–92%</td><td>Tinggi</td><td>Isolasi galvanik, skalabel</td></tr>
        </table>
      </div>
    </div>
  </section>

  <!-- ═══════════════════════════════════════════════════════ -->
  <!-- 10. SOC ESTIMATION -->
  <!-- ═══════════════════════════════════════════════════════ -->
  <section id="soc">
    <h2>10. SOC Estimation (State of Charge)</h2>
    <p>SOC adalah persentase kapasitas yang tersisa dalam baterai. Ini bukan parameter yang bisa diukur langsung — harus diestimasi menggunakan algoritma.</p>

    <div class="tbl-wrap">
      <table>
        <tr><th>Metode</th><th>Prinsip</th><th>Akurasi</th><th>Kelemahan</th></tr>
        <tr><td><strong>OCV Lookup</strong></td><td>V_OC → SOC via kurva karakteristik</td><td>±2–5%</td><td>Hanya saat rest, LFP kurva datar</td></tr>
        <tr><td><strong>Coulomb Counting</strong></td><td>SOC = SOC₀ − ∫I·dt / C_nominal</td><td>±1–3%</td><td>Error akumulasi, butuh kalibrasi</td></tr>
        <tr><td><strong>EKF (Extended Kalman)</strong></td><td>State observer + model baterai</td><td>±1–2%</td><td>Kompleks, perlu model parameter</td></tr>
        <tr><td><strong>Machine Learning</strong></td><td>Data-driven V/I/T → SOC</td><td>±0.5–1%</td><td>Butuh training data, komputasi</td></tr>
      </table>
    </div>

    <div class="callout callout-info">
      <strong>Praktis untuk embedded BMS:</strong> Gunakan <em>Coulomb Counting + OCV reset</em>. Coulomb counting digunakan saat baterai aktif. Saat baterai istirahat (rest > 2 jam), lakukan OCV lookup untuk mereset/mengkoreksi akumulasi error.
    </div>

    <div class="eq-wrap">
      <span class="eq">SOC(t) = SOC(0) − (1/C_nom) × ∫₀ᵗ I(τ) × η(I,T) dτ</span>
    </div>
    <p>Di mana η(I,T) adalah coulombic efficiency, fungsi dari arus dan temperatur (biasanya 0.98–0.999 untuk discharge, ~1.00 untuk charge pada suhu normal).</p>
  </section>

  <!-- ═══════════════════════════════════════════════════════ -->
  <!-- 11. PEMILIHAN IC BMS -->
  <!-- ═══════════════════════════════════════════════════════ -->
  <section id="ic">
    <h2>11. Panduan Pemilihan IC BMS</h2>
    <p>Pemilihan IC BMS ditentukan oleh jumlah sel, fitur yang dibutuhkan, dan segmen aplikasi. Berikut perbandingan IC populer di pasaran:</p>

    <div class="tbl-wrap">
      <table>
        <tr><th>IC</th><th>Vendor</th><th>Sel</th><th>Balancing</th><th>Komunikasi</th><th>Harga</th><th>Cocok untuk</th></tr>
        <tr><td><strong>bq77915</strong></td><td>TI</td><td>3–5S</td><td>Passive (ext)</td><td>-</td><td>$1–2</td><td>Consumer, proteksi dasar</td></tr>
        <tr><td><strong>bq76920</strong></td><td>TI</td><td>3–5S</td><td>Passive built-in</td><td>I2C</td><td>$3–5</td><td>DIY, prototyping</td></tr>
        <tr><td><strong>bq76930</strong></td><td>TI</td><td>6–10S</td><td>Passive built-in</td><td>I2C</td><td>$4–6</td><td>E-bike, power tool</td></tr>
        <tr><td><strong>bq76940</strong></td><td>TI</td><td>9–15S</td><td>Passive built-in</td><td>I2C/HDQ</td><td>$5–8</td><td>UPS, energy storage</td></tr>
        <tr><td><strong>ISL94202</strong></td><td>Renesas</td><td>3–8S</td><td>Passive built-in</td><td>I2C/SPI</td><td>$4–6</td><td>Mid-range consumer</td></tr>
        <tr><td><strong>BQ76PL455A</strong></td><td>TI</td><td>hingga 16S</td><td>Active capable</td><td>UART daisy</td><td>$8–15</td><td>Automotive, EV</td></tr>
        <tr><td><strong>ADBMS6830</strong></td><td>ADI</td><td>6–18S</td><td>Passive + ext</td><td>SPI isoSPI</td><td>$10–20</td><td>Industrial, EV</td></tr>
      </table>
    </div>

    <h3>Decision Tree Pemilihan IC</h3>
    <div class="diagram-wrap">
      <svg width="100%" viewBox="0 0 700 340" role="img">
        <title>Decision tree pemilihan IC BMS</title>
        <defs>
          <marker id="arr7" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse">
            <path d="M2 1L8 5L2 9" fill="none" stroke="context-stroke" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
          </marker>
        </defs>
        <!-- Root -->
        <rect x="250" y="10" width="200" height="44" rx="8" fill="rgba(163,113,247,.2)" stroke="#a371f7" stroke-width="1.5"/>
        <text x="350" y="36" fill="#a371f7" font-size="13" font-weight="600" text-anchor="middle">Berapa jumlah sel?</text>
        <!-- Lines from root -->
        <line x1="300" y1="54" x2="130" y2="110" stroke="#484f58" stroke-width="1.5" marker-end="url(#arr7)"/>
        <line x1="400" y1="54" x2="570" y2="110" stroke="#484f58" stroke-width="1.5" marker-end="url(#arr7)"/>
        <text x="200" y="95" fill="#8b949e" font-size="11">3–5S</text>
        <text x="480" y="95" fill="#8b949e" font-size="11">6S+</text>
        <!-- Left branch: 3-5S -->
        <rect x="60" y="110" width="160" height="44" rx="8" fill="rgba(56,139,253,.15)" stroke="#388bfd" stroke-width="1.5"/>
        <text x="140" y="132" fill="#388bfd" font-size="12" text-anchor="middle" font-weight="500">Butuh I2C/komunikasi?</text>
        <!-- Left-left: No comms -->
        <line x1="100" y1="154" x2="70" y2="210" stroke="#484f58" stroke-width="1.5" marker-end="url(#arr7)"/>
        <text x="60" y="195" fill="#8b949e" font-size="11">Tidak</text>
        <rect x="20" y="210" width="110" height="44" rx="8" fill="rgba(63,185,80,.2)" stroke="#3fb950" stroke-width="1.5"/>
        <text x="75" y="232" fill="#3fb950" font-size="12" text-anchor="middle" font-weight="600">bq77915</text>
        <text x="75" y="246" fill="#8b949e" font-size="10" text-anchor="middle">Proteksi dasar</text>
        <!-- Left-right: With comms -->
        <line x1="180" y1="154" x2="210" y2="210" stroke="#484f58" stroke-width="1.5" marker-end="url(#arr7)"/>
        <text x="195" y="195" fill="#8b949e" font-size="11">Ya</text>
        <rect x="150" y="210" width="110" height="44" rx="8" fill="rgba(63,185,80,.2)" stroke="#3fb950" stroke-width="1.5"/>
        <text x="205" y="232" fill="#3fb950" font-size="12" text-anchor="middle" font-weight="600">bq76920</text>
        <text x="205" y="246" fill="#8b949e" font-size="10" text-anchor="middle">I2C + balancing</text>
        <!-- Right branch: 6S+ -->
        <rect x="480" y="110" width="180" height="44" rx="8" fill="rgba(56,139,253,.15)" stroke="#388bfd" stroke-width="1.5"/>
        <text x="570" y="132" fill="#388bfd" font-size="12" text-anchor="middle" font-weight="500">Automotive grade?</text>
        <!-- Right-left: No automotive -->
        <line x1="530" y1="154" x2="490" y2="210" stroke="#484f58" stroke-width="1.5" marker-end="url(#arr7)"/>
        <text x="490" y="195" fill="#8b949e" font-size="11">Tidak</text>
        <rect x="430" y="210" width="120" height="44" rx="8" fill="rgba(63,185,80,.2)" stroke="#3fb950" stroke-width="1.5"/>
        <text x="490" y="232" fill="#3fb950" font-size="12" text-anchor="middle" font-weight="600">bq76940</text>
        <text x="490" y="246" fill="#8b949e" font-size="10" text-anchor="middle">9–15S, I2C</text>
        <!-- Right-right: Automotive -->
        <line x1="620" y1="154" x2="640" y2="210" stroke="#484f58" stroke-width="1.5" marker-end="url(#arr7)"/>
        <text x="640" y="195" fill="#8b949e" font-size="11">Ya</text>
        <rect x="560" y="210" width="120" height="44" rx="8" fill="rgba(210,153,34,.2)" stroke="#d29922" stroke-width="1.5"/>
        <text x="620" y="232" fill="#d29922" font-size="12" text-anchor="middle" font-weight="600">BQ76PL455A</text>
        <text x="620" y="246" fill="#8b949e" font-size="10" text-anchor="middle">Automotive, EV</text>
        <!-- Bottom note -->
        <rect x="200" y="300" width="300" height="32" rx="6" fill="rgba(248,81,73,.08)" stroke="#f85149" stroke-width="1"/>
        <text x="350" y="320" fill="#f85149" font-size="11" text-anchor="middle">Selalu verifikasi dengan datasheet terbaru!</text>
      </svg>
      <p class="diagram-caption">Gambar 7 — Decision tree sederhana pemilihan IC BMS</p>
    </div>
  </section>

  <!-- ═══════════════════════════════════════════════════════ -->
  <!-- 12. PEMILIHAN MOSFET -->
  <!-- ═══════════════════════════════════════════════════════ -->
  <section id="mosfet-select">
    <h2>12. Pemilihan MOSFET Power Path</h2>
    <p>MOSFET adalah komponen kritis yang menentukan rugi daya dan batas arus sistem. Parameter utama yang harus diperhatikan:</p>

    <h3>Kalkulator MOSFET</h3>
    <div class="interactive-box">
      <div class="ctrl-row">
        <span class="ctrl-label">Tegangan Pack Maks (V)</span>
        <input type="range" id="vpack" min="12" max="72" value="16.8" step="0.1" oninput="calcFet()">
        <span class="ctrl-val" id="vpack-val">16.8 V</span>
      </div>
      <div class="ctrl-row">
        <span class="ctrl-label">Arus Maks (A)</span>
        <input type="range" id="imax" min="5" max="200" value="30" oninput="calcFet()">
        <span class="ctrl-val" id="imax-val">30 A</span>
      </div>
      <div class="ctrl-row">
        <span class="ctrl-label">R_DS(on) per FET (mΩ)</span>
        <input type="range" id="rds" min="1" max="30" value="5" oninput="calcFet()">
        <span class="ctrl-val" id="rds-val">5 mΩ</span>
      </div>
      <div class="readout-grid">
        <div class="readout">
          <div class="readout-label">V_DS minimum</div>
          <div class="readout-val" id="vds-min" style="color:var(--blue)">21.8 V</div>
        </div>
        <div class="readout">
          <div class="readout-label">Rugi Daya (2 FET)</div>
          <div class="readout-val" id="plos" style="color:var(--amber)">9.0 W</div>
        </div>
        <div class="readout">
          <div class="readout-label">Perlu Heatsink?</div>
          <div class="readout-val" id="hs-need" style="color:var(--green)">Tidak</div>
        </div>
        <div class="readout">
          <div class="readout-label">I_D minimum</div>
          <div class="readout-val" id="id-min" style="color:var(--purple)">30 A</div>
        </div>
      </div>
      <div id="fet-status" class="status-bar status-ok">
        <div class="dot"></div>
        <span id="fet-msg">Parameter MOSFET dalam batas wajar</span>
      </div>
    </div>

    <div class="callout callout-info">
      <strong>Rule of thumb:</strong> Pilih MOSFET dengan V_DS ≥ 1.3× V_pack_max. Untuk pack 4S NMC (16.8V), pilih minimal 25V, idealnya 30V. Untuk R_DS(on): semakin kecil semakin baik. Pertimbangkan paralel 2 MOSFET jika arus > 50A.
    </div>
  </section>

  <!-- ═══════════════════════════════════════════════════════ -->
  <!-- 13. PCB LAYOUT TIPS -->
  <!-- ═══════════════════════════════════════════════════════ -->
  <section id="pcb">
    <h2>13. PCB Layout Tips</h2>
    <p>Layout PCB yang buruk adalah penyebab utama pengukuran tidak akurat dan interferensi noise pada BMS. Ikuti prinsip berikut:</p>

    <div class="tabs">
      <div class="tab active" onclick="pcbTab('ground')">Ground Separation</div>
      <div class="tab" onclick="pcbTab('routing')">Signal Routing</div>
      <div class="tab" onclick="pcbTab('thermal')">Thermal Management</div>
    </div>

    <div id="pcb-ground" class="tab-content active">
      <div class="callout callout-warn">
        <strong>Aturan Terpenting:</strong> Pisahkan ground analog (AGND) dan ground power (PGND). Kedua ground harus bertemu di SATU titik (star ground) yang dekat dengan IC BMS.
      </div>
      <div class="tbl-wrap">
        <table>
          <tr><th>Domain</th><th>Komponen</th><th>Ground</th><th>Alasan</th></tr>
          <tr><td>Analog</td><td>IC BMS, NTC divider, VC filter cap</td><td>AGND</td><td>Sensitif terhadap noise switching</td></tr>
          <tr><td>Power</td><td>MOSFET, Shunt, kapasitor bulk</td><td>PGND</td><td>Arus besar → voltage bounce</td></tr>
          <tr><td>Digital</td><td>MCU, optocoupler output</td><td>DGND</td><td>Switching noise dari MCU</td></tr>
        </table>
      </div>
    </div>
    <div id="pcb-routing" class="tab-content">
      <div class="tbl-wrap">
        <table>
          <tr><th>Signal</th><th>Panduan Routing</th></tr>
          <tr><td><code>VC0–VC5</code> (cell voltage)</td><td>Trace pendek &lt;10mm, filter RC 100Ω+100nF dekat pin IC, jauhi trace power</td></tr>
          <tr><td><code>SRP/SRN</code> (current sense)</td><td>Routing diferensial, panjang sama, jauhi switching node MOSFET</td></tr>
          <tr><td><code>TS</code> (temp sense)</td><td>Trace ke NTC bisa lebih panjang, tapi beri filter 1kΩ+100nF</td></tr>
          <tr><td><code>PACK+/PACK−</code> (power)</td><td>Trace lebar ≥1mm per ampere, atau gunakan copper pour</td></tr>
          <tr><td><code>Gate DSG/CHG</code></td><td>R_gate seri 10–22Ω untuk damping osilasi, trace pendek</td></tr>
        </table>
      </div>
    </div>
    <div id="pcb-thermal" class="tab-content">
      <p>MOSFET menghasilkan panas proporsional dengan I²·R_DS(on). Manajemen termal yang baik menentukan umur komponen.</p>
      <div class="eq-wrap"><span class="eq">T_junction = T_ambient + P_loss × (R_θJA)</span></div>
      <div class="tbl-wrap">
        <table>
          <tr><th>Metode</th><th>ΔT Typis</th><th>Cocok untuk</th></tr>
          <tr><td>Copper pour (2oz)</td><td>−15–20°C</td><td>P_loss &lt;5W</td></tr>
          <tr><td>Thermal via array</td><td>−20–30°C</td><td>P_loss 5–10W</td></tr>
          <tr><td>Heatsink external</td><td>−30–50°C</td><td>P_loss &gt;10W</td></tr>
          <tr><td>MOSFET paralel ×2</td><td>−50% P_loss</td><td>Arus &gt;50A</td></tr>
        </table>
      </div>
    </div>
  </section>

  <!-- ═══════════════════════════════════════════════════════ -->
  <!-- 14. TROUBLESHOOTING -->
  <!-- ═══════════════════════════════════════════════════════ -->
  <section id="troubleshoot">
    <h2>14. Troubleshooting Guide</h2>
    <p>Panduan diagnosis sistematis untuk masalah BMS yang paling umum ditemui.</p>

    <div class="tbl-wrap">
      <table>
        <tr>
          <th>Gejala</th>
          <th>Kemungkinan Penyebab</th>
          <th>Langkah Diagnosis</th>
          <th>Solusi</th>
        </tr>
        <tr>
          <td><strong>BMS trip terus saat discharge</strong></td>
          <td>OC threshold terlalu rendah; R_DS(on) FET terlalu besar</td>
          <td>Ukur I aktual dengan clamp meter; cek V_shunt</td>
          <td>Naikkan OC threshold; ganti FET R_DS(on) lebih kecil; atau paralel FET</td>
        </tr>
        <tr>
          <td><strong>Pack tidak mau dicharge</strong></td>
          <td>UV latch belum reset; OV dari satu sel; CHG FET rusak</td>
          <td>Cek tegangan per sel; cek fault register IC</td>
          <td>Pulse charge eksternal untuk recovery UV; ganti sel OV; ganti FET</td>
        </tr>
        <tr>
          <td><strong>Sel tidak balance setelah charge penuh</strong></td>
          <td>R_bal terlalu besar; waktu balancing kurang; balancing disabled</td>
          <td>Ukur arus balancing; cek register CELL_BAL</td>
          <td>Kurangi R_bal; aktifkan balancing lebih awal (V_diff &gt;10mV); extend charge time</td>
        </tr>
        <tr>
          <td><strong>BMS panas berlebih</strong></td>
          <td>R_DS(on) FET terlalu besar; arus melebihi spec; thermal management buruk</td>
          <td>Ukur T_junction FET dengan termometer IR; hitung P_loss</td>
          <td>Ganti FET lebih baik; tambah heatsink; paralel FET; kurangi arus maks</td>
        </tr>
        <tr>
          <td><strong>Tegangan sel terbaca tidak akurat</strong></td>
          <td>PCB layout buruk; routing VC lines panjang; filter cap hilang</td>
          <td>Bandingkan dengan multimeter presisi; cek layout PCB</td>
          <td>Tambah filter RC 100Ω+100nF; persingkat trace VC; pisahkan AGND-PGND</td>
        </tr>
        <tr>
          <td><strong>SOC drift seiring waktu</strong></td>
          <td>Coulomb counting error akumulasi; efisiensi belum dikalibrasi</td>
          <td>Plot SOC vs OCV saat istirahat; cek integrasi arus</td>
          <td>Implement OCV reset saat rest &gt;2 jam; kalibrasi η(I,T)</td>
        </tr>
        <tr>
          <td><strong>BMS tidak terdeteksi via I2C</strong></td>
          <td>Pull-up resistor hilang; alamat I2C salah; BOOT sequence gagal</td>
          <td>Oscilloscope SDA/SCL; scan I2C address</td>
          <td>Pasang 4.7kΩ pull-up ke VDD; verifikasi alamat dari datasheet; cek urutan power-up</td>
        </tr>
      </table>
    </div>
  </section>

  <!-- ═══════════════════════════════════════════════════════ -->
  <!-- 15. KUMPULAN FORMULA -->
  <!-- ═══════════════════════════════════════════════════════ -->
  <section id="formula">
    <h2>15. Kumpulan Formula Penting</h2>

    <h3>Sensing &amp; Pengukuran</h3>
    <div class="grid2">
      <div>
        <h4>Current Sensing (Shunt)</h4>
        <div class="eq-wrap"><span class="eq">I = V_SRP − V_SRN / R_SNS</span></div>
        <div class="eq-wrap"><span class="eq">P_shunt = I² × R_SNS</span></div>
      </div>
      <div>
        <h4>NTC Voltage Divider</h4>
        <div class="eq-wrap"><span class="eq">V_TS = VDD × R_NTC / (R_pu + R_NTC)</span></div>
        <div class="eq-wrap"><span class="eq">R_pu = R_NTC(T_mid) untuk resolusi optimal</span></div>
      </div>
    </div>

    <h3>Proteksi &amp; MOSFET</h3>
    <div class="grid2">
      <div>
        <h4>Rugi Daya MOSFET</h4>
        <div class="eq-wrap"><span class="eq">P_loss = I² × R_DS(on) × 2</span></div>
        <div class="eq-wrap"><span class="eq">T_j = T_amb + P_loss × R_θJA</span></div>
      </div>
      <div>
        <h4>V_DS Minimum</h4>
        <div class="eq-wrap"><span class="eq">V_DS_min = V_pack_max × 1.3</span></div>
        <div class="eq-wrap"><span class="eq">I_D_min = I_max × 1.2</span></div>
      </div>
    </div>

    <h3>Balancing</h3>
    <div class="grid2">
      <div>
        <h4>Passive Balancing Current</h4>
        <div class="eq-wrap"><span class="eq">I_bal = (V_max − V_min) / R_bal</span></div>
        <div class="eq-wrap"><span class="eq">P_bal = I_bal² × R_bal</span></div>
      </div>
      <div>
        <h4>Waktu Balancing</h4>
        <div class="eq-wrap"><span class="eq">t_bal = ΔC / I_bal (jam)</span></div>
        <div class="eq-wrap"><span class="eq">ΔC = C_sel × ΔSOCmaks</span></div>
      </div>
    </div>

    <h3>SOC Estimation</h3>
    <div class="eq-wrap"><span class="eq">SOC(t) = SOC₀ − (1/C_nom) × ∫₀ᵗ η × I dτ</span></div>
    <div class="eq-wrap"><span class="eq">SOC_reset = f(V_OC) saat I ≈ 0, t_rest &gt; 2 jam</span></div>

    <h3>Thermal (Pack)</h3>
    <div class="grid2">
      <div>
        <h4>Energi Pack</h4>
        <div class="eq-wrap"><span class="eq">E = V_nom × C_Ah × n_seri (Wh)</span></div>
      </div>
      <div>
        <h4>C-rate</h4>
        <div class="eq-wrap"><span class="eq">I_C1 = C_Ah (arus di 1C)</span></div>
        <div class="eq-wrap"><span class="eq">I_Cx = x × C_Ah</span></div>
      </div>
    </div>

    <div class="callout callout-success" style="margin-top:32px">
      <strong>Repository ini aktif dikembangkan.</strong> Kontribusi, issue, dan diskusi teknis sangat disambut. Lihat CONTRIBUTING.md untuk panduan berkontribusi.
    </div>

  </section>

</main>
</div>

<script>
// ── Shunt Calculator ──────────────────────────────────────────
function calcShunt() {
  const r = parseFloat(document.getElementById('r-shunt').value);
  const i = parseFloat(document.getElementById('i-max').value);
  document.getElementById('r-val').textContent = r + ' mΩ';
  document.getElementById('i-val').textContent = i + ' A';
  const vShunt = (i * r).toFixed(1);
  const pLoss = (i * i * r / 1000).toFixed(2);
  const eff = (100 - (i * r / 1000 / (i * 3.7) * 100)).toFixed(1);
  const adc = r < 3 ? '16-bit' : r < 8 ? '12-bit' : '10-bit';
  document.getElementById('v-shunt').textContent = vShunt + ' mV';
  document.getElementById('p-loss').textContent = pLoss + ' W';
  document.getElementById('eff').textContent = eff + '%';
  document.getElementById('adc-rec').textContent = adc;
  const status = document.getElementById('shunt-status');
  const msg = document.getElementById('shunt-msg');
  if (parseFloat(pLoss) > 5) {
    status.className = 'status-bar status-err';
    msg.textContent = 'Rugi daya terlalu besar! Kurangi R_SNS atau gunakan paralel.';
  } else if (parseFloat(vShunt) < 20) {
    status.className = 'status-bar status-warn';
    msg.textContent = 'Sinyal V_shunt terlalu kecil. Butuh ADC presisi tinggi atau op-amp.';
  } else {
    status.className = 'status-bar status-ok';
    msg.textContent = 'Parameter optimal untuk aplikasi umum.';
  }
}

// ── Simulation ─────────────────────────────────────────────────
let simChem = { ovT: 4.20, ovR: 4.15, uvT: 2.80, uvR: 3.00, ocD: 50, ocC: 30, otC: 45, otD: 60 };
const chemPresets = {
  nmc: { ovT: 4.20, ovR: 4.15, uvT: 2.80, uvR: 3.00, ocD: 50, ocC: 30, otC: 45, otD: 60 },
  lfp: { ovT: 3.65, ovR: 3.55, uvT: 2.50, uvR: 2.80, ocD: 50, ocC: 30, otC: 45, otD: 60 }
};
function simTab(t) {
  simChem = chemPresets[t];
  document.querySelectorAll('#proteksi-sim .tab').forEach((tab, i) => {
    tab.classList.toggle('active', (i === 0 && t === 'nmc') || (i === 1 && t === 'lfp'));
  });
  simUpdate();
}
function simUpdate() {
  const v = parseFloat(document.getElementById('sim-v').value);
  const i = parseFloat(document.getElementById('sim-i').value);
  const t = parseFloat(document.getElementById('sim-t').value);
  document.getElementById('sim-v-val').textContent = v.toFixed(2) + ' V';
  document.getElementById('sim-i-val').textContent = (i >= 0 ? '+' : '') + i + ' A';
  document.getElementById('sim-t-val').textContent = t + ' °C';

  let faults = [];
  let dsgOn = true, chgOn = true;
  if (v >= simChem.ovT) { faults.push('OV'); chgOn = false; }
  if (v <= simChem.uvT) { faults.push('UV'); dsgOn = false; }
  if (i > simChem.ocD) { faults.push('OCD'); dsgOn = false; }
  if (i < -simChem.ocC) { faults.push('OCC'); chgOn = false; }
  if (t >= simChem.otD) { faults.push('OTD'); dsgOn = false; }
  if (t >= simChem.otC && i < 0) { faults.push('OTC'); chgOn = false; }

  const dsgEl = document.getElementById('dsg-state');
  const chgEl = document.getElementById('chg-state');
  dsgEl.textContent = dsgOn ? 'ON' : 'OFF';
  dsgEl.style.color = dsgOn ? 'var(--green)' : 'var(--red)';
  chgEl.textContent = chgOn ? 'ON' : 'OFF';
  chgEl.style.color = chgOn ? 'var(--green)' : 'var(--red)';

  const power = dsgOn && i > 0 ? (v * 4 * i).toFixed(1) : '0.0';
  document.getElementById('sim-power').textContent = power + ' W';
  document.getElementById('fault-code').textContent = faults.length ? faults.join(', ') : 'NONE';
  document.getElementById('fault-code').style.color = faults.length ? 'var(--red)' : 'var(--green)';

  const simStatus = document.getElementById('sim-status');
  const simMsg = document.getElementById('sim-msg');
  if (faults.length) {
    simStatus.className = 'status-bar status-err';
    simMsg.textContent = 'FAULT: ' + faults.join(', ') + ' — Proteksi aktif!';
  } else {
    simStatus.className = 'status-bar status-ok';
    simMsg.textContent = 'Semua parameter dalam batas aman. MOSFET aktif.';
  }

  // Progress bars
  const ovPct = Math.min(100, (v / simChem.ovT) * 100).toFixed(0);
  const ocPct = Math.min(100, (Math.abs(i) / simChem.ocD) * 100).toFixed(0);
  const otPct = Math.min(100, (t / simChem.otD) * 100).toFixed(0);
  document.getElementById('ov-pct').textContent = ovPct + '%';
  document.getElementById('oc-pct').textContent = ocPct + '%';
  document.getElementById('ot-pct').textContent = otPct + '%';
  const ovBar = document.getElementById('ov-bar');
  const ocBar = document.getElementById('oc-bar');
  const otBar = document.getElementById('ot-bar');
  ovBar.style.width = ovPct + '%';
  ovBar.style.background = ovPct > 95 ? 'var(--red)' : ovPct > 85 ? 'var(--amber)' : 'var(--blue)';
  ocBar.style.width = ocPct + '%';
  ocBar.style.background = ocPct > 80 ? 'var(--red)' : ocPct > 60 ? 'var(--amber)' : 'var(--green)';
  otBar.style.width = otPct + '%';
  otBar.style.background = otPct > 80 ? 'var(--red)' : otPct > 60 ? 'var(--amber)' : 'var(--green)';
}

// ── FET Calculator ─────────────────────────────────────────────
function calcFet() {
  const vp = parseFloat(document.getElementById('vpack').value);
  const im = parseFloat(document.getElementById('imax').value);
  const rd = parseFloat(document.getElementById('rds').value);
  document.getElementById('vpack-val').textContent = vp.toFixed(1) + ' V';
  document.getElementById('imax-val').textContent = im + ' A';
  document.getElementById('rds-val').textContent = rd + ' mΩ';
  const vdsMin = (vp * 1.3).toFixed(1);
  const plos = (im * im * rd / 1000 * 2).toFixed(1);
  const needHs = parseFloat(plos) > 5 ? 'Ya' : 'Tidak';
  const idMin = (im * 1.2).toFixed(0);
  document.getElementById('vds-min').textContent = vdsMin + ' V';
  document.getElementById('plos').textContent = plos + ' W';
  document.getElementById('hs-need').textContent = needHs;
  document.getElementById('hs-need').style.color = needHs === 'Ya' ? 'var(--amber)' : 'var(--green)';
  document.getElementById('id-min').textContent = idMin + ' A';
  const status = document.getElementById('fet-status');
  const msg = document.getElementById('fet-msg');
  if (parseFloat(plos) > 15) {
    status.className = 'status-bar status-err';
    msg.textContent = 'Rugi daya sangat besar! Pertimbangkan paralel MOSFET atau ganti ke FET R_DS lebih kecil.';
  } else if (parseFloat(plos) > 5) {
    status.className = 'status-bar status-warn';
    msg.textContent = 'Perlu heatsink. Pertimbangkan MOSFET dengan R_DS(on) lebih kecil.';
  } else {
    status.className = 'status-bar status-ok';
    msg.textContent = 'Parameter MOSFET dalam batas wajar.';
  }
}

// ── Tabs ──────────────────────────────────────────────────────
function balTab(t) {
  document.getElementById('bal-passive').classList.toggle('active', t === 'passive');
  document.getElementById('bal-active').classList.toggle('active', t === 'active');
  document.querySelectorAll('#balancing .tab').forEach((tab, i) => {
    tab.classList.toggle('active', (i === 0 && t === 'passive') || (i === 1 && t === 'active'));
  });
}
function pcbTab(t) {
  ['ground','routing','thermal'].forEach(n => {
    document.getElementById('pcb-'+n).classList.toggle('active', n === t);
  });
  document.querySelectorAll('#pcb .tab').forEach((tab, i) => {
    tab.classList.toggle('active', ['ground','routing','thermal'][i] === t);
  });
}

// ── Sidebar Active ─────────────────────────────────────────────
const sections = document.querySelectorAll('section');
const navLinks = document.querySelectorAll('nav a');
const observer = new IntersectionObserver(entries => {
  entries.forEach(e => {
    if (e.isIntersecting) {
      navLinks.forEach(l => l.classList.remove('active'));
      const id = e.target.id;
      const active = document.querySelector('nav a[href="#'+id+'"]');
      if (active) active.classList.add('active');
    }
  });
}, { threshold: 0.3 });
sections.forEach(s => observer.observe(s));

// Init
calcShunt(); simUpdate(); calcFet();
</script>
</body>
</html>
