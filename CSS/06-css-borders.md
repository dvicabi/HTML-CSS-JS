# 🧱ו CSS Borders – מסגרות עיצוביות לכל אלמנט במשחקים

---

## 🎯 למה להשתמש במסגרות?

- 📦 להבליט כרטיסים ודמויות
- 🧪 לסמן חפצים מיוחדים
- 🎮 להפריד בין אזורים
- ✨ ליצור סגנון ייחודי

---

## 🔹 התחביר הבסיסי

```css
selector {
  border: [width] [style] [color];
}
````

דוגמה:

```css
.card {
  border: 3px solid gold;
}
```

---

## 🔸 מאפיינים נפרדים

```css
.card {
  border-width: 4px;
  border-style: dashed;
  border-color: orange;
}
```

---

## 🔸 צדדים ספציפיים

```css
.card {
  border-top: 3px solid red;
  border-bottom: 3px dashed blue;
}
```

---

## 🧩 סוגי קווים (`border-style`)

| ערך      | תוצאה     |
| -------- | --------- |
| `solid`  | קו רגיל   |
| `dashed` | קו מקווקו |
| `dotted` | נקודות    |
| `double` | קו כפול   |
| `groove` | חריץ      |
| `ridge`  | בליטה     |
| `inset`  | שקוע      |
| `outset` | בולט      |
| `none`   | ללא מסגרת |

---

## 🔹 עיגול פינות (`border-radius`)

```css
.box {
  border: 2px solid cyan;
  border-radius: 12px;
}
```

🔸 פינה עגולה = מראה נעים יותר, מתאים לחפצים או כפתורים

---

## 🔸 עיגול מושלם (עבור תמונה עגולה)

```css
.avatar {
  border: 3px solid white;
  border-radius: 50%;
  width: 120px;
  height: 120px;
}
```

---

## 🎨 דוגמה לכרטיס דמות

```html
<div class="character">
  <h3>🧙‍♂️ דביר</h3>
  <p>כוח: 70<br>חיים: 💖💖💖</p>
</div>
```

```css
.character {
  border: 3px double gold;
  border-radius: 10px;
  padding: 10px;
  width: 250px;
  background: #1a1a1a;
  color: white;
  box-shadow: 0 0 10px cyan;
}
```

---

## 🧠 טיפים למפתחי משחקים

* השתמש ב־`dashed` או `dotted` לחפצים קסומים
* `double` טוב לכרטיסים חשובים או בוסים
* `inset` / `outset` יוצרים עומק
* השתמש ב־`border-radius: 50%` לעיצוב אייקונים
