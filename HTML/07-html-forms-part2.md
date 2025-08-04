# 🧾 טפסים ב־HTML – חלק 2 מתוך 2 (קלטים מורחבים + עיצוב + מבנים מורכבים)

---

## 📝 `<textarea>` – שדה טקסט מרובה שורות

```html
<label for="story">ספר בקצרה את הרפתקתך:</label><br />
<textarea id="story" name="story" rows="4" cols="50">
ביום סגריר יצאתי מהכפר עם מגן חלוד...
</textarea>
````

---

## 🔽 `<select>` – תפריט בחירה נפתחת

```html
<label for="class">בחר מקצוע:</label>
<select id="class" name="class">
  <option value="mage">🧙‍♂️ קוסם</option>
  <option value="warrior">🛡️ לוחם</option>
  <option value="archer">🏹 קשת</option>
</select>
```

🔸 אפשרות התחלתית נבחרת לפי מיקום או `selected`:

```html
<option selected value="warrior">🛡️ לוחם</option>
```

---

## 🎯 `<button>` – כפתור גמיש

```html
<button type="submit">🚀 התחל את המסע</button>
<button type="button" onclick="alert('בהצלחה!')">🎉 ברכה לשחקן</button>
```

---

## 🧩 `<fieldset>` + `<legend>` – קיבוץ שדות

```html
<fieldset>
  <legend>🎮 פרטי שחקן</legend>
  <label for="name">שם:</label>
  <input type="text" id="name" name="name" /><br />

  <label for="level">רמה:</label>
  <input type="number" id="level" name="level" /><br />
</fieldset>
```

---

## 🎨 עיצוב טופס בסיסי ב־CSS

```html
<style>
  form {
    background-color: #111;
    padding: 20px;
    border-radius: 12px;
    width: 300px;
    margin: auto;
    color: #eee;
    font-family: 'Segoe UI', sans-serif;
  }

  input, select, textarea, button {
    width: 100%;
    padding: 8px;
    margin: 8px 0;
    border: none;
    border-radius: 6px;
  }

  button {
    background-color: gold;
    color: black;
    font-weight: bold;
  }

  button:hover {
    background-color: orange;
  }
</style>
```

---

## 📋 דוגמה מלאה – טופס יצירת דמות

```html
<form action="/create-character" method="post">
  <fieldset>
    <legend>🧝 צור דמות חדשה</legend>

    <label for="hero">שם דמות:</label>
    <input type="text" id="hero" name="hero" />

    <label for="class">סוג דמות:</label>
    <select id="class" name="class">
      <option>קוסם</option>
      <option>לוחם</option>
      <option>גנב</option>
    </select>

    <label for="bio">תיאור רקע:</label>
    <textarea id="bio" name="bio"></textarea>

    <button type="submit">🎮 התחל משחק</button>
  </fieldset>
</form>
```

