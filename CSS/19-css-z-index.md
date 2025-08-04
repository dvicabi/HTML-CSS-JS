# 🧩ו CSS Z-Index – שכבות בעולם המשחקים

---

## 🎯 למה צריך z-index?

- 🪄 לקבוע איזה אלמנט "מעל" או "מתחת"
- 🎮 לבנות חלונות קופצים, תפריטים, דמויות בשכבות
- 🧱 למנוע בעיות כשהרכיבים נסתרים או חופפים

---

## 🔹 איך זה עובד?

```css
.popup {
  position: absolute;
  z-index: 10;
}
````

🔸 ככל שהמספר **גבוה יותר** – האלמנט **יותר קדמי**

---

## 🔹 תנאים לשימוש ב־z-index

* עובד רק אם לאלמנט יש `position` שהוא:

  * `relative`
  * `absolute`
  * `fixed`
  * `sticky`

---

## 🔢 דוגמה פשוטה

```html
<div class="behind">🧱 קיר</div>
<div class="front">🧙 דמות</div>
```

```css
.behind {
  position: absolute;
  z-index: 1;
}

.front {
  position: absolute;
  z-index: 5;
}
```

🔸 הדמות תופיע **מעל** הקיר

---

## 🔸 שימוש מתקדם: תפריט קופץ מעל המשחק

```html
<div class="game">🎮 שטח המשחק</div>
<div class="popup">💬 הודעה מהאח</div>
```

```css
.game {
  position: relative;
  z-index: 1;
}

.popup {
  position: absolute;
  top: 50px;
  left: 50px;
  background: white;
  color: black;
  padding: 12px;
  z-index: 999;
}
```

---

## 🎮 דוגמה: סרגל סטטוס קבוע מקדימה

```css
.status {
  position: fixed;
  top: 0;
  width: 100%;
  background: #222;
  color: white;
  padding: 10px;
  z-index: 1000;
}
```

---

## 🧠 טיפים למפתחי משחקים

* תכנן שכבות מראש: HUD, דמויות, כפתורים, חלונות
* אל תשתמש ב־z-index גבוהים סתם – עדיף להשתמש בשליטה לוגית
* נהל את השכבות לפי סוג האלמנט (משחק, תפריט, דיאלוג, רקע)
* אם משהו "נעלם" – בדוק אם אלמנט אחר עם z-index גדול יותר מכסה עליו
