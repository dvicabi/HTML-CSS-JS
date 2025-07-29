---

### 📄 שם הקובץ: `07-html-forms-part1.md`

````markdown
# 🧾 טפסים ב־HTML – חלק 1 מתוך X (מבנה בסיסי + קלטים עיקריים)

---

## 🧱 מבנה בסיסי של טופס

```html
<form action="/submit" method="post">
  <label for="username">שם משתמש:</label>
  <input type="text" id="username" name="username" />
  <br />
  <button type="submit">🎯 התחל לשחק</button>
</form>
````

* `<form>` – עוטף את הטופס כולו
* `action` – לאן הנתונים נשלחים
* `method` – אופן שליחה (`get` או `post`)
* `<label>` – תיאור עבור שדה
* `<input>` – שדה קלט
* `<button>` – כפתור

---

## 🔤 `type="text"` – טקסט רגיל

```html
<label for="player">שם שחקן:</label>
<input type="text" id="player" name="player" />
```

---

## 🔒 `type="password"` – סיסמה (מוסתרת)

```html
<label for="code">קוד סודי:</label>
<input type="password" id="code" name="code" />
```

---

## 📅 `type="date"` – בחירת תאריך

```html
<label for="birth">תאריך לידה:</label>
<input type="date" id="birth" name="birth" />
```

---

## 🔢 `type="number"` – מספר בלבד

```html
<label for="level">רמת דמות:</label>
<input type="number" id="level" name="level" min="1" max="100" />
```

---

## 📧 `type="email"` – אימייל תקני

```html
<label for="email">שלח אליי עדכונים:</label>
<input type="email" id="email" name="email" />
```

---

## 📞 `type="tel"` – מספר טלפון

```html
<label for="phone">טלפון:</label>
<input type="tel" id="phone" name="phone" />
```

---

## 🎯 `type="submit"` – כפתור שליחה

```html
<input type="submit" value="🚀 שגר טופס" />
```

---

## 🔘 `type="radio"` – בחירה אחת מתוך כמה

```html
<p>בחר דמות התחלתית:</p>
<input type="radio" id="mage" name="char" value="mage" />
<label for="mage">🧙‍♂️ קוסם</label><br />

<input type="radio" id="warrior" name="char" value="warrior" />
<label for="warrior">🗡️ לוחם</label><br />
```

🔸 לשם (`name`) חייב להיות אותו ערך כדי לאפשר בחירה בודדת.

---

## ✅ `type="checkbox"` – בחירה מרובה

```html
<p>בחר ציוד התחלתי:</p>
<input type="checkbox" id="sword" name="gear" value="sword" />
<label for="sword">⚔️ חרב</label><br />

<input type="checkbox" id="potion" name="gear" value="potion" />
<label for="potion">🧪 שיקוי</label><br />
```

---

## 🧠 טיפ: `label for="..."` תמיד צריך להתאים ל־`id="..."`

```html
<label for="hero">שם גיבור:</label>
<input id="hero" name="hero" />
```

🔸 זה משפר נגישות ונותן לחיצה נוחה יותר.
