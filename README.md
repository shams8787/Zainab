<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>عيد ميلاد سعيد زينب حسن 🎂</title>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/fontsource/fonts/dancing-script@latest/arabic-400-normal.css">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/fontsource/fonts/amiri@latest/arabic-400-normal.css">
<style>
  * { margin: 0; padding: 0; box-sizing: border-box; }
  
  body {
    font-family: 'Amiri', serif;
    background: linear-gradient(135deg, #1a0033 0%, #330066 30%, #660066 60%, #cc0066 100%);
    min-height: 100vh;
    overflow-x: hidden;
    color: white;
    position: relative;
  }
  
  /* Stars background */
  .stars {
    position: fixed;
    top: 0; left: 0;
    width: 100%; height: 100%;
    pointer-events: none;
    z-index: 0;
  }
  
  .star {
    position: absolute;
    background: white;
    border-radius: 50%;
    animation: twinkle 3s infinite;
  }
  
  @keyframes twinkle {
    0%, 100% { opacity: 0.3; transform: scale(1); }
    50% { opacity: 1; transform: scale(1.5); }
  }
  
  /* Balloons */
  .balloon {
    position: fixed;
    width: 50px;
    height: 65px;
    border-radius: 50%;
    animation: float 8s ease-in-out infinite;
    z-index: 1;
  }
  
  .balloon::after {
    content: '';
    position: absolute;
    bottom: -40px;
    left: 50%;
    width: 1px;
    height: 40px;
    background: rgba(255,255,255,0.5);
  }
  
  @keyframes float {
    0%, 100% { transform: translateY(0) rotate(-5deg); }
    50% { transform: translateY(-30px) rotate(5deg); }
  }
  
  /* Main container */
  .container {
    position: relative;
    z-index: 10;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding: 40px 20px;
    text-align: center;
  }
  
  /* Title */
  .title {
    font-family: 'Dancing Script', cursive;
    font-size: clamp(3rem, 8vw, 6rem);
    background: linear-gradient(45deg, #ffd700, #ff69b4, #ffd700, #ff69b4);
    background-size: 300% 300%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    animation: shimmer 3s ease-in-out infinite;
    margin-bottom: 10px;
    text-shadow: 0 0 30px rgba(255, 215, 0, 0.5);
  }
  
  @keyframes shimmer {
    0%, 100% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
  }
  
  .arabic-title {
    font-family: 'Amiri', serif;
    font-size: clamp(1.5rem, 4vw, 2.5rem);
    color: #ffd700;
    margin-bottom: 40px;
    text-shadow: 0 0 20px rgba(255, 215, 0, 0.6);
    animation: pulse 2s ease-in-out infinite;
  }
  
  @keyframes pulse {
    0%, 100% { transform: scale(1); }
    50% { transform: scale(1.05); }
  }
  
  /* Cake */
  .cake-wrapper {
    position: relative;
    cursor: pointer;
    transition: transform 0.3s;
    margin: 20px 0;
  }
  
  .cake-wrapper:hover {
    transform: scale(1.05);
  }
  
  .cake {
    position: relative;
    width: 300px;
    height: 280px;
  }
  
  /* Cake layers */
  .cake-layer {
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
    border-radius: 15px;
    box-shadow: 0 5px 20px rgba(0,0,0,0.3);
  }
  
  .layer-bottom {
    bottom: 0;
    width: 280px;
    height: 90px;
    background: linear-gradient(180deg, #ff69b4 0%, #ff1493 100%);
    border-radius: 15px 15px 20px 20px;
  }
  
  .layer-bottom::before {
    content: '';
    position: absolute;
    top: -10px;
    left: 0;
    right: 0;
    height: 20px;
    background: linear-gradient(180deg, #fff 0%, #ffb6d9 100%);
    border-radius: 50% 50% 0 0 / 100% 100% 0 0;
  }
  
  .layer-middle {
    bottom: 85px;
    width: 220px;
    height: 75px;
    background: linear-gradient(180deg, #ff1493 0%, #c71585 100%);
  }
  
  .layer-middle::before {
    content: '';
    position: absolute;
    top: -10px;
    left: 0;
    right: 0;
    height: 20px;
    background: linear-gradient(180deg, #fff 0%, #ff69b4 100%);
    border-radius: 50% 50% 0 0 / 100% 100% 0 0;
  }
  
  .layer-top {
    bottom: 155px;
    width: 160px;
    height: 65px;
    background: linear-gradient(180deg, #ff69b4 0%, #ff1493 100%);
  }
  
  .layer-top::before {
    content: '';
    position: absolute;
    top: -10px;
    left: 0;
    right: 0;
    height: 20px;
    background: linear-gradient(180deg, #fff 0%, #ffb6d9 100%);
    border-radius: 50% 50% 0 0 / 100% 100% 0 0;
  }
  
  /* Decorations on cake */
  .decoration {
    position: absolute;
    width: 8px;
    height: 8px;
    background: #ffd700;
    border-radius: 50%;
    box-shadow: 0 0 10px #ffd700;
  }
  
  /* Candles */
  .candles {
    position: absolute;
    bottom: 215px;
    left: 50%;
    transform: translateX(-50%);
    display: flex;
    gap: 25px;
  }
  
  .candle {
    position: relative;
    width: 10px;
    height: 40px;
    background: linear-gradient(180deg, #fff 0%, #ffd700 50%, #ff69b4 100%);
    border-radius: 3px;
  }
  
  .flame {
    position: absolute;
    bottom: 100%;
    left: 50%;
    transform: translateX(-50%);
    width: 14px;
    height: 22px;
    background: radial-gradient(circle at 50% 70%, #fff 0%, #ffeb3b 30%, #ff9800 60%, #ff5722 100%);
    border-radius: 50% 50% 20% 20%;
    animation: flicker 0.3s ease-in-out infinite alternate;
    box-shadow: 0 0 20px #ff9800, 0 0 40px #ff5722;
    transition: opacity 0.5s, transform 0.5s;
  }
  
  .flame::after {
    content: '';
    position: absolute;
    bottom: -3px;
    left: 50%;
    transform: translateX(-50%);
    width: 6px;
    height: 6px;
    background: #2196f3;
    border-radius: 50%;
    opacity: 0.7;
  }
  
  @keyframes flicker {
    0% { transform: translateX(-50%) scale(1) rotate(-2deg); }
    100% { transform: translateX(-50%) scale(1.1) rotate(2deg); }
  }
  
  .flame.out {
    opacity: 0;
    transform: translateX(-50%) scale(0) rotate(0);
  }
  
  /* Smoke */
  .smoke {
    position: absolute;
    bottom: 100%;
    left: 50%;
    transform: translateX(-50%);
    width: 10px;
    height: 10px;
    background: rgba(200,200,200,0.6);
    border-radius: 50%;
    opacity: 0;
    pointer-events: none;
  }
  
  .smoke.active {
    animation: smokeRise 2s ease-out forwards;
  }
  
  @keyframes smokeRise {
    0% { opacity: 0.8; transform: translateX(-50%) translateY(0) scale(0.5); }
    100% { opacity: 0; transform: translateX(-50%) translateY(-80px) scale(2); }
  }
  
  .instruction {
    margin-top: 30px;
    font-size: 1.3rem;
    color: #ffd700;
    animation: bounce 1.5s ease-in-out infinite;
    font-family: 'Amiri', serif;
  }
  
  @keyframes bounce {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-10px); }
  }
  
  /* Clapping hands */
  .clap-container {
    position: fixed;
    top: 0; left: 0;
    width: 100%; height: 100%;
    pointer-events: none;
    z-index: 100;
    display: none;
  }
  
  .clap-container.active {
    display: block;
  }
  
  .clap-hand {
    position: absolute;
    font-size: 4rem;
    animation: clapAnim 1s ease-in-out infinite;
    filter: drop-shadow(0 0 10px rgba(255, 215, 0, 0.8));
  }
  
  @keyframes clapAnim {
    0%, 100% { transform: scale(1) rotate(-10deg); }
    50% { transform: scale(1.3) rotate(10deg); }
  }
  
  /* Confetti */
  .confetti {
    position: fixed;
    width: 10px;
    height: 10px;
    top: -10px;
    z-index: 50;
    animation: confettiFall 4s linear forwards;
  }
  
  @keyframes confettiFall {
    0% { transform: translateY(0) rotate(0deg); opacity: 1; }
    100% { transform: translateY(100vh) rotate(720deg); opacity: 0; }
  }
  
  /* Message after candles blown */
  .wish-message {
    margin-top: 30px;
    font-family: 'Dancing Script', cursive;
    font-size: clamp(2rem, 5vw, 3.5rem);
    color: #fff;
    opacity: 0;
    transform: translateY(30px);
    transition: opacity 1s, transform 1s;
    text-shadow: 0 0 20px rgba(255, 215, 0, 0.8);
  }
  
  .wish-message.show {
    opacity: 1;
    transform: translateY(0);
  }
  
  .wish-message .name {
    color: #ffd700;
    font-size: 1.3em;
    display: block;
    margin-top: 10px;
  }
  
  /* Music button */
  .music-btn {
    position: fixed;
    top: 20px;
    left: 20px;
    width: 50px;
    height: 50px;
    border-radius: 50%;
    background: linear-gradient(135deg, #ff69b4, #ff1493);
    border: 2px solid #ffd700;
    color: white;
    font-size: 1.5rem;
    cursor: pointer;
    z-index: 200;
    display: flex;
    align-items: center;
    justify-content: center;
    box-shadow: 0 0 20px rgba(255, 105, 180, 0.6);
    transition: transform 0.3s;
  }
  
  .music-btn:hover {
    transform: scale(1.1);
  }
  
  .music-btn.playing {
    animation: musicPulse 1s ease-in-out infinite;
  }
  
  @keyframes musicPulse {
    0%, 100% { box-shadow: 0 0 20px rgba(255, 105, 180, 0.6); }
    50% { box-shadow: 0 0 40px rgba(255, 215, 0, 0.9); }
  }
  
  /* Hearts floating */
  .heart {
    position: fixed;
    font-size: 2rem;
    animation: heartFloat 4s ease-in-out forwards;
    pointer-events: none;
    z-index: 50;
  }
  
  @keyframes heartFloat {
    0% { transform: translateY(0) scale(0); opacity: 0; }
    20% { opacity: 1; transform: translateY(-20px) scale(1); }
    100% { transform: translateY(-300px) scale(1.5); opacity: 0; }
  }
  
  @media (max-width: 600px) {
    .cake { transform: scale(0.85); }
    .balloon { width: 35px; height: 45px; }
  }
</style>
</head>
<body>

<div class="stars" id="stars"></div>

<button class="music-btn" id="musicBtn" title="تشغيل الموسيقى">🎵</button>

<div class="container">
  <h1 class="title">Happy Birthday</h1>
  <p class="arabic-title">✨ عيد ميلاد سعيد ✨</p>
  
  <div class="cake-wrapper" id="cakeWrapper">
    <div class="cake">
      <!-- Candles -->
      <div class="candles" id="candles">
        <div class="candle"><div class="flame"></div><div class="smoke"></div></div>
        <div class="candle"><div class="flame"></div><div class="smoke"></div></div>
        <div class="candle"><div class="flame"></div><div class="smoke"></div></div>
        <div class="candle"><div class="flame"></div><div class="smoke"></div></div>
        <div class="candle"><div class="flame"></div><div class="smoke"></div></div>
      </div>
      
      <!-- Cake layers -->
      <div class="cake-layer layer-top"></div>
      <div class="cake-layer layer-middle"></div>
      <div class="cake-layer layer-bottom"></div>
      
      <!-- Decorations -->
      <div class="decoration" style="bottom: 40px; left: 30px;"></div>
      <div class="decoration" style="bottom: 60px; left: 80px;"></div>
      <div class="decoration" style="bottom: 40px; left: 130px;"></div>
      <div class="decoration" style="bottom: 60px; left: 180px;"></div>
      <div class="decoration" style="bottom: 40px; left: 230px;"></div>
    </div>
  </div>
  
  <p class="instruction" id="instruction">🕯️ اضغط على الكيكة لإطفاء الشموع 🕯️</p>
  
  <div class="wish-message" id="wishMessage">
    Happy Birthday to You!
    <span class="name">زينب حسن 💖</span>
  </div>
</div>

<div class="clap-container" id="clapContainer"></div>

<script>
  // Create stars
  const starsContainer = document.getElementById('stars');
  for (let i = 0; i < 80; i++) {
    const star = document.createElement('div');
    star.className = 'star';
    const size = Math.random() * 3 + 1;
    star.style.width = size + 'px';
    star.style.height = size + 'px';
    star.style.top = Math.random() * 100 + '%';
    star.style.left = Math.random() * 100 + '%';
    star.style.animationDelay = Math.random() * 3 + 's';
    starsContainer.appendChild(star);
  }
  
  // Create balloons
  const colors = ['#ff69b4', '#ffd700', '#ff1493', '#9370db', '#00ced1', '#ff6347'];
  for (let i = 0; i < 10; i++) {
    const balloon = document.createElement('div');
    balloon.className = 'balloon';
    balloon.style.background = `radial-gradient(circle at 30% 30%, ${colors[i % colors.length]}, ${colors[(i+2) % colors.length]})`;
    balloon.style.left = Math.random() * 100 + '%';
    balloon.style.top = (Math.random() * 60 + 20) + '%';
    balloon.style.animationDelay = Math.random() * 5 + 's';
    balloon.style.animationDuration = (Math.random() * 4 + 6) + 's';
    document.body.appendChild(balloon);
  }
  
  // Happy Birthday melody using Web Audio API
  let audioCtx = null;
  let isPlaying = false;
  let melodyTimeout = [];
  
  // Happy Birthday notes (frequencies in Hz) and durations
  const melody = [
    // Happy birthday to you
    { note: 'C4', dur: 0.3 }, { note: 'C4', dur: 0.3 }, { note: 'D4', dur: 0.6 },
    { note: 'C4', dur: 0.6 }, { note: 'F4', dur: 0.6 }, { note: 'E4', dur: 1.2 },
    // Happy birthday to you
    { note: 'C4', dur: 0.3 }, { note: 'C4', dur: 0.3 }, { note: 'D4', dur: 0.6 },
    { note: 'C4', dur: 0.6 }, { note: 'G4', dur: 0.6 }, { note: 'F4', dur: 1.2 },
    // Happy birthday dear Zainab
    { note: 'C4', dur: 0.3 }, { note: 'C4', dur: 0.3 }, { note: 'C5', dur: 0.6 },
    { note: 'A4', dur: 0.6 }, { note: 'F4', dur: 0.6 }, { note: 'E4', dur: 0.6 }, { note: 'D4', dur: 1.2 },
    // Happy birthday to you
    { note: 'Bb4', dur: 0.3 }, { note: 'Bb4', dur: 0.3 }, { note: 'A4', dur: 0.6 },
    { note: 'F4', dur: 0.6 }, { note: 'G4', dur: 0.6 }, { note: 'F4', dur: 1.5 }
  ];
  
  const noteFreqs = {
    'C4': 261.63, 'D4': 293.66, 'E4': 329.63, 'F4': 349.23,
    'G4': 392.00, 'A4': 440.00, 'Bb4': 466.16, 'B4': 493.88,
    'C5': 523.25
  };
  
  function playNote(freq, startTime, duration) {
    const osc = audioCtx.createOscillator();
    const gain = audioCtx.createGain();
    
    osc.type = 'sine';
    osc.frequency.value = freq;
    
    // Add harmonics for richer sound
    const osc2 = audioCtx.createOscillator();
    const gain2 = audioCtx.createGain();
    osc2.type = 'triangle';
    osc2.frequency.value = freq * 2;
    gain2.gain.value = 0.1;
    
    gain.gain.setValueAtTime(0, startTime);
    gain.gain.linearRampToValueAtTime(0.3, startTime + 0.02);
    gain.gain.linearRampToValueAtTime(0.25, startTime + duration * 0.7);
    gain.gain.linearRampToValueAtTime(0, startTime + duration);
    
    gain2.gain.setValueAtTime(0, startTime);
    gain2.gain.linearRampToValueAtTime(0.08, startTime + 0.02);
    gain2.gain.linearRampToValueAtTime(0, startTime + duration);
    
    osc.connect(gain);
    osc2.connect(gain2);
    gain.connect(audioCtx.destination);
    gain2.connect(audioCtx.destination);
    
    osc.start(startTime);
    osc.stop(startTime + duration);
    osc2.start(startTime);
    osc2.stop(startTime + duration);
  }
  
  function playMelody() {
    if (!audioCtx) audioCtx = new (window.AudioContext || window.webkitAudioContext)();
    
    let time = audioCtx.currentTime + 0.1;
    melody.forEach(n => {
      playNote(noteFreqs[n.note], time, n.dur);
      time += n.dur;
    });
    
    return time - audioCtx.currentTime;
  }
  
  const musicBtn = document.getElementById('musicBtn');
  musicBtn.addEventListener('click', () => {
    if (!isPlaying) {
      const duration = playMelody();
      isPlaying = true;
      musicBtn.classList.add('playing');
      musicBtn.textContent = '🎶';
      
      // Loop the melody
      const loopInterval = setInterval(() => {
        if (isPlaying) {
          playMelody();
        } else {
          clearInterval(loopInterval);
        }
      }, duration * 1000);
      melodyTimeout.push(loopInterval);
    } else {
      isPlaying = false;
      musicBtn.classList.remove('playing');
      musicBtn.textContent = '🎵';
      if (audioCtx) audioCtx.close();
      audioCtx = null;
    }
  });
  
  // Auto-play on first interaction
  let autoPlayed = false;
  document.addEventListener('click', () => {
    if (!autoPlayed && !isPlaying) {
      autoPlayed = true;
      musicBtn.click();
    }
  }, { once: false });
  
  // Cake click - blow out candles
  const cakeWrapper = document.getElementById('cakeWrapper');
  const flames = document.querySelectorAll('.flame');
  const smokes = document.querySelectorAll('.smoke');
  const instruction = document.getElementById('instruction');
  const wishMessage = document.getElementById('wishMessage');
  const clapContainer = document.getElementById('clapContainer');
  let candlesBlown = false;
  
  cakeWrapper.addEventListener('click', () => {
    if (candlesBlown) return;
    candlesBlown = true;
    
    // Blow out flames one by one
    flames.forEach((flame, i) => {
      setTimeout(() => {
        flame.classList.add('out');
        smokes[i].classList.add('active');
      }, i * 200);
    });
    
    // After all candles out
    setTimeout(() => {
      instruction.style.display = 'none';
      wishMessage.classList.add('show');
      clapContainer.classList.add('active');
      startClapping();
      launchConfetti();
      launchHearts();
    }, flames.length * 200 + 500);
  });
  
  // Clapping hands animation
  function startClapping() {
    const hands = ['👏', '🙌', '👏', '🙌', '👏'];
    const positions = [
      { top: '15%', left: '10%' },
      { top: '20%', right: '10%' },
      { top: '60%', left: '5%' },
      { top: '65%', right: '8%' },
      { top: '80%', left: '15%' },
      { top: '80%', right: '12%' },
      { top: '40%', left: '3%' },
      { top: '40%', right: '3%' }
    ];
    
    positions.forEach((pos, i) => {
      const hand = document.createElement('div');
      hand.className = 'clap-hand';
      hand.textContent = hands[i % hands.length];
      Object.keys(pos).forEach(k => hand.style[k] = pos[k]);
      hand.style.animationDelay = (i * 0.15) + 's';
      clapContainer.appendChild(hand);
    });
  }
  
  // Confetti
  function launchConfetti() {
    const confettiColors = ['#ff69b4', '#ffd700', '#ff1493', '#9370db', '#00ced1', '#ff6347', '#7fff00'];
    const shapes = ['circle', 'square'];
    
    for (let i = 0; i < 80; i++) {
      setTimeout(() => {
        const confetti = document.createElement('div');
        confetti.className = 'confetti';
        confetti.style.left = Math.random() * 100 + '%';
        confetti.style.background = confettiColors[Math.floor(Math.random() * confettiColors.length)];
        confetti.style.animationDuration = (Math.random() * 2 + 3) + 's';
        confetti.style.animationDelay = Math.random() * 0.5 + 's';
        if (shapes[Math.floor(Math.random() * 2)] === 'circle') {
          confetti.style.borderRadius = '50%';
        }
        confetti.style.width = (Math.random() * 8 + 6) + 'px';
        confetti.style.height = confetti.style.width;
        document.body.appendChild(confetti);
        
        setTimeout(() => confetti.remove(), 5000);
      }, i * 50);
    }
    
    // Repeat confetti
    setInterval(() => {
      for (let i = 0; i < 30; i++) {
        setTimeout(() => {
          const confetti = document.createElement('div');
          confetti.className = 'confetti';
          confetti.style.left = Math.random() * 100 + '%';
          confetti.style.background = confettiColors[Math.floor(Math.random() * confettiColors.length)];
          confetti.style.animationDuration = (Math.random() * 2 + 3) + 's';
          confetti.style.borderRadius = Math.random() > 0.5 ? '50%' : '0';
          confetti.style.width = (Math.random() * 8 + 6) + 'px';
          confetti.style.height = confetti.style.width;
          document.body.appendChild(confetti);
          setTimeout(() => confetti.remove(), 5000);
        }, i * 80);
      }
    }, 4000);
  }
  
  // Floating hearts
  function launchHearts() {
    const heartEmojis = ['💖', '💕', '💗', '💝', '✨', '🌟'];
    
    setInterval(() => {
      const heart = document.createElement('div');
      heart.className = 'heart';
      heart.textContent = heartEmojis[Math.floor(Math.random() * heartEmojis.length)];
      heart.style.left = Math.random() * 100 + '%';
      heart.style.bottom = '0';
      heart.style.animationDuration = (Math.random() * 2 + 3) + 's';
      document.body.appendChild(heart);
      setTimeout(() => heart.remove(), 5000);
    }, 400);
  }
</script>

</body>
</html>
