# Legend
Larpcat Meme Coin
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>$LARP — Fake It. Pump It.</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #05070c;
  color: white;
  overflow-x: hidden;
}

/* Background glow */
body::before {
  content: "";
  position: fixed;
  width: 200%;
  height: 200%;
  background: radial-gradient(circle, #00ff88 0%, transparent 60%);
  animation: pulse 6s infinite;
  opacity: 0.1;
}

@keyframes pulse {
  0% { transform: scale(1); }
  50% { transform: scale(1.2); }
  100% { transform: scale(1); }
}

/* Header */
header {
  padding: 50px 20px;
  text-align: center;
}

h1 {
  font-size: 4rem;
  color: #00ff88;
  text-shadow: 0 0 20px #00ff88;
}

.tagline {
  font-size: 1.3rem;
  opacity: 0.8;
}

/* Hero Image */
.hero img {
  width: 320px;
  border-radius: 20px;
  margin-top: 20px;
  box-shadow: 0 0 30px #00ff88;
}

/* Floating money */
.money {
  position: fixed;
  top: -50px;
  font-size: 24px;
  animation: fall linear infinite;
}

@keyframes fall {
  to {
    transform: translateY(110vh);
  }
}

/* Sections */
.section {
  padding: 60px 20px;
  text-align: center;
}

h2 {
  color: #00ff88;
}

/* Cards */
.tokenomics {
  display: flex;
  justify-content: center;
  gap: 20px;
  flex-wrap: wrap;
}

.card {
  background: #0f1524;
  padding: 25px;
  border-radius: 15px;
  width: 200px;
  box-shadow: 0 0 15px rgba(0,255,136,0.2);
}

/* Buttons */
.btn {
  display: inline-block;
  padding: 15px 30px;
  margin: 10px;
  background: #00ff88;
  color: black;
  font-weight: bold;
  border-radius: 10px;
  text-decoration: none;
  transition: 0.2s;
}

.btn:hover {
  transform: scale(1.1);
  box-shadow: 0 0 20px #00ff88;
}

/* Fake chart animation */
.chart {
  width: 100%;
  height: 200px;
  background: linear-gradient(transparent, #00ff8840);
  position: relative;
  overflow: hidden;
}

.chart-line {
  position: absolute;
  width: 200%;
  height: 2px;
  background: #00ff88;
  top: 60%;
  animation: moveChart 4s linear infinite;
}

@keyframes moveChart {
  from { left: -100%; }
  to { left: 0; }
}

footer {
  padding: 20px;
  opacity: 0.6;
}
</style>
</head>

<body>

<header>
  <h1>$LARP</h1>
  <div class="tagline">Fake it. Post it. Pump it.</div>
</header>

<div class="hero">
  <img src="your-image.png" alt="LARP Coin">
</div>

<div class="chart">
  <div class="chart-line"></div>
</div>

<div class="section">
  <h2>🚀 About</h2>
  <p>
    The most delusional coin on the internet. Built for TikTok flexers,
    fake millionaires, and people who WILL make it (eventually).
  </p>
</div>

<div class="section">
  <h2>📊 Tokenomics</h2>
  <div class="tokenomics">
    <div class="card">Supply<br><strong>1B</strong></div>
    <div class="card">Tax<br><strong>0%</strong></div>
    <div class="card">Liquidity<br><strong>Burned 🔥</strong></div>
  </div>
</div>

<div class="section">
  <h2>🔥 Join the Pump</h2>
  <a href="#" class="btn">Buy on Pump.fun</a>
  <a href="#" class="btn">Join Telegram</a>
</div>

<footer>
  Not financial advice. Pure LARP. © 2026
</footer>

<script>
/* Floating money generator */
function createMoney() {
  const money = document.createElement("div");
  money.classList.add("money");
  money.innerText = "💸";
  money.style.left = Math.random() * 100 + "vw";
  money.style.animationDuration = (Math.random() * 3 + 2) + "s";
  document.body.appendChild(money);

  setTimeout(() => {
    money.remove();
  }, 5000);
}

setInterval(createMoney, 300);
</script>

</body>
</html>
