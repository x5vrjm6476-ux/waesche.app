<!doctype html>
<html lang="de">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Wäsche Counter</title>
  <style>
    :root{
      color-scheme: dark;
      --bg:#0b0b0f;
      --card1: rgba(255,255,255,.07);
      --card2: rgba(255,255,255,.05);
      --stroke: rgba(255,255,255,.12);
      --text: rgba(255,255,255,.92);
      --muted: rgba(255,255,255,.55);
      --muted2: rgba(255,255,255,.35);
      --shadow: 0 18px 55px rgba(0,0,0,.55);
      --r: 18px;
      --r2: 14px;
    }

    *{ box-sizing:border-box; }
    body{
      margin:0;
      font-family: ui-sans-serif, -apple-system, BlinkMacSystemFont, "SF Pro Text",
                   "Helvetica Neue", Arial, system-ui, sans-serif;
      min-height:100svh;
      display:grid;
      place-items:center;
      padding:24px;
      background:
        radial-gradient(1100px 700px at 20% 10%, rgba(255,255,255,.06), transparent 60%),
        radial-gradient(900px 600px at 80% 20%, rgba(255,255,255,.04), transparent 55%),
        radial-gradient(800px 600px at 50% 110%, rgba(255,255,255,.05), transparent 60%),
        var(--bg);
      color:var(--text);
    }

    .wrap{ width:min(680px, 100%); }

    .header{
      display:flex;
      justify-content:space-between;
      align-items:baseline;
      gap:16px;
      margin-bottom:14px;
    }
    h1{
      margin:0;
      font-size:20px;
      font-weight:700;
      letter-spacing:.2px;
    }
    .sub{
      margin:0;
      font-size:13px;
      color:var(--muted);
    }

    .grid{
      display:grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap:14px;
    }
    @media (max-width: 560px){
      .grid{ grid-template-columns:1fr; }
    }

    .card{
      position:relative;
      background: linear-gradient(180deg, var(--card1), var(--card2));
      border:1px solid var(--stroke);
      border-radius: var(--r);
      box-shadow: var(--shadow);
      padding:16px;
      overflow:hidden;
    }

    /* purely visual highlight, cannot block taps */
    .card::before{
      content:"";
      position:absolute;
      inset:-2px;
      background: radial-gradient(320px 180px at 25% 0%, rgba(255,255,255,.08), transparent 60%);
      pointer-events:none; /* critical */
      z-index:0;
    }

    .cardTop{
      position:relative;
      z-index:2;
      display:flex;
      justify-content:space-between;
      align-items:flex-start;
      gap:12px;
    }

    .label{
      margin:0 0 6px 0;
      font-size:13px;
      color:var(--muted);
      letter-spacing:.2px;
    }
    .value{
      margin:0;
      font-size:34px;
      font-weight:800;
      letter-spacing:-.6px;
      line-height:1;
    }
    .price{
      margin-top:6px;
      font-size:12px;
      color:var(--muted2);
    }

    .plusBtn{
      -webkit-tap-highlight-color: transparent;
      position:relative;
      z-index:3;
      width:48px;
      height:48px;
      border-radius: var(--r2);
      border:1px solid rgba(255,255,255,.16);
      background: rgba(255,255,255,.08);
      color: rgba(255,255,255,.92);
      font-size:22px;
      display:grid;
      place-items:center;
      cursor:pointer;
      user-select:none;
      touch-action: manipulation; /* better iOS tap behavior */
      transition: transform .08s ease, background .2s ease, border-color .2s ease;
    }
    .plusBtn:active{
      transform: scale(.98);
      background: rgba(255,255,255,.11);
      border-color: rgba(255,255,255,.22);
    }

    .sumCard{
      margin-top:14px;
      background: rgba(255,255,255,.04);
      border:1px solid rgba(255,255,255,.10);
      border-radius: var(--r);
      padding:16px;
      display:flex;
      justify-content:space-between;
      align-items:center;
      gap:12px;
    }
    .sumLabel{
      margin:0;
      font-size:13px;
      color:var(--muted);
    }
    .sumValue{
      margin:4px 0 0 0;
      font-size:22px;
      font-weight:800;
      letter-spacing:-.2px;
      white-space:nowrap;
    }
    .sumMeta{
      font-size:12px;
      color:var(--muted2);
      text-align:right;
      white-space:nowrap;
    }

    .tinyReset{
      margin-top:22px;
      text-align:center;
    }
    .tinyReset button{
      -webkit-tap-highlight-color: transparent;
      background:transparent;
      border:none;
      color: rgba(255,255,255,.28);
      font-size:12px;
      cursor:pointer;
      padding:8px 10px;
      border-radius:10px;
      touch-action: manipulation;
      transition: color .2s ease, background .2s ease;
    }
    .tinyReset button:hover{
      color: rgba(255,255,255,.42);
      background: rgba(255,255,255,.03);
    }

    dialog{
      border:1px solid rgba(255,255,255,.12);
      border-radius:18px;
      padding:0;
      background: rgba(20,20,24,.92);
      color: var(--text);
      box-shadow: var(--shadow);
      width: min(420px, calc(100% - 24px));
    }
    dialog::backdrop{
      background: rgba(0,0,0,.55);
      backdrop-filter: blur(8px);
    }
    .modal{ padding:16px; }
    .modal h3{
      margin:0 0 6px 0;
      font-size:16px;
      font-weight:800;
      letter-spacing:-.2px;
    }
    .modal p{
      margin:0 0 14px 0;
      font-size:13px;
      color: var(--muted);
      line-height:1.35;
    }
    .actions{
      display:flex;
      justify-content:flex-end;
      gap:10px;
    }
    .btn{
      -webkit-tap-highlight-color: transparent;
      border:1px solid rgba(255,255,255,.14);
      background: rgba(255,255,255,.06);
      color: var(--text);
      padding:10px 12px;
      border-radius:12px;
      font-size:13px;
      cursor:pointer;
      touch-action: manipulation;
      transition: transform .08s ease, background .2s ease, border-color .2s ease;
    }
    .btn:active{ transform: scale(.99); }
    .btnPrimary{
      border-color: rgba(255,255,255,.18);
      background: rgba(255,255,255,.10);
    }
  </style>
