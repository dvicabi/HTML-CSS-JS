## 🔷 חלק 1: מבנה עמוד, כותרות, טקסטים בסיסיים

```html
<body>

  <!-- 🟦 כותרות H1–H6 (סמנטיקה לפי סדר חשיבות) -->
  <h1>כותרת ראשית</h1> <!-- יש רק אחת כזו לעמוד -->
  <h2>כותרת משנית</h2>
  <h3>כותרת תוכן פנימי</h3>
  <h4>כותרת רמה 4</h4>
  <h5>כותרת רמה 5</h5>
  <h6>כותרת רמה 6</h6>

  <!-- 🟦 <p>: פסקה רגילה -->
  <p>פסקת טקסט רגילה עם תוכן בסיסי.</p>

  <!-- 🟦 <br>: ירידת שורה בודדת בתוך פסקה -->
  שורה ראשונה<br>שורה שנייה

  <!-- 🟦 <hr>: קו אופקי להפרדה -->
  <hr>

  <!-- 🟦 טקסטים עם משמעויות סמנטיות -->
  <strong>טקסט חשוב (גם ל־SEO)</strong>
  <em>הדגשה טונאלית (כמו באינטונציה)</em>
  <mark>טקסט מסומן (צהוב)</mark>
  <small>טקסט מוקטן (הערה/כיתוב)</small>
  <sub>טקסט תחתי (כמו H<sub>2</sub>O)</sub>
  <sup>טקסט עליון (כמו X<sup>2</sup>)</sup>
  <abbr title="HyperText Markup Language">HTML</abbr> <!-- מציג הסבר בהצבעה -->
  <bdo dir="rtl">שינוי כיוון טקסט לימין</bdo>
```

---

## 🔷 חלק 2: קוד, ציטוטים ויישור טקסט

```html
  <!-- 🟦 <code>: קוד תכנות -->
  <code>console.log("Hello Dvir")</code>

  <!-- 🟦 <kbd>: קיצור מקשים (למשל Ctrl+C) -->
  <kbd>Ctrl</kbd> + <kbd>C</kbd>

  <!-- 🟦 <pre>: טקסט מיושר בדיוק כפי שנכתב -->
  <pre>
    שורה אחת
      רווח פנימי נשמר
  </pre>

  <!-- 🟦 <blockquote>: ציטוט חיצוני -->
  <blockquote cite="https://example.com">
    ציטוט מתוך מאמר אחר
  </blockquote>

  <!-- 🟦 <q>: ציטוט קצר בתוך משפט -->
  <p><q>ציטוט קצר</q> באמצע משפט</p>
```

---

## 🔷 חלק 3: מבנה עמוד סמנטי (החלקים הגדולים)

```html
  <!-- 🟩 <header>: אזור כותרת עמוד (בדרך כלל עם לוגו/תפריט) -->
  <header>
    <h1>ברוכים הבאים לאתר שלי</h1>
  </header>

  <!-- 🟩 <nav>: אזור ניווט – תמיד מופיע עם קישורים -->
  <nav>
    <a href="#home">דף הבית</a>
    <a href="#about">אודות</a>
  </nav>

  <!-- 🟩 <main>: התוכן המרכזי של הדף – מותר אחד בלבד -->
  <main>
    <p>זהו התוכן המרכזי של הדף.</p>
  </main>

  <!-- 🟩 <section>: חלוקה נושאית – באה עם <h2> ומעלה -->
  <section>
    <h2>שירותים</h2>
    <p>הסבר על השירותים.</p>
  </section>

  <!-- 🟩 <article>: יחידת תוכן עצמאית – פוסט, תגובה, כתבה -->
  <article>
    <h2>פוסט: למה HTML זה מדהים</h2>
    <p>בפוסט הזה נדבר על...</p>
  </article>

  <!-- 🟩 <aside>: תוכן צדדי – לרוב פרסומות או מידע משלים -->
  <aside>
    <p>פרסומת צדדית או טיפים שימושיים</p>
  </aside>

  <!-- 🟩 <footer>: תחתית עמוד או קטע -->
  <footer>
    <p>© 2025 כל הזכויות שמורות לדביר כבשה</p>
  </footer>

  <!-- 🟩 <div>: קופסה כללית – אינה סמנטית -->
  <div class="box">
    <p>אני div רגיל, נהדר לעיצוב</p>
  </div>

  <!-- 🟩 <span>: אינליין, לתוך טקסט רגיל -->
  <p>זהו טקסט עם <span style="color:blue;">מילה כחולה</span> באמצע</p>
```

