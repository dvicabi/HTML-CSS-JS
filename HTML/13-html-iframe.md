# 🪞 תגית `<iframe>` – הצגת תכנים מוטמעים בתוך העמוד

---

## 🧱 שימוש בסיסי

תגית `<iframe>` מאפשרת להטמיע בתוך עמוד HTML:

- 🌍 עמוד אינטרנט אחר
- 🎬 סרטון YouTube
- 🗺️ מפה אינטראקטיבית
- 🧩 משחקים מוטמעים

```html
<iframe src="https://example.com" width="600" height="400"></iframe>
````

---

## 🔹 תכונות עיקריות של `<iframe>`

| תכונה             | הסבר                                   |
| ----------------- | -------------------------------------- |
| `src`             | כתובת העמוד שמוטמע בפנים               |
| `width`           | רוחב החלון (בפיקסלים / אחוזים)         |
| `height`          | גובה החלון                             |
| `title`           | תיאור נגישות (עוזר לקוראי מסך)         |
| `loading`         | `lazy` – טוען רק כשצריך (משפר ביצועים) |
| `allowfullscreen` | מאפשר מסך מלא (לסרטונים)               |

```html
<iframe
  src="https://example.com"
  width="500"
  height="300"
  title="עולם מקביל"
  loading="lazy"
></iframe>
```

---

## 🎥 הטמעת סרטון YouTube

```html
<iframe
  width="560"
  height="315"
  src="https://www.youtube.com/embed/VIDEO_ID"
  title="סרטון הדרכה"
  frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowfullscreen
></iframe>
```

🔸 החלף את `VIDEO_ID` בקוד של הסרטון הרצוי.
🎮 ניתן להציג סצנה פתיחה, הסבר של שלב, או טיזר למשחק.

---

## 🗺️ הטמעת מפה

```html
<iframe
  src="https://www.google.com/maps/embed?pb=..."
  width="600"
  height="450"
  style="border:0;"
  allowfullscreen=""
  loading="lazy"
  referrerpolicy="no-referrer-when-downgrade"
></iframe>
```

🧠 ניתן להשתמש כדי להציג אזור במשחק שמבוסס על מיקום אמיתי או פנטזיה.

---

## 🧩 שימושים יצירתיים לילדים מפתחי משחקים

* 🎬 מדריך מוטמע בתוך הדף (YouTube)
* 🧠 עזרה בצד ימין בתוך `<aside>`
* 🕹️ הצגת מיני־משחקים מתוך אתרים חיצוניים
* 🌐 קישור לעולמות נוספים במשחק

---

## ⚠️ שים לב!

* לא כל אתר מאפשר להטמיע אותו (`X-Frame-Options: DENY`)
* אם משהו לא נטען – נסה אתר אחר או ווידאו מ־YouTube
