# 🎮 פרויקט אינטראקטיבי בסיסי – שילוב HTML + CSS + JavaScript

---

## 📁 מבנה קבצים מומלץ

```

/project/
├── index.html
├── style.css
└── game.js

````

---

## 📄 `index.html`

```html
<!DOCTYPE html>
<html lang="he">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>משחק לחיצות מהירות</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="container">
      <h1>🎯 משחק הלחיצה</h1>
      <p id="score">נקודות: 0</p>
      <button id="clickBtn">לחץ עליי!</button>
    </div>

    <script src="game.js"></script>
  </body>
</html>
````

---

## 🎨 `style.css`

```css
body {
  background-color: #111;
  color: #fff;
  font-family: "Segoe UI", sans-serif;
  text-align: center;
  padding: 40px;
}

.container {
  background-color: #222;
  padding: 30px;
  border-radius: 12px;
  box-shadow: 0 0 20px cyan;
  display: inline-block;
}

button {
  font-size: 24px;
  padding: 10px 30px;
  margin-top: 20px;
  background-color: gold;
  border: none;
  border-radius: 8px;
  cursor: pointer;
  transition: background 0.3s ease;
}

button:hover {
  background-color: orange;
}
```

---

## 🧠 `game.js`

```javascript
let score = 0;

document.getElementById("clickBtn").onclick = function () {
  score++;
  document.getElementById("score").innerHTML = "נקודות: " + score;

  if (score === 10) {
    alert("🎉 כל הכבוד! הגעת ל־10 נקודות!");
  }
};
```

---

## 🎮 איך זה עובד?

* 👆 הילד לוחץ על כפתור
* 🧠 JavaScript מעלה את הניקוד
* 🌟 בעיצוב צבעוני ונעים
* 🧩 מבוסס על מה שלמדנו בפרקים 01–14
