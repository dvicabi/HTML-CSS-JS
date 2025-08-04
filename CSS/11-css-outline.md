# 🔲ו CSS Outline – קווי מתאר לפוקוס, נגישות והדגשות

---

## 🎯 מה זה Outline?

🔹 **Outline = קו מתאר** סביב אלמנט  
🔹 דומה למסגרת (`border`), אבל:
- אינו תופס מקום (לא משפיע על הגודל)
- יכול לעבור מעל אלמנטים אחרים
- משמש להדגשות זמניות, פוקוס, גישה נגישה 🔍

---

## 🔹 התחביר הבסיסי

```css
button {
  outline: 2px solid cyan;
}
````

🔸 קו כחול מסביב לכפתור

---

## 🔸 מאפיינים נפרדים

```css
input {
  outline-width: 3px;
  outline-style: dotted;
  outline-color: lime;
}
```

---

## 🔸 הסרת קו מתאר (לא מומלץ לנגישות)

```css
button {
  outline: none;
}
```

⚠️ השתמש בזה בזהירות – קו הפוקוס חשוב למשתמשים עם מקלדת

---

## 🔹 Outline בפוקוס (`:focus`)

```css
input:focus {
  outline: 3px solid gold;
}
```

🔸 מופיע רק כאשר המשתמש לוחץ או נכנס לשדה עם TAB

---

## 🎮 דוגמה: כפתור קסם בפוקוס

```css
button.magic:focus {
  outline: 4px dashed magenta;
}
```

```html
<button class="magic">🪄 הטל לחשים</button>
```

---

## 🧠 שימושים נפוצים במשחקים

| שימוש                   | דוגמה                              |
| ----------------------- | ---------------------------------- |
| פוקוס לשדות קלט         | `input:focus { outline: ... }`     |
| הדגשת כפתור נבחר        | `button.selected { outline: ... }` |
| קו מתאר זמני למעבר עכבר | `div:hover { outline: ... }`       |
| שימוש באפקטים מבריקים   | outline בצבעים מתחלפים או זוהרים ✨ |

---

## 🔧 שילוב עם אנימציה (מתקדמים)

```css
.card:focus {
  outline: 3px solid transparent;
  box-shadow: 0 0 8px 4px gold;
}
```

🔸 שילוב outline עם `box-shadow` יוצר אפקט זוהר 👑

---

## 🧠 טיפים למפתחי משחקים

* תמיד אפשר להיעזר ב־outline כדי להדגיש רכיב בלי להזיז דברים סביבו
* אל תבטל outline לגמרי – אלא אם אתה מוסיף משהו אחר במקום (כמו `box-shadow`)
* outline לא נספר כחלק מגודל האלמנט – זה יתרון לעיצוב זמני
