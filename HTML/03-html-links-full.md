# 🔗 תגית `<a>` – קישורים ב־HTML (מימוש מלא)

---

## 🧱 שימוש בסיסי בקישור

```html
<a href="https://example.com">🌍 קישור לאתר חיצוני</a>
````

* `href`: היעד של הקישור (כתובת URL או קובץ מקומי)

---

## 📂 קישורים פנימיים (לעמודים או קבצים באתר)

```html
<a href="about.html">📄 עמוד אודות</a>
<a href="docs/rules.pdf">📥 הורד את חוקי המשחק</a>
```

---

## 🪟 פתיחה בכרטיסייה חדשה

```html
<a href="https://example.com" target="_blank" rel="noopener noreferrer">
  🆕 פתח בכרטיסייה חדשה
</a>
```

* `target="_blank"`: פותח קישור בכרטיסייה חדשה
* `rel="noopener noreferrer"`: אבטחה + ביצועים

---

## 📸 תמונה כקישור

```html
<a href="level2.html">
  <img src="images/door.png" alt="פתח לשלב 2" width="150" />
</a>
```

---

## 🪝 קישור לעוגן פנימי באותו עמוד

```html
<a href="#boss">🏃 קפוץ לקרב עם הבוס</a>

...

<h2 id="boss">💥 הבוס הגדול</h2>
```

* `id="..."`: מזהה עוגן בתוך עמוד
* `href="#..."`: קישור אליו

---

## 📞 `tel:` – חיוג ישיר ממכשיר

```html
<a href="tel:+972500000000">📱 התקשר למוקד הקוסמים</a>
```

---

## 📬 `mailto:` – פתיחת מייל

```html
<a href="mailto:help@magicland.com">📧 תמיכה טכנית</a>
<a href="mailto:help@magicland.com?subject=עזרה&body=נתקעתי בשלב 3">
  ❓ שלח מייל עם שאלה
</a>
```

---

## ⬇️ `download` – קובץ להורדה

```html
<a href="files/map.pdf" download>📥 הורד מפה</a>
<a href="files/weapon.png" download="secret-sword.png">
  🗡️ הורד חרב סודית
</a>
```

---

## 🔄 קישור ריק (לכפתורים או JavaScript)

```html
<a href="#">🔘 כפתור שעדיין לא פעיל</a>
<a href="javascript:void(0);">⛔ בלי פעולה</a>
```

---

## 🧪 כל התכונות יחד

```html
<a
  href="docs/guide.pdf"
  download="guide_for_players.pdf"
  target="_blank"
  rel="noopener noreferrer"
>
  📚 מדריך לשחקנים (PDF)
</a>
```

---

## 🧩 שימושים במשחקים

🔸 תפריט ניווט:

```html
<a href="index.html">🏠 בית</a>
<a href="levels.html">🗺️ שלבים</a>
<a href="shop.html">🛒 חנות</a>
```

🔸 מסך סוף:

```html
<a href="restart.html">🔁 התחל מחדש</a>
<a href="exit.html">🚪 יציאה</a>
```

🔸 עם עיצוב ככפתור (CSS בהמשך):

```html
<a class="button" href="level1.html">▶️ התחל שלב 1</a>
```
