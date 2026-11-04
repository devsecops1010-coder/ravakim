# Chai's Ravakim · Budapest 2026 — התקנה על GitHub Pages

קישור קבוע וחינמי. שתי דרכים — בחר אחת.

## דרך א' · דרך האתר (בלי טרמינל, הכי פשוט)
1. היכנס ל-https://github.com/new
2. שם ה-repo: `ravakim` · בחר **Public** · לחץ **Create repository**
3. במסך הבא לחץ **uploading an existing file**
4. גרור לשם את **כל הקבצים** מתוך `ravakim-app` (index.html, manifest.json, sw.js, icon.png, .nojekyll) · לחץ **Commit changes**
5. לך ל-**Settings → Pages** → תחת *Branch* בחר **main** ושמור (Save)
6. אחרי דקה-שתיים הכתובת הקבועה תופיע למעלה:
   **https://<שם-המשתמש-שלך>.github.io/ravakim/**

## דרך ב' · דרך הטרמינל (אם יש לך git מקומי)
כבר יצרתי repo עם commit ראשוני. צור repo ריק בשם `ravakim` ב-GitHub, ואז:

```bash
cd ravakim-app
git remote add origin https://github.com/<שם-המשתמש>/ravakim.git
git push -u origin main
```
אחר כך Settings → Pages → Branch: main → Save.

## התקנה על האייפון (אחרי שיש כתובת)
1. פתח את הכתובת **ב-Safari**
2. בחר מי אתה (קובע את האייקון האישי)
3. כפתור שיתוף ⬆️ → **הוסף למסך הבית** → הוסף
4. פתח את האייקון — נפתח במסך מלא כמו אפליקציה 🎉

## הערות
- הנתונים כרגע מקומיים לכל מכשיר (localStorage). לסנכרון בין כולם צריך Firebase — שכבת הנתונים כבר מוכנה לזה.
- הגרפיקה היא placeholders עד שיוזנו נכסים אמיתיים.