## 🔷 חלק 4: קישורים, תמונות, מדיה

```html
  <!-- 🔹 <a>: קישור – תמיד בא עם href. ניתן להוסיף:
        target="_blank" לפתיחה בטאב חדש
        rel="noopener noreferrer" לביטחון -->
  <a href="https://www.example.com" target="_blank" rel="noopener noreferrer">
    מעבר לאתר חיצוני
  </a>

  <!-- 🔹 <img>: תמונה – תכונות חשובות:
        src – כתובת התמונה
        alt – טקסט חלופי (לנגישות ו-SEO)
        width / height – מימדים בפיקסלים
        loading="lazy" – טעינה עצלה -->
  <img src="logo.png" alt="לוגו החברה" width="150" height="150" loading="lazy">

  <!-- 🔹 <picture> + <source> + <img>: באים יחד – תמונות רספונסיביות לפי מדיה -->
  <picture>
    <source srcset="logo-large.png" media="(min-width: 800px)">
    <source srcset="logo-small.png" media="(max-width: 799px)">
    <img src="logo-fallback.png" alt="לוגו מותאם">
  </picture>

  <!-- 🔹 <audio>: נגינת קול – פרופרטיז:
        controls – מציג כפתורים
        autoplay – מתחיל לנגן אוטומטית
        loop – מנגן בלופ
        muted – שקט כברירת מחדל
        preload – כיצד לטעון: none / metadata / auto -->
  <audio src="sound.mp3" controls autoplay loop muted preload="auto"></audio>

  <!-- 🔹 <video>: נגן וידאו – אותם פרופרטיז כמו <audio> +
        width/height – מימדים
        poster – תמונה לפני התחלת וידאו -->
  <video src="video.mp4" controls autoplay loop muted width="320" height="240" poster="preview.jpg"></video>

  <!-- 🔹 <source>: תוויות קובץ חלופי – בתוך <audio> או <video> בלבד -->
  <video controls>
    <source src="video.webm" type="video/webm">
    <source src="video.mp4" type="video/mp4">
    הדפדפן לא תומך בוידאו
  </video>

  <!-- 🔹 <track>: כתוביות לווידאו – באה בתוך <video> -->
  <video controls>
    <source src="video.mp4" type="video/mp4">
    <track src="subtitles.vtt" kind="subtitles" srclang="he" label="עברית">
  </video>

  <!-- 🔹 <iframe>: הטמעת עמוד פנימי – תכונות:
        src – כתובת
        width/height – גודל
        title – חובה לנגישות
        loading="lazy" – שיפור ביצועים -->
  <iframe src="https://www.example.com" width="600" height="400" title="עמוד מוטמע" loading="lazy"></iframe>

  <!-- 🔹 <embed>: הטמעת תוכן – קבצים חיצוניים (PDF, סרטים) -->
  <embed src="document.pdf" type="application/pdf" width="500" height="600">

  <!-- 🔹 <object>: דומה ל-embed, עם שליטה על התוכן הפנימי -->
  <object data="file.svg" type="image/svg+xml" width="300" height="300">
    קובץ לא נטען
  </object>
```

---

## 🔷 חלק 5: טפסים וקלט

