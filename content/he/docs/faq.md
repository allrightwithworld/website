---
title: שו״ת
linkTitle: שאלות ותשובות (שו״ת)
slug: faq
top_graphic: 1
lastmod: 2020-02-20
menu:
  main:
    weight: 30
    parent: about
---

{{< lastmod >}}

שו״ת זה מפוצל לסעיפים הבאים:

* [שאלות כלליות](#general)
* [שאלות טכניות](#technical)

# <a id="general">שאלות כלליות</a>

## אילו שירותים מוצעים על ידי Let's Encrypt?

Let's Encrypt היא רשות אישורים גלובלית (CA). אנו מאפשירם לאנשים ולארגונים מסביב לעולם, לקבל, לחדש ולנהל אישורי SSL/TLS. אתרים יכולים להשתמש באישורים שלנו כדי להפעיל חיבורי HTTPS מאובטחים.

Let's Encrypt מציעה אישורי תיקוף שם תחום (DV - Domain Validation). אנו לא מציעים תיקוף ארגון (OV - Organization Validation) או תיקוף מורחב (EV - Extended Validation) בעיקר כיוון שאין לנו אפשרות ליצור אוטומציה להנפקה של אישורים מהסוגים האלו.

כדי להתחיל להשתמש ב־ Let's Encrypt, נא לבקר בעמוד [איך מתחילים](/getting-started) שלנו.

## כמה עולה להשתמש ב־Let's Encrypt? זה באמת בחינם?

איננו גובים עמלה על האישורים שלנו. Let's Encrypt אינה למטרות רווח, המשימה שלנו היא ליצור רשת אינטרנט מאובטחת ומכבדת פרטיות יותר על ידי קידום אימוץ HTTPS על ידי הקהל הרחב. השירותים שלנו הם בחינם וקלים לשימוש כדי שכל אתר יוכל להטמיע HTTPS.

אנו דורשים תרומות מתורמים נדיבים, נותני מענקים ואנשים פרטיים כדי לספק את השירותים שלנו בחינם בכל רחבי העולם. אם מעניין אותך לתמוך בנו, נא לשקול [לתרום](/donate) או [לתת חסות](/become-a-sponsor).

בחלק מהמקרים, גופים שמשלבים את המוצרים שלנו בשלהם (כמו למשל, ספקי אחסון) ייגבו עמלה סמלית שמשקפת את העלויות התפעוליות והניהוליות שהם נוטלים כדי לספק אישורים של Let's Encrypt.

## איזה סוג של תמיכה מוענקת?

Let's Encrypt מופעלת על ידי קבוצה קטנה ונסמכת על אוטומציה כדי לשמור על עלויות נמוכות. כיוון שזה המצב, אין לנו אפשרות להציע תמיכה ישירות למנויים שלנו. עם זאת, יש לנו מגוון אפשרויות תמיכה נהדרות:

1. יש לנו [תיעוד](/docs) מועיל במיוחד.
2. יש לנו [פורומים לתמיכה קהילתית](https://community.letsencrypt.org/) שהם מאוד פעילים ומועילים. חברי הקהילה שלנו עושים עבודה נהדרת במענה על שאלות ורבות מן השאלות הנפוצות ביותר כבר נענו.

להלן [סרטון שנושא חן בעינינו](https://www.youtube.com/watch?v=Xe1TZaElTAs) על הכוח שבתמיכה קהילתית מצוינת.

## אתר שמשתמש ב־Let's Encrypt מעורב בפעילות דיוג/תכנה זדונית/הונאה… מה עלי לעשות?

אנו ממליצים לדווח על אתרים כאלה ל־Google Safe Browsing (גלישה בטוחה בחסות Google) ולתכנית SmartScreen מבית Microsoft שיכולות להגן על משתמשים בצורה יעילה יותר. להלן כתובת הדיווח של Google:

[https://safebrowsing.google.com/safebrowsing/report_badware/](https://safebrowsing.google.com/safebrowsing/report_badware/)

אם מעניין אותך לקרוא עוד על מסמכי המדיניות שלנו ומה עומד מאחוריהם, ניתן לעשות זאת כאן:

https://letsencrypt.org/2015/10/29/phishing-and-malware.html

# <a id="technical">שאלות טכניות</a>

## האם אישורים מבית Let's Encrypt נחשבים על ידי הדפדפן שלי למהימנים?

עבור רוב הדפדפנים ומערכות ההפעלה, כן. ניתן לעיין ב[רשימת התאימות](/docs/cert-compat) למידע נוסף.

## האם ב־Let's Encrypt מונפקים אישורים לדברים אחרים מלבד SSL/TLS לאתרים?

האישורים של Let's Encrypt הם אישורי תיקוף שם תחום תקניים, לכן ניתן להשתמש בהם בכל שרת שמשתמש בשם תחום, כגון שרתי אינטרנט, שרתי דוא״ל, שרתי FTP ועוד רבים וטובים.

הצפנת דוא״ל וחתימת קוד דורשים סוגים אחרים של אישורים ש־Let's Encrypt אינה מנפיקה.

## האם Let's Encrypt מייצרת או מאחסנת את המפתחות הפרטיים לאישורים שלי בשרתים של Let's Encrypt?

לא. לעולם לא.

המפתח הפרטי תמיד נוצר ומנוהל על השרתים שלך, לא על ידי רשות האישורים Let's Encrypt.

## מה אורך החיים של אישורים מבית Let's Encrypt? למשך כמה זמן הם תקפים?

האישורים שלנו תקפים למשך 90 יום. הסיבה לכך מופיעה [כאן](/2015/11/09/why-90-days.html).

אין דרך לשנות זאת, אין יוצאים מן הכלל. אנו ממליצים לחדש את האישורים שלך אוטומטית כל 60 יום.

## האם Let's Encrypt תנפיק אישורי תיקוף ארגון (OV) או תיקוף מורחב (EV)?

אין לנו תכניות להנפיק אישורי OV או EV.

## אוכל לקבל אישור למגוון שמות תחום (אישורי SAN או UCC)?

כאן, אותו האישור יכול להכיל מספר שמות שונים באמצעות מנגנון SAN (שם חלופי לנושא - Subject Alternative Name).

## האם Let's Encrypt מנפיקה אישורים כוללניים?

כן. הנפקה כוללנית חובה לבצע דרך ACMEv2 באמצעות אתגר DNS-01. ב[רשומה הזאת](https://community.letsencrypt.org/t/acme-v2-production-environment-wildcards/55578) יש קצת יותר פירוט טכני.

## האם יש לקוח של Let's Encrypt‏ (ACME) למערכת ההפעלה שלי?

יש מספר גדול של [לקוחות ACME](/docs/client-options) זמינים. סביר להניח שלפחות אחד מהם עובד נכון על מערכת ההפעלה שלך. אנו ממליצים להתחיל עם [Certbot](https://certbot.eff.org/).

## אוכל להשתמש במפתח פרטי קיים או בבקשת חתימת אישור (CSR)?

כן, אבל לא כל תכניות צד הלקוח תומכות בתכונה הזאת. [Certbot](https://certbot.eff.org/) תומך.

## באילו כתובות IP משתמשת Let's Encrypt כדי לתקף את שרת האינטרנט שלי?

איננו מפרסמים את רשימת כתובות ה־IP בהן אנו משתמשים למטרות תיקוף וכתובות ה־IP האלה עשויות להשתנות בכל עת. כדאי לשים לב שנכון לעכשיו אנו [מתקפים ממגוון כתובות IP](https://letsencrypt.org/2020/02/19/multi-perspective-validation.html).

## חידשתי אישור בהצלחה אך התיקוף לא התרחש כרגע - איך זה יתכן?

לאחר השלמת האתגרים לשם תחום, ההרשאה שמתקבלת נשמרת במטמון של החשבון שלך לשימוש חוזר בעתיד. הרשאות נשמרות למשך 30 יום מרגע התיקוף. אם לאישור שביקשת יש את כל ההרשאות השמורות הנחוצות אז התיקוף לא יתרחש שוב עד לתפוגת תוקף ההרשאות הנוכחיות.