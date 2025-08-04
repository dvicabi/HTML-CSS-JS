# 🧪 תגיות אינטראקטיביות ב־HTML – מידע מוסתר, חלונות קופצים ועוד

---

## 🔹 `<details>` ו־`<summary>` – קיפול/פתיחה של תוכן

🧩 מצוין להצגת מידע נוסף: תיאור חפצים, טיפים, משימות סודיות…

```html
<details>
  <summary>🧪 מידע על שיקוי כחול</summary>
  <p>מחזיר 50 חיים ונותן חיסון זמני לאש.</p>
</details>
````

* `<summary>` – מה שרואים ככותרת
* התוכן שבתוך `<details>` – נפתח בלחיצה

---

## 🎮 דוגמה עם כמה פריטים:

```html
<h2>📦 חפצים בתרמיל</h2>

<details>
  <summary>🗡️ חרב אפלה</summary>
  <p>נזק: 60<br>יכולת מיוחדת: פיצול אויבים</p>
</details>

<details>
  <summary>🛡️ מגן קרח</summary>
  <p>הגנה: 40<br>יכולת: בלימת נזק קפוא</p>
</details>
```

---

## 🔹 `<dialog>` – חלון קופץ (modal) (נתמך בדפדפנים מודרניים)

🧠 משמש להצגת הודעות מיוחדות, הסכמות, תפריטים חכמים במשחק

```html
<dialog id="msg">
  <p>🔥 ניצחת את הדרקון!</p>
  <button onclick="document.getElementById('msg').close()">סגור</button>
</dialog>

<button onclick="document.getElementById('msg').showModal()">📣 הצג הודעה</button>
```

* `showModal()` – פותח את החלון
* `close()` – סוגר אותו

---

## 🔸 עיצוב `dialog` עם CSS

```html
dialog {
  border: none;
  border-radius: 12px;
  padding: 20px;
  box-shadow: 0 0 20px cyan;
  background: #111;
  color: white;
  font-family: sans-serif;
}
```

---

## 🧠 שימושים אמיתיים לילדים מפתחי משחקים

* 🕵️ סודות במשחק (details)
* 📝 תיאור מורחב של שלב
* 🔔 חלון לניצחון או כישלון
* 📥 קופצת שמציגה קוד בונוס
* 🧩 עזרה בצדדים מבלי להעמיס את המסך הראשי