```html
  <!-- 🔹 <form>: טופס שליחה – בא עם:
        action – כתובת שליחה
        method – GET / POST -->
  <form action="/submit" method="POST">

    <!-- 🔸 <fieldset> + <legend> באים יחד – מסגרת לקבוצת שדות -->
    <fieldset>
      <legend>פרטי משתמש</legend>

      <!-- 🔹 <label>: תווית לשדה – באה עם for שתואם ל־id -->
      <label for="name">שם מלא:</label>

      <!-- 🔹 <input>: שדה קלט – כל פרופרטי משתנה לפי type -->
      <input
        type="text"     <!-- סוג הקלט -->
        id="name"       <!-- מזהה ייחודי -->
        name="name"     <!-- שם שדה – חובה כדי שיישלח -->
        placeholder="הכנס שם מלא"
        required        <!-- חובה למלא -->
        minlength="2"   <!-- מינימום תווים -->
        maxlength="50"  <!-- מקסימום תווים -->
      >

      <label for="email">אימייל:</label>
      <input
        type="email"
        id="email"
        name="email"
        placeholder="you@example.com"
        required
      >

      <!-- 🔹 <textarea>: שדה טקסט רב־שורות -->
      <label for="message">הודעה:</label>
      <textarea
        id="message"
        name="message"
        rows="4"
        cols="50"
        placeholder="כתוב כאן את ההודעה שלך..."
      ></textarea>

      <!-- 🔹 <select>: תפריט נפתח -->
      <label for="language">בחר שפה:</label>
      <select name="language" id="language" required>
        <!-- 🔸 <optgroup> + <option> – באים יחד כקבוצות -->
        <optgroup label="Frontend">
          <option value="html">HTML</option>
          <option value="css">CSS</option>
        </optgroup>
        <optgroup label="Backend">
          <option value="python">Python</option>
          <option value="node">Node.js</option>
        </optgroup>
      </select>

      <!-- 🔹 checkbox / radio – חובה name ותיאום -->
      <p>בחר מין:</p>
      <input type="radio" id="male" name="gender" value="male" checked>
      <label for="male">זכר</label>
      <input type="radio" id="female" name="gender" value="female">
      <label for="female">נקבה</label>

      <p>תחומי עניין:</p>
      <input type="checkbox" id="ai" name="interests" value="ai" checked>
      <label for="ai">בינה מלאכותית</label>
      <input type="checkbox" id="web" name="interests" value="web">
      <label for="web">פיתוח אתרים</label>

      <!-- 🔹 כפתורי שליחה ואיפוס -->
      <input type="submit" value="שלח טופס">
      <input type="reset" value="אפס טופס">

    </fieldset>
  </form>

  <!-- 🔹 <datalist>: רשימת הצעות עבור <input list="..."> -->
  <label for="browser">בחר דפדפן:</label>
  <input list="browsers" id="browser" name="browser">
  <datalist id="browsers">
    <option value="Chrome">
    <option value="Firefox">
    <option value="Edge">
  </datalist>

  <!-- 🔹 <output>: הצגת תוצאה מחישוב – יכול להיות מקושר ל-JavaScript -->
  <label>תוצאה:</label>
  <output name="result" id="result">0</output>
```

---
# 🔷 חלק 6: רשימות וטבלאות
## 🔷 חלק 6.1: רשימות (Lists)

```html
  <!-- 🔹 <ul>: רשימה לא ממוספרת – באה עם <li> -->
  <ul>
    <li>תפוח</li>
    <li>בננה</li>
    <li>אגס</li>
  </ul>

  <!-- 🔹 <ol>: רשימה ממוספרת – באה עם <li>
        תכונות:
        type – סוג המספור: 1 / A / a / I / i
        start – מאיזה מספר להתחיל
        reversed – רשימה יורדת -->
  <ol type="A" start="3" reversed>
    <li>שלב ראשון</li>
    <li>שלב שני</li>
  </ol>

  <!-- 🔹 <li>: פריט ברשימה – משמש בתוך <ul> או <ol> בלבד -->

  <!-- 🔹 <dl>: רשימה תיאורית – באה עם <dt> + <dd> -->
  <dl>
    <dt>HTML</dt>     <!-- Term – מונח -->
    <dd>שפת תגיות</dd> <!-- Description – הגדרה -->
    <dt>CSS</dt>
    <dd>שפת עיצוב</dd>
  </dl>
```

---

## 🔷 חלק 6.2: טבלאות (Tables)

```html
  <!-- 🔹 <table>: טבלה – כוללת שורות, תאים, כותרות -->
  <table border="1">

    <!-- 🔹 <caption>: כותרת עליונה לטבלה -->
    <caption>טבלת ציונים</caption>

    <!-- 🔹 <thead> + <tbody> + <tfoot>: אזורים בטבלה – באים יחד -->
    <thead>
      <tr>
        <th scope="col">שם</th>     <!-- תא כותרת לטור -->
        <th scope="col">ציון</th>
      </tr>
    </thead>

    <tbody>
      <tr>
        <td>דביר</td>               <!-- תא רגיל -->
        <td>100</td>
      </tr>
      <tr>
        <td>יוסי</td>
        <td>95</td>
      </tr>
    </tbody>

    <tfoot>
      <tr>
        <td colspan="2">סה״כ: שני תלמידים</td> <!-- colspan – מיזוג עמודות -->
      </tr>
    </tfoot>
  </table>

  <!-- 🔹 תכונות נוספות לטבלאות:
        cellspacing / cellpadding – מרווחים (לא מומלץ – ב־CSS)
        width / height – גודל (עדיף ב־CSS)
        rowspan – מיזוג שורות -->
  <table border="1">
    <tr>
      <th rowspan="2">שם</th>
      <td>דביר</td>
    </tr>
    <tr>
      <td>יוסי</td>
    </tr>
  </table>

  <!-- 🔹 <colgroup> + <col>: עיצוב טורים – באים יחד -->
  <table border="1">
    <colgroup>
      <col style="background-color: #eee">
      <col style="background-color: #ddd">
    </colgroup>
    <tr><th>שם</th><th>גיל</th></tr>
    <tr><td>דביר</td><td>25</td></tr>
  </table>
```
---
# **חלק 7: אינטראקטיביות ו־UI מתקדם**

