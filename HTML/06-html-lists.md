# 📝 רשימות ב־HTML – כל הסוגים והשימושים (מימוש מלא)

---

## 🔹 רשימה לא ממוספרת `<ul>`

```html
<ul>
  <li>🧪 שיקוי חיים</li>
  <li>🗡️ חרב ברזל</li>
  <li>🛡️ מגן קרח</li>
</ul>
````

* `ul` = unordered list – ללא מספרים
* `li` = list item – כל פריט

---

## 🔹 רשימה ממוספרת `<ol>`

```html
<ol>
  <li>🎯 התחל משימה</li>
  <li>🧭 מצא את המפה</li>
  <li>🚪 פתח את השער הסודי</li>
</ol>
```

* `ol` = ordered list – עם מספרים לפי הסדר

---

## 🔹 סוגי מספור לרשימה ממוספרת (`type`)

```html
<ol type="1">  <!-- 1, 2, 3 -->
<ol type="A">  <!-- A, B, C -->
<ol type="a">  <!-- a, b, c -->
<ol type="I">  <!-- I, II, III -->
<ol type="i">  <!-- i, ii, iii -->
```

```html
<ol type="A">
  <li>שלב א</li>
  <li>שלב ב</li>
  <li>שלב ג</li>
</ol>
```

---

## 🔹 התחלת מספור ממספר מסוים (`start`)

```html
<ol start="5">
  <li>שלב 5</li>
  <li>שלב 6</li>
</ol>
```

---

## 🔹 רשימה מקוננת (רשימה בתוך רשימה)

```html
<ul>
  <li>🧙‍♂️ קוסם
    <ul>
      <li>כישוף אש</li>
      <li>כישוף קרח</li>
    </ul>
  </li>
  <li>🛡️ לוחם
    <ul>
      <li>חרב כבדה</li>
      <li>מגן זהב</li>
    </ul>
  </li>
</ul>
```

---

## 🎨 עיצוב מותאם לרשימות

```html
<style>
  ul.custom {
    list-style-type: "🎮 ";
    padding-left: 20px;
  }

  ol.custom {
    list-style-type: upper-roman;
    color: gold;
  }

  li {
    margin: 6px 0;
    font-family: "Segoe UI", sans-serif;
  }
</style>

<ul class="custom">
  <li>אסוף זהב</li>
  <li>שדרג נשק</li>
  <li>מצא שיקויים</li>
</ul>
```

---

## 🧠 שימושים לילדים שמפתחים משחקים:

* ✅ צ'ק ליסט של משימות
* 🛒 רשימת קניות בחנות
* 🕹️ תפריט אפשרויות
* 📜 סיכום שלבי המשחק
* 🧠 קונספטים של עץ מיומנויות (נלמד בהמשך עם `<details>`)

```
