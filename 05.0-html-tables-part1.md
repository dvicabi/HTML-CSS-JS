# 📊 תגית `<table>` – טבלאות ב־HTML (חלק 1 מתוך X)

---

## 📌 מטרה

טבלאות מאפשרות לנו להציג מידע בצורה מסודרת:  
🧝‍♂️ רשימות דמויות  
🛡️ טבלת חפצים  
⚔️ נתוני קרב  
🧩 סטטיסטיקות במשחק  
ועוד...

---

## 🧱 מבנה בסיסי של טבלה

```html
<table border="1">
  <tr>
    <th>🎮 שחקן</th>
    <th>💖 חיים</th>
    <th>⚔️ כוח</th>
  </tr>
  <tr>
    <td>דביר</td>
    <td>3</td>
    <td>80</td>
  </tr>
  <tr>
    <td>נועה</td>
    <td>2</td>
    <td>90</td>
  </tr>
</table>
````

---

## 🔍 הסבר תגיות:

🔸 `<table>` – עוטף את כל הטבלה
🔸 `<tr>` – Table Row – שורה בטבלה
🔸 `<th>` – Table Header – כותרת של עמודה (מודגשת)
🔸 `<td>` – Table Data – תא רגיל בטבלה

---

## 🔢 טבלה עם נתונים מספריים

```html
<table border="1">
  <tr>
    <th>🏹 כלי נשק</th>
    <th>נזק</th>
    <th>טווח</th>
  </tr>
  <tr>
    <td>חץ קסום</td>
    <td>25</td>
    <td>רחוק</td>
  </tr>
  <tr>
    <td>גרזן כבד</td>
    <td>50</td>
    <td>קצר</td>
  </tr>
</table>
```

---

## 🧪 מימוש בסיסי בעיצוב טבלה (ב־CSS):

```html
<style>
  table {
    border-collapse: collapse;
    width: 80%;
    margin: 20px auto;
    background-color: #111;
    color: white;
    font-family: sans-serif;
  }

  th, td {
    border: 1px solid #888;
    padding: 10px;
    text-align: center;
  }

  th {
    background-color: #333;
    color: gold;
  }

  tr:hover {
    background-color: #222;
  }
</style>
```

---

## 🧠 טיפ

טבלאות הן לא רק להצגת נתונים – הן מצוינות גם לתפריטים של חנויות במשחקים, השוואות בין דמויות, וסטטיסטיקות מתקדמות!

```
