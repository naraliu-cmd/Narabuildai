<!doctype html>
<html lang="zh-Hant">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>生日活動分工系統 - Cyberpunk Command Center</title>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&family=Roboto+Mono&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg-dark: #050a18;
      --neon-cyan: #00f2ff;
      --neon-pink: #ff00ff;
      --neon-gold: #ffcc00; /* 新增備忘錄專用色 */
      --text-glow: 0 0 5px var(--neon-cyan), 0 0 10px var(--neon-cyan);
      --box-glow: 0 0 10px rgba(0, 242, 255, 0.5), inset 0 0 10px rgba(0, 242, 255, 0.2);
      --card-bg: rgba(10, 20, 40, 0.7);
      --border-color: rgba(0, 242, 255, 0.4);
    }

    body {
      margin: 0; min-height: 100vh;
      font-family: 'Orbitron', "Microsoft JhengHei", sans-serif;
      background-color: var(--bg-dark);
      background-image: 
        radial-gradient(circle at 20% 30%, rgba(0, 85, 255, 0.2) 0%, transparent 40%),
        radial-gradient(circle at 80% 70%, rgba(255, 0, 255, 0.15) 0%, transparent 40%),
        radial-gradient(white 1px, transparent 1px),
        radial-gradient(white 0.5px, transparent 0.5px);
      background-size: 100% 100%, 100% 100%, 50px 50px, 20px 20px;
      color: #fff; display: flex; justify-content: center; align-items: center; padding: 20px;
    }

    .wrap {
      width: 100%; max-width: 1150px;
      display: grid; grid-template-columns: 1fr 1fr; gap: 30px; position: relative;
    }
    
    .main-title-decor {
      position: absolute; top: -50px; left: 0; font-size: 24px;
      color: var(--neon-pink); text-shadow: 0 0 10px var(--neon-pink);
      display: flex; align-items: center; gap: 10px;
    }

    .cyber-card {
      background: var(--card-bg); border: 1px solid var(--border-color);
      border-radius: 15px; padding: 25px; box-shadow: var(--box-glow);
      backdrop-filter: blur(10px); position: relative; overflow: hidden;
      display: flex; flex-direction: column;
    }

    h1, h2 {
      margin: 0 0 15px; color: var(--neon-cyan); text-shadow: var(--text-glow);
      font-size: 22px; display: flex; align-items: center; gap: 10px;
    }

    textarea {
      width: 100%; height: 160px; background: rgba(0, 0, 0, 0.5);
      border: 1px solid var(--border-color); border-radius: 10px;
      padding: 15px; color: var(--neon-cyan); font-family: 'Roboto Mono', monospace;
      resize: none; outline: none; box-sizing: border-box; transition: 0.3s;
    }

    .btn-group { display: flex; gap: 10px; margin: 15px 0; }

    button {
      flex: 1; padding: 12px; border: 1px solid var(--neon-cyan);
      background: rgba(0, 242, 255, 0.1); color: var(--neon-cyan);
      font-family: 'Orbitron', sans-serif; font-weight: bold;
      border-radius: 8px; cursor: pointer; transition: 0.3s; text-transform: uppercase;
    }

    button:hover:not(:disabled) {
      background: var(--neon-cyan); color: var(--bg-dark); box-shadow: 0 0 20px var(--neon-cyan);
    }

    button.secondary { border-color: var(--neon-pink); color: var(--neon-pink); background: rgba(255, 0, 255, 0.1); }

    .status-monitor {
      margin-top: 5px; padding: 12px; background: rgba(0,0,0,0.3);
      border-radius: 10px; border: 1px dashed var(--border-color);
    }

    .monitor-line { display: flex; justify-content: space-between; font-size: 11px; color: var(--neon-cyan); margin-bottom: 5px; }
    
    .waveform { display: flex; align-items: flex-end; gap: 2px; height: 25px; }
    .wave-bar { flex: 1; background: var(--neon-cyan); height: 10%; animation: pulse 1.5s infinite ease-in-out; }
    @keyframes pulse { 0%, 100% { height: 10%; opacity: 0.3; } 50% { height: 100%; opacity: 1; } }

    .log-container {
      height: 100px; background: rgba(0, 10, 20, 0.8);
      border: 1px solid var(--border-color); border-radius: 10px;
      padding: 10px; overflow-y: auto; font-family: 'Roboto Mono', monospace;
      font-size: 11px; color: #0f0; text-shadow: 0 0 5px #0f0; margin-top: 10px;
    }

    /* 結果區塊樣式 */
    .role-block {
      background: rgba(0, 0, 0, 0.3); border: 1px solid rgba(0, 242, 255, 0.2);
      border-radius: 12px; padding: 12px; margin-bottom: 12px;
      display: flex; align-items: center;
    }
    .role-info { flex: 1; margin-left: 15px; }
    .role-title { font-size: 11px; color: rgba(255, 255, 255, 0.5); margin-bottom: 3px; }
    .role-name { font-size: 18px; color: var(--neon-cyan); text-shadow: 0 0 5px var(--neon-cyan); font-weight: bold; }
    .role-name.locked { animation: lock-flash 0.6s ease-out; }

    @keyframes lock-flash { 0% { transform: scale(1.1); filter: brightness(2); } 100% { transform: scale(1); } }

    /* 新增：貼心小提醒區 (Protocol Reminders) */
    .reminders-box {
      margin-top: 5px;
      padding: 15px;
      background: rgba(255, 204, 0, 0.05);
      border: 1px solid rgba(255, 204, 0, 0.3);
      border-radius: 12px;
      position: relative;
    }
    .reminders-box h3 {
      margin: 0 0 10px;
      font-size: 14px;
      color: var(--neon-gold);
      text-transform: uppercase;
      letter-spacing: 1px;
      display: flex; align-items: center; gap: 8px;
    }
    .reminders-box h3::after {
      content: "ACTIVE";
      font-size: 8px; padding: 2px 4px; background: var(--neon-gold);
      color: #000; border-radius: 3px; animation: blink 1s infinite;
    }
    @keyframes blink { 0%, 100% { opacity: 1; } 50% { opacity: 0.3; } }

    .reminder-list {
      list-style: none; padding: 0; margin: 0;
      font-family: 'Roboto Mono', sans-serif;
      font-size: 12px; color: #ffeb99;
    }
    .reminder-list li {
      margin-bottom: 6px; display: flex; align-items: flex-start; gap: 8px;
      line-height: 1.4;
    }
    .reminder-list li::before {
      content: ">>"; color: var(--neon-gold); font-weight: bold;
    }

    ::-webkit-scrollbar { width: 4px; }
    ::-webkit-scrollbar-thumb { background: var(--neon-cyan); }
  </style>
