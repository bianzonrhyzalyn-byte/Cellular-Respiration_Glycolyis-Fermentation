<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Pyruvate Crossroads</title>
<meta name="claude:viewport-fit-sides" content="cover">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Bricolage+Grotesque:opsz,wght@12..96,500;12..96,700;12..96,800&family=Source+Sans+3:wght@400;600;700&family=JetBrains+Mono:wght@400;600&display=swap">
<style>
/* Layout: a single learning path down the page — scenario, trace, simulate, check — with a sticky stage bar. Cytosol-teal ground, ATP gold, NADH violet as the only signal colors. */
:root{
  --bg:#F1F5F3; --surface:#FFFFFF; --sunk:#E6EDEA; --ink:#12201C; --muted:#56655F; --line:#D3DDD9;
  --accent:#0B7A64; --accent-ink:#FFFFFF; --atp:#B87300; --nadh:#6A45C2; --lac:#C2412A; --mito:#2C6CAD; --good:#1F8A4C; --bad:#C2412A;
  --display:"Bricolage Grotesque", "Segoe UI", system-ui, sans-serif;
  --body:"Source Sans 3", "Segoe UI", system-ui, sans-serif;
  --mono:"JetBrains Mono", ui-monospace, Menlo, Consolas, monospace;
}
@media (prefers-color-scheme: dark){:root:not([data-theme="light"]){
  --bg:#0D1513; --surface:#15201D; --sunk:#1B2824; --ink:#E3ECE8; --muted:#97A8A2; --line:#2A3A35;
  --accent:#3BC29F; --accent-ink:#06231C; --atp:#F0B43C; --nadh:#AA8CF2; --lac:#F27C63; --mito:#6EA7E2; --good:#4CC782; --bad:#F27C63; color-scheme:dark}}
:root[data-theme="dark"]{
  --bg:#0D1513; --surface:#15201D; --sunk:#1B2824; --ink:#E3ECE8; --muted:#97A8A2; --line:#2A3A35;
  --accent:#3BC29F; --accent-ink:#06231C; --atp:#F0B43C; --nadh:#AA8CF2; --lac:#F27C63; --mito:#6EA7E2; --good:#4CC782; --bad:#F27C63; color-scheme:dark}
*{box-sizing:border-box}
body{background:var(--bg);color:var(--ink);font-family:var(--body);font-size:16px;line-height:1.55}
body::before{content:"";position:fixed;inset:0 0 auto;height:env(safe-area-inset-top,0px);z-index:10;background:var(--surface)}
.wrap{max-width:1080px;margin:0 auto;padding-left:max(16px,env(safe-area-inset-left,0px));padding-right:max(16px,env(safe-area-inset-right,0px))}
h1,h2,h3{font-family:var(--display);text-wrap:balance;margin:0;line-height:1.1}
h2{font-size:clamp(1.5rem,3.2vw,2.1rem);font-weight:800;letter-spacing:-.01em}
h3{font-size:1.1rem;font-weight:700}
p{margin:0}
.mono{font-family:var(--mono);font-variant-numeric:tabular-nums}
.eyebrow{font-family:var(--mono);font-size:.74rem;letter-spacing:.12em;text-transform:uppercase;color:var(--accent);font-weight:600}
.muted{color:var(--muted)}
button{font:inherit;cursor:pointer}
:focus-visible{outline:3px solid var(--accent);outline-offset:2px}

/* header */
header.top{background:var(--surface);border-bottom:1px solid var(--line)}
header.top .wrap{padding-block:28px 22px;display:grid;gap:14px}
header h1{font-size:clamp(2rem,5.5vw,3.4rem);font-weight:800;letter-spacing:-.02em}
header h1 .eq{display:block;font-family:var(--mono);font-size:clamp(.72rem,1.6vw,.9rem);font-weight:400;letter-spacing:0;color:var(--muted);margin-top:10px;line-height:1.5}
header h1 .eq b{color:var(--atp);font-weight:600}
header h1 .eq i{font-style:normal;color:var(--nadh);font-weight:600}
.lede{max-width:64ch;color:var(--muted);font-size:1.05rem}

nav.stages{position:sticky;top:env(safe-area-inset-top,0px);z-index:5;background:var(--surface);border-bottom:1px solid var(--line)}
nav.stages .wrap{display:flex;gap:4px;overflow-x:auto;padding-block:8px}
nav.stages a{flex:0 0 auto;text-decoration:none;color:var(--muted);font-weight:600;font-size:.92rem;padding:6px 12px;border-radius:999px;white-space:nowrap}
nav.stages a span{font-family:var(--mono);font-size:.78rem;margin-right:6px;color:var(--accent)}
nav.stages a:hover{background:var(--sunk);color:var(--ink)}

section.stage{padding-block:48px 8px;scroll-margin-top:60px}
.stage-head{display:grid;gap:8px;margin-bottom:22px;max-width:70ch}

/* scenarios */
.scen-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(230px,1fr));gap:12px}
.scen{text-align:left;background:var(--surface);border:1px solid var(--line);border-radius:10px;padding:16px;color:var(--ink);display:grid;gap:6px;align-content:start;transition:border-color .15s, transform .15s}
.scen:hover{border-color:var(--accent);transform:translateY(-2px)}
.scen[aria-pressed="true"]{border-color:var(--accent);box-shadow:0 0 0 2px var(--accent) inset}
.scen .tag{font-family:var(--mono);font-size:.7rem;letter-spacing:.08em;text-transform:uppercase;color:var(--muted)}
.scen strong{font-family:var(--display);font-size:1.08rem}
.scen p{font-size:.92rem;color:var(--muted)}

/* tracer */
.tracer{display:grid;grid-template-columns:minmax(0,1.5fr) minmax(0,1fr);gap:16px}
@media (max-width:820px){.tracer{grid-template-columns:1fr}}
.panel{background:var(--surface);border:1px solid var(--line);border-radius:12px;padding:20px;min-width:0}
.steprail{display:flex;gap:4px;margin-bottom:16px;flex-wrap:wrap}
.steprail i{flex:1 1 18px;height:6px;border-radius:3px;background:var(--sunk)}
.steprail i.inv{background:color-mix(in srgb,var(--atp) 35%,var(--sunk))}
.steprail i.done{background:var(--accent)}
.phase{font-family:var(--mono);font-size:.75rem;letter-spacing:.08em;text-transform:uppercase;padding:3px 8px;border-radius:4px;background:var(--sunk);color:var(--muted);display:inline-block}
.mol-stage{background:var(--sunk);border-radius:10px;min-height:150px;display:flex;flex-wrap:wrap;align-items:center;justify-content:center;gap:26px;padding:22px 12px;margin:14px 0}
.mol{display:grid;justify-items:center;gap:10px}
.chain{display:flex;align-items:center}
.c{width:30px;height:30px;border-radius:50%;background:var(--ink);color:var(--bg);font-family:var(--mono);font-size:.72rem;display:grid;place-items:center;position:relative;flex:0 0 auto}
.bond{width:10px;height:3px;background:var(--ink);flex:0 0 auto}
.c .p{position:absolute;top:-22px;left:50%;transform:translateX(-50%);width:20px;height:20px;border-radius:50%;background:var(--atp);color:#1d1300;font-size:.62rem;font-weight:700;display:grid;place-items:center}
.mol .name{font-weight:700;font-size:.95rem;text-align:center}
.mol .x2{font-family:var(--mono);font-size:.75rem;color:var(--accent);font-weight:600}
.reaction{font-family:var(--mono);font-size:.85rem;background:var(--bg);border:1px dashed var(--line);border-radius:8px;padding:10px 12px;overflow-x:auto;white-space:nowrap}
.ask{margin-top:16px;display:grid;gap:10px}
.opts{display:flex;flex-wrap:wrap;gap:8px}
.opt{border:1px solid var(--line);background:var(--surface);color:var(--ink);padding:9px 14px;border-radius:8px;font-weight:600}
.opt:hover{border-color:var(--accent)}
.opt.right{background:var(--good);border-color:var(--good);color:#fff}
.opt.wrong{border-color:var(--bad);color:var(--bad)}
.fb{font-size:.95rem;min-height:1.5em}
.fb.ok{color:var(--good)} .fb.no{color:var(--bad)}
.note{font-size:.95rem;color:var(--muted);border-left:3px solid var(--line);padding-left:12px}
.row{display:flex;gap:8px;flex-wrap:wrap;align-items:center}
.btn{background:var(--accent);color:var(--accent-ink);border:0;padding:10px 16px;border-radius:8px;font-weight:700}
.btn:disabled{opacity:.4;cursor:not-allowed}
.btn.ghost{background:transparent;color:var(--ink);border:1px solid var(--line)}
.ledger{display:grid;gap:10px}
.lrow{display:grid;grid-template-columns:1fr auto;gap:8px;align-items:center;padding:10px 0;border-bottom:1px solid var(--line)}
.lrow:last-child{border-bottom:0}
.lrow .v{font-family:var(--mono);font-size:1.3rem;font-weight:600;font-variant-numeric:tabular-nums}
.tokens{display:flex;flex-wrap:wrap;gap:4px;grid-column:1/-1;min-height:14px}
.tok{width:14px;height:14px;border-radius:3px}
.tok.atp{background:var(--atp)} .tok.used{background:transparent;border:2px solid var(--atp)} .tok.nadh{background:var(--nadh)} .tok.pyr{background:var(--accent);border-radius:50%}
.net{background:var(--sunk);border-radius:8px;padding:12px;font-family:var(--mono);font-size:.85rem}

/* simulator */
.sim{display:grid;grid-template-columns:minmax(0,320px) minmax(0,1fr);gap:16px}
@media (max-width:860px){.sim{grid-template-columns:1fr}}
.ctrl{display:grid;gap:18px;align-content:start}
.field{display:grid;gap:6px}
.field label{font-weight:600;display:flex;justify-content:space-between;gap:8px}
.field label .mono{color:var(--accent)}
input[type=range]{width:100%;accent-color:var(--accent)}
.seg{display:flex;background:var(--sunk);border-radius:8px;padding:3px;gap:3px}
.seg button{flex:1;border:0;background:transparent;color:var(--muted);padding:7px 8px;border-radius:6px;font-weight:600;font-size:.92rem}
.seg button[aria-pressed="true"]{background:var(--surface);color:var(--ink);box-shadow:0 1px 2px rgba(0,0,0,.12)}
.toggle{display:flex;align-items:flex-start;gap:10px;font-size:.95rem}
.toggle input{width:18px;height:18px;margin-top:3px;accent-color:var(--accent);flex:0 0 auto}
.out{display:grid;gap:14px;min-width:0}
.status{border-radius:10px;padding:12px 14px;background:var(--sunk);font-size:.98rem;border-left:4px solid var(--accent)}
.status.warn{border-left-color:var(--atp)}
.status.crit{border-left-color:var(--bad)}
.meters{display:grid;grid-template-columns:repeat(4,minmax(0,1fr));gap:10px}
@media (max-width:620px){.meters{grid-template-columns:repeat(2,minmax(0,1fr))}}
.meter{background:var(--surface);border:1px solid var(--line);border-radius:10px;padding:12px;display:grid;gap:4px;min-width:0}
.meter .k{font-family:var(--mono);font-size:.68rem;letter-spacing:.08em;text-transform:uppercase;color:var(--muted)}
.meter .v{font-family:var(--mono);font-size:1.35rem;font-weight:600;font-variant-numeric:tabular-nums}
.meter .bar{height:6px;border-radius:3px;background:var(--sunk);overflow:hidden}
.meter .bar i{display:block;height:100%;width:0;transition:width .15s linear}
.pathway{background:var(--surface);border:1px solid var(--line);border-radius:12px;padding:8px;overflow-x:auto}
.pathway svg{display:block;width:100%;min-width:520px;height:auto}
.pathway text{font-family:var(--body);fill:var(--ink)}
.pathway .sm{font-family:var(--mono);font-size:11px;fill:var(--muted)}
.chartbox{background:var(--surface);border:1px solid var(--line);border-radius:12px;padding:12px}
.chartbox canvas{width:100%;height:190px;display:block}
.legend{display:flex;gap:16px;flex-wrap:wrap;font-size:.85rem;color:var(--muted);margin-top:6px}
.legend span::before{content:"";display:inline-block;width:14px;height:3px;border-radius:2px;margin-right:6px;vertical-align:middle;background:var(--c)}

/* compare */
.compare{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:16px}
@media (max-width:760px){.compare{grid-template-columns:1fr}}
.path{display:grid;gap:8px;margin-top:10px}
.pstep{display:grid;grid-template-columns:1fr;gap:4px;background:var(--sunk);border-radius:8px;padding:10px 12px}
.pstep .enz{font-family:var(--mono);font-size:.78rem;color:var(--accent)}
.pstep .rx{font-family:var(--mono);font-size:.86rem}
.where{font-size:.92rem;color:var(--muted);margin-top:10px}

/* quiz */
.quiz{display:grid;gap:14px}
.q{background:var(--surface);border:1px solid var(--line);border-radius:12px;padding:18px;display:grid;gap:12px}
.q .qn{font-family:var(--mono);font-size:.75rem;color:var(--muted)}
.q .prompt{font-weight:600;font-size:1.03rem}
.q .choices{display:grid;gap:8px}
.choice{text-align:left;border:1px solid var(--line);background:var(--bg);color:var(--ink);padding:10px 12px;border-radius:8px}
.choice:hover:not(:disabled){border-color:var(--accent)}
.choice:disabled{cursor:default}
.choice.right{border-color:var(--good);background:color-mix(in srgb,var(--good) 14%,var(--bg))}
.choice.wrong{border-color:var(--bad);background:color-mix(in srgb,var(--bad) 12%,var(--bg))}
.explain{font-size:.95rem;padding:10px 12px;border-radius:8px;background:var(--sunk)}
.score{position:sticky;bottom:12px;margin-top:16px;background:var(--ink);color:var(--bg);border-radius:12px;padding:14px 18px;display:flex;justify-content:space-between;gap:12px;flex-wrap:wrap;align-items:center}
.score .btn{background:var(--bg);color:var(--ink)}
footer{padding-block:40px 60px;color:var(--muted);font-size:.9rem}
footer .obj{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:16px;margin-top:12px}
@media (prefers-reduced-motion:reduce){*{transition:none!important;animation:none!important}}
</style>
</head>
<body style="margin:0">

<header class="top">
  <div class="wrap">
    <span class="eyebrow">BIO 2 · Topic 4 · Cellular Respiration</span>
    <h1>Pyruvate Crossroads
      <span class="eq">C₆H₁₂O₆ + 2 NAD⁺ + 2 ADP + 2 Pᵢ → 2 pyruvate + <i>2 NADH</i> + 2 H⁺ + <b>2 ATP</b> + 2 H₂O</span>
    </h1>
    <p class="lede">Every cell splits glucose the same way. What happens to the pyruvate afterwards depends on one question: is there a way to turn NADH back into NAD⁺? Trace glycolysis step by step, then control oxygen and enzymes to see when a cell must ferment.</p>
  </div>
</header>

<nav class="stages" aria-label="Learning stages">
  <div class="wrap">
    <a href="#scenario"><span>1</span>Pick a scenario</a>
    <a href="#trace"><span>2</span>Trace glycolysis</a>
    <a href="#simulate"><span>3</span>NAD⁺ simulator</a>
    <a href="#ferment"><span>4</span>Two fermentations</a>
    <a href="#check"><span>5</span>Check yourself</a>
  </div>
</nav>

<main class="wrap">

<section class="stage" id="scenario">
  <div class="stage-head">
    <span class="eyebrow">Stage 1 · Real-world anchor</span>
    <h2>Where does this happen in real life?</h2>
    <p class="muted">Each case below loads its conditions into the simulator in Stage 3. Start with any one; you'll come back to compare.</p>
  </div>
  <div class="scen-grid" id="scenGrid"></div>
</section>

<section class="stage" id="trace">
  <div class="stage-head">
    <span class="eyebrow">Stage 2 · Glycolysis in the cytosol</span>
    <h2>Trace the six carbons through ten steps</h2>
    <p class="muted">Before each step runs, pick the enzyme that catalyzes it. Watch the ledger: the cell spends 2 ATP first, then earns 4 ATP and 2 NADH.</p>
  </div>
  <div class="tracer">
    <div class="panel">
      <div class="steprail" id="rail" aria-hidden="true"></div>
      <div class="row" style="justify-content:space-between">
        <h3 id="stepTitle">Starting molecule</h3>
        <span class="phase" id="phase">Ready</span>
      </div>
      <div class="mol-stage" id="molStage" aria-live="polite"></div>
      <div class="reaction" id="rxn">Glucose enters the cell through a GLUT transporter.</div>
      <div class="ask" id="ask"></div>
      <p class="note" id="stepNote" style="margin-top:14px">Glucose is a 6-carbon sugar. Glycolysis needs no oxygen and happens in every living cell.</p>
      <div class="row" style="margin-top:16px">
        <button class="btn ghost" id="resetTrace">Restart</button>
        <button class="btn ghost" id="revealBtn">Show answer</button>
      </div>
    </div>
    <div class="panel ledger" aria-live="polite">
      <h3>Energy ledger <span class="muted" style="font-weight:400;font-size:.9rem">(per glucose)</span></h3>
      <div class="lrow"><span>ATP spent</span><span class="v" id="lUsed" style="color:var(--atp)">0</span><div class="tokens" id="tUsed"></div></div>
      <div class="lrow"><span>ATP made <span class="muted">(substrate-level)</span></span><span class="v" id="lMade" style="color:var(--atp)">0</span><div class="tokens" id="tMade"></div></div>
      <div class="lrow"><span>NADH made</span><span class="v" id="lNadh" style="color:var(--nadh)">0</span><div class="tokens" id="tNadh"></div></div>
      <div class="lrow"><span>Pyruvate</span><span class="v" id="lPyr" style="color:var(--accent)">0</span><div class="tokens" id="tPyr"></div></div>
      <div class="net" id="netBox">Net ATP so far: <b class="mono" id="lNet">0</b></div>
    </div>
  </div>
</section>

<section class="stage" id="simulate">
  <div class="stage-head">
    <span class="eyebrow">Stage 3 · The NAD⁺ bottleneck</span>
    <h2>Control the cell. Keep NAD⁺ flowing.</h2>
    <p class="muted">A cell has only a small pool of NAD⁺. Step 6 of glycolysis uses it up. Oxygen (through the electron transport chain) or fermentation must regenerate it, or glycolysis stops. Values are relative units in a teaching model, not measured rates.</p>
  </div>
  <div class="sim">
    <div class="panel ctrl">
      <div class="field">
        <label>Cell type</label>
        <div class="seg" id="cellSeg">
          <button data-v="muscle" aria-pressed="true">Muscle cell</button>
          <button data-v="yeast" aria-pressed="false">Yeast</button>
        </div>
      </div>
      <div class="field">
        <label for="o2">Oxygen available <span class="mono" id="o2v">100%</span></label>
        <input type="range" id="o2" min="0" max="100" value="100">
      </div>
      <div class="field">
        <label for="dem">ATP demand <span class="mono" id="demv">24</span></label>
        <input type="range" id="dem" min="6" max="80" value="24">
      </div>
      <label class="toggle"><input type="checkbox" id="ferm" checked><span><b id="fermLbl">Lactate dehydrogenase (LDH) active</b><br><span class="muted">Turn off to see what happens if the cell cannot ferment.</span></span></label>
      <label class="toggle"><input type="checkbox" id="cyan"><span><b>Cyanide present</b><br><span class="muted">Blocks Complex IV (cytochrome c oxidase) of the ETC.</span></span></label>
      <div class="row">
        <button class="btn" id="playBtn">Pause</button>
        <button class="btn ghost" id="simReset">Reset cell</button>
      </div>
    </div>
    <div class="out">
      <div class="status" id="status" aria-live="polite">Loading…</div>
      <div class="meters">
        <div class="meter"><span class="k">NAD⁺ free</span><span class="v" id="mNad">100%</span><div class="bar"><i id="bNad" style="background:var(--nadh)"></i></div></div>
        <div class="meter"><span class="k">Demand met</span><span class="v" id="mAtp">100%</span><div class="bar"><i id="bAtp" style="background:var(--atp)"></i></div></div>
        <div class="meter"><span class="k">Glucose used / s</span><span class="v" id="mGlc">0.0</span><div class="bar"><i id="bGlc" style="background:var(--accent)"></i></div></div>
        <div class="meter"><span class="k" id="mProdK">Muscle pH</span><span class="v" id="mProd">7.10</span><div class="bar"><i id="bProd" style="background:var(--lac)"></i></div></div>
      </div>
      <div class="pathway">
        <svg viewBox="0 0 640 230" role="img" aria-label="Pathway diagram: glucose to pyruvate, then to mitochondrion or fermentation, with arrow thickness showing flow">
          <defs>
            <marker id="ah" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="5" markerHeight="5" orient="auto"><path d="M0,0 L10,5 L0,10 z" fill="var(--muted)"/></marker>
          </defs>
          <rect x="8" y="8" width="380" height="214" rx="12" fill="var(--sunk)"/>
          <text x="20" y="28" class="sm">CYTOSOL</text>
          <rect x="430" y="18" width="200" height="88" rx="40" fill="none" stroke="var(--mito)" stroke-width="2"/>
          <text x="530" y="46" text-anchor="middle" font-weight="700" style="fill:var(--mito)">Mitochondrion</text>
          <text x="530" y="64" text-anchor="middle" class="sm">PDH → Krebs → ETC</text>
          <text x="530" y="82" text-anchor="middle" class="sm" id="mitoTxt">O₂ is final e⁻ acceptor</text>
          <line id="xCyan" x1="452" y1="30" x2="608" y2="96" stroke="var(--bad)" stroke-width="4" opacity="0"/>
          <text x="40" y="122" font-weight="700">Glucose</text>
          <text x="40" y="140" class="sm">6C</text>
          <path id="aGly" d="M110,117 L228,117" stroke="var(--accent)" stroke-width="6" fill="none" stroke-linecap="round"/>
          <text x="169" y="106" text-anchor="middle" class="sm">10 steps</text>
          <text x="245" y="122" font-weight="700">2 Pyruvate</text>
          <text x="245" y="140" class="sm">3C each</text>
          <path id="aMito" d="M330,105 C380,70 395,62 428,62" stroke="var(--mito)" stroke-width="2" fill="none" stroke-linecap="round" marker-end="url(#ah)"/>
          <path id="aFerm" d="M330,135 C380,170 395,178 428,178" stroke="var(--lac)" stroke-width="2" fill="none" stroke-linecap="round" marker-end="url(#ah)"/>
          <rect x="430" y="140" width="200" height="76" rx="10" fill="none" stroke="var(--lac)" stroke-width="2" stroke-dasharray="5 4"/>
          <text x="530" y="168" text-anchor="middle" font-weight="700" style="fill:var(--lac)" id="fermTitle">Lactate</text>
          <text x="530" y="188" text-anchor="middle" class="sm" id="fermSub">via LDH · regenerates NAD⁺</text>
          <text x="530" y="205" text-anchor="middle" class="sm" id="fermBlock"></text>
          <path d="M300,185 C260,205 200,205 170,160" stroke="var(--nadh)" stroke-width="2" stroke-dasharray="4 4" fill="none" marker-end="url(#ah)" id="aNad"/>
          <text x="196" y="210" class="sm" style="fill:var(--nadh)">NAD⁺ returned to step 6</text>
          <text x="20" y="210" class="sm" id="pyrPool"></text>
        </svg>
      </div>
      <div class="chartbox">
        <canvas id="chart" height="190" aria-label="Line chart of NAD⁺ available and ATP demand met over the last 20 seconds"></canvas>
        <div class="legend"><span style="--c:var(--nadh)">NAD⁺ free (%)</span><span style="--c:var(--atp)">ATP demand met (%)</span><span style="--c:var(--accent)">Glucose use (% of max)</span></div>
      </div>
    </div>
  </div>
</section>

<section class="stage" id="ferment">
  <div class="stage-head">
    <span class="eyebrow">Stage 4 · Two ways to recycle NAD⁺</span>
    <h2>Same goal, different products</h2>
    <p class="muted">Neither fermentation makes extra ATP. Both exist only to oxidize NADH back to NAD⁺ so step 6 of glycolysis can keep running. Fermentation's ATP is the 2 ATP from glycolysis.</p>
  </div>
  <div class="compare">
    <div class="panel">
      <span class="eyebrow" style="color:var(--lac)">Lactic acid fermentation</span>
      <h3 style="margin-top:6px">Muscle cells, red blood cells, <i>Lactobacillus</i></h3>
      <div class="path">
        <div class="pstep"><span class="enz">Lactate dehydrogenase (LDH) · one step</span><span class="rx">pyruvate (3C) + NADH + H⁺ → lactate (3C) + NAD⁺</span></div>
      </div>
      <p class="where">No carbon is lost and no CO₂ forms. In a sprinting thigh muscle, lactate and H⁺ build up; the liver later converts lactate back to glucose (Cori cycle). Red blood cells have no mitochondria, so they rely on this path all the time. Bacteria use it to make <i>burong mangga</i>, yogurt and atchara.</p>
      <p class="mono" style="margin-top:10px;font-size:.85rem">Per glucose: 2 lactate · net 2 ATP</p>
    </div>
    <div class="panel">
      <span class="eyebrow" style="color:var(--atp)">Alcoholic fermentation</span>
      <h3 style="margin-top:6px">Yeast such as <i>Saccharomyces cerevisiae</i></h3>
      <div class="path">
        <div class="pstep"><span class="enz">1 · Pyruvate decarboxylase</span><span class="rx">pyruvate (3C) → acetaldehyde (2C) + CO₂</span></div>
        <div class="pstep"><span class="enz">2 · Alcohol dehydrogenase (ADH)</span><span class="rx">acetaldehyde + NADH + H⁺ → ethanol (2C) + NAD⁺</span></div>
      </div>
      <p class="where">One carbon leaves as CO₂. That gas makes pan de sal dough rise and puts the fizz in fresh tuba; the ethanol is what makes tuba and lambanog alcoholic. Humans lack pyruvate decarboxylase, so our muscles cannot make ethanol.</p>
      <p class="mono" style="margin-top:10px;font-size:.85rem">Per glucose: 2 ethanol + 2 CO₂ · net 2 ATP</p>
    </div>
  </div>
</section>

<section class="stage" id="check">
  <div class="stage-head">
    <span class="eyebrow">Stage 5 · Formative check</span>
    <h2>Check yourself</h2>
    <p class="muted">Each answer shows why it is right or wrong. Use the simulator to test any question you are unsure about.</p>
  </div>
  <div class="quiz" id="quiz"></div>
  <div class="score" id="scoreBar">
    <span><b class="mono" id="scoreNum">0 / 0</b> answered correctly</span>
    <button class="btn" id="quizReset">Try again</button>
  </div>
</section>

</main>

<footer>
  <div class="wrap">
    <span class="eyebrow">Learning objectives</span>
    <div class="obj">
      <p>Sequence the ten reactions of glycolysis and name the enzyme for each, identifying the investment and payoff phases.</p>
      <p>Account for the net yield of glycolysis per glucose: 2 ATP by substrate-level phosphorylation, 2 NADH and 2 pyruvate.</p>
      <p>Explain why fermentation is needed to regenerate NAD⁺, and predict what happens to glycolysis when oxygen is absent or Complex IV is blocked.</p>
      <p>Compare lactic acid and alcoholic fermentation by enzymes, carbon fate, products and real-world examples.</p>
    </div>
    <p style="margin-top:20px">Simulator values are relative units for teaching. The ~30–32 ATP per glucose for full aerobic respiration is the modern textbook estimate; older sources state 36–38.</p>
  </div>
</footer>

<script>
(function(){
"use strict";
const $=s=>document.querySelector(s);

/* ---------- Scenarios (CTL anchors) ---------- */
const SCEN=[
 {id:"rest",tag:"Baseline",title:"Resting at the plaza",text:"Plenty of oxygen reaches the muscle. Pyruvate goes into the mitochondria.",cell:"muscle",o2:100,dem:24,ferm:true,cyan:false},
 {id:"sprint",tag:"Sports science",title:"100-m dash at the intramurals",text:"Demand jumps and oxygen delivery can't keep up. Why do the legs burn?",cell:"muscle",o2:15,dem:60,ferm:true,cyan:false},
 {id:"cassava",tag:"Clinical · toxicology",title:"Raw cassava poisoning",text:"Poorly processed cassava releases cyanide. Blood has oxygen, yet cells suffocate.",cell:"muscle",o2:100,dem:40,ferm:true,cyan:true},
 {id:"pandesal",tag:"Food science",title:"Pan de sal dough rising",text:"Yeast in the dough runs low on oxygen. Where does the gas come from?",cell:"yeast",o2:10,dem:12,ferm:true,cyan:false},
 {id:"tuba",tag:"Local industry",title:"Tuba in a sealed container",text:"Coconut sap ferments with no oxygen. Compare sugar use with an aerated jar.",cell:"yeast",o2:0,dem:12,ferm:true,cyan:false},
 {id:"block",tag:"Thought experiment",title:"No oxygen, LDH blocked",text:"Remove both ways of recycling NAD⁺. Which glycolysis step stops first?",cell:"muscle",o2:0,dem:30,ferm:false,cyan:false}
];
const grid=$("#scenGrid");
SCEN.forEach(s=>{
  const b=document.createElement("button");
  b.className="scen";b.setAttribute("aria-pressed","false");b.dataset.id=s.id;
  b.innerHTML=`<span class="tag">${s.tag}</span><strong>${s.title}</strong><p>${s.text}</p>`;
  b.addEventListener("click",()=>{loadScenario(s);document.getElementById("simulate").scrollIntoView({behavior:matchMedia("(prefers-reduced-motion: reduce)").matches?"auto":"smooth"});});
  grid.appendChild(b);
});

/* ---------- Glycolysis tracer ---------- */
const ENZ=["Hexokinase","Phosphoglucose isomerase","Phosphofructokinase-1 (PFK-1)","Aldolase","Triose phosphate isomerase","Glyceraldehyde-3-P dehydrogenase","Phosphoglycerate kinase","Phosphoglycerate mutase","Enolase","Pyruvate kinase"];
const M=(name,n,p)=>({name,n,p});
const STEPS=[
 {phase:"Investment",mols:[M("Glucose-6-phosphate",6,[6])],x2:false,rx:"Glucose + ATP → Glucose-6-phosphate + ADP",d:{used:1},note:"Phosphorylation traps glucose inside the cell: the negatively charged G6P cannot cross the membrane. Irreversible."},
 {phase:"Investment",mols:[M("Fructose-6-phosphate",6,[6])],x2:false,rx:"Glucose-6-phosphate ⇌ Fructose-6-phosphate",d:{},note:"An isomerization: same atoms, rearranged from an aldose (6-membered ring) to a ketose (5-membered ring)."},
 {phase:"Investment",mols:[M("Fructose-1,6-bisphosphate",6,[1,6])],x2:false,rx:"Fructose-6-phosphate + ATP → Fructose-1,6-bisphosphate + ADP",d:{used:1},note:"The committed step and main control point. High ATP and citrate inhibit PFK-1; AMP activates it."},
 {phase:"Investment",mols:[M("DHAP",3,[1]),M("Glyceraldehyde-3-P",3,[3])],x2:false,rx:"Fructose-1,6-bisphosphate ⇌ DHAP + Glyceraldehyde-3-phosphate",d:{},note:"The 6-carbon sugar is cleaved into two 3-carbon sugars, each carrying one phosphate."},
 {phase:"Investment",mols:[M("Glyceraldehyde-3-P",3,[3])],x2:true,rx:"DHAP ⇌ Glyceraldehyde-3-phosphate",d:{},note:"DHAP is converted to a second G3P. From here every reaction happens twice per glucose."},
 {phase:"Payoff",mols:[M("1,3-Bisphosphoglycerate",3,[1,3])],x2:true,rx:"G3P + NAD⁺ + Pᵢ → 1,3-Bisphosphoglycerate + NADH + H⁺   (×2)",d:{nadh:2},note:"The only oxidation in glycolysis. It needs NAD⁺. If the cell cannot regenerate NAD⁺, glycolysis stops right here."},
 {phase:"Payoff",mols:[M("3-Phosphoglycerate",3,[3])],x2:true,rx:"1,3-BPG + ADP → 3-Phosphoglycerate + ATP   (×2)",d:{made:2},note:"Substrate-level phosphorylation: a phosphate moves directly from a substrate to ADP. The 2 ATP invested are now paid back."},
 {phase:"Payoff",mols:[M("2-Phosphoglycerate",3,[2])],x2:true,rx:"3-Phosphoglycerate ⇌ 2-Phosphoglycerate   (×2)",d:{},note:"The phosphate shifts from carbon 3 to carbon 2, setting up the next step."},
 {phase:"Payoff",mols:[M("Phosphoenolpyruvate (PEP)",3,[2])],x2:true,rx:"2-Phosphoglycerate → Phosphoenolpyruvate + H₂O   (×2)",d:{},note:"Removing water creates PEP, which holds its phosphate in a very high-energy bond."},
 {phase:"Payoff",mols:[M("Pyruvate",3,[])],x2:true,rx:"PEP + ADP → Pyruvate + ATP   (×2)",d:{made:2,pyr:2},note:"Second substrate-level phosphorylation, irreversible. Net result: 2 ATP, 2 NADH, 2 pyruvate. Now pyruvate reaches the crossroads."}
];
let step=0, L={used:0,made:0,nadh:0,pyr:0}, answered=false;
function shuffle(a){for(let i=a.length-1;i>0;i--){const j=Math.floor(Math.random()*(i+1));[a[i],a[j]]=[a[j],a[i]];}return a;}
function molHTML(m,x2){
  let ch="";for(let i=1;i<=m.n;i++){ch+=`<span class="c">C${i}${m.p.includes(i)?'<span class="p">P</span>':''}</span>`;if(i<m.n)ch+='<span class="bond"></span>';}
  return `<div class="mol"><div class="chain" style="padding-top:22px">${ch}</div><span class="name">${m.name}</span>${x2?'<span class="x2">× 2 per glucose</span>':''}</div>`;
}
function tokens(el,n,cls){el.innerHTML=Array.from({length:n},()=>`<span class="tok ${cls}"></span>`).join("");}
function renderLedger(){
  $("#lUsed").textContent=L.used;$("#lMade").textContent=L.made;$("#lNadh").textContent=L.nadh;$("#lPyr").textContent=L.pyr;
  tokens($("#tUsed"),L.used,"used");tokens($("#tMade"),L.made,"atp");tokens($("#tNadh"),L.nadh,"nadh");tokens($("#tPyr"),L.pyr,"pyr");
  const net=L.made-L.used;$("#lNet").textContent=(net>0?"+":"")+net;
}
function renderRail(){
  $("#rail").innerHTML=STEPS.map((s,i)=>`<i class="${i<step?'done':(s.phase==='Investment'?'inv':'')}"></i>`).join("");
}
function renderTrace(){
  renderRail();renderLedger();
  const ask=$("#ask");answered=false;
  if(step===0){
    $("#stepTitle").textContent="Starting molecule";$("#phase").textContent="Ready";
    $("#molStage").innerHTML=molHTML(M("Glucose",6,[]),false);
    $("#rxn").textContent="Glucose enters the cell through a GLUT transporter.";
    $("#stepNote").textContent="Glucose is a 6-carbon sugar. Glycolysis needs no oxygen and happens in the cytosol of every living cell.";
  }
  if(step<STEPS.length){
    const s=STEPS[step];
    $("#phase").textContent=`Next: step ${step+1} · ${s.phase}`;
    const correct=ENZ[step];
    const pool=ENZ.filter(e=>e!==correct);shuffle(pool);
    const opts=shuffle([correct,pool[0],pool[1]]);
    ask.innerHTML=`<b>Which enzyme catalyzes step ${step+1}?</b><div class="opts">${opts.map(o=>`<button class="opt" data-o="${o}">${o}</button>`).join("")}</div><div class="fb" id="fb"></div>`;
    ask.querySelectorAll(".opt").forEach(b=>b.addEventListener("click",()=>choose(b,correct)));
    $("#revealBtn").disabled=false;
  }else{
    $("#phase").textContent="Complete";
    ask.innerHTML=`<div class="fb ok"><b>Glycolysis complete.</b> Net yield: 2 ATP, 2 NADH, 2 pyruvate, 2 H₂O. The cell now has 2 NADH that must be turned back into NAD⁺.</div><div class="row"><a class="btn" href="#simulate" style="text-decoration:none">Go to the NAD⁺ simulator</a></div>`;
    $("#revealBtn").disabled=true;
  }
}
function choose(btn,correct){
  if(answered)return;
  const fb=$("#fb");
  if(btn.dataset.o===correct){answered=true;btn.classList.add("right");fb.className="fb ok";fb.textContent="Correct.";setTimeout(advance,650);}
  else{btn.classList.add("wrong");btn.disabled=true;fb.className="fb no";fb.textContent=hint(step);}
}
function hint(i){
  return ["Hint: this enzyme adds a phosphate to a hexose (six-carbon sugar).","Hint: the reaction only rearranges atoms, so look for an isomerase.","Hint: this is the rate-limiting, committed step; its name says it adds a phosphate to fructose.","Hint: this enzyme splits a 6C sugar into two 3C pieces.","Hint: DHAP and G3P are isomers of each other.","Hint: an oxidation that reduces NAD⁺ needs a dehydrogenase.","Hint: a kinase moves a phosphate onto ADP; which substrate is it here?","Hint: a mutase shifts a group to another position in the same molecule.","Hint: this enzyme removes water (dehydration) to form an enol.","Hint: the last kinase of glycolysis is named after its product."][i];
}
function advance(){
  const s=STEPS[step];
  $("#stepTitle").textContent=`Step ${step+1}: ${ENZ[step]}`;
  $("#molStage").innerHTML=s.mols.map(m=>molHTML(m,s.x2)).join("");
  $("#rxn").textContent=s.rx;$("#stepNote").textContent=s.note;
  for(const k in s.d)L[k]+=s.d[k];
  step++;renderTrace();
  $("#stepTitle").textContent=`Step ${step}: ${ENZ[step-1]}`;
}
$("#revealBtn").addEventListener("click",()=>{if(step>=STEPS.length)return;const b=[...document.querySelectorAll(".opt")].find(x=>x.dataset.o===ENZ[step]);if(b)choose(b,ENZ[step]);});
$("#resetTrace").addEventListener("click",()=>{step=0;L={used:0,made:0,nadh:0,pyr:0};renderTrace();});
renderTrace();

/* ---------- NAD+ simulator ---------- */
const P={cell:"muscle",o2:100,dem:24,ferm:true,cyan:false};
const T=100, JMAX=6, AMAX=8, DT=0.1;
let S, hist=[], running=true;
function resetSim(){S={nad:T,pyr:0,lac:0,eth:0,co2:0,J:0,a:0,f:0,atp:0,met:1};hist=[];}
function tick(){
  const A=AMAX*(P.o2/100)*(P.cyan?0:1);
  const sat=(S.nad/T)/(0.15+S.nad/T)*1.15;
  const Jcap=Math.min(JMAX*sat, S.nad/(2*DT));
  let J1=P.dem/30, Jneed = (2*J1<=A)? J1 : Math.max(0,(P.dem-14*A)/2);
  const J=Math.max(0,Math.min(Jneed,Jcap));
  const pyr=2*J, a=Math.min(pyr,A), rest=pyr-a;
  const f=P.ferm?rest:0;
  S.nad-=2*J*DT;
  const nadh=T-S.nad;
  const reox=Math.min(nadh,(a+f)*DT);
  S.nad=Math.min(T,S.nad+reox);
  // pyruvate pool when it cannot be processed
  S.pyr+= (rest-f)*DT;
  const aer=P.o2/100*(P.cyan?0:1);
  if(P.cell==="muscle"){S.lac+=f*DT;S.lac-=S.lac*(0.01+0.05*aer)*DT;}
  else{S.eth+=f*DT;S.co2+=(f+3*a)*DT;}
  S.J=J;S.a=a;S.f=f;S.atp=2*J+14*a;S.met=Math.min(1,S.atp/P.dem);
  hist.push([S.nad/T,S.met,J/JMAX]);if(hist.length>200)hist.shift();
}
function setW(id,v){$(id).setAttribute("stroke-width",(1.5+v*14).toFixed(1));}
function render(){
  const nadPct=S.nad/T*100;
  $("#mNad").textContent=nadPct.toFixed(0)+"%";$("#bNad").style.width=nadPct+"%";
  $("#mAtp").textContent=(S.met*100).toFixed(0)+"%";$("#bAtp").style.width=(S.met*100)+"%";
  $("#mGlc").textContent=S.J.toFixed(2);$("#bGlc").style.width=(S.J/JMAX*100)+"%";
  if(P.cell==="muscle"){
    const pH=7.1-0.7*(S.lac/(S.lac+150));
    $("#mProdK").textContent="Cell pH";$("#mProd").textContent=pH.toFixed(2);$("#bProd").style.width=((7.1-pH)/0.7*100)+"%";
  }else{
    $("#mProdK").textContent="Ethanol made";$("#mProd").textContent=S.eth.toFixed(0);$("#bProd").style.width=Math.min(100,S.eth/3)+"%";
  }
  const tot=Math.max(S.a+S.f+(2*S.J-S.a-S.f),0.0001);
  setW("#aGly",S.J/JMAX);setW("#aMito",S.a/AMAX);setW("#aFerm",S.f/12);
  $("#xCyan").setAttribute("opacity",P.cyan?1:0);
  $("#mitoTxt").textContent=P.cyan?"Complex IV blocked":(P.o2<5?"No O₂: ETC stalled":"O₂ is final e⁻ acceptor");
  $("#fermTitle").textContent=P.cell==="muscle"?"Lactate":"Ethanol + CO₂";
  $("#fermSub").textContent=P.cell==="muscle"?"via LDH · regenerates NAD⁺":"via PDC + ADH · regenerates NAD⁺";
  $("#fermBlock").textContent=P.ferm?"":"enzyme blocked";
  $("#aNad").setAttribute("opacity",(S.a+S.f)>0.05?1:0.2);
  $("#pyrPool").textContent=S.pyr>1?`Pyruvate piling up: ${S.pyr.toFixed(0)}`:"";
  // status
  const st=$("#status");let cls="",msg="";
  const aerShare=S.atp>0?(14*S.a)/S.atp:0;
  if(nadPct<15){cls="crit";msg=`<b>Glycolysis has stalled at step 6.</b> Almost no NAD⁺ is left for glyceraldehyde-3-P dehydrogenase. With no oxygen-driven ETC and no fermentation, NADH cannot be reoxidized, so ATP production collapses.`;}
  else if(P.cyan){cls="crit";msg=`<b>Cyanide has shut down the ETC.</b> Oxygen is present but cannot accept electrons at Complex IV, so the mitochondria make almost no ATP. The cell survives briefly on glycolysis plus ${P.cell==="muscle"?"lactic acid":"alcoholic"} fermentation; in the body, lactate builds up and blood pH drops (lactic acidosis).`;}
  else if(S.f<0.05){msg=`<b>Fully aerobic.</b> The ETC reoxidizes NADH and each pyruvate is oxidized in the mitochondrion. About ${aerShare>0?(aerShare*100).toFixed(0):0}% of ATP comes from oxidative phosphorylation, so the cell needs very little glucose.`;}
  else if(S.a<0.05){cls="warn";msg=`<b>Fully fermentative.</b> All pyruvate goes to ${P.cell==="muscle"?"lactate":"ethanol and CO₂"} to regenerate NAD⁺. Only 2 ATP per glucose, so the cell burns glucose much faster to keep up${S.met<0.98?" and still falls short of demand":""}.`;}
  else {cls="warn";msg=`<b>Mixed.</b> Oxygen covers ${(S.a/(S.a+S.f)*100).toFixed(0)}% of pyruvate; the rest is fermented to ${P.cell==="muscle"?"lactate":"ethanol"} to keep NAD⁺ available. ${S.met<0.98?"ATP supply is below demand.":""}`;}
  st.className="status "+cls;st.innerHTML=msg;
  drawChart();
}
const cv=$("#chart"),ctx=cv.getContext("2d");
function drawChart(){
  const dpr=window.devicePixelRatio||1,w=cv.clientWidth,h=190;
  if(cv.width!==Math.round(w*dpr)){cv.width=Math.round(w*dpr);cv.height=Math.round(h*dpr);}
  ctx.setTransform(dpr,0,0,dpr,0,0);ctx.clearRect(0,0,w,h);
  const cs=getComputedStyle(document.documentElement),col=n=>cs.getPropertyValue(n).trim();
  const L=34,R=8,Tp=8,B=22,pw=w-L-R,ph=h-Tp-B;
  ctx.font="11px "+col("--mono");ctx.fillStyle=col("--muted");ctx.strokeStyle=col("--line");ctx.lineWidth=1;
  [0,50,100].forEach(v=>{const y=Tp+ph*(1-v/100);ctx.beginPath();ctx.moveTo(L,y);ctx.lineTo(L+pw,y);ctx.stroke();ctx.textAlign="right";ctx.textBaseline="middle";ctx.fillText(v+"%",L-6,y);});
  ctx.textAlign="left";ctx.textBaseline="alphabetic";ctx.fillText("−20 s",L,h-5);ctx.textAlign="right";ctx.fillText("now",L+pw,h-5);
  [["--nadh",0],["--atp",1],["--accent",2]].forEach(([c,k])=>{
    ctx.strokeStyle=col(c);ctx.lineWidth=2.2;ctx.beginPath();
    hist.forEach((p,i)=>{const x=L+pw*(i+(200-hist.length))/199,y=Tp+ph*(1-Math.max(0,Math.min(1,p[k])));i?ctx.lineTo(x,y):ctx.moveTo(x,y);});
    ctx.stroke();
  });
}
let last=0,acc=0;
function loop(t){
  if(running){acc+=Math.min(200,t-(last||t));while(acc>=50){tick();acc-=50;}}
  last=t;render();requestAnimationFrame(loop);
}
// controls
function syncControls(){
  $("#o2").value=P.o2;$("#o2v").textContent=P.o2+"%";$("#dem").value=P.dem;$("#demv").textContent=P.dem;
  $("#ferm").checked=P.ferm;$("#cyan").checked=P.cyan;
  $("#fermLbl").textContent=P.cell==="muscle"?"Lactate dehydrogenase (LDH) active":"Pyruvate decarboxylase + ADH active";
  document.querySelectorAll("#cellSeg button").forEach(b=>b.setAttribute("aria-pressed",b.dataset.v===P.cell));
}
function clearScen(){document.querySelectorAll(".scen").forEach(b=>b.setAttribute("aria-pressed","false"));}
function loadScenario(s){Object.assign(P,{cell:s.cell,o2:s.o2,dem:s.dem,ferm:s.ferm,cyan:s.cyan});resetSim();syncControls();clearScen();document.querySelector(`.scen[data-id="${s.id}"]`).setAttribute("aria-pressed","true");running=true;$("#playBtn").textContent="Pause";}
$("#o2").addEventListener("input",e=>{P.o2=+e.target.value;$("#o2v").textContent=P.o2+"%";clearScen();});
$("#dem").addEventListener("input",e=>{P.dem=+e.target.value;$("#demv").textContent=P.dem;clearScen();});
$("#ferm").addEventListener("change",e=>{P.ferm=e.target.checked;clearScen();});
$("#cyan").addEventListener("change",e=>{P.cyan=e.target.checked;clearScen();});
document.querySelectorAll("#cellSeg button").forEach(b=>b.addEventListener("click",()=>{P.cell=b.dataset.v;resetSim();syncControls();clearScen();}));
$("#playBtn").addEventListener("click",()=>{running=!running;$("#playBtn").textContent=running?"Pause":"Resume";});
$("#simReset").addEventListener("click",resetSim);
resetSim();loadScenario(SCEN[0]);requestAnimationFrame(loop);

/* ---------- Quiz ---------- */
const Q=[
 {q:"Which glycolysis step stops first when a cell runs out of NAD⁺?",c:["Step 1, hexokinase","Step 3, phosphofructokinase-1","Step 6, glyceraldehyde-3-phosphate dehydrogenase","Step 10, pyruvate kinase"],a:2,e:"Step 6 is the only oxidation in glycolysis. It transfers electrons from G3P to NAD⁺, forming NADH. Without NAD⁺, this reaction cannot proceed and everything after it stops."},
 {q:"What is the net yield of glycolysis from one glucose molecule?",c:["4 ATP, 2 NADH, 2 pyruvate","2 ATP, 2 NADH, 2 pyruvate","2 ATP, 2 FADH₂, 2 acetyl-CoA","36 ATP, 6 CO₂"],a:1,e:"Glycolysis makes 4 ATP but spends 2 in the investment phase (steps 1 and 3), so the net is 2 ATP, plus 2 NADH and 2 pyruvate."},
 {q:"During the 100-m dash, the main reason muscle cells make lactate is to:",c:["Produce extra ATP from pyruvate","Regenerate NAD⁺ so glycolysis can continue","Store energy for the Krebs cycle","Release CO₂ from the muscle"],a:1,e:"LDH converts pyruvate to lactate using NADH, returning NAD⁺ to step 6. The lactate step makes no ATP; the cell still gets only the 2 ATP from glycolysis."},
 {q:"Pan de sal dough rises because yeast:",c:["Produce CO₂ when pyruvate decarboxylase removes a carbon from pyruvate","Produce lactate, which expands as it forms","Release oxygen during glycolysis","Convert ethanol into water vapor"],a:0,e:"In alcoholic fermentation, pyruvate decarboxylase turns pyruvate (3C) into acetaldehyde (2C) plus CO₂. The trapped CO₂ makes the dough rise; the ethanol evaporates in the oven."},
 {q:"A patient ate improperly processed cassava and has cyanide poisoning. Their blood oxygen is normal, yet their blood lactate is high. Why?",c:["Cyanide blocks hexokinase, so glucose builds up","Cyanide blocks Complex IV, so the ETC cannot use O₂ and cells rely on glycolysis plus lactic acid fermentation","Cyanide turns pyruvate directly into lactate","Cyanide stops the lungs from absorbing oxygen"],a:1,e:"Cyanide binds cytochrome c oxidase (Complex IV). Oxygen is delivered but cannot accept electrons, so NADH is not reoxidized by the ETC. Cells shift to fermentation, and lactate accumulates (lactic acidosis). Try it in the simulator with cyanide on."},
 {q:"In which steps does glycolysis make ATP by substrate-level phosphorylation?",c:["Steps 1 and 3","Steps 6 and 9","Steps 7 and 10","Only step 10"],a:2,e:"Phosphoglycerate kinase (step 7) and pyruvate kinase (step 10) each transfer a phosphate from a substrate directly to ADP. Each runs twice per glucose, giving 4 ATP total."},
 {q:"Yeast in a sealed tuba container uses sugar much faster than the same yeast with plenty of oxygen. Why?",c:["Fermentation yields only 2 ATP per glucose versus about 30 aerobically, so more glucose is needed for the same ATP","Oxygen destroys glucose","Ethanol speeds up hexokinase","Sealed containers are warmer"],a:0,e:"This is the Pasteur effect. Without oxygen, each glucose gives far less ATP, so the cell must run glycolysis much faster to meet the same demand. Compare glucose use in the simulator at 0% and 100% oxygen."},
 {q:"Per glucose, alcoholic fermentation produces:",c:["2 lactate","2 ethanol and 2 CO₂","1 ethanol and 1 CO₂","2 acetyl-CoA and 2 CO₂"],a:1,e:"Glucose gives 2 pyruvate. Each pyruvate loses one CO₂ and becomes one ethanol, so the total is 2 ethanol and 2 CO₂ (and the net 2 ATP from glycolysis)."}
];
let qState=[];
function renderQuiz(){
  qState=Q.map(()=>null);
  $("#quiz").innerHTML=Q.map((x,i)=>`<div class="q" data-i="${i}"><span class="qn">Question ${i+1} of ${Q.length}</span><p class="prompt">${x.q}</p><div class="choices">${x.c.map((c,j)=>`<button class="choice" data-j="${j}">${c}</button>`).join("")}</div><div class="explain" hidden></div></div>`).join("");
  document.querySelectorAll(".q").forEach(qd=>{
    const i=+qd.dataset.i;
    qd.querySelectorAll(".choice").forEach(b=>b.addEventListener("click",()=>{
      if(qState[i]!==null)return;
      const j=+b.dataset.j,ok=j===Q[i].a;qState[i]=ok;
      qd.querySelectorAll(".choice").forEach((c,k)=>{c.disabled=true;if(k===Q[i].a)c.classList.add("right");});
      if(!ok)b.classList.add("wrong");
      const ex=qd.querySelector(".explain");ex.hidden=false;
      ex.innerHTML=`<b style="color:var(${ok?"--good":"--bad"})">${ok?"Correct.":"Not quite."}</b> ${Q[i].e}`;
      updScore();
    }));
  });
  updScore();
}
function updScore(){const done=qState.filter(v=>v!==null).length,right=qState.filter(v=>v).length;$("#scoreNum").textContent=`${right} / ${done}`;if(done===Q.length)$("#scoreNum").textContent=`${right} / ${Q.length} · ${right===Q.length?"mastered":right>=6?"proficient":"review Stages 2–4"}`;}
$("#quizReset").addEventListener("click",renderQuiz);
renderQuiz();
})();
</script>
</body>
</html>
