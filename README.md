# LARPCAT LEGEND
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>$LARP — The Internet’s Biggest Delusion</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, sans-serif;
}

body {
  background: radial-gradient(circle at top, #0b1220, #02050a);
  color: white;
  overflow-x: hidden;
}

/* NAVBAR */
nav {
  position: fixed;
  width: 100%;
  top: 0;
  padding: 15px 30px;
  display: flex;
  justify-content: space-between;
  backdrop-filter: blur(10px);
  background: rgba(0,0,0,0.4);
  z-index: 1000;
}

nav h2 {
  color: #00ff88;
}

nav a {
  color: white;
  text-decoration: none;
  margin-left: 20px;
  font-size: 0.9rem;
}

/* HERO */
.hero {
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  text-align: center;
}

.hero h1 {
  font-size: 4rem;
  background: linear-gradient(90deg, #00ff88, #00c3ff);
  -webkit-background-clip: text;
  color: transparent;
}

.hero p {
  margin-top: 15px;
  opacity: 0.8;
}

.hero img {
  width: 300px;
  margin-top: 30px;
  border-radius: 20px;
  box-shadow: 0 0 40px #00ff88;
}

/* BUTTON */
.btn {
  margin-top: 25px;
  padding: 15px 35px;
  background: linear-gradient(90deg, #00ff88, #00c3ff);
  border-radius: 10px;
  color: black;
  font-weight: bold;
  text-decoration: none;
  transition: 0.2s;
}

.btn:hover {
  transform: scale(1.1);
}

/* SECTION */
.section {
  padding: 100px 20px;
  text-align: center;
}

/* GLASS CARDS */
.glass {
  background: rgba(255,255,255,0.05);
  backdrop-filter: blur(12px);
  border-radius: 20px;
  padding: 30px;
  margin: 20px auto;
  max-width: 800px;
}

/* TOKENOMICS */
.tokenomics {
  display: flex;
  justify-content: center;
  gap: 20px;
  flex-wrap: wrap;
}

.card {
  background: rgba(0,255,136,0.05);
  padding: 20px;
  border-radius: 15px;
  width: 180px;
}

/* ROADMAP */
.roadmap {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.step {
  background: rgba(0,0,0,0.4);
  padding: 20px;
  border-left: 4px solid #00ff88;
  text-align: left;
}

/* FOOTER */
footer {
  padding: 30px;
  text-align: center;
  opacity: 0.6;
}

/* FLOATING MONEY */
.money {
  position: fixed;
  top: -50px;
  animation: fall linear infinite;
}

@keyframes fall {
  to { transform: translateY(110vh); }
}

</style>
</head>

<body>

<nav>
  <h2>$LARP</h2>
  <div>
    <a href="#about">About</a>
    <a href="#tokenomics">Tokenomics</a>
    <a href="#roadmap">Roadmap</a>
  </div>
</nav>

<div class="hero">
  <h1>$LARP</h1>
  <p>The most delusional coin ever created</p>
  <img src="your-image.png">
  <a href="#" class="btn">🚀 BUY NOW</a>
</div>

<div id="about" class="section">
  <div class="glass">
    <h2>🚀 What is LARP?</h2>
    <p>
      LARP is not just a coin. It's a lifestyle.
      Fake success. Viral flexing. Infinite delusion.
      Built for TikTok kings and future millionaires.
    </p>
  </div>
</div>

<div id="tokenomics" class="section">
  <h2>📊 Tokenomics</h2>
  <div class="tokenomics">
    <div class="card">Supply<br><strong>1B</strong></div>
    <div class="card">Tax<br><strong>0%</strong></div>
    <div class="card">Liquidity<br><strong>Burned</strong></div>
  </div>
</div>

<div id="roadmap" class="section">
  <h2>🗺 Roadmap</h2>
  <div class="roadmap">
    <div class="step">Phase 1 — Launch & Meme Domination</div>
    <div class="step">Phase 2 — Viral TikTok Explosion</div>
    <div class="step">Phase 3 — Influencer Takeover</div>
    <div class="step">Phase 4 — $100M Market Cap 🚀</div>
  </div>
</div>

<footer>
  Not financial advice. Just vibes. © 2026 LARP
</footer>

<script>
function createMoney() {
  const el = document.createElement("div");
  el.className = "money";
  el.innerText = "💸";
  el.style.left = Math.random() * 100 + "vw";
  el.style.animationDuration = (Math.random()*3+2)+"s";
  document.body.appendChild(el);
  setTimeout(()=>el.remove(),5000);
}
setInterval(createMoney, 300);
</script>

</body>
</html>


