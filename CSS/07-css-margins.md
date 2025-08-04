# 📏ו CSS Margins – ריווחים חיצוניים בין רכיבי המשחק

---

## 🎯 למה Margin חשוב?

- 📦 יוצר ריווח חיצוני בין אלמנטים
- 🎮 מונע צפיפות במסכים
- ✨ עוזר לבנות ממשק מסודר ואסתטי

---

## 🔹 התחביר הבסיסי

```css
selector {
  margin: value;
}
````

```css
.card {
  margin: 20px;
}
```

🔸 יוצר רווח חיצוני מכל הצדדים (top, right, bottom, left)

---

## 🔸 Margin לפי צד

```css
.card {
  margin-top: 20px;
  margin-right: 10px;
  margin-bottom: 15px;
  margin-left: 10px;
}
```

---

## 🔸 קיצור דרך לפי סדר (TRBL)

```css
.card {
  margin: 10px 20px 15px 5px;
}
/* top: 10px, right: 20px, bottom: 15px, left: 5px */
```

```css
.card {
  margin: 20px 10px;
}
/* top+bottom: 20px, right+left: 10px */
```

---

## 🔹 שימוש ב־`auto` למרכז רכיבים

```css
.container {
  width: 400px;
  margin: 0 auto;
}
```

🔸 מרכז את הקופסה בתוך המסך (ימין ושמאל)

---

## 🔸 ריווח בין קלפים במשחק

```css
.card {
  margin-bottom: 20px;
}
```

🔸 כך ניתן ליצור מרווח בין כל כרטיס לכרטיס מתחתיו

---

## 🎮 דוגמה לעיצוב לוח דמויות

```html
<div class="card">🧙 קוסם</div>
<div class="card">🛡️ לוחם</div>
<div class="card">🏹 קשת</div>
```

```css
.card {
  background: #222;
  color: white;
  padding: 10px;
  border-radius: 8px;
  margin-bottom: 16px;
}
```

---

## 🧠 טיפים למפתחי משחקים

* תמיד תן מרווח בין כפתורים (כדי שלא ילחצו בטעות)
* תן `margin-top` או `margin-bottom` לרכיבים מוערמים
* השתמש ב־`margin: auto` כדי למרכז תפריטים, כרטיסים, אזורי משחק
