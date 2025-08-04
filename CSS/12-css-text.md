# ו 🅰️ CSS Text – עיצוב טקסטים למשחקים

---

## 🎯 למה לעצב טקסט?

- 🎮 להפוך כותרת למשימה אפית
- 💬 להבליט דיבור של דמויות
- 🧪 לייצר זהות גרפית ייחודית למשחק
- 🧠 לעזור בקריאות וברגש של השחקן

---

## 🔹 צבע טקסט (`color`)

```css
p {
  color: white;
}
````

---

## 🔹 יישור טקסט (`text-align`)

```css
h1 {
  text-align: center;
}
```

| ערך       | תוצאה             |
| --------- | ----------------- |
| `left`    | יישור לשמאל       |
| `right`   | יישור לימין       |
| `center`  | למרכז             |
| `justify` | יישור לשני הצדדים |

---

## 🔹 קישוטים (`text-decoration`)

```css
a {
  text-decoration: none;
}
```

| ערך            | תוצאה        |
| -------------- | ------------ |
| `none`         | בלי קו תחתון |
| `underline`    | קו תחתון     |
| `line-through` | קו חוצה      |
| `overline`     | קו מעל       |

---

## 🔹 שינוי אותיות (`text-transform`)

```css
h2 {
  text-transform: uppercase;
}
```

| ערך          | תוצאה            |
| ------------ | ---------------- |
| `uppercase`  | אותיות גדולות    |
| `lowercase`  | אותיות קטנות     |
| `capitalize` | אות ראשונה גדולה |

---

## 🔹 ריווח בין אותיות (`letter-spacing`)

```css
h3 {
  letter-spacing: 2px;
}
```

---

## 🔹 ריווח בין שורות (`line-height`)

```css
p {
  line-height: 1.5;
}
```

---

## 🔹 צל טקסט (`text-shadow`)

```css
h1 {
  color: gold;
  text-shadow: 2px 2px 4px black;
}
```

🔸 פורמט: `הסטה ימינה, הסטה למטה, טשטוש, צבע`

---

## 🎮 דוגמה: טקסט משימת פתיחה

```html
<h1 class="mission">💥 שלב 1: קרב הקסמים</h1>
```

```css
.mission {
  color: cyan;
  text-align: center;
  text-transform: uppercase;
  text-shadow: 3px 3px 6px black;
  letter-spacing: 2px;
}
```

---

## 🧠 טיפים למפתחי משחקים

* השתמש ב־`text-shadow` להבלטה דרמטית של טקסטים
* יישר טקסטים לפי מבנה המשחק (מרכז זה חגיגי, שמאל זה אינפורמטיבי)
* תמיד תדאג לניגודיות טובה בין צבע הטקסט לרקע
* השתמש בריווח בין אותיות לכותרות – זה משדר עוצמה
