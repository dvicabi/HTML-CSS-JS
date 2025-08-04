🔹 **🔸 קטגוריה: תגיות מבנה בסיסי (Structural Elements)**

| תגית        | תיאור                          | דוגמה                                                    |
| ----------- | ------------------------------ | -------------------------------------------------------- |
| `<header>`  | כותרת עמוד או אזור ראשי        | `<header><h1>ברוכים הבאים</h1></header>`                 |
| `<nav>`     | ניווט בין עמודים/קטעים         | `<nav><a href="#">בית</a> <a href="#">צור קשר</a></nav>` |
| `<main>`    | התוכן המרכזי של העמוד          | `<main><h2>מאמר ראשי</h2></main>`                        |
| `<section>` | קטע נפרד בעמוד (כמו פרק)       | `<section><h3>על אודות</h3><p>...</p></section>`         |
| `<article>` | יחידת תוכן עצמאית (כמו פוסט)   | `<article><h2>פוסט</h2></article>`                       |
| `<aside>`   | תוכן צדדי, כמו סרגל צד         | `<aside><p>פרסומת</p></aside>`                           |
| `<footer>`  | תחתית עמוד/קטע                 | `<footer><p>© 2025 דביר</p></footer>`                    |
| `<div>`     | בלוק כללי ללא משמעות סמנטית    | `<div class="קופסא">...</div>`                           |
| `<span>`    | תגית אינליין ללא משמעות סמנטית | `<span style="color:red">טקסט אדום</span>`               |

---

🔹 **🔸 קטגוריה: תגיות טקסט וכותרות**

| תגית              | תיאור                  | דוגמה                                                 |
| ----------------- | ---------------------- | ----------------------------------------------------- |
| `<h1>` – `<h6>`   | כותרות בדרגות שונות    | `<h1>כותרת ראשית</h1>`                                |
| `<p>`             | פסקה                   | `<p>זהו טקסט בפסקה.</p>`                              |
| `<br>`            | ירידת שורה             | `שלום<br>עולם`                                        |
| `<hr>`            | קו אופקי מפריד         | `<hr>`                                                |
| `<blockquote>`    | ציטוט חיצוני           | `<blockquote>ציטוט גדול</blockquote>`                 |
| `<q>`             | ציטוט בתוך שורה        | `<q>אמרו לי שזה נכון</q>`                             |
| `<pre>`           | טקסט עם עימוד כפי שהוא | `<pre>   טקסט מיושר</pre>`                            |
| `<code>`          | קוד תוכנה              | `<code>print("Hello")</code>`                         |
| `<kbd>`           | קיצור מקשים            | `<kbd>Ctrl</kbd> + <kbd>C</kbd>`                      |
| `<mark>`          | סימון/הדגשה של טקסט    | `<mark>חשוב</mark>`                                   |
| `<strong>`        | הדגשה משמעותית (SEO)   | `<strong>הערה חשובה</strong>`                         |
| `<em>`            | הדגשה טונאלית          | `<em>מושג</em>`                                       |
| `<small>`         | טקסט מוקטן             | `<small>הערה שולית</small>`                           |
| `<sub>` / `<sup>` | טקסט תחתון/עליון       | `H<sub>2</sub>O` או `X<sup>2</sup>`                   |
| `<abbr>`          | קיצור + משמעות         | `<abbr title="HyperText Markup Language">HTML</abbr>` |
| `<bdo>`           | שינוי כיוון טקסט       | `<bdo dir="rtl">Right to Left</bdo>`                  |

---

🔹 **🔸 קטגוריה: תגיות קישורים ומדיה**

| תגית       | תיאור                                          | דוגמה                                                                    |
| ---------- | ---------------------------------------------- | ------------------------------------------------------------------------ |
| `<a>`      | קישור                                          | `<a href="https://google.com">לגוגל</a>`                                 |
| `<img>`    | תמונה                                          | `<img src="logo.png" alt="לוגו" width="100">`                            |
| `<audio>`  | קול/מוזיקה                                     | `<audio controls src="sound.mp3"></audio>`                               |
| `<video>`  | וידאו                                          | `<video controls width="320" src="video.mp4"></video>`                   |
| `<source>` | מקור לקובץ מדיה (בפנים של `<audio>`/`<video>`) | `<source src="media.mp3" type="audio/mp3">`                              |
| `<track>`  | כתוביות/תרגום בווידאו                          | `<track src="sub.vtt" kind="subtitles" srclang="he" label="עברית">`      |
| `<iframe>` | מסגרת פנימית לעמוד אחר                         | `<iframe src="https://example.com"></iframe>`                            |
| `<embed>`  | הטמעת קובץ (PDF, וידאו)                        | `<embed src="file.pdf" width="500">`                                     |
| `<object>` | קובץ מוטמע עם קונטרול                          | `<object data="file.swf" type="application/x-shockwave-flash"></object>` |