## 🔷 חלק 7.1: `<details>` + `<summary>` (באים תמיד ביחד)

```html
  <!-- 🔹 <details>: קופסה נפתחת/נסגרת – מגיעה יחד עם <summary>
       פרופרטיז:
       open – מציין שהתיבה פתוחה כברירת מחדל -->
  <details open> <!-- מופיע פתוח כברירת מחדל -->
    <summary>לחץ כאן לפרטים</summary> <!-- תמיד בא יחד -->
    <p>זהו המידע הנוסף שניתן להסתיר או להציג לפי בחירה.</p>
  </details>
```

---

## 🔷 חלק 7.2: `<dialog>` – תיבת דו־שיח מודאלית

```html
  <!-- 🔹 <dialog>: תיבת פופאפ – אפשר לפתוח/לסגור עם JS
       פרופרטיז:
       open – אם מופיע בעמוד, התיבה מוצגת -->
  <dialog open>
    <p>שלום! זו הודעה קופצת.</p>
    <button onclick="this.closest('dialog').close()">סגור</button>
  </dialog>

  <!-- 🔸 פתיחה באמצעות JavaScript:
       document.getElementById('myDialog').showModal(); -->
```

---

## 🔷 חלק 7.3: `<meter>` – מד מדידה (כמו סוללה, חום)

```html
  <!-- 🔹 <meter>: מציג ערך בתחום מסוים – לא להתקדמות אלא למדידה יחסית
       פרופרטיז:
       min / max – התחום הכללי
       value – הערך הנוכחי
       low / high / optimum – טווחים משמעותיים (לצבעים) -->
  <label for="battery">רמת סוללה:</label>
  <meter id="battery" min="0" max="100" low="20" high="80" optimum="100" value="65">
    65%
  </meter>
```

---

## 🔷 חלק 7.4: `<progress>` – פס התקדמות (דינמי או קבוע)

```html
  <!-- 🔹 <progress>: מציג התקדמות של תהליך
       פרופרטיז:
       value – כמה התקדם
       max – מה היעד הסופי -->
  <label for="upload">העלאה מתבצעת:</label>
  <progress id="upload" value="30" max="100">30%</progress>
```

---

## 🔷 חלק 7.5: הרחבה ל־`<output>` – תוצאה מחישוב

```html
  <!-- 🔹 <output>: מציג תוצאה (למשל חישוב) – ניתן לחבר לפקדים -->
  <form oninput="res.value = parseInt(a.value) + parseInt(b.value)">
    <input type="number" id="a" value="5"> +
    <input type="number" id="b" value="3"> =
    <output name="res" for="a b">8</output>
  </form>
```

---

## 🔷 חלק 7.6: חיזוק ל־`<fieldset>` + `<legend>` – כוסה קודם, אך שוב כאן

```html
  <!-- 🔹 <fieldset>: קבוצת שדות – יוצרת מסגרת עם כותרת -->
  <fieldset>
    <legend>פרטי התחברות</legend> <!-- תמיד בא עם fieldset -->
    <label for="user">שם משתמש:</label>
    <input id="user" type="text" name="user">
  </fieldset>
```

---


# **חלק 8: גרפיקה וציור – `<canvas>` ו־`<svg>`**

## 🔷 חלק 8.1: `<canvas>` – ציור עם JavaScript