</head>
<body>
  <div class="wrap">
    <div class="main-title-decor">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 2L2 7l10 5 10-5-10-5zM2 17l10 5 10-5M2 12l10 5 10-5"/></svg>
        Hm. 企劃課生日慶生準備工作
    </div>

    <div class="cyber-card">
      <h1>控制台 // CONTROLLER</h1>
      <textarea id="names" oninput="updateCount()">Nara
Mini
MP
呱呱
蛋蛋
白白
喜徳
10
MIO
RN
榮大</textarea>

      <div class="btn-group">
        <button id="drawBtn">執行分配程序</button>
        <button id="clearBtn" class="secondary">系統重置</button>
      </div>

      <div class="status-monitor">
        <div class="monitor-line">
          <span>NEURAL LINK: <b style="color:var(--neon-pink)">ONLINE</b></span>
          <span>MEMBERS: <b id="memberCount">10</b></span>
        </div>
        <div class="waveform" id="waveform"></div>
        <div id="log" class="log-container">> System ready...</div>
      </div>
    </div>

    <div class="cyber-card">
      <h2>分配結果 // ALLOCATION</h2>
      
      <div class="role-block">
        <div style="width:8px;height:8px;background:var(--neon-cyan);border-radius:50%;box-shadow:0 0 8px var(--neon-cyan)"></div>
        <div class="role-info">
          <div class="role-title">ROLE // 想卡片內容</div>
          <div class="role-name" id="roleA">STANDBY...</div>
        </div>
      </div>

      <div class="role-block">
        <div style="width:8px;height:8px;background:var(--neon-pink);border-radius:50%;box-shadow:0 0 8px var(--neon-pink)"></div>
        <div class="role-info">
          <div class="role-title">ROLE // 寫卡片內容</div>
          <div class="role-name" id="roleB" style="color:var(--neon-pink);text-shadow:0 0 5px var(--neon-pink)">STANDBY...</div>
        </div>
      </div>

      <div class="role-block">
        <div style="width:8px;height:8px;background:#fff;border-radius:50%;box-shadow:0 0 8px #fff"></div>
        <div class="role-info">
          <div class="role-title">ROLE // 準備生日小遊戲</div>
          <div class="role-name" id="roleC" style="color:#fff;text-shadow:0 0 5px #fff">STANDBY...</div>
        </div>
      </div>

      <div class="reminders-box">
        <h3>Protocol Reminders // 任務備忘</h3>
        <ul class="reminder-list">
          <li>蛋糕預訂任務：確認口味後即刻下訂。</li>
          <li>裝備領取：蠟燭與打火機請至管理部申領。</li>
          <li>遊戲規範：小遊戲主題務必與「博弈/機率」相關。</li>
          <li>認證程序：卡片務必請全體成員親筆簽名。</li>
          <li>空間鎖定：確認當日會議室預約狀態。</li>
        </ul>
      </div>

      <div style="margin-top:auto; font-size:10px; color:rgba(255,255,255,0.2); text-align:right; padding-top:10px;">
        AUTH_LEVEL: 04 // UNIT_77 // MISSION_BIRTHDAY
      </div>
    </div>
  </div>

