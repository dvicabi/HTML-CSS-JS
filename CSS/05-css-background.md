# 🖼️ו CSS Background – כל האפשרויות לרקע במשחקים

---

## 🔹 רקע בצבע אחד

```css
body {
  background-color: #121212;
}
````

🎨 מתאים למשחקים כהים, תפריטי שלבים, מסכים דרמטיים

---

## 🔹 רקע מתמונה (`background-image`)

```css
body {
  background-image: url("images/forest.png");
}
```

🔸 הקובץ צריך להיות נגיש לתיקייה
🔸 תמיד לתת גם צבע רקע לטעינה איטית:

```css
body {
  background-color: black;
  background-image: url("bg.jpg");
}
```

---

## 🔹 חזרת רקע (`background-repeat`)

| ערך         | משמעות                       |
| ----------- | ---------------------------- |
| `repeat`    | חוזר על כל הציר (ברירת מחדל) |
| `no-repeat` | מוצג פעם אחת בלבד            |
| `repeat-x`  | רק לאורך (אופקית)            |
| `repeat-y`  | רק לאורך (אנכית)             |

```css
body {
  background-image: url("texture.png");
  background-repeat: repeat-x;
}
```

---

## 🔹 מיקום רקע (`background-position`)

```css
body {
  background-image: url("map.png");
  background-repeat: no-repeat;
  background-position: center top;
}
```

| ערך אפשרי | דוגמה        |
| --------- | ------------ |
| `left`    | צד שמאל      |
| `right`   | צד ימין      |
| `top`     | למעלה        |
| `bottom`  | למטה         |
| `center`  | אמצע         |
| יחידות    | `50px 100px` |

---

## 🔹 גודל רקע (`background-size`)

| ערך         | תוצאה                    |
| ----------- | ------------------------ |
| `auto`      | גודל מקורי של התמונה     |
| `cover`     | מכסה את כל האלמנט        |
| `contain`   | מתאים לגבולות מבלי לחתוך |
| `100% 100%` | מותאם ידנית              |

```css
body {
  background-size: cover;
}
```

---

## 🔹 קיבוע רקע (`background-attachment`)

```css
body {
  background-attachment: fixed;
}
```

🔸 שומר את הרקע במיקום קבוע – יוצר אפקט פרלקסה נחמד!

---

## 🧠 שילוב הכול יחד – `background` shorthand

```css
body {
  background: url("bg.jpg") no-repeat center center / cover fixed;
}
```

מבנה:

```
background: image repeat position / size attachment;
```

---

## 🎮 דוגמה למסך פתיחה למשחק

```css
body {
  background: url("images/intro.jpg") no-repeat center center / cover;
  color: white;
  text-align: center;
  font-family: "Segoe UI", sans-serif;
}
```

---

## 🧠 טיפים למפתחי משחקים

* השתמש ב־`cover` כדי להתאים למסכים שונים
* תן צבע רקע כהגנה אם התמונה לא תיטען
* רצוי לא להשתמש בתמונות כבדות
* תכנן שכבות רקע (נעשה בהמשך עם `::before`)
