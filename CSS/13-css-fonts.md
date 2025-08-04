# 🔤ו CSS Fonts – שימוש בגופנים בעולם המשחקים

---

## 🎯 למה חשוב לבחור גופן?

- 🧙‍♂️ גופן יוצר סגנון עולם (קסום, עתידני, קומיקס...)
- 📜 טקסט קריא = חוויית משחק חלקה
- 🎨 עיצוב אחיד מגביר מקצועיות

---

## 🔹 תכונה `font-family`

```css
p {
  font-family: Arial, sans-serif;
}
````

🔸 תמיד שמים גופן עיקרי ואז "fallback" למקרה שהוא לא קיים

---

## 🔸 משפחות גופנים עיקריות

| משפחה        | סגנון         |
| ------------ | ------------- |
| `sans-serif` | מודרני, פשוט  |
| `serif`      | קלאסי, עתיק   |
| `monospace`  | קוד, טכנולוגי |
| `cursive`    | כתב יד קסום   |
| `fantasy`    | יצירתי        |

---

## 🎮 דוגמה: סגנונות לפי עולם המשחק

```css
.mystic {
  font-family: "Segoe Script", cursive;
}

.code-display {
  font-family: "Courier New", monospace;
}

.futuristic {
  font-family: "Orbitron", sans-serif;
}
```

---

## 🔹 גודל טקסט (`font-size`)

```css
h1 {
  font-size: 48px;
}
```

🔸 ניתן גם ב־`em`, `rem`, `%`

---

## 🔹 משקל גופן (`font-weight`)

```css
h2 {
  font-weight: bold;
}
```

| ערך       | תוצאה        |
| --------- | ------------ |
| `normal`  | רגיל         |
| `bold`    | מודגש        |
| `lighter` | קליל         |
| `100–900` | שליטה מדויקת |

---

## 🔹 סגנון (`font-style`)

```css
blockquote {
  font-style: italic;
}
```

| ערך       | תוצאה         |
| --------- | ------------- |
| `normal`  | רגיל          |
| `italic`  | נטוי          |
| `oblique` | אלכסוני/מרומז |

---

## 🔹 יישור לגובה קו (`vertical-align`)

```css
sup {
  vertical-align: super;
}
```

---

## 🔹 ייבוא גופנים מ־Google Fonts

1. בחר גופן: [Google Fonts](https://fonts.google.com)
2. הדבק `<link>` בתוך `<head>` ב־HTML:

```html
<link href="https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap" rel="stylesheet">
```

3. השתמש בו ב־CSS:

```css
body {
  font-family: "Press Start 2P", cursive;
}
```

🎮 מעולה למשחקים רטרו או סגנון פיקסלים!

---

## 🧠 טיפים למפתחי משחקים

* בחר גופן שמתאים לז'אנר: קסם ≠ עתידנות
* ודא שהגופן תומך בעברית אם אתה מציג טקסטים בשפה זו
* גופנים רטרו כמו `"Press Start 2P"` או `"Orbitron"` = 🔥 למשחקים
* אל תשתמש ביותר מדי גופנים בעמוד אחד – שמור על אחידות

