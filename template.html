<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Verifikasi Email</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;600;700&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --bg: #0A0E16;
    --bg-2: #0D1220;
    --surface: #121826;
    --surface-2: #171F30;
    --border: #232C40;
    --text: #E9ECF3;
    --text-muted: #8890A3;
    --violet: #7C5CFC;
    --violet-soft: #7C5CFC33;
    --cyan: #45E0D0;
    --danger: #FF6B6B;
    --success: #34D399;
    --ease: cubic-bezier(.65,0,.35,1);
    --bouncy: cubic-bezier(.34,1.56,.64,1);
  }
  *{ box-sizing: border-box; }
  html, body{
    margin:0; padding:0; min-height:100%;
    background: var(--bg); color: var(--text);
    font-family:'Inter', sans-serif;
    overflow-x:hidden; overflow-y:auto;
  }

  .backdrop{
    position: fixed; inset:0; z-index:0;
    background:
      radial-gradient(ellipse 900px 600px at 15% 20%, #7C5CFC22, transparent 60%),
      radial-gradient(ellipse 800px 700px at 85% 80%, #45E0D01c, transparent 60%),
      var(--bg);
  }
  .orb{ position:absolute; border-radius:50%; filter:blur(70px); opacity:.5; animation: drift 24s ease-in-out infinite; }
  .orb.a{ width:420px; height:420px; background: radial-gradient(circle, #7C5CFC 0%, transparent 70%); top:-10%; left:-8%; }
  .orb.b{ width:360px; height:360px; background: radial-gradient(circle, #45E0D0 0%, transparent 70%); bottom:-12%; right:-6%; animation-delay:-8s; }
  @keyframes drift{
    0%,100%{ transform: translate(0,0) scale(1); }
    50%{ transform: translate(24px,-30px) scale(1.06); }
  }

  .stage{
    position:relative; z-index:2; min-height:100dvh; width:100%;
    display:flex; align-items:center; justify-content:center; padding:24px;
  }

  .card{
    width:min(440px, 100%);
    background: linear-gradient(180deg, var(--surface), var(--bg-2));
    border:1px solid var(--border);
    border-radius:22px;
    padding: 42px 36px 38px;
    text-align:center;
    box-shadow: 0 40px 100px -30px #00000090;
    animation: cardIn .6s var(--bouncy) both;
  }
  @keyframes cardIn{
    from{ opacity:0; transform: translateY(24px) scale(.96); }
    to{ opacity:1; transform: translateY(0) scale(1); }
  }
  .card.flash-ok{ animation: glowOk .7s var(--ease); }
  .card.flash-bad{ animation: glowBad .5s var(--ease); }
  @keyframes glowOk{
    0%{ box-shadow: 0 40px 100px -30px #00000090; }
    35%{ box-shadow: 0 0 0 3px #34D39955, 0 40px 100px -30px #00000090; }
    100%{ box-shadow: 0 40px 100px -30px #00000090; }
  }
  @keyframes glowBad{
    0%{ box-shadow: 0 40px 100px -30px #00000090; }
    35%{ box-shadow: 0 0 0 3px #FF6B6B55, 0 40px 100px -30px #00000090; }
    100%{ box-shadow: 0 40px 100px -30px #00000090; }
  }

  .icon-badge{
    width:64px; height:64px; margin:0 auto 20px;
    border-radius:18px;
    background: linear-gradient(135deg, #7C5CFC33, #45E0D022);
    border:1px solid var(--border);
    display:flex; align-items:center; justify-content:center;
    animation: badgeFloat 3.2s ease-in-out infinite;
  }
  @keyframes badgeFloat{
    0%,100%{ transform: translateY(0) rotate(0deg); }
    50%{ transform: translateY(-6px) rotate(-3deg); }
  }
  .icon-badge svg{ width:30px; height:30px; }

  h1{
    font-family:'Space Grotesk', sans-serif; font-size:22px; font-weight:600; margin:0 0 8px;
  }
  .sub{ color:var(--text-muted); font-size:14px; line-height:1.6; margin:0 0 30px; }
  .sub b{ color: var(--text); font-weight:600; }

  /* ---------- OTP boxes ---------- */
  .otp-stage{
    position: relative;
    min-height: 78px;
    display:flex; align-items:center; justify-content:center;
    margin-bottom: 22px;
  }
  .otp-wrap{
    display:flex; gap:10px; justify-content:center;
  }
  .otp-box{
    width:48px; height:60px;
    background: var(--surface-2);
    border:1.5px solid var(--border);
    border-radius:13px;
    color:var(--text);
    font-family:'Space Grotesk', sans-serif;
    font-size:24px; font-weight:600; text-align:center;
    outline:none;
    caret-color: var(--violet);
    transition: border-color .2s var(--ease), box-shadow .2s var(--ease), background .2s var(--ease);
  }
  /* Kondisi "sembunyi lalu terbang masuk" cuma aktif lewat class .enter,
     dan class ini dilepas via JS begitu animasinya selesai — jadi rule
     lain (seperti .filled) nggak akan pernah nabrak/mematikan animasi ini lagi. */
  .otp-box.enter{
    opacity:0; transform: translateY(46px) rotate(-10deg) scale(.55);
    animation: boxFlyIn .55s var(--bouncy) forwards;
  }
  .otp-box.enter:nth-child(1){ animation-delay: .05s; }
  .otp-box.enter:nth-child(2){ animation-delay: .11s; }
  .otp-box.enter:nth-child(3){ animation-delay: .17s; }
  .otp-box.enter:nth-child(4){ animation-delay: .23s; }
  .otp-box.enter:nth-child(5){ animation-delay: .29s; }
  .otp-box.enter:nth-child(6){ animation-delay: .35s; }
  @keyframes boxFlyIn{
    to{ opacity:1; transform: translateY(0) rotate(0deg) scale(1); }
  }
  .otp-box:focus{
    border-color: var(--violet);
    box-shadow: 0 0 0 4px var(--violet-soft);
    background:#141C2E;
  }
  .otp-box.filled{ border-color:#3A4560; }
  .otp-box.pop{ animation: popWiggle .38s var(--bouncy); }
  @keyframes popWiggle{
    0%{ transform: scale(1) rotate(0deg); }
    35%{ transform: scale(1.18) rotate(-6deg); }
    65%{ transform: scale(1.05) rotate(4deg); }
    100%{ transform: scale(1) rotate(0deg); }
  }
  .otp-wrap.shake .otp-box{ animation: shakeBox .45s var(--ease); border-color: var(--danger); }
  @keyframes shakeBox{
    0%,100%{ transform: translateX(0); }
    20%{ transform: translateX(-8px); }
    40%{ transform: translateX(8px); }
    60%{ transform: translateX(-5px); }
    80%{ transform: translateX(5px); }
  }

  /* ---------- Process box: kotak gabungan dgn bingkai spin -> hijau/merah ---------- */
  .process-box{
    position:absolute; left:50%; top:50%;
    width:48px; height:60px;
    margin:-30px 0 0 -24px;
    border-radius:13px;
    background: var(--bg-2);
    display:flex; align-items:center; justify-content:center;
    opacity:0; transform: scale(.7);
    transition: opacity .3s var(--ease), transform .4s var(--bouncy);
    z-index:1;
  }
  .process-box::before{
    content:''; position:absolute; inset:-3px; border-radius:16px; z-index:-1;
    background: conic-gradient(from 0deg, var(--violet), var(--cyan) 50%, var(--violet) 100%);
    animation: spinBorder 0.9s linear infinite;
    transition: background .25s var(--ease);
  }
  .process-box.show{ opacity:1; transform: scale(1); }
  .process-box.show.pulse{ animation: mergePulse .4s var(--bouncy); }
  @keyframes mergePulse{
    0%{ transform: scale(.7); }
    55%{ transform: scale(1.14); }
    100%{ transform: scale(1); }
  }
  @keyframes spinBorder{ to{ transform: rotate(360deg); } }
  .process-box.success::before{ background: var(--success); animation:none; }
  .process-box.error::before{ background: var(--danger); animation:none; }
  .process-box.error{ animation: shakeBox .45s var(--ease); }

  .result-icon{ width:24px; height:24px; }
  .result-icon .tick{
    fill:none; stroke:#0A0E16; stroke-width:4; stroke-linecap:round; stroke-linejoin:round;
    stroke-dasharray: 30; stroke-dashoffset:30;
    animation: draw .3s var(--ease) .12s forwards;
  }
  @keyframes draw{ to{ stroke-dashoffset:0; } }
  .result-icon .cross{ stroke:#0A0E16; stroke-width:4; stroke-linecap:round; }

  .status-text{
    min-height: 20px; font-size:13.5px; margin-bottom: 18px;
    color: var(--text-muted); transition: color .2s;
  }
  .status-text.err{ color: var(--danger); }
  .status-text.ok{ color: var(--cyan); }

  .verify-btn{
    width:100%; padding:15px 18px; border:none; border-radius:12px;
    background: linear-gradient(135deg, var(--violet), #5A3FE0);
    color:#fff; font-family:'Inter',sans-serif; font-weight:600; font-size:14.5px;
    cursor:pointer; position:relative; overflow:hidden;
    box-shadow: 0 10px 24px -10px #7C5CFC80;
    transition: transform .18s var(--ease), box-shadow .18s var(--ease), opacity .2s;
  }
  .verify-btn:hover{ transform: translateY(-2px); box-shadow: 0 16px 30px -10px #7C5CFCa0; }
  .verify-btn:disabled{ opacity:.45; cursor:not-allowed; transform:none; box-shadow:none; }

  .resend{ margin-top:20px; font-size:13.5px; color:var(--text-muted); }
  .resend button{
    background:none; border:none; color:var(--cyan); font-weight:600; cursor:pointer;
    font-size:13.5px; padding:0;
  }
  .resend button:disabled{ color:#4A5270; cursor:not-allowed; }

  .back-link{ display:block; margin-top:16px; font-size:13px; color:var(--text-muted); text-decoration:none; }
  .back-link:hover{ color: var(--cyan); }

  .toast{
    position: fixed; left:50%; bottom: 28px; transform: translateX(-50%) translateY(20px);
    background: var(--surface-2); border:1px solid var(--border); color: var(--text);
    padding: 12px 18px; border-radius: 12px; font-size: 13.5px;
    display:flex; align-items:center; gap:10px;
    opacity:0; pointer-events:none; transition: all .35s var(--bouncy);
    z-index: 10; box-shadow: 0 20px 40px -20px #000;
  }
  .toast.show{ opacity:1; transform: translateX(-50%) translateY(0); }
  .toast .tick{
    width:18px; height:18px; border-radius:50%; background: var(--cyan);
    display:flex; align-items:center; justify-content:center; color:#0A0E16; font-size:12px; flex:none;
  }
  .particle{ position:fixed; z-index:9; pointer-events:none; border-radius:50%; animation: pop .8s var(--ease) forwards; }
  @keyframes pop{
    0%{ transform: translate(0,0) scale(1); opacity:1; }
    100%{ transform: translate(var(--dx), var(--dy)) scale(0); opacity:0; }
  }

  @media (max-width:420px){
    .otp-box{ width:40px; height:52px; font-size:20px; }
    .otp-wrap{ gap:7px; }
    .card{ padding:34px 20px 30px; }
  }
  @media (prefers-reduced-motion: reduce){
    *{ animation-duration: .01ms !important; }
  }
</style>
</head>
<body>

<div class="backdrop"><div class="orb a"></div><div class="orb b"></div></div>

<div class="stage">
  <div class="card">
    <div class="icon-badge">
      <svg viewBox="0 0 24 24" fill="none"><path d="M3 6l9 6 9-6M4 5h16a1 1 0 011 1v12a1 1 0 01-1 1H4a1 1 0 01-1-1V6a1 1 0 011-1z" stroke="url(#g1)" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"/><defs><linearGradient id="g1" x1="0" y1="0" x2="24" y2="24"><stop stop-color="#7C5CFC"/><stop offset="1" stop-color="#45E0D0"/></linearGradient></defs></svg>
    </div>
    <h1>Verifikasi Email Kamu</h1>
    <p class="sub">Kode 6 digit sudah dikirim ke <b id="emailTarget">n***@gmail.com</b>. Masukkan di bawah ini.</p>

    <div class="otp-stage">
      <div class="otp-wrap" id="otpWrap">
        <input class="otp-box enter" type="text" inputmode="numeric" maxlength="1" autocomplete="one-time-code">
        <input class="otp-box enter" type="text" inputmode="numeric" maxlength="1">
        <input class="otp-box enter" type="text" inputmode="numeric" maxlength="1">
        <input class="otp-box enter" type="text" inputmode="numeric" maxlength="1">
        <input class="otp-box enter" type="text" inputmode="numeric" maxlength="1">
        <input class="otp-box enter" type="text" inputmode="numeric" maxlength="1">
      </div>
      <div class="process-box" id="processBox">
        <svg class="result-icon" id="okIcon" viewBox="0 0 24 24" style="display:none">
          <path class="tick" d="M5 12.5 L10 17.5 L19 6.5"/>
        </svg>
        <svg class="result-icon" id="badIcon" viewBox="0 0 24 24" style="display:none">
          <line class="cross" x1="6" y1="6" x2="18" y2="18"/>
          <line class="cross" x1="18" y1="6" x2="6" y2="18"/>
        </svg>
      </div>
    </div>

    <div class="status-text" id="statusText">&nbsp;</div>

    <button class="verify-btn" id="verifyBtn" disabled>Verifikasi</button>

    <div class="resend">
      Nggak dapat kode? <button id="resendBtn" disabled>Kirim ulang (<span id="countdown">60</span>s)</button>
    </div>
    <a href="#" class="back-link">Ganti alamat email</a>
  </div>
</div>

<div class="toast" id="toast"><span class="tick">✓</span><span id="toastMsg">Berhasil</span></div>

<script>
  const otpWrap = document.getElementById('otpWrap');
  const boxes = Array.from(document.querySelectorAll('.otp-box'));
  const verifyBtn = document.getElementById('verifyBtn');
  const processBox = document.getElementById('processBox');
  const cardEl = document.querySelector('.card');
  const okIcon = document.getElementById('okIcon');
  const badIcon = document.getElementById('badIcon');
  const statusText = document.getElementById('statusText');
  const resendBtn = document.getElementById('resendBtn');
  const countdownEl = document.getElementById('countdown');

  const CORRECT_CODE = '123456'; // --- ganti logic ini dengan panggilan API verifikasi email kamu ---

  // Lepas class 'enter' PER KOTAK begitu animasi terbang-masuknya sendiri kelar
  // (lebih akurat daripada nebak total durasi), supaya nggak ada jeda di mana
  // kotak yang udah selesai animasi tapi belum "dibersihkan" bentrok kalau diketik duluan.
  boxes.forEach(b => b.addEventListener('animationend', ()=> b.classList.remove('enter')));
  // Jaring pengaman kalau animationend nggak sempat kepanggil (mis. device tertentu)
  setTimeout(()=> boxes.forEach(b => b.classList.remove('enter')), 950);

  function currentCode(){ return boxes.map(b => b.value).join(''); }

  function updateVerifyState(){
    verifyBtn.disabled = currentCode().length !== 6;
  }

  boxes.forEach((box, i)=>{
    box.addEventListener('input', ()=>{
      box.classList.remove('enter');
      box.value = box.value.replace(/[^0-9]/g, '').slice(0,1);
      if(box.value){
        box.classList.add('filled','pop');
        setTimeout(()=> box.classList.remove('pop'), 380);
        if(i < boxes.length - 1){ boxes[i+1].focus(); }
        else { box.blur(); attemptVerify(); }
      } else {
        box.classList.remove('filled');
      }
      updateVerifyState();
    });

    box.addEventListener('keydown', (e)=>{
      if(e.key === 'Backspace' && !box.value && i > 0){
        boxes[i-1].focus();
        boxes[i-1].value = '';
        boxes[i-1].classList.remove('filled');
        updateVerifyState();
      }
      if(e.key === 'ArrowLeft' && i > 0) boxes[i-1].focus();
      if(e.key === 'ArrowRight' && i < boxes.length-1) boxes[i+1].focus();
    });

    box.addEventListener('paste', (e)=>{
      e.preventDefault();
      const digits = (e.clipboardData.getData('text').match(/[0-9]/g) || []).slice(0,6);
      digits.forEach((d, idx)=>{
        setTimeout(()=>{
          if(!boxes[idx]) return;
          boxes[idx].classList.remove('enter');
          boxes[idx].value = d;
          boxes[idx].classList.add('filled','pop');
          setTimeout(()=> boxes[idx].classList.remove('pop'), 380);
          if(idx === digits.length - 1){
            (boxes[idx+1] || boxes[idx]).focus();
            updateVerifyState();
            if(digits.length === 6) attemptVerify();
          }
        }, idx * 70);
      });
    });
  });

  verifyBtn.addEventListener('click', ()=> attemptVerify());

  function attemptVerify(){
    if(currentCode().length !== 6) return;
    verifyBtn.disabled = true;
    statusText.textContent = '';
    statusText.className = 'status-text';
    convergeBoxes();
  }

  function convergeBoxes(){
    const wrapRect = otpWrap.getBoundingClientRect();
    const centerX = wrapRect.left + wrapRect.width/2;
    const centerY = wrapRect.top + wrapRect.height/2;
    // Kotak2 bergerak ke tengah TANPA mengecil (ukuran tetap), cuma geser + muter dikit,
    // jadi kerasa "ngumpul jadi satu" bukan "menghilang".
    boxes.forEach((box, i)=>{
      const r = box.getBoundingClientRect();
      const bx = r.left + r.width/2, by = r.top + r.height/2;
      const dx = centerX - bx, dy = centerY - by;
      box.style.zIndex = 10 + i;
      box.style.transition = `transform .5s var(--bouncy) ${i*35}ms`;
      box.style.transform = `translate(${dx}px, ${dy}px) rotate(${(i-2.5)*12}deg)`;
    });

    // Begitu semua kotak sampai numpuk di tengah, langsung ganti jadi process-box
    // (posisinya persis sama) supaya transisinya mulus, nggak ada jeda "kosong".
    setTimeout(()=>{
      boxes.forEach(b=> b.style.opacity = '0');
      processBox.classList.add('show','pulse');
      statusText.textContent = 'Memverifikasi kode...';
    }, 480);

    setTimeout(()=> checkResult(), 480 + 1300);
  }

  function checkResult(){
    const ok = currentCode() === CORRECT_CODE;
    processBox.classList.remove('pulse');
    if(ok){
      okIcon.style.display = 'block';
      processBox.classList.add('success');
      statusText.textContent = 'Email berhasil diverifikasi!';
      statusText.className = 'status-text ok';
      cardEl.classList.add('flash-ok');
      burstConfetti();
      verifyBtn.textContent = 'Lanjut ke Dashboard';
      verifyBtn.disabled = false;
    } else {
      badIcon.style.display = 'block';
      processBox.classList.add('error');
      statusText.textContent = 'Kode salah, coba lagi.';
      statusText.className = 'status-text err';
      cardEl.classList.add('flash-bad');
      setTimeout(resetBoxes, 1300);
    }
  }

  function resetBoxes(){
    processBox.classList.remove('show','success','error','pulse');
    cardEl.classList.remove('flash-bad');
    badIcon.style.display = 'none';
    okIcon.style.display = 'none';
    otpWrap.classList.add('shake');
    boxes.forEach((box, i)=>{
      box.value = '';
      box.classList.remove('filled');
      box.style.zIndex = '';
      box.style.transition = 'none';
      box.style.transform = 'translateY(46px) rotate(-10deg) scale(.55)';
      box.style.opacity = '0';
      requestAnimationFrame(()=>{
        box.style.transition = `transform .5s var(--bouncy) ${i*45}ms, opacity .4s ease ${i*45}ms`;
        box.style.transform = 'translateY(0) rotate(0deg) scale(1)';
        box.style.opacity = '1';
      });
    });
    setTimeout(()=>{
      otpWrap.classList.remove('shake');
      boxes[0].focus();
      statusText.textContent = '';
      updateVerifyState();
    }, 650);
  }

  function showToast(msg){
    const toast = document.getElementById('toast');
    document.getElementById('toastMsg').textContent = msg;
    toast.classList.add('show');
    setTimeout(()=> toast.classList.remove('show'), 2600);
  }

  function burstConfetti(){
    const colors = ['#7C5CFC','#45E0D0','#FF6B9D'];
    const originX = window.innerWidth/2, originY = window.innerHeight/2 - 40;
    for(let i=0;i<22;i++){
      const p = document.createElement('div');
      p.className = 'particle';
      const size = 5 + Math.random()*5;
      p.style.width = p.style.height = size + 'px';
      p.style.left = originX + 'px';
      p.style.top = originY + 'px';
      p.style.background = colors[i % colors.length];
      const angle = Math.random()*Math.PI*2;
      const dist = 60 + Math.random()*90;
      p.style.setProperty('--dx', Math.cos(angle)*dist + 'px');
      p.style.setProperty('--dy', Math.sin(angle)*dist + 'px');
      document.body.appendChild(p);
      setTimeout(()=> p.remove(), 850);
    }
  }

  /* ---------- Resend countdown ---------- */
  let secondsLeft = 60;
  const timer = setInterval(()=>{
    secondsLeft--;
    countdownEl.textContent = secondsLeft;
    if(secondsLeft <= 0){
      clearInterval(timer);
      resendBtn.disabled = false;
      resendBtn.textContent = 'Kirim ulang kode';
    }
  }, 1000);

  resendBtn.addEventListener('click', ()=>{
    if(resendBtn.disabled) return;
    // --- ganti dengan panggilan API kirim ulang kode kamu ---
    showToast('Kode baru sudah dikirim!');
    resendBtn.disabled = true;
    secondsLeft = 60;
    resendBtn.innerHTML = 'Kirim ulang (<span id="countdown">60</span>s)';
    const newCountdownEl = document.getElementById('countdown');
    const t2 = setInterval(()=>{
      secondsLeft--;
      newCountdownEl.textContent = secondsLeft;
      if(secondsLeft <= 0){
        clearInterval(t2);
        resendBtn.disabled = false;
        resendBtn.textContent = 'Kirim ulang kode';
      }
    }, 1000);
  });

  boxes[0].focus();
</script>

</body>
</html>