```html
  <!-- 🔹 <canvas>: אזור ציור – מייצג קנבס ריק לציור עם JavaScript
       פרופרטיז:
       id – לזיהוי בקוד JS
       width / height – גודל הקנבס בפיקסלים (לא ב־CSS!) -->
  <canvas id="myCanvas" width="300" height="150">
    הדפדפן שלך אינו תומך ב־Canvas.
  </canvas>

  <!-- 🔸 בשימוש עם JavaScript:
       const ctx = document.getElementById('myCanvas').getContext('2d');
       ctx.fillStyle = 'red';
       ctx.fillRect(0, 0, 150, 75); -->
```

---

## 🔷 חלק 8.2: `<svg>` – גרפיקה וקטורית (Scalable Vector Graphics)

```html
  <!-- 🔹 <svg>: גרפיקה בקוד – כולל child elements לציור
       פרופרטיז:
       width / height – גודל
       viewBox – התאמה רספונסיבית -->
  <svg width="200" height="200" viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
```

---

### 📦 Child Elements בתוך `<svg>` – באים יחד!

```html
    <!-- 🔹 <circle>: עיגול
         cx / cy – מיקום המרכז
         r – רדיוס
         fill – צבע פנימי -->
    <circle cx="100" cy="100" r="50" fill="blue" />

    <!-- 🔹 <rect>: מלבן
         x / y – מיקום
         width / height – מידות
         rx / ry – פינות מעוגלות -->
    <rect x="20" y="20" width="50" height="50" fill="red" rx="10" ry="10" />

    <!-- 🔹 <line>: קו
         x1/y1 – נקודת התחלה
         x2/y2 – נקודת סיום -->
    <line x1="0" y1="0" x2="200" y2="200" stroke="black" stroke-width="2" />

    <!-- 🔹 <ellipse>: אליפסה -->
    <ellipse cx="100" cy="50" rx="50" ry="25" fill="green" />

    <!-- 🔹 <polygon>: מצולע סגור לפי נקודות -->
    <polygon points="60,20 100,40 100,80 60,100 20,80 20,40" fill="purple" />

    <!-- 🔹 <polyline>: קווים מחוברים – לא סגור -->
    <polyline points="0,0 50,25 50,75 100,100" fill="none" stroke="orange" />

    <!-- 🔹 <path>: צורת Freeform מורכבת מאוד -->
    <path d="M10 80 C 40 10, 65 10, 95 80 S 150 150, 180 80" stroke="black" fill="transparent" />

    <!-- 🔹 <text>: טקסט בתוך SVG -->
    <text x="50" y="50" font-family="Verdana" font-size="20" fill="black">שלום SVG</text>

    <!-- 🔹 <g>: קיבוץ של אלמנטים – עם style משותף -->
    <g fill="gray" stroke="black">
      <circle cx="30" cy="30" r="10" />
      <circle cx="60" cy="30" r="10" />
    </g>
```

---

### 🧩 שיתוף קוד, שימוש חוזר:

```html
    <!-- 🔹 <defs>: הגדרות שלא מוצגות – בא עם <symbol>, <linearGradient>, וכו' -->
    <defs>
      <circle id="dot" r="5" fill="blue" />
    </defs>

    <!-- 🔹 <use>: שימוש חוזר בקוד מתוך <defs> -->
    <use href="#dot" x="100" y="100" />
    <use href="#dot" x="120" y="120" />

    <!-- 🔹 <symbol>: אייקון לשימוש חוזר -->
    <symbol id="icon-heart" viewBox="0 0 100 100">
      <path d="..."/>
    </symbol>
    <use href="#icon-heart" x="0" y="0" width="50" height="50"/>
```

---

### 🧩 תוספות SVG מתקדמות:

```html
    <!-- 🔹 <foreignObject>: לשלב HTML בתוך SVG -->
    <foreignObject x="20" y="20" width="160" height="100">
      <body xmlns="http://www.w3.org/1999/xhtml">
        <p style="font-size: 14px;">טקסט רגיל בתוך SVG!</p>
      </body>
    </foreignObject>
  </svg>
```

---

# **חלק 9: סקריפטים, תבניות ודינמיקה מתקדמת**
## 🔷 חלק 9.1: `<script>` – טעינת קוד JavaScript

