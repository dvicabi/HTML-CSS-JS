# 🧱ו CSS Display – תצוגת רכיבים בעולם המשחקים

---

## 🎯 למה חשוב `display`?

- 🧩 לשלוט איך אלמנטים מוצגים (כבלוקים, שורות, גרידים)
- 🎮 ליצור לוחות, קלפים, תפריטים
- 👻 להעלים רכיבים (למשל אחרי שהשחקן סיים שלב)

---

## 🔹 Display: Block

```css
div {
  display: block;
}
````

* תופס את כל הרוחב
* נשבר לשורה חדשה

🔸 ברירת מחדל של:

* `<div>`, `<p>`, `<h1>`…

---

## 🔹 Display: Inline

```css
span {
  display: inline;
}
```

* בשורה אחת עם אחרים
* *לא* אפשר לקבוע גובה/רוחב

🔸 ברירת מחדל של:

* `<span>`, `<a>`, `<strong>`

---

## 🔹 Display: Inline-block

```css
.card {
  display: inline-block;
  width: 200px;
}
```

* כמו inline, אבל כן אפשר גובה/רוחב
* מתאים לכפתורים, קלפים בשורה

---

## 🔹 Display: None

```css
.secret {
  display: none;
}
```

🔸 האלמנט נעלם לגמרי מהמסך

---

## 🎮 דוגמה: הצגת קלפים זה לצד זה

```html
<div class="card">🧙‍♂️ דביר</div>
<div class="card">🏹 רוני</div>
```

```css
.card {
  display: inline-block;
  width: 160px;
  height: 200px;
  margin: 10px;
  background: #2a2a2a;
  color: white;
  padding: 10px;
  text-align: center;
}
```

---

## 🔹 שינוי תצוגה ב־JavaScript

```javascript
document.getElementById("popup").style.display = "none";
```

🔸 מעולה להחביא תיבות הודעה, חלונות קופצים ועוד

---

## 🧠 טיפים למפתחי משחקים

* השתמש ב־`inline-block` לכרטיסים, אייקונים, תפריטים
* `display: none` הוא כלי מעולה לפופ־אפים, מסכים זמניים, ומצבי "המשחק נגמר"
* תבין איזה אלמנט מציג איך – זה משפיע על מיקומים ועיצוב

