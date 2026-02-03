# valentine-for-baby
just me asking my girlfriend to be my valentine
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>For Baby 💕</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
* { box-sizing: border-box; }

body {
  margin: 0;
  font-family: 'Georgia', serif;
  background:
    linear-gradient(rgba(0,0,0,0.55), rgba(0,0,0,0.75)),
    url("BACKGROUND_IMAGE_URL") center/cover no-repeat fixed;
  color: white;
  overflow-x: hidden;
}

section {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 40px 20px;
  text-align: center;
}

.card {
  background: rgba(255,255,255,0.95);
  color: #5a1a2e;
  padding: 40px;
  border-radius: 22px;
  max-width: 650px;
  box-shadow: 0 25px 50px rgba(0,0,0,0.35);
  animation: fadeIn 1.6s ease;
}

h1 {
  font-size: 2.3em;
  margin-bottom: 20px;
}

p {
  line-height: 1.7;
  font-size: 1.05em;
}

.hidden { display: none; }

button {
  padding: 14px 32px;
  border-radius: 30px;
  border: none;
  font-size: 1em;
  cursor: pointer;
  margin: 15px;
  background: #ff4d6d;
  color: white;
  transition: transform 0.2s;
}
button:hover { transform: scale(1.1); }

.gift {
  font-size: 90px;
  cursor: pointer;
  animation: bounce 1.4s infinite;
}

.envelope {
  font-size: 80px;
  cursor: pointer;
}

@keyframes bounce {
  0%,100% { transform: translateY(0); }
  50% { transform: translateY(-18px); }
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}

/* NO button runaway */
#noBtn {
  background: #aaa;
  position: relative;
}

/* Hearts */
.heart {
  position: fixed;
  bottom: -20px;
  font-size: 22px;
  animation: floatUp 6s linear forwards;
}

@keyframes floatUp {
  to {
    transform: translateY(-120vh);
    opacity: 0;
  }
}

/* Meme overlay */
#meme {
  position: fixed;
  inset: 0;
  background: rgba(0,0,0,0.85);
  display: none;
  justify-content: center;
  align-items: center;
  z-index: 999;
}
#meme img {
  max-width: 90%;
  border-radius: 20px;
}
</style>
</head>

<body>

<!-- GIFT -->
<section>
  <div class="card">
    <h1>Hey baby 💕</h1>
    <p>I made something for you.</p>
    <div class="gift" onclick="openGift()">🎁</div>
    <p><em>Tap the gift</em></p>
  </div>
</section>

<!-- POEM -->
<section id="poem" class="hidden">
  <div class="card">
    <h1>My handsome wife,</h1>

    <p>
      this is my way of saying I want to do life with you.<br>
      Not someday. Not halfway.<br>
      Fully.
    </p>

    <p>
      From the first moment I saw you,<br>
      from the way I fit into your arms<br>
      and you held me like you meant it,<br>
      I knew I belonged with you.<br>
      I knew I was meant to be yours.
    </p>

    <p>
      I love the softness of your lips,<br>
      the way you touch me with care,<br>
      the way you love me with intention<br>
      and never by accident.
    </p>

    <p>
      You choose me in how you show up,<br>
      how you protect me,<br>
      how you hold me—<br>
      emotionally and physically.
    </p>

    <p>
      I am thankful for you.<br>
      For your passion that feels steady,<br>
      your gentleness that feels strong,<br>
      your presence that makes me feel safe<br>
      and deeply wanted at the same time.
    </p>

    <p>
      I love you.<br>
      And I pray our love is seen and blessed by God.<br>
      I pray He chooses you for me—
    </p>

    <p>
      because I choose you for me,<br>
      every day, without hesitation.
    </p>

    <p><em>Scroll down…</em></p>
  </div>
</section>

<!-- ENVELOPE -->
<section id="letter" class="hidden">
  <div class="card">
    <div class="envelope" onclick="openLetter()">💌</div>
    <p>Open this</p>
  </div>
</section>

<!-- QUESTION -->
<section id="question" class="hidden">
  <div class="card">
    <h1>So hey…</h1>
    <h1>Will you do Valentine’s Day with me? 💖</h1>

    <button onclick="sayYes()">Yes 💘</button>
    <button id="noBtn" onmouseover="runAway()">No</button>
  </div>
</section>

<!-- MEME -->
<div id="meme">
  <img src="DANCING_GIF_URL">
</div>

<script>
function openGift() {
  document.getElementById("poem").classList.remove("hidden");
  window.scrollTo({ top: window.innerHeight, behavior: "smooth" });
}

function openLetter() {
  document.getElementById("question").classList.remove("hidden");
  window.scrollTo({ top: document.body.scrollHeight, behavior: "smooth" });
}

function runAway() {
  const btn = document.getElementById("noBtn");
  btn.style.left = Math.random() * 200 - 100 + "px";
  btn.style.top = Math.random() * 200 - 100 + "px";
}

function sayYes() {
  document.getElementById("meme").style.display = "flex";
  for (let i = 0; i < 35; i++) {
    createHeart();
  }
}

function createHeart() {
  const heart = document.createElement("div");
  heart.className = "heart";
  heart.innerHTML = "❤️";
  heart.style.left = Math.random() * 100 + "vw";
  document.body.appendChild(heart);
  setTimeout(() => heart.remove(), 6000);
}
</script>

</body>
</html>
https://imgur.com/a/ZozJfrx
https://imgur.com/a/cwdFLSG