```html
  <!-- 🔹 <script>: משמש לטעינת קוד JavaScript
       בא גם בתור inline וגם עם src.
       פרופרטיז:
       src – קובץ חיצוני
       type – סוג הסקריפט (למשל module)
       defer – טוען את הסקריפט רק אחרי שהעמוד נטען
       async – טוען במקביל (לא שומר סדר!)
       integrity – hash לאבטחת הקובץ
       crossorigin – שליטה בבקשות חוצות דומיין
       nomodule – לסקריפטים חלופיים לדפדפנים ישנים -->
  
  <!-- 📦 דוגמה עם defer (שומר על הסדר, מומלץ ל־HTML מודרני): -->
  <script src="script.js" defer></script>

  <!-- 📦 דוגמה עם async (עשוי להריץ סקריפט לפני שאר הסקריפטים): -->
  <script src="analytics.js" async></script>

  <!-- 📦 סקריפט מודולרי (ES6) – עם type="module": -->
  <script type="module" src="module.js"></script>

  <!-- 📦 סקריפט fallback לדפדפנים שלא תומכים במודולים – nomodule: -->
  <script nomodule src="legacy.js"></script>

  <!-- 📦 סקריפט עם hash לאימות (Content Integrity): -->
  <script src="cdn-script.js"
          integrity="sha384-x123..."
          crossorigin="anonymous"></script>

  <!-- 📦 סקריפט פנימי בתוך הדף: -->
  <script>
    console.log('קוד JavaScript נטען');
  </script>
```

---

## 🔷 חלק 9.2: `<noscript>` – תוכן למשתמשים ללא JavaScript

```html
  <!-- 🔹 <noscript>: מוצג רק אם JavaScript לא פעיל בדפדפן -->
  <noscript>
    <p>אנא אפשר JavaScript כדי להשתמש באתר.</p>
  </noscript>
```

---

## 🔷 חלק 9.3: `<template>` – תבנית HTML שלא נטענת אוטומטית

```html
  <!-- 🔹 <template>: HTML שמופעל רק דרך JavaScript
       לא מוצג בדף – מתאים ליצירת מרכיבים דינמיים -->
  <template id="card-template">
    <div class="card">
      <h3>כותרת כרטיס</h3>
      <p>תוכן כרטיס</p>
    </div>
  </template>

  <!-- 📦 בשימוש עם JavaScript:
       const tpl = document.getElementById('card-template');
       const clone = tpl.content.cloneNode(true);
       document.body.appendChild(clone); -->
```

---

## 🔷 חלק 9.4: `<slot>` – מקום לתוכן חיצוני בתוך Web Component

```html
  <!-- 🔹 <slot>: משמש בתוך Web Component – מחליף מקום שמוזן מבחוץ -->
  <template id="my-component">
    <div class="box">
      <slot name="title">כותרת ברירת מחדל</slot>
      <slot name="content"></slot>
    </div>
  </template>

  <!-- 📦 בשימוש: -->
  <my-component>
    <h1 slot="title">ברוך הבא</h1>
    <p slot="content">זהו התוכן שלך</p>
  </my-component>
```

---


מצוין דביר! הנה 🔷 **חלק 9: סקריפטים, תבניות ודינמיקה מתקדמת**
נכסה כאן את כל תגיות השליטה והאינטגרציה ב־JavaScript ו־Web Components – כולל כל פרופרטי והקשרים ביניהם.

---

## 🔷 חלק 9.1: `<script>` – טעינת קוד JavaScript

```html
  <!-- 🔹 <script>: משמש לטעינת קוד JavaScript
       בא גם בתור inline וגם עם src.
       פרופרטיז:
       src – קובץ חיצוני
       type – סוג הסקריפט (למשל module)
       defer – טוען את הסקריפט רק אחרי שהעמוד נטען
       async – טוען במקביל (לא שומר סדר!)
       integrity – hash לאבטחת הקובץ
       crossorigin – שליטה בבקשות חוצות דומיין
       nomodule – לסקריפטים חלופיים לדפדפנים ישנים -->
  
  <!-- 📦 דוגמה עם defer (שומר על הסדר, מומלץ ל־HTML מודרני): -->
  <script src="script.js" defer></script>

  <!-- 📦 דוגמה עם async (עשוי להריץ סקריפט לפני שאר הסקריפטים): -->
  <script src="analytics.js" async></script>

  <!-- 📦 סקריפט מודולרי (ES6) – עם type="module": -->
  <script type="module" src="module.js"></script>

  <!-- 📦 סקריפט fallback לדפדפנים שלא תומכים במודולים – nomodule: -->
  <script nomodule src="legacy.js"></script>

  <!-- 📦 סקריפט עם hash לאימות (Content Integrity): -->
  <script src="cdn-script.js"
          integrity="sha384-x123..."
          crossorigin="anonymous"></script>

  <!-- 📦 סקריפט פנימי בתוך הדף: -->
  <script>
    console.log('קוד JavaScript נטען');
  </script>
```

