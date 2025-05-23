### 🐞 תרגיל 2: Debugging עם DevTools

**מטרה:** להבין איך לעצור קוד בעזרת Breakpoints ולבחון את זרימת הקריאות (Call Stack).

**איך מתחילים?**
1. פתחו קובץ HTML חדש והעתיקו אליו את הקוד הבא בתוך `<script>`:

```javascript
function multiply(a, b) {
  let result = a * b;
  return result;
}

function calculateTotal(price, tax) {
  let total = multiply(price, tax);
  return total;
}

let totalPrice = calculateTotal(100);
console.log("Total:", totalPrice);
```

2. פתחו את הדף בדפדפן ופתחו את DevTools בלשונית Sources.

**הנחיות:**
- הוסיפו Breakpoint באחת הפונקציות – איזו בחירה תעזור לכם להבין טוב יותר את זרימת הנתונים?
אחרי כניסה ל2 הפוקנקציות
- אילו ערכים עוברים בין הפונקציות? האם הכל נראה תקין?
מכניסים בחישוב סהכ את פונקציה הכפלה אז מיסים ומחיר נכנסים אבל מיסים כרגע זה ערך ריק כי שולחים רק 100 שנכנס למחיר
- האם יש נתון שלא הוזן? מה הייתם מצפים שיקרה במצב כזה?
b לא מוגדר
וtax לא מוגדר