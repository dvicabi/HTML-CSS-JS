# 📊 תגית `<table>` – טבלאות ב־HTML (חלק 2 מתוך 2)

---

## 🔗 מיזוג עמודות (`colspan`)

```html
<table border="1">
  <tr>
    <th colspan="3">🏆 תוצאות קרב</th>
  </tr>
  <tr>
    <th>שחקן</th>
    <th>נזק</th>
    <th>מצב</th>
  </tr>
  <tr>
    <td>דביר</td>
    <td>100</td>
    <td>מנצח 🎉</td>
  </tr>
</table>
````

🔹 `colspan="3"` ממזג 3 תאים אופקית לכותרת אחת מרכזית.

---

## 🔗 מיזוג שורות (`rowspan`)

```html
<table border="1">
  <tr>
    <th rowspan="2">🧙‍♂️ שחקן</th>
    <th colspan="2">נתונים</th>
  </tr>
  <tr>
    <th>חיים</th>
    <th>אנרגיה</th>
  </tr>
  <tr>
    <td rowspan="2">דביר</td>
    <td>3</td>
    <td>80</td>
  </tr>
  <tr>
    <td>2</td>
    <td>95</td>
  </tr>
</table>
```

🔸 `rowspan="2"` ממזג תאים אנכית לאורך שתי שורות.

---

## 🧩 טבלה מקוננת (טבלה בתוך תא)

```html
<table border="1">
  <tr>
    <th>🎒 חפצים</th>
    <th>תכונות</th>
  </tr>
  <tr>
    <td>שיקוי</td>
    <td>
      <table border="1">
        <tr>
          <td>סוג</td>
          <td>ריפוי</td>
        </tr>
        <tr>
          <td>חוזק</td>
          <td>+50 HP</td>
        </tr>
      </table>
    </td>
  </tr>
</table>
```

🧠 שימושי להצגת מידע מרובה בתוך תא אחד (כמו סטטיסטיקות חפץ או כישוף).

---

## 🎨 עיצוב מתקדם

```html
<style>
  .stats-table {
    width: 100%;
    border-collapse: collapse;
    font-family: 'Courier New', monospace;
  }

  .stats-table th {
    background-color: #2e2e2e;
    color: #00ffd0;
    font-size: 1.1em;
    padding: 8px;
  }

  .stats-table td {
    padding: 6px;
    text-align: center;
    background-color: #1a1a1a;
    color: #fff;
  }

  .stats-table tr:nth-child(even) {
    background-color: #222;
  }

  .stats-table tr:hover {
    background-color: #333;
  }
</style>

<table class="stats-table">
  <tr>
    <th>🧝 דמות</th>
    <th>חיים</th>
    <th>כוח</th>
  </tr>
  <tr>
    <td>שדון</td>
    <td>5</td>
    <td>40</td>
  </tr>
  <tr>
    <td>אביר</td>
    <td>8</td>
    <td>70</td>
  </tr>
</table>
```

---

## 🧠 טיפ מתקדם למפתחי משחקים

טבלה יכולה לשמש גם ל־:

* תפריט חנות עם מחירים
* סיכום שלבים
* מערך של משימות עם סטטוס
* שילוב בין `<img>` לטבלת דמויות 🎮