---

🔹 **🔸 קטגוריה: תגיות טפסים וקלט (Forms & Inputs)**

| תגית         | תיאור                 | דוגמה                                                                               |
| ------------ | --------------------- | ----------------------------------------------------------------------------------- |
| `<form>`     | טופס שליחה            | `<form action="/submit" method="POST">...</form>`                                   |
| `<input>`    | שדה קלט               | `<input type="text" name="username">`                                               |
| `<textarea>` | שדה טקסט רב שורות     | `<textarea rows="4" cols="30">הערה...</textarea>`                                   |
| `<button>`   | כפתור                 | `<button type="submit">שלח</button>`                                                |
| `<select>`   | רשימה נפתחת           | `<select><option>אופציה</option></select>`                                          |
| `<option>`   | פריט ברשימה נפתחת     | `<option value="1">אחד</option>`                                                    |
| `<optgroup>` | קיבוץ בתוך `<select>` | `<optgroup label="מספרים">...</optgroup>`                                           |
| `<label>`    | תווית לשדה            | `<label for="email">אימייל</label>`                                                 |
| `<fieldset>` | קיבוץ שדות בטופס      | `<fieldset><legend>פרטים</legend>...</fieldset>`                                    |
| `<legend>`   | כותרת לקבוצת שדות     | `<legend>פרטים אישיים</legend>`                                                     |
| `<datalist>` | רשימה של הצעות        | `<input list="browsers"><datalist id="browsers"><option value="Chrome"></datalist>` |
| `<output>`   | פלט מחושב             | `<output name="result">42</output>`                                                 |

---

🔹 **🔸 סוגי `<input type="...">` זמינים**

| סוג קלט                            | דוגמה                                               |
| ---------------------------------- | --------------------------------------------------- |
| `text`                             | `<input type="text">`                               |
| `email`                            | `<input type="email">`                              |
| `password`                         | `<input type="password">`                           |
| `number`                           | `<input type="number" min="0" max="100" step="5">`  |
| `range`                            | `<input type="range" min="0" max="100">`            |
| `search`                           | `<input type="search">`                             |
| `url`                              | `<input type="url">`                                |
| `tel`                              | `<input type="tel">`                                |
| `date` / `time` / `datetime-local` | `<input type="date">`                               |
| `month` / `week`                   | `<input type="month">`                              |
| `color`                            | `<input type="color">`                              |
| `checkbox`                         | `<input type="checkbox" checked>`                   |
| `radio`                            | `<input type="radio" name="gender" value="male">`   |
| `file`                             | `<input type="file" accept=".jpg,.png">`            |
| `hidden`                           | `<input type="hidden" name="token" value="abc123">` |
| `submit`                           | `<input type="submit" value="שלח">`                 |
| `reset`                            | `<input type="reset">`                              |
| `button`                           | `<input type="button" value="לחץ">`                 |
| `image`                            | `<input type="image" src="submit.png">`             |

---

🔹 **🔸 קטגוריה: רשימות (Lists)**

| תגית   | תיאור               | דוגמה                                      |
| ------ | ------------------- | ------------------------------------------ |
| `<ul>` | רשימה לא ממוספרת    | `<ul><li>תפוח</li></ul>`                   |
| `<ol>` | רשימה ממוספרת       | `<ol><li>שלב ראשון</li></ol>`              |
| `<li>` | פריט ברשימה         | `<li>פריט</li>`                            |
| `<dl>` | רשימה תיאורית       | `<dl><dt>HTML</dt><dd>שפת תגיות</dd></dl>` |
| `<dt>` | מונח ברשימה תיאורית | `<dt>CSS</dt>`                             |
| `<dd>` | תיאור למונח         | `<dd>עיצוב</dd>`                           |

---

🔹 **🔸 קטגוריה: טבלאות (Tables)**

| תגית              | תיאור              | דוגמה                                                   |
| ----------------- | ------------------ | ------------------------------------------------------- |
| `<table>`         | טבלה               | `<table>...</table>`                                    |
| `<thead>`         | אזור ראש טבלה      | `<thead><tr><th>כותרת</th></tr></thead>`                |
| `<tbody>`         | גוף הטבלה          | `<tbody><tr><td>נתון</td></tr></tbody>`                 |
| `<tfoot>`         | תחתית הטבלה        | `<tfoot><tr><td>סה״כ</td></tr></tfoot>`                 |
| `<tr>`            | שורת טבלה          | `<tr>...</tr>`                                          |
| `<th>`            | תא כותרת           | `<th>שם</th>`                                           |
| `<td>`            | תא רגיל            | `<td>דביר</td>`                                         |
| `<caption>`       | כותרת עליונה לטבלה | `<caption>טבלת ציונים</caption>`                        |
| `colgroup`, `col` | עיצוב טורים        | `<colgroup><col style="background:yellow;"></colgroup>` |

