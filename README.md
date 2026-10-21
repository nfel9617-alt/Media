# إعداد التطبيق مع Google Sheets (حوالي 10 دقائق، مجاني)
1. أنشئ Google Sheet جديد (اسمه مثلاً: NCCF Media).
2. Extensions ← Apps Script. احذف الكود الموجود والصق محتوى Code.gs.
3. غيّر ADMIN_PIN إلى رمز سري للمسؤولين. (اختياري: TG_TOKEN وTG_CHAT لبوت تلغرام.)
4. اختر الدالة setup من القائمة واضغط Run، ووافق على الصلاحيات (مرة واحدة). ستُنشأ الأوراق تلقائياً.
5. Deploy ← New deployment ← النوع: Web app ← Execute as: Me ← Who has access: Anyone ← Deploy، وانسخ رابط Web app.
6. افتح index.html وضع الرابط في C.api.
7. انشر المجلد على استضافة HTTPS مجانية (مثل Netlify Drop بسحب المجلد، أو GitHub Pages). التثبيت كتطبيق يحتاج HTTPS.
8. ضع رابط الموقع في APP_URL داخل Code.gs ثم Deploy ← Manage deployments ← Edit ← New version.
9. كل عضو يثبّت تطبيق ntfy ويشترك في الموضوع المكتوب في NTFY_TOPIC.
10. أول دخول كمسؤول: الإدارة ← اكتب الرمز ← استيراد برنامج اليوم 1. ويمكنك تعديل ورقة program مباشرة في الجدول.
ملاحظة: بعد أي تعديل في Code.gs لازم تنشر نسخة جديدة (Manage deployments ← New version).
