# 🎵🎥 תגיות מולטימדיה ב־HTML – שמע ווידאו (מימוש מלא)

---

## 🎧 תגית `<audio>` – השמעת סאונד

```html
<audio controls>
  <source src="sounds/magic.wav" type="audio/wav" />
  <source src="sounds/magic.mp3" type="audio/mpeg" />
  הדפדפן שלך לא תומך בהשמעת אודיו 🎵
</audio>
````

🔹 `controls` – מציג כפתורי השמעה/השהיה/ווליום
🔹 `source` – מאפשר טעינה לפי סוג קובץ (mp3, ogg, wav)
🔹 תוכן בין התגיות – יוצג רק אם הדפדפן לא תומך

---

## 🎯 מאפיינים נוספים ל־`<audio>`

| מאפיין           | הסבר                                          |
| ---------------- | --------------------------------------------- |
| `autoplay`       | מתחיל לנגן אוטומטית עם עליית העמוד            |
| `loop`           | חוזר בלופ                                     |
| `muted`          | מתחיל כשהשמע כבוי                             |
| `preload="auto"` | טוען את כל הקובץ מראש (או `none`, `metadata`) |

```html
<audio src="sounds/theme.mp3" autoplay loop muted></audio>
```

---

## 🎥 תגית `<video>` – הצגת וידאו במשחק

```html
<video width="320" height="240" controls>
  <source src="cutscene.mp4" type="video/mp4" />
  <source src="cutscene.webm" type="video/webm" />
  הדפדפן לא תומך בווידאו 🎬
</video>
```

🔸 ממש כמו `<audio>`, אך עם מסך תצוגה

---

## 🎯 מאפיינים ל־`<video>`

| מאפיין         | תיאור                           |
| -------------- | ------------------------------- |
| `controls`     | כפתורי שליטה (play, pause וכו') |
| `autoplay`     | מפעיל אוטומטית                  |
| `loop`         | חוזר בלולאה                     |
| `muted`        | מושתק כברירת מחדל               |
| `poster="..."` | תמונת שער לפני התחלת ניגון      |

```html
<video src="intro.mp4" autoplay muted loop poster="poster.png" width="400"></video>
```

---

## 📃 כתוביות עם `<track>`

```html
<video controls>
  <source src="cutscene.mp4" type="video/mp4" />
  <track src="subs.vtt" kind="subtitles" srclang="he" label="עברית" default />
</video>
```

* `track` – משמש לכתוביות או תיאור שמע
* פורמט: `.vtt` (WebVTT)

---

## 🧠 שימושים לילדים שמפתחים משחקים

* 🎵 מוזיקת רקע (`<audio autoplay loop>`)
* 🔊 אפקטים לכפתורים (בהמשך עם JS)
* 🎬 סצנות מעבר לפני שלבים
* 🎙️ קריינות, תיאורים קוליים
* 🧙‍♂️ סאונד של כישוף, מכה, עלייה ברמה

---

## 📁 ניהול קבצים

שים את קבצי הסאונד/וידאו בתקיות מסודרות:

* `/sounds` – לסאונד
* `/videos` – לווידאו
* `/subtitles` – לכתוביות
