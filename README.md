
<!DOCTYPE html>
<html lang="sk">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>FC GUĽKO</title>
<style>
* { box-sizing: border-box; }
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #160b29;
  color: white;
  text-align: center;
}
header {
  padding: 25px;
  background: linear-gradient(120deg,#7026c9,#246ee8);
}
h1 { font-size: 32px; margin: 5px; }
nav {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  background: #25123e;
  padding: 10px;
  gap: 8px;
}
button {
  background: #7026c9;
  color: white;
  border: 0;
  border-radius: 10px;
  padding: 12px 16px;
  cursor: pointer;
}
main { padding: 20px; }
.card {
  background: #2c1948;
  border: 1px solid #7652aa;
  border-radius: 18px;
  padding: 22px;
  margin: 18px auto;
  max-width: 500px;
}
.teams {
  display: flex;
  align-items: center;
  justify-content: space-around;
  gap: 10px;
  font-weight: bold;
}
.team { flex: 1; }
.vs { color: #b99aff; font-size: 25px; }
.arena { color: #b99aff; font-size: 22px; }
section { display: none; }
section.active { display: block; }
footer {
  padding: 20px;
  color: #cbb6ed;
}
</style>
</head>
<body>

<header>
  <h1>⚽ FC GUĽKO</h1>
  <p>ONE CLUB. ONE FAMILY.</p>
</header>

<nav>
  <button onclick="showPage('home')">Domov</button>
  <button onclick="showPage('matches')">Zápasy</button>
  <button onclick="showPage('team')">Tím</button>
  <button onclick="showPage('news')">Novinky</button>
</nav>

<main>
<section id="home" class="active">
  <h2>VITAJ V FC GUĽKO!</h2>
  <div class="card">
    <h2>🏆 NAJBLIŽŠÍ ZÁPAS</h2>
    <div class="teams">
      <div class="team">💜<br>FC GUĽKO</div>
      <div class="vs">VS</div>
      <div class="team">🔺<br>FC TROJUHOLNÍK PREŠOV</div>
    </div>
    <h2 class="arena">🏟️ GUĽ ARENA</h2>
    <p>Domáci štadión FC Guľko</p>
    <p>Dátum: Bude doplnený</p>
  </div>
</section>

<section id="matches">
  <h2>⚽ ZÁPASY</h2>
  <div class="card">
    FC GUĽKO vs FC TROJUHOLNÍK PREŠOV
    <h3>GUĽ ARENA</h3>
  </div>
</section>

<section id="team">
  <h2>👥 NÁŠ TÍM</h2>
  <div class="card">
    <p>🧤 Brankári</p>
    <p>🛡️ Obrancovia</p>
    <p>⚽ Záložníci</p>
    <p>🔥 Útočníci</p>
  </div>
</section>

<section id="news">
  <h2>📰 NOVINKY</h2>
  <div class="card">
    <h3>FC GUĽKO</h3>
    <p>Vitaj na oficiálnej stránke nášho klubu!</p>
  </div>
</section>
</main>

<footer>
  FC GUĽKO © 2026<br>
  💜 FIALOVÁ • 🤍 BIELA • 💙 MODRÁ
</footer>

<script>
function showPage(page) {
  document.querySelectorAll('main section')
    .forEach(s => s.classList.remove('active'));
  document.getElementById(page).classList.add('active');
}
</script>

</body>
</html>


