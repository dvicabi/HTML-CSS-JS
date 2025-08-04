# 📊ו CSS Tables – עיצוב טבלאות להצגת מידע במשחקים

---

## 🎯 מתי להשתמש בטבלה?

- 🏆 לוח ניקוד שחקנים
- 🗃️ רשימת שלבים/חפצים
- 📦 סטטיסטיקות דמות
- 🎮 השוואה בין פריטים

---

## 🔹 מבנה בסיסי של טבלה

```html
<table>
  <tr>
    <th>שחקן</th>
    <th>נקודות</th>
    <th>שלב</th>
  </tr>
  <tr>
    <td>🧙 דביר</td>
    <td>1500</td>
    <td>3</td>
  </tr>
  <tr>
    <td>🏹 רוני</td>
    <td>980</td>
    <td>2</td>
  </tr>
</table>
````

| תגית      | תפקיד                |
| --------- | -------------------- |
| `<table>` | הטבלה עצמה           |
| `<tr>`    | שורת טבלה            |
| `<th>`    | כותרת עמודה (מודגשת) |
| `<td>`    | תא נתונים            |

---

## 🔸 עיצוב טבלאות בסיסי

```css
table {
  width: 100%;
  border-collapse: collapse;
}

th, td {
  border: 2px solid #555;
  padding: 12px;
  text-align: center;
}

th {
  background-color: #222;
  color: gold;
}
```

---

## 🔸 ריחוף מעל שורה (`:hover`)

```css
tr:hover {
  background-color: #333;
}
```

🔸 מעולה להדגיש שורה שמצביעים עליה

---

## 🔸 גבול אחיד ומקוצר (`border-collapse`)

* `collapse` – מחבר קווים סמוכים לקו אחד
* `separate` – משאיר מרווח בין קווים (ברירת מחדל)

```css
table {
  border-collapse: collapse;
}
```

---

## 🎮 דוגמה: טבלת ניקוד מעוצבת

```html
<table class="scoreboard">
  <tr>
    <th>🥇 מקום</th>
    <th>שחקן</th>
    <th>ניקוד</th>
  </tr>
  <tr>
    <td>1</td>
    <td>דביר</td>
    <td>2040</td>
  </tr>
  <tr>
    <td>2</td>
    <td>רוני</td>
    <td>1900</td>
  </tr>
</table>
```

```css
.scoreboard {
  width: 80%;
  margin: 20px auto;
  border-collapse: collapse;
  background-color: #1a1a1a;
  color: white;
  font-family: 'Segoe UI', sans-serif;
}

.scoreboard th,
.scoreboard td {
  border: 1px solid #888;
  padding: 10px 16px;
}

.scoreboard th {
  background-color: #333;
  color: gold;
}
```

---

## 🧠 טיפים למפתחי משחקים

* השתמש ב־`<th>` לכותרות כדי לשמור על קריאות
* בחר צבעים עם ניגודיות גבוהה למשחקים כהים
* סגנן שורות עם `:nth-child` או `:hover` כדי ליצור חוויית משתמש נוחה
* שלב אימוג'ים להוספת סגנון מהנה לטבלה
