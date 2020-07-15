<div dir="rtl" lang="he">

# חיפוש פונטי 

התקבלתם לעבודה במשרדו של חוקר פרטי,
והמשימה הראשונה שקיבלתם היא לעבור על תמלילים של שיחות טלפון באנגלית ולחפש שם מילים חשודות.

הבעיה היא, שמי שתימלל את שיחות הטלפון עשה הרבה שגיאות כתיב.
בפרט, הוא החליף (לפעמים) בין האותיות:

* v, w
* b, f, p
* g, j
* c, k, q
* s, z 
* d, t 
* o, u
* i, y

והפך (לפעמים) אותיות קטנות לגדולות או להיפך.

המטרה שלכם היא לכתוב פונקציה המוצאת מילה בטקסט, גם אם המילה כתובה בטקסט עם שגיאות כתיב.
הפונקציה צריכה להחזיר את המילה כפי שהיא כתובה בטקסט.

למשל: נניח שהטקסט המתומלל הוא: 
"Dond vorri be haffy".

אם המילה שצריך לחפש היא "dont"
אז הפלט יהיה "Dond" - זו אותה מילה רק עם חילוף של 
t ב-d וחילוף של אות גדולה בקטנה.

שימו לב - המתמלל לא תמיד טועה, הוא טועה רק מדי פעם.
למשל, אם המילה שמחפשים היא "be" 
אז הפלט יהיה "be" - זו אותה מילה בדיוק - בלי שגיאות.

ניתן להניח שבמחרוזת יש רק אותיות אנגליות גדולות וקטנות, ורווחים
(ללא סימני פיסוק).
יש לחפש רק מילים שלמות. 

מקרים מיוחדים:

* אם המילה שמחפשים לא מופיעה בטקסט - יש לזרוק חריגה.
* אם המילה שמחפשים מופיעה פעמיים או יותר (עם טעויות שונות) - יש להחזיר את ההופעה הראשונה.
* אם המילה שמחפשים היא ריקה, או שהיא לא מילה אחת (מכילה רווח) - יש לזרוק חריגה.

כדי לראות איך הפונקציה אמורה לעבוד, ראו בקובץ
[Demo.cpp](Demo.cpp)
המצורף.

בשלב א עליכם לכתוב את הקבצים הדרושים כך שהפקודות הבאות יעבדו ללא שגיאות קימפול:

<div dir='ltr'>

    make demo && ./demo
	make test && ./test

</div>

בפרט, עליכם לכתוב את  הקבצים הבאים:

* PhoneticFinder.hpp - כותרת לפונקציה.
* PhoneticFinder.cpp - מימוש בסיסי של הפונקציה - לא חייב להיות מלא - צריך רק להתקמפל.
* Test.cpp - בדיקות-יחידה בפורמט doctest. יש לכתוב בדיקות מפורטות ולהתייחס למקרי קצה.
   * ניתן לראות דוגמה לבדיקות בקובץ TestExample.cpp, אבל יש לכתוב הרבה בדיקות נוספות.

במטלות בקורס זה אנחנו כותבים את הבדיקות לפני המימוש.
זה אומר שבשלב א, יהיו לנו הרבה בדיקות, ורובן ייכשלו.

שימו לב!
אין לשנות קבצים קיימים, אלא רק להוסיף קבצים חדשים.

</div>