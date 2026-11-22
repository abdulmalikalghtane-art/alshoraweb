# Majlis Al-Shura | مجلس الشورى

* **بناء الهوية البصرية:** قمت بتصميم الهوية المرئية وتوزيع العناصر والألوان بنفسي في ملفات الواجهة (`index.html` و `profile.html` و `memmber.html` و `script.js`).
* **تصميم عناصر المحادثة:** قمت بابتكار وتنسيق صناديق الرسائل، شريط التنقل الجانبي بين الغرف، وحقول كتابة النصوص، وقوائم الأعضاء من الصفر.
* **التعديل والتجربة المستمرة:** قمت بإعادة هيكلة وتوزيع الواجهات عشرات المرات بعد تجربتها عملياً على المتصفح للوصول إلى أفضل توزيع بصري.
* **تنسيق الهوامش والخطوط:** عدّلت الهوامش الداخلية والخارجية (Margins & Padding)، واخترت الخطوط وألوان العناصر لضمان وضوح النصوص وراحة العين.
* **استجابة الشاشات (Responsive Design):** قمت بضبط وتجربة استجابة العناصر على مختلف الأجهزة (جوالات وكمبيوتر) لمنع تداخل الأزرار أو النصوص أثناء التصفح.
* **سلاسة التنقل:** اختبرت وضبطت تنقل المستخدم بين غرف المحادثة والصفحات الشخصية لضمان تجربة استخدام سهلة ودون بطء.
* **إدارة الهيكلية البرمجية:** قمت بتنظيم الأكواد وتوزيع الوظائف داخل ملف `script.js` وربطها المباشر بعناصر الـ HTML.
* **التحكم بعناصر الصفحة (DOM Manipulation):** برمجت الاستجابة المباشرة للأزرار، القوائم الجانبية، والناظر التفاعلية داخل الواجهة.
* **التمرير التلقائي (Auto-Scroll):** قمت ببرمجة ميزة التمرير الآلي لأسفل المحادثة فور وصول أي رسالة جديدة لضمان متابعة المحادثة دون تدخل يدوي.
* **معالجة النصوص والمدخلات:** كتبت أكواد فحص النصوص المكتوبة وتنظيفها قبل إرسالها لمنع الأخطاء البرمجية وضمان سلامة البيانات.
* **تتبع الأخطاء في المتصفح:** قضيت ساعات طويلة أمام أدوات المطور (F12 Developer Console) لتتبع الأكواد خطوة بخطوة وفحص سلوك كل زر وحقل.
* **معالجة استثنائيات الشبكة:** قمت بكتابة أكواد للتعامل مع بطء الاستجابة أو انقطاع الاتصال المفاجئ لضمان استقرار التطبيق
* **هندسة الجداول:** قمت بتصميم وتنفيذ هيكلية البيانات في Supabase وربط العلاقة بين جدول الرسائل (`messages`) وجداول الحسابات.
* **الربط الحقيقي (WebSockets):** فعلت ميزة التحديث المباشر عبر بروتوكول WebSockets واستدعاء `postgres_changes` لمراقبة جدول الرسائل فورياً.
* **جلب واستخراج البيانات:** برمجت آلية استخراج محتوى الرسالة، اسم المُرسل، رتبته، صورته الشخصية، والتوقيت فور إضافة أي سجل جديد.
* **العرض اللحظي:** قمت بضبط الواجهة لعرض الرسائل القادمة فوراً داخل الروم دون الحاجة لإعادة تحميل الصفحة أو إجراء استعلامات مكررة.
* **إدارة الدومين والـ DNS:** قمت بربط وتثبيت اسم النطاق الخاص بالمنصة وتوجيه سجلات الـ DNS بالكامل عبر منصة Cloudflare.
* **إعداد وحدات التخزين السحابية:** قمت بتهيئة حاويات التخزين (Storage Buckets) في Cloudflare لاستقبال الصور الفيديوهات المرفوعة من الأعضاء.
* **مسار رفع الوسائط:** برمجت آلية استقبال الملفات من الواجهة الأمامية ورفعها كـ Binary Stream مباشر إلى وحدات التخزين.
* **توليد الروابط المباشرة:** قمت ببرمجة استخراج الرابط العام المباشر (Public URL) فور مكتمل الرفع، وحفظه داخل سجل الرسالة في قاعدة البيانات.
* **عرض الوسائط المدمج:** قمت بتهيئة الواجهة الأمامية لقراءة روابط الوسائط وعرض الصور والفيديوهات بشكل مدمج داخل المحادثة مباشرة.
* **تصميم البروفايل الشخصي:** أنشأت واجهات البروفايل لكل عضو لعرض اسمه، صورته الشخصية (Avatar)، رتبته، وحالته التفاعلية.
* **إدارة الرتب والصلاحيات:** قمت بتوزيع الصلاحيات داخل المنصة وتصنيف الأعضاء (عضو / مشرف / أدمن) وتفعيل الخصائص المخصصة لكل رتبة.
* **بناء جدول الحظر:** قمت بإنشاء جدول الحظر (`ban:`) في قاعدة البيانات وفحص بيانات الحسابات المقيّدة.
* **الفحص الآلي عند الدخول:** برمجت السكربت لفحص هوية المستخدم وحالته في جدول الحظر فور تسجيل الدخول وأثناء التنقل.
* **تقييد الوصول آلياً:** في حال وجود الحساب في قائمة الحظر، يتم قفل حقول الكتابة، تعطيل أزرار الإرسال، وإخفاء واجهات الغرف تلقائياً.

* **التعامل مع توقف الخدمة:** عند توقف خدمة Firebase بشكل غير متوقع، قمت بالتدخل المباشر لحماية سجلات وحسابات الأعضاء من الضياع.
* **الاستخراج اليدوي للبيانات:** قمت بسحب الملفات الخام وقواعد البيانات يدوياً قبل إغلاق الخدمة أو تقييد الوصول إليها.
* **فك تشفير السجلات:** كتبت وسيّرت سكربتات خاصة لفك تشفير البيانات الحساسة وسجلات الحسابات المسحوبة.
* **التدقيق اليدوي لسلامة البيانات:** قمت بمراجعة البيانات والحقول خطوة بخطوة يدوياً للتحقق من عدم تلف أي سجل أو حساب.
* **إعادة الهيكلة والنقل الكامل:** أعدت بناء الجداول والنظام على Supabase وربطت التخزين بـ Cloudflare، ونقلت كامل البيانات بنجاح 100% (Zero Data Loss).

* **Visual Identity Setup:** Designed the platform's visual identity, layout architecture, and color schemes across `index.html`, `profile.html`, `memmber.html`, and `script.js`.
* **Custom Chat UI Components:** Built custom visual elements from scratch, including message containers, room navigation sidebars, text input fields, and active user lists.
* **Iterative Layout Testing:** Re-architected and adjusted element layouts through dozens of browser testing iterations to establish an optimal visual structure.
* **Typography & Spacing Adjustments:** Fine-tuned margin spacing, padding, font choices, and element contrast to ensure readability and comfortable visual hierarchy.
* **Responsive Layout Optimization:** Tested layout responsiveness across mobile and desktop viewports to prevent element overlap and UI breaking.
* **Smooth Room Navigation:** Tested and optimized room switching and profile toggling to guarantee seamless user transitions without visual lag.
* **Codebase Architecture:** Structured frontend execution logic inside `script.js` and managed component bindings with HTML documents.
* **DOM Manipulation Engine:** Programmed real-time client-side interactions for button triggers, side drawers, dynamic modals, and room feeds.
* **Automatic Smooth-Scroll:** Implemented automatic view-scrolling script logic to lock scroll positions to the latest message upon insertion.
* **Input Validation & Sanitization:** Wrote text validation routines to handle incoming input data, preventing runtime injection errors and malformed payloads.
* **Browser Console Debugging:** Conducted extensive debugging sessions inside browser developer tools (F12) to trace execution flow line-by-line.
* **Network Exception Handling:** Programmed client-side error handling to manage network latency, request timeouts, and unexpected disconnections gracefully.
* **Schema Architecture:** Designed relational database schemas in Supabase linking profile data with the chat message repository (`messages`).
* **WebSocket Integration:** Configured realtime WebSocket listeners using `postgres_changes` on the `messages` table to monitor new rows dynamically.
* **Payload Extraction:** Programmed parsing logic to extract message body content, sender handle, user rank, avatar URL, and timestamps upon insertion.
* **Instant Feed Rendering:** Dynamically updated active room interfaces with new incoming messages without requiring page reloads or polling.
* **DNS & Domain Setup:** Managed custom domain routing, SSL security, and DNS record settings through Cloudflare's management console.
* **Cloud Storage Buckets:** Configured Cloudflare Storage Buckets dedicated to storing user-uploaded images and videos within active chat rooms.
* **Media Upload Pipeline:** Programmed client-side upload routines to stream binary media files directly from client devices to cloud storage.
* **Public URL Generation:** Automated the generation of public URLs upon upload completion and recorded these media links directly into database payloads.
* **Inline Media Rendering:** Configured message components to parse stored media links and render inline image/video players directly in chat feeds.
* **Profile Component Design:** Engineered individual user profile interfaces displaying account usernames, custom avatar URLs, user ranks, and status.
* **Role-Based Access Control:** Configured platform permission levels (User / Moderator / Admin) to handle feature authorization dynamically.
* **Ban Table System:** Implemented a dedicated ban tracking table (`ban:`) in the database to store and query restricted account identifiers.
* **Automated Identity Auditing:** Programmed authentication scripts to validate session tokens against the ban list during login and navigation.
* **Access Revocation:** Automatically locked text inputs, disabled send buttons, and revoked room visibility if an account was flagged as restricted.
* **Emergency Incident Intervention:** Responded immediately to an unannounced Firebase provider disruption to safeguard stored user records.
* **Manual Data Extraction:** Extracted raw database dumps and user logs prior to service lock-out.
* **Decryption Processing:** Wrote and executed custom decryption scripts to recover encrypted credentials and database records.
* **Line-by-Line Data Audit:** Manually verified database rows and user records line-by-line to ensure full structural integrity.
* **Backend Migration:** Re-built backend schemas on Supabase paired with Cloudflare storage, achieving 100% data preservation with zero record loss.****
