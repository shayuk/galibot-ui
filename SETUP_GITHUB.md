# הוראות העלאה ל-GitHub

## שלב 1: יצירת Repository ב-GitHub

1. לך ל-https://github.com/new
2. שם ה-repository: `galibot-ui`
3. בחר Public או Private (לפי העדפתך)
4. **אל תוסיף** README, .gitignore או רישיון (כבר יש לנו)
5. לחץ על "Create repository"

## שלב 2: חיבור ל-GitHub

לאחר יצירת ה-repository, הרץ את הפקודות הבאות:

```bash
cd galibot-ui
git remote add origin https://github.com/shayuk/galibot-ui.git
git push -u origin main
```

או אם אתה משתמש ב-SSH:

```bash
cd galibot-ui
git remote add origin git@github.com:shayuk/galibot-ui.git
git push -u origin main
```

## הערות

- אם ה-repository כבר קיים ב-GitHub, פשוט הרץ את הפקודות מ-שלב 2
- אם יש שגיאה, ודא שה-repository נוצר ב-GitHub לפני הרצת הפקודות

