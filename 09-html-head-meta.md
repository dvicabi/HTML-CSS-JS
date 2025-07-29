# 🧠 תגיות `<head>` – מטא-מידע, SEO וניידים (מימוש מלא)

---

## 🧱 מה זה `<head>`?

תגית `<head>` מופיעה בתחילת כל מסמך HTML ומכילה מידע **על העמוד** – ולא תוכן שנראה בעין.  
היא משפיעה על:

- 🏷️ שם הלשונית (title)
- 📱 התאמה לניידים
- 🔍 קידום במנועי חיפוש (SEO)
- 🌐 קישורים לקבצי עיצוב (`CSS`)
- 📷 תצוגה מקדימה לשיתוף

---

## 🔹 `<title>` – שם הלשונית

```html
<title>משחק המבוך של דביר</title>
````

📌 מופיע בלשונית הדפדפן וגם ככותרת בתוצאות חיפוש.

---

## 🔹 `<meta charset="UTF-8">` – תמיכה בעברית

```html
<meta charset="UTF-8" />
```

🔸 חובה בכל עמוד – מאפשר להציג עברית בצורה תקינה.

---

## 🔹 `<meta name="viewport">` – התאמה לניידים

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

📱 חובה כדי לגרום לעמוד להיראות טוב במובייל.
משפיע על הגדלים, טקסטים, רזולוציה.

---

## 🔹 `<meta name="description">` – תיאור קצר למנועי חיפוש

```html
<meta name="description" content="הצטרף למשחק הרפתקאות קסום שבו אתה מגלה אוצרות ונלחם בדרקונים." />
```

🔎 יוצג בתוצאות בגוגל כתקציר.

---

## 🔹 `<meta name="keywords">` – מילות מפתח (פחות נפוץ היום)

```html
<meta name="keywords" content="משחק, דרקון, קוסם, הרפתקה, HTML לילדים" />
```

💡 בעבר זה עזר ל־SEO, היום זה פחות בשימוש – אבל לא מזיק.

---

## 🔹 `<meta name="author">` – שם היוצר

```html
<meta name="author" content="Dvir Cabessa" />
```

🧠 שימושי גם לזיהוי עצמי או דינמיקה בין מפתחים.

---

## 🔹 `<link rel="icon">` – אייקון ללשונית (favicon)

```html
<link rel="icon" type="image/png" href="images/icon.png" />
```

🔸 יופיע ליד שם העמוד בלשונית הדפדפן
🔸 גודל מומלץ: `32x32` פיקסלים

---

## 🔹 `<link rel="stylesheet">` – קישור לקובץ CSS

```html
<link rel="stylesheet" href="style.css" />
```

🧩 מאפשר להפריד עיצוב מהמבנה – חובה בכל פרויקט רציני.

---

## 🔹 Open Graph – תצוגת שיתוף ברשתות

```html
<meta property="og:title" content="משחק האוצר האבוד" />
<meta property="og:description" content="האם תמצא את האוצר לפני שהדרקון יתעורר?" />
<meta property="og:image" content="images/preview.png" />
<meta property="og:type" content="website" />
```

🔗 ישפר תצוגה כשמשתפים קישור ב־WhatsApp, פייסבוק, טלגרם וכו'.

---

## 🧠 טיפ

בכל עמוד HTML, תמיד כלול את הבסיס הבא:

```html
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>שם העמוד</title>
  <link rel="stylesheet" href="style.css" />
</head>
```