<script>
  const $ = (id) => document.getElementById(id);
  const logEl = $("log");
  let drawing = false;

  const waveform = $("waveform");
  for(let i=0; i<30; i++) {
    const bar = document.createElement("div");
    bar.className = "wave-bar";
    bar.style.animationDelay = `${i * 0.05}s`;
    waveform.appendChild(bar);
  }

  function updateCount() {
    const names = cleanNames($("names").value);
    $("memberCount").innerText = names.length;
  }

  function cleanNames(raw){
    return raw.split(/\r?\n/).map(s => s.trim()).filter(Boolean);
  }

  function shuffle(arr){
    const a = [...arr];
    for(let i=a.length-1; i>0; i--){
      const j = Math.floor(Math.random() * (i+1));
      [a[i], a[j]] = [a[j], a[i]];
    }
    return a;
  }
  
  function addLog(message) {
    const ts = new Date().toLocaleTimeString('en-US', { hour12: false });
    logEl.innerHTML = `> [${ts}] ${message}<br>` + logEl.innerHTML;
  }

  async function draw(){
    if(drawing) return;
    const names = cleanNames($("names").value);
    if(names.length < 3){ alert("Error: 樣本數不足 3 人！"); return; }

    drawing = true;
    $("drawBtn").disabled = true;
    addLog("Rerouting neural pathways...");

    const roles = ['roleA', 'roleB', 'roleC'].map(id => $(id));
    const duration = 1500;
    const interval = 60;
    let currentStep = 0;

    const rollingId = setInterval(() => {
      roles.forEach(r => {
        r.innerText = names[Math.floor(Math.random() * names.length)];
        r.classList.remove('locked');
      });
      currentStep++;
      if(currentStep >= duration/interval) {
        clearInterval(rollingId);
        const pool = shuffle(names);
        roles.forEach((r, i) => {
          r.innerText = pool[i];
          r.classList.add('locked');
        });
        addLog("SUCCESS: Data locked. Protocol engaged.");
        drawing = false;
        $("drawBtn").disabled = false;
      }
    }, interval);
  }

  $("drawBtn").onclick = draw;
  $("clearBtn").onclick = () => { location.reload(); };
  updateCount();
</script>
</body>
</html>
