<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>For Baby 💕</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
body {
  margin: 0;
  font-family: Georgia, serif;
  background:
    linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.8)),
    url("https://i.postimg.cc/kGdGztcX/IMG-20251025-WA0050.jpg") center / cover no-repeat fixed;
  color: white;
}

section {
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 30px;
}

.card {
  background: rgba(255,255,255,0.95);
  color: #5a1a2e;
  padding: 35px;
  border-radius: 20px;
  max-width: 700px;
  box-shadow: 0 20px 40px rgba(0,0,0,0.4);
}

h1 {
  margin-bottom: 20px;
}

button {
  padding: 14px 32px;
  border-radius: 30px;
  border: none;
  font-size: 1em;
  cursor: pointer;
  background: #ff4d6d;
  color: white;
  margin: 10px;
}

button:hover {
  transform: scale(1.08);
}

.gift, .envelope {
  font-size: 90px;
  cursor: pointer;
}

#noBtn {
  background: #aaa;
  position: relative;
}

.heart {
  position: fixed;
  bottom: -20px;
  font-size: 22px;
  animation: float 6s linear forwards;
}

@keyframes float {
  to {
    transform: translateY(-120vh);
    opacity: 0;
  }
}

#meme {
  position: fixed;
  inset: 0;
  background: rgba(0,0,0,0.85);
  display: none;
  align-items: center;
  justify-content: center;
  z-index: 999;
}

#meme img {
  max-width: 90%;
  border-radius: 20px;
}
</style>
</head>

<body>

<!-- SECTION 1 -->
<section>
  <div class="card">
    <h1>Hey baby 💕</h1>
    <p>I made something just for you.</p>
    <div class="gift" onclick="scrollToPoem()">🎁</div>
    <p><em>Tap the gift</em></p>
  </div>
</section>

<!-- SECTION 2 -->
<section id="poem">
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

    <p><em>Scroll down 💌</em></p>
  </div>
</section>

<!-- SECTION 3 -->
<section>
  <div class="card">
    <div class="envelope" onclick="scrollToQuestion()">💌</div>
    <p>Open this</p>
  </div>
</section>

<!-- SECTION 4 -->
<section id="question">
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
function scrollToPoem() {
  document.getElementById("poem").scrollIntoView({ behavior: "smooth" });
}

function scrollToQuestion() {
  document.getElementById("question").scrollIntoView({ behavior: "smooth" });
}

function runAway() {
  const btn = document.getElementById("noBtn");
  btn.style.left = Math.random() * 200 - 100 + "px";
  btn.style.top = Math.random() * 200 - 100 + "px";
}

function sayYes() {
  document.getElementById("meme").style.display = "flex";
  for (let i = 0; i < 30; i++) {
    const heart = document.createElement("div");
    heart.className = "heart";
    heart.innerHTML = "❤️";
    heart.style.left = Math.random() * 100 + "vw";
    document.body.appendChild(heart);
    setTimeout(() => heart.remove(), 6000);
  }
}
</script>

</body>
</html>
https://i.postimg.cc/kGdGztcX/IMG-20251025-WA0050.jpg
https://i.postimg.cc/HkjYS2md/872a6e8fa6aafc89c25de032d63c0966.jpg