---

## 🔷 חלק 9.2: `<noscript>` – תוכן למשתמשים ללא JavaScript

```html
  <!-- 🔹 <noscript>: מוצג רק אם JavaScript לא פעיל בדפדפן -->
  <noscript>
    <p>אנא אפשר JavaScript כדי להשתמש באתר.</p>
  </noscript>
```

---

## 🔷 חלק 9.3: `<template>` – תבנית HTML שלא נטענת אוטומטית

```html
  <!-- 🔹 <template>: HTML שמופעל רק דרך JavaScript
       לא מוצג בדף – מתאים ליצירת מרכיבים דינמיים -->
  <template id="card-template">
    <div class="card">
      <h3>כותרת כרטיס</h3>
      <p>תוכן כרטיס</p>
    </div>
  </template>

  <!-- 📦 בשימוש עם JavaScript:
       const tpl = document.getElementById('card-template');
       const clone = tpl.content.cloneNode(true);
       document.body.appendChild(clone); -->
```

---

## 🔷 חלק 9.4: `<slot>` – מקום לתוכן חיצוני בתוך Web Component

```html
  <!-- 🔹 <slot>: משמש בתוך Web Component – מחליף מקום שמוזן מבחוץ -->
  <template id="my-component">
    <div class="box">
      <slot name="title">כותרת ברירת מחדל</slot>
      <slot name="content"></slot>
    </div>
  </template>

  <!-- 📦 בשימוש: -->
  <my-component>
    <h1 slot="title">ברוך הבא</h1>
    <p slot="content">זהו התוכן שלך</p>
  </my-component>
```

---



# **חלק 10: פרופרטיז נגישות (`aria-*`) ותגיות Deprecated**

## 🔷 חלק 10.1: נגישות – `aria-*`, `role`, `tabindex`

```html
  <!-- 🔹 tabindex: קובע את סדר הניווט בלחיצה על TAB -->
  <button tabindex="1">כפתור ראשון</button>
  <button tabindex="2">כפתור שני</button>

  <!-- 🔹 role: תיאור סמנטי של רכיב – משפר נגישות לקוראי מסך -->
  <section role="region">
    <h2>אזור מידע</h2>
    <p>תוכן אזור סמנטי</p>
  </section>

  <!-- 🔹 aria-label: תיאור טקסטואלי לרכיב שלא רואים -->
  <a href="#" aria-label="מעבר לעמוד הבית">
    <img src="home-icon.svg" alt="">
  </a>

  <!-- 🔹 aria-hidden: מסתיר את האלמנט מנגישות (אבל לא מהעין) -->
  <span aria-hidden="true">★</span>

  <!-- 🔹 aria-live: אזור עם עדכון חי – כמו צ'אט -->
  <div aria-live="polite">
    <p>הודעה חדשה התקבלה</p>
  </div>

  <!-- 🔹 aria-expanded / aria-pressed: מציין אם פתוח או לחוץ -->
  <button aria-expanded="true">תפריט פתוח</button>
  <button aria-pressed="false">מופעל/כבוי</button>
```

---

## 🔷 חלק 10.2: תגיות deprecated – לא מומלצות לשימוש אך עדיין קיימות

```html
  <!-- ⚠️ <b>: במקום <strong> -->
  <b>טקסט מודגש – לא מומלץ</b>

  <!-- ⚠️ <i>: במקום <em> -->
  <i>טקסט נטוי – לא מומלץ</i>

  <!-- ⚠️ <u>: במקום CSS עם text-decoration -->
  <u>קו תחתון – עדיף ב־CSS</u>

  <!-- ⚠️ <font>: שליטה בגופן – הועבר ל־CSS -->
  <font color="red" size="4" face="Arial">טקסט בעיצוב ישן</font>

  <!-- ⚠️ <center>: יישור למרכז – עדיף ב־CSS -->
  <center>תוכן ממורכז</center>

  <!-- ⚠️ <marquee>: אנימציית טקסט – לא תקני -->
  <marquee direction="right">טקסט נע ←</marquee>

  <!-- ⚠️ <blink>: טקסט מהבהב – לא נתמך בפועל -->
  <blink>זה היה פעם מגניב</blink>
```