</head>

<body>
  <main class="wrap">
    <div class="header">
      <h1>Wäsche Counter</h1>
      <p class="sub">Speichert lokal im Browser</p>
    </div>

    <section class="grid" aria-label="Counter">
      <article class="card">
        <div class="cardTop">
          <div>
            <p class="label">60° Wäsche</p>
            <p class="value" id="countHot">0</p>
            <div class="price">CHF 1.50 pro Wäsche</div>
          </div>
          <button class="plusBtn" id="btnHot" type="button" aria-label="60° Wäsche +1">+</button>
        </div>
      </article>

      <article class="card">
        <div class="cardTop">
          <div>
            <p class="label">Normale Wäsche</p>
            <p class="value" id="countNormal">0</p>
            <div class="price">CHF 1.00 pro Wäsche</div>
          </div>
          <button class="plusBtn" id="btnNormal" type="button" aria-label="Normale Wäsche +1">+</button>
        </div>
      </article>
    </section>

    <section class="sumCard" aria-label="Summe">
      <div>
        <p class="sumLabel">Summe</p>
        <p class="sumValue" id="sumText">CHF 0.00</p>
      </div>
      <div class="sumMeta"><span id="sumCount">0</span> Wäschen</div>
    </section>

    <div class="tinyReset">
      <button id="resetLink" type="button">zurücksetzen</button>
    </div>

    <dialog id="confirmDialog" aria-label="Zurücksetzen bestätigen">
      <div class="modal">
        <h3>Wirklich zurücksetzen?</h3>
        <p>Alle Zähler werden auf 0 gesetzt. Das kann nicht rückgängig gemacht werden.</p>
        <div class="actions">
          <button class="btn" id="cancelReset" type="button">Abbrechen</button>
          <button class="btn btnPrimary" id="confirmReset" type="button">Zurücksetzen</button>
        </div>
      </div>
    </dialog>
  </main>

  <script>
    // Prices
    const PRICE_HOT = 1.50;
    const PRICE_NORMAL = 1.00;

    // Storage key
    const KEY = "laundry_counter_v1";

    // Elements
    const elHot = document.getElementById("countHot");
    const elNormal = document.getElementById("countNormal");
    const elSum = document.getElementById("sumText");
    const elSumCount = document.getElementById("sumCount");

    const btnHot = document.getElementById("btnHot");
    const btnNormal = document.getElementById("btnNormal");

    const resetLink = document.getElementById("resetLink");
    const dialog = document.getElementById("confirmDialog");
    const cancelReset = document.getElementById("cancelReset");
    const confirmReset = document.getElementById("confirmReset");

    // State
    let state = loadState();

    function clampInt(v){
      const n = Number(v);
      if (!Number.isFinite(n)) return 0;
      return Math.max(0, Math.floor(n));
    }

    function loadState(){
      try{
        const raw = localStorage.getItem(KEY);
        if(!raw) return { hot: 0, normal: 0 };
        const parsed = JSON.parse(raw);
        return { hot: clampInt(parsed.hot), normal: clampInt(parsed.normal) };
      } catch {
        return { hot: 0, normal: 0 };
      }
    }

    function saveState(){
      localStorage.setItem(KEY, JSON.stringify(state));
    }

    function formatCHF(amount){
      return "CHF " + amount.toFixed(2);
    }

    function render(){
      elHot.textContent = String(state.hot);
      elNormal.textContent = String(state.normal);

      const sum = (state.hot * PRICE_HOT) + (state.normal * PRICE_NORMAL);
      const count = state.hot + state.normal;

      elSum.textContent = formatCHF(sum);
      elSumCount.textContent = String(count);
    }

    function incHot(){
      state.hot += 1;
      saveState();
      render();
    }

    function incNormal(){
      state.normal += 1;
      saveState();
      render();
    }

    function openResetConfirm(){
      if (dialog && typeof dialog.showModal === "function") {
        dialog.showModal();
      } else {
        const ok = confirm("Wirklich zurücksetzen? Alle Zähler werden auf 0 gesetzt.");
        if (ok) doReset();
      }
    }

    function closeDialog(){
      if (dialog && dialog.open) dialog.close();
    }

    function doReset(){
      state = { hot: 0, normal: 0 };
      saveState();
      render();
    }

    // Bind events (click + touch fallback for picky WebViews)
    btnHot.addEventListener("click", incHot);
    btnNormal.addEventListener("click", incNormal);

    btnHot.addEventListener("touchend", (e) => { e.preventDefault(); incHot(); }, { passive: false });
    btnNormal.addEventListener("touchend", (e) => { e.preventDefault(); incNormal(); }, { passive: false });

    resetLink.addEventListener("click", openResetConfirm);
    resetLink.addEventListener("touchend", (e) => { e.preventDefault(); openResetConfirm(); }, { passive: false });

    cancelReset.addEventListener("click", closeDialog);
    confirmReset.addEventListener("click", () => { doReset(); closeDialog(); });

    // Dialog cancel (ESC)
    if (dialog){
      dialog.addEventListener("cancel", (e) => {
        e.preventDefault();
        closeDialog();
      });
    }

    render();
  </script>
</body>
</html>
