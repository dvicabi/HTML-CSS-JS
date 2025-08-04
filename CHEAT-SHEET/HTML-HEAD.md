🔹 **🔸 תגיות בסיסיות בתוך `<head>`**

| תגית       | תיאור                               | פרופרטיז / מאפיינים                                                                       | דוגמה                                                |
| ---------- | ----------------------------------- | ----------------------------------------------------------------------------------------- | ---------------------------------------------------- |
| `<title>`  | כותרת הדף שמופיעה בטאב של הדפדפן    | טקסט חופשי                                                                                | `<title>My Site</title>`                             |
| `<meta>`   | מידע על הדף (SEO, קידוד, מדיה וכו') | `charset`, `name`, `content`, `http-equiv` ועוד                                           | ראו טבלה נפרדת למטה 🔸                               |
| `<link>`   | קישור חיצוני (ל-CSS, אייקונים וכו') | `rel`, `href`, `type`, `media`, `sizes`, `crossorigin`                                    | `<link rel="stylesheet" href="style.css">`           |
| `<style>`  | כתיבת CSS פנימי                     | ללא פרופרטיז – מכיל קוד CSS                                                               | `<style>body { color: red; }</style>`                |
| `<script>` | הוספת קוד JavaScript                | `src`, `type`, `async`, `defer`, `integrity`, `crossorigin`, `nomodule`, `referrerpolicy` | `<script src="script.js" defer></script>`            |
| `<base>`   | הגדרת URL בסיסי לקישורים/תמונות בדף | `href`, `target`                                                                          | `<base href="https://example.com/" target="_blank">` |

---

🔹 **🔸 מאפיינים חשובים ל־`<meta>`**

| name / http-equiv              | content                                 | שימוש                      |
| ------------------------------ | --------------------------------------- | -------------------------- |
| `charset`                      | למשל: `UTF-8`                           | הגדרת קידוד הדף            |
| `viewport`                     | `width=device-width, initial-scale=1.0` | התאמה רספונסיבית לנייד     |
| `description`                  | תיאור קצר                               | משפיע על SEO               |
| `keywords`                     | מילות מפתח מופרדות בפסיקים              | משפיע מעט על SEO           |
| `author`                       | שם הכותב                                | מידע לדפדפן ומנועי חיפוש   |
| `robots`                       | `index, follow` או `noindex, nofollow`  | הנחיות למנועי חיפוש        |
| `http-equiv="X-UA-Compatible"` | `IE=edge`                               | תאימות ל־Internet Explorer |
| `http-equiv="refresh"`         | `30` או `5; url=https://example.com`    | רענון או הפניה אוטומטית    |
| `theme-color`                  | `#ffffff`                               | צבע הטאב בדפדפנים ניידים   |
| `og:title`                     | שם לשיתוף בפייסבוק                      | חלק מ־Open Graph           |
| `og:image`                     | קישור לתמונה                            | משתף תמונה ברשתות חברתיות  |
| `twitter:card`                 | `summary_large_image`                   | תצוגה בטוויטר              |
| `meta name="application-name"`                      | שם קצר של האפליקציה                       | לשימוש ב־PWA                    |
| `meta name="apple-mobile-web-app-capable"`          | `yes` / `no`                              | הפעלת מסך מלא ב-iOS             |
| `meta name="apple-mobile-web-app-status-bar-style"` | `default` / `black` / `black-translucent` | צבע שורת מצב ב-iOS              |
| `meta name="apple-mobile-web-app-title"`            | שם אפליקציה                               | כמו title אבל לאייפון           |
| `meta name="mobile-web-app-capable"`                | `yes` / `no`                              | גרסה כללית של fullscreen        |
| `meta name="msapplication-TileColor"`               | צבע למשל: `#ffffff`                       | עבור Windows tile               |
| `meta name="msapplication-TileImage"`               | קישור לאייקון                             | מופיע על מסך הבית של Windows    |
| `meta name="google-site-verification"`              | קוד ייחודי                                | אימות מול Google Search Console |
| `meta http-equiv="Content-Security-Policy"`         | `default-src 'self';` וכו'                | אבטחת סקריפטים                  |

---

🔹 **🔸 תגיות SEO, שיתוף ואבטחה נפוצות נוספות**

| תגית                             | תיאור                                       | דוגמה                                                   |
| -------------------------------- | ------------------------------------------- | ------------------------------------------------------- |
| `<meta property="og:...">`       | תגיות Open Graph לשיתוף ברשתות חברתיות      | `<meta property="og:title" content="My Page Title">`    |
| `<meta name="twitter:...">`      | תגיות שיתוף בטוויטר                         | `<meta name="twitter:image" content="image.jpg">`       |
| `<meta name="referrer">`         | שליטה על כותרת ה-Referer                    | `<meta name="referrer" content="no-referrer">`          |
| `<meta name="color-scheme">`     | הגדרת מצב כהה/בהיר                          | `<meta name="color-scheme" content="light dark">`       |
| `<meta name="format-detection">` | מניעת זיהוי אוטומטי (מספרים, אימיילים וכו') | `<meta name="format-detection" content="telephone=no">` |
| `apple-touch-icon` | `icon192.png` או אחר          | אייקון למסכי בית ב-iOS                                                                                  |
| `mask-icon`        | קובץ SVG + צבע                | אייקון למצב כהה / ספארי                                                                                 |
| `pingback`         | כתובת פינג באק                | לבלוגים (בעיקר WordPress)                                                                               |

---

🔹 **🔸 תגיות `<link>` מתקדמות מעבר ל־CSS**

| rel            | href                                 | תיאור                                                                |
| -------------- | ------------------------------------ | -------------------------------------------------------------------- |
| `icon`         | favicon.ico / תמונה                  | אייקון הדפדפן                                                        |
| `manifest`     | manifest.json                        | לאפליקציות PWA                                                       |
| `preconnect`   | קישור מוקדם לשרת                     | `<link rel="preconnect" href="https://fonts.googleapis.com">`        |
| `dns-prefetch` | ביצוע DNS מראש                       | `<link rel="dns-prefetch" href="//example.com">`                     |
| `preload`      | טעינה מוקדמת של משאב (סקריפט, תמונה) | `<link rel="preload" as="script" href="app.js">`                     |
| `canonical`    | קישור לגרסה המקורית של הדף           | `<link rel="canonical" href="https://example.com/page">`             |
| `alternate`    | גרסה אחרת של הדף (לשפה אחרת)         | `<link rel="alternate" hreflang="en" href="https://example.com/en">` |
| `stylesheet`   | קובץ CSS                             | `<link rel="stylesheet" href="styles.css">`                          |
| `license`          | קישור לרישיון                 | `<link rel="license" href="LICENSE.txt">`                                                               |
| `search`           | XML חיפוש מותאם               | `<link rel="search" href="opensearch.xml" type="application/opensearchdescription+xml" title="Search">` |
| `modulepreload`    | כמו preload אבל ל־ES6 modules | `<link rel="modulepreload" href="module.js">`                                                           |

---

🔹 **🔸 תגיות SCRIPT מיוחדות**

| מאפיין          | שימוש                                         |
| --------------- | --------------------------------------------- |
| `type="module"` | תומך ב־ES6 Modules                            |
| `async`         | מריץ את הסקריפט מייד כשמוכן (עשוי לשבור סדר)  |
| `defer`         | ממתין עד שהדף נטען ורק אז מריץ                |
| `nomodule`      | מריץ את הסקריפט רק אם הדפדפן לא תומך במודולים |
| `integrity`     | בדיקת תוכן הקובץ מול hash                     |
| `crossorigin`   | שליטה על בקשות חוצות דומיין                   |

---
🔹 **🔸 דגשים מיוחדים**

| נושא             | הסבר                                                                                      |
| ---------------- | ----------------------------------------------------------------------------------------- |
| **טעינה מוקדמת** | תגיות preload ו־modulepreload עוזרות לביצועים ע"י התחלת טעינה לפני הצורך                  |
| **אבטחה**        | Content-Security-Policy, integrity, referrer, crossorigin – חשובים מאוד בפרויקטים אמיתיים |
| **שיתוף**        | Open Graph (og:) ו־Twitter Cards מאפשרים שליטה איך הדף מוצג כשמשתפים אותו                 |




🔹 **🔸 תוספות מתקדמות שחסרות**:

| תגית/מאפיין                              | תיאור                                               | דוגמה                                                                        |
| ---------------------------------------- | --------------------------------------------------- | ---------------------------------------------------------------------------- |
| `<meta name="referrer">`                 | שליטה על איך כתובת ההפניה נשלחת                     | `<meta name="referrer" content="no-referrer">`                               |
| `<meta name="viewport-fit">`             | התאמה למסכים עם חריץ (notch)                        | `<meta name="viewport-fit" content="cover">`                                 |
| `<meta name="subject">`                  | נושא כללי לדף                                       | `<meta name="subject" content="HTML Cheatsheet">`                            |
| `<meta name="rating">`                   | דירוג תוכן (לפי גיל וכו')                           | `<meta name="rating" content="general">`                                     |
| `<meta name="distribution">`             | טווח פרסום                                          | `<meta name="distribution" content="global">`                                |
| `<meta name="copyright">`                | הצהרת זכויות יוצרים                                 | `<meta name="copyright" content="© 2025 Dvir Cabessa">`                      |
| `<meta name="language">`                 | שפת התוכן (למנועי חיפוש ישנים)                      | `<meta name="language" content="he">`                                        |
| `<meta name="revised">`                  | תאריך עדכון אחרון                                   | `<meta name="revised" content="Monday, August 04, 2025">`                    |
| `<meta name="generator">`                | מערכת שיצרה את הדף                                  | `<meta name="generator" content="WordPress">`                                |
| `<meta http-equiv="Permissions-Policy">` | מגבלות API של הדפדפן                                | `<meta http-equiv="Permissions-Policy" content="geolocation=(), camera=()">` |
| `<link rel="shortlink">`                 | קישור מקוצר לגרסה זמינה של הדף                      | `<link rel="shortlink" href="https://example.com/?p=123">`                   |
| `<link rel="pingback">`                  | שליחה אוטומטית של התראה בקישור (בלוגים)             | `<link rel="pingback" href="https://example.com/xmlrpc.php">`                |
| `<link rel="prev">` / `next`             | לניווט בין עמודים (לדוג' עמודי בלוג)                | `<link rel="next" href="page2.html">`                                        |
| `<meta name="apple-itunes-app">`         | קישור לאפליקציית iOS                                | `<meta name="apple-itunes-app" content="app-id=123456789">`                  |
| `<meta name="al:ios:url">`               | קישור לעמוד ספציפי באפליקציה דרך Facebook App Links | `<meta property="al:ios:url" content="applinks://details">`                  |