---


🔹 **🔸 קטגוריה: תגיות אינטראקטיביות (Interactive Elements)**

| תגית        | תיאור                  | דוגמה                                                           |
| ----------- | ---------------------- | --------------------------------------------------------------- |
| `<details>` | אזור שניתן לפתוח/לסגור | `<details><summary>הסבר</summary><p>פרטים נסתרים</p></details>` |
| `<summary>` | הכותרת של `<details>`  | `<summary>פתח מידע</summary>`                                   |
| `<dialog>`  | תיבת דו־שיח (מודאל)    | `<dialog open>שלום!</dialog>`                                   |

---

🔹 **🔸 קטגוריה: תגיות Canvas, SVG, ואובייקטים גרפיים**

| תגית                                | תיאור                    | דוגמה                                                                              |
| ----------------------------------- | ------------------------ | ---------------------------------------------------------------------------------- |
| `<canvas>`                          | קנבס לציור עם JavaScript | `<canvas id="myCanvas" width="300" height="150"></canvas>`                         |
| `<svg>`                             | גרפיקה וקטורית           | `<svg width="100" height="100"><circle cx="50" cy="50" r="40" fill="red" /></svg>` |
| `<circle>`, `<rect>`, `<line>` וכו' | צורות בתוך SVG           | `<circle cx="50" cy="50" r="40"/>`                                                 |
| `<object>`                          | הטמעת קובץ חיצוני        | `<object data="chart.svg" type="image/svg+xml"></object>`                          |
| `<embed>`                           | הטמעת מדיה (כמו PDF)     | `<embed src="example.pdf" type="application/pdf" width="600" height="500">`        |
| `<iframe>`                          | טעינת אתר בתוך עמוד      | `<iframe src="https://example.com" width="300"></iframe>`                          |

---

🔹 **🔸 קטגוריה: סקריפטים וטעינת קוד**

| תגית         | תיאור                                 | דוגמה                                                                 |
| ------------ | ------------------------------------- | --------------------------------------------------------------------- |
| `<script>`   | סקריפט JS פנימי או חיצוני             | `<script src="main.js" defer></script>`                               |
| `<noscript>` | תוכן למקרה שאין תמיכה ב-JS            | `<noscript>יש לאפשר JavaScript כדי להמשיך</noscript>`                 |
| `<template>` | תבנית HTML לא פעילה (נטענת רק דרך JS) | `<template id="card-template"><div class="card">...</div></template>` |
| `<slot>`     | מקום לתוכן דינמי בתוך Web Component   | `<slot name="title"></slot>`                                          |

---

🔹 **🔸 קטגוריה: תגיות גישה, ARIA ודינמיקה מתקדמת**

| תגית       | תיאור                                               | דוגמה                                    |
| ---------- | --------------------------------------------------- | ---------------------------------------- |
| `aria-*`   | מאפיינים לשיפור נגישות (ללא תגית נפרדת, אלא כתכונה) | `<div aria-label="תפריט ראשי">...</div>` |
| `tabindex` | שליטה על סדר ניווט בטאב                             | `<div tabindex="0">טאב ראשון</div>`      |
| `role`     | תיאור תפקידי לאובייקטים (לנגישות)                   | `<section role="region">...</section>`   |

---

🔹 **🔸 קטגוריה: תגיות Deprecated (לא מומלצות אך קיימות)**

| תגית        | מצב                             | דוגמה                           |
| ----------- | ------------------------------- | ------------------------------- |
| `<font>`    | לא מומלץ – עיצוב עובר ל־CSS     | `<font color="red">טקסט</font>` |
| `<center>`  | לא מומלץ – השתמש ב־CSS          | `<center>מרוכז</center>`        |
| `<b>`       | השתמש ב־`<strong>`              | `<b>מודגש</b>`                  |
| `<i>`       | השתמש ב־`<em>`                  | `<i>נטוי</i>`                   |
| `<u>`       | השתמש ב־CSS (`text-decoration`) | `<u>קו תחתון</u>`               |
| `<marquee>` | לא תקני – טקסט נע               | `<marquee>נע ימינה</marquee>`   |
| `<blink>`   | לא נתמך ברוב הדפדפנים           | `<blink>מהבהב</blink>`          |

---

