# 🧙‍♂️ פרויקט 2 – ממשק משחק Mini RPG (HTML + CSS + JS)

---

## 🎯 מטרת הפרויקט

- יצירת דמות
- הצגת סטטיסטיקות
- לחצני פעולה אינטראקטיביים
- עיצוב מקצועי + קוד מופרד

---

## 📁 מבנה תיקיות

```

/mini-rpg/
├── index.html
├── style.css
└── rpg.js

````

---

## 📄 index.html

```html
<!DOCTYPE html>
<html lang="he">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Mini RPG - דביר</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <h1>🏰 Mini RPG – עולם הקסם</h1>
  </header>

  <main>
    <section id="hero-card">
      <h2>🧙‍♂️ דמות: דביר</h2>
      <p>💖 חיים: <span id="hp">100</span></p>
      <p>⭐ ניסיון: <span id="xp">0</span></p>
    </section>

    <section id="actions">
      <button onclick="fight()">⚔️ קרב</button>
      <button onclick="heal()">🧪 ריפוי</button>
      <button onclick="reset()">🔄 אתחול</button>
    </section>

    <section id="log">
      <h3>📜 יומן משחק</h3>
      <ul id="log-list"></ul>
    </section>
  </main>

  <footer>
    ⓒ נבנה על ידי דביר 2025
  </footer>

  <script src="rpg.js"></script>
</body>
</html>
````

---

## 🎨 style.css

```css
body {
  background: #121212;
  color: #fff;
  font-family: 'Segoe UI', sans-serif;
  text-align: center;
  margin: 0;
  padding: 0;
}

header, footer {
  background: #1a1a1a;
  padding: 10px;
  color: gold;
}

main {
  padding: 20px;
}

#hero-card {
  background: #222;
  padding: 20px;
  border-radius: 10px;
  margin-bottom: 20px;
  box-shadow: 0 0 10px cyan;
}

#actions button {
  margin: 10px;
  padding: 12px 20px;
  font-size: 18px;
  background-color: gold;
  border: none;
  border-radius: 8px;
  cursor: pointer;
}

#actions button:hover {
  background-color: orange;
}

#log {
  background: #2a2a2a;
  padding: 15px;
  border-radius: 8px;
  margin-top: 20px;
}

#log-list {
  list-style-type: "🗡️ ";
  padding-left: 20px;
  text-align: left;
}
```

---

## 🧠 rpg.js

```javascript
let hp = 100;
let xp = 0;

function fight() {
  const damage = Math.floor(Math.random() * 30) + 1;
  hp -= damage;
  xp += 10;
  updateStats();
  logAction(`נלחמת ונפגעת ב־${damage} נקודות!`);
}

function heal() {
  const healAmount = Math.floor(Math.random() * 20) + 10;
  hp += healAmount;
  if (hp > 100) hp = 100;
  logAction(`💚 נרפאת ב־${healAmount} נקודות`);
  updateStats();
}

function reset() {
  hp = 100;
  xp = 0;
  document.getElementById("log-list").innerHTML = "";
  updateStats();
  logAction("🔄 המשחק אופס");
}

function updateStats() {
  document.getElementById("hp").textContent = hp;
  document.getElementById("xp").textContent = xp;
}

function logAction(msg) {
  const li = document.createElement("li");
  li.textContent = msg;
  document.getElementById("log-list").prepend(li);
}
```

---

## 💡 הפרויקט כולל:

* שימוש ב־HTML סמנטי
* עיצוב מודרני ב־CSS
* לוגיקת משחק פשוטה ב־JS
* ניהול חיים, ניסיון, לוג קרבות
