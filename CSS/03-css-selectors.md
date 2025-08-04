# 🎯ו CSS Selectors – כל סוגי הסלקטורים לשליטה מדויקת בעיצוב

---

## 🔹 מה זה Selector?

Selector ב־CSS הוא הדרך שלנו **לבחור אלמנטים** מתוך ה־HTML,  
כדי לעצב אותם בצורה מדויקת 🎯

---

## 🧩 סוגי סלקטורים בסיסיים

| סלקטור | דוגמה | מה הוא בוחר |
|--------|--------|-------------|
| תגית   | `p`     | כל הפסקאות (`<p>`) |
| מחלקה  | `.hero` | כל אלמנט עם `class="hero"` |
| מזהה   | `#menu` | אלמנט אחד עם `id="menu"` |

---

## 🔸 סלקטור תגית

```css
h1 {
  color: gold;
}
````

🎨 כל תגית `<h1>` תהיה בצבע זהב

---

## 🔸 סלקטור מחלקה (class)

```css
.title {
  font-size: 36px;
  text-shadow: 2px 2px black;
}
```

HTML:

```html
<h2 class="title">שלב 1: שער המוות</h2>
```

---

## 🔸 סלקטור מזהה (ID)

```css
#mainMenu {
  background-color: #222;
  padding: 10px;
}
```

HTML:

```html
<div id="mainMenu">...</div>
```

🔸 ID חייב להיות **ייחודי** בעמוד
🔸 class יכול לחזור כמה פעמים

---

## 🧠 סלקטורים משולבים

| סלקטור        | משמעות                                |
| ------------- | ------------------------------------- |
| `div p`       | כל `<p>` בתוך `<div>`                 |
| `.hero p`     | כל פסקה בתוך מחלקה בשם hero           |
| `h1.title`    | `<h1>` שיש לו גם מחלקה בשם title      |
| `section > p` | רק פסקאות **ישירות** בתוך `<section>` |
| `ul li`       | כל פריט בתוך רשימה                    |

---

## 🎮 דוגמה מציאותית במשחק

```html
<div class="card boss">
  <h3 class="name">👹 בוס: שר האש</h3>
  <p class="info">נזק: 50🔥</p>
</div>
```

```css
.card {
  background: #111;
  padding: 10px;
  border-radius: 10px;
}

.boss {
  border: 2px solid red;
}

.card .info {
  color: orange;
}
```

---

## 🧠 טיפים חשובים

* class מתחיל ב־`.` (נקודה)
* id מתחיל ב־`#` (סולמית)
* עדיף לעבוד עם מחלקות (class) – קל לשכפל ולעצב קבוצות

