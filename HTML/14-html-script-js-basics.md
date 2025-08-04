# 📜 תגית `<script>` – התחלת JavaScript בתוך HTML

---

## 🧠 מה זה JavaScript?

JavaScript (JS) היא שפת תכנות המאפשרת **אינטראקטיביות**:  
- 🎯 כפתורים שמגיבים  
- 🧪 מצבים משתנים במשחק  
- 🕹️ שליטה על תנועה, ניקוד, ועוד!

---

## 🔹 התחלה בסיסית עם `<script>`

```html
<script>
  alert("🎮 ברוך הבא למשחק של דביר!");
</script>
````

* יוצג חלון קופץ כשנטען העמוד

---

## 🔹 סקריפט בתוך כפתור

```html
<button onclick="alert('🧙‍♂️ כישוף הופעל!')">הפעל כישוף</button>
```

* `onclick` – אירוע של לחיצה
* ניתן להציב בתוך `tag` או בתוך `script`

---

## 🔹 שינוי תוכן עם JavaScript

```html
<p id="result">💤 אין פעולה עדיין</p>
<button onclick="document.getElementById('result').innerHTML = '🔥 כישוף הופעל!'">
  בצע פעולה
</button>
```

---

## 🔹 קוד בתוך תגית `<script>` בסוף הדף

```html
<p id="score">נקודות: 0</p>
<button id="btn">+ נקודה</button>

<script>
  let score = 0;
  document.getElementById("btn").onclick = function () {
    score++;
    document.getElementById("score").innerHTML = "נקודות: " + score;
  };
</script>
```

---

## 🔸 קישור לקובץ JavaScript חיצוני

```html
<script src="game.js"></script>
```

📁 שם הקובץ: `game.js`

```javascript
alert("🎮 התחלת המשחק");
```

---

## ⚠️ איפה למקם את הסקריפט?

1. בתחתית `<body>` – מומלץ (כדי שכל האלמנטים ייטענו קודם)
2. או עם `defer` בתוך `<head>`:

```html
<script src="game.js" defer></script>
```

---

## 🧠 שימושים לילדים מפתחי משחקים

* 🕹️ שינוי נקודות
* 💡 פתיחת שלב חדש בלחיצה
* 🔒 הצגת תפריט רק אחרי פעולה
* ⏱️ מדידת זמן (שנעשה בהמשך)
