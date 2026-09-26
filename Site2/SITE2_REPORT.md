undefined

## 2026-09-26 — سرویس پیامکی پیشنهادی کارآفرینک: Kpanel / IPPanel

- سرویس پیامکی تهیه‌شده برای شروع پروژه: **Kpanel**، پنل مسی.
- آدرس پنل: https://sms.kpanel.ir/dashboard
- سایت سرویس: https://kpanel.ir/
- مستندات API: https://docs.ippanel.com/docs/
- Base URL رسمی API: `https://edge.ippanel.com/v1`.
- احراز هویت API از طریق هدر `Authorization` انجام می‌شود.
- API Key از مسیر پنل `Developers > Access Keys` ساخته می‌شود؛ API Key برخلاف Token منقضی نمی‌شود.
- یک API Key با عنوان **«کارآفرینک – WooCommerce»** برای اتصال آینده ساخته شده است. مقدار کلید نباید در GitHub یا گزارش‌ها ذخیره شود.

### قابلیت‌های ثبت‌شده برای استفاده در کارآفرینک
- ارسال پیامک عادی و خدماتی
- OTP / کد فعال‌سازی
- پیامک‌های متغیردار با Pattern
- گزارش ارسال و وضعیت پیامک
- Web Service / API برای اتصال سایت و اپلیکیشن
- امکانات دریافت پیامک و مدیریت مخاطبین در پنل

### گزینه افزونه WordPress / WooCommerce
Kpanel در بخش افزونه‌ها این مسیر را معرفی می‌کند:
1. نصب و فعال‌سازی افزونه اصلی **Persian WooCommerce SMS** از WordPress.org.
2. نصب و فعال‌سازی افزونه مکمل Kpanel برای سازگاری با سرویس پیامکی.

افزونه معرفی‌شده:
https://wordpress.org/plugins/persian-woocommerce-sms/

Kpanel همچنین گزینه‌ای با عنوان **«افزونه پیامکی WordPress با قابلیت ارسال پترن»** معرفی می‌کند که افزونه مکمل WP-SMS است و برای پیامک‌های پترنی قابل بررسی است.

### تصمیم اجرایی
- برای مشتریانی که در سفارش طراحی سایت درخواست **سرویس پیامکی** دارند، Kpanel به‌عنوان سرویس پیشنهادی/مرجع پیش‌فرض کارآفرینک ثبت شود، مگر اینکه نیاز یا سرویس دیگری از طرف مشتری مطرح شود.
- هزینه خرید پنل و اعتبار پیامکی سرویس شخص ثالث از هزینه خدمات اجرایی کارآفرینک جداست.
- قبل از اجرای نهایی در WordPress، افزونه مناسب Kpanel/WooCommerce و پشتیبانی آن از Pattern/OTP بررسی و تست می‌شود.
- API Key فقط در تنظیمات امن سمت سرور/WordPress نگهداری خواهد شد و هرگز در GitHub، فایل عمومی JavaScript یا گزارش پروژه قرار نمی‌گیرد.

### اطلاعات تجاری فعلی پنل مسی
- هزینه پنل: ۵۵٬۰۰۰ تومان
- شارژ اولیه: ۵۰٬۰۰۰ تومان
- تعرفه پایه ارسال: ۲۸۴٫۸ تومان برای هر پیامک
- طبق اطلاعات ارائه‌شده از پنل، سرعت و زمان ارسال مسی و نقره‌ای مشابه است و تفاوت اصلی هزینه پنل و تعرفه ارسال است.

این بخش به‌عنوان مرجع اولیه سرویس پیامکی ثبت شده و اطلاعات تکمیلی که بعداً از پنل Kpanel ارائه شود باید در همین گزارش تکمیل شود.


## 2026-09-26 — ثبت مرجع افزونه سرویس پیامکی در ریپوی Plugins

مستندات بدون اطلاعات محرمانه سرویس Kpanel/IPPanel برای استفاده در پیاده‌سازی افزونه‌های کارآفرینک در ریپوی خصوصی زیر ثبت شد:
- Repository: `samadkarami-boop/Karafarinak-Plugins`
- Path: `sms/kpanel/README.md`
- Commit: `00b368e7e8cbff766206636c6660cde3873daae1`

این فایل شامل آدرس سایت و پنل، مستندات API، Base URL، روش احراز هویت، قابلیت Pattern/OTP، افزونه‌های معرفی‌شده توسط Kpanel، سیاست نگهداری API Key و مشخصات پنل مسی خریداری‌شده است.

از این پس در سفارش‌هایی که مشتری «سرویس پیامکی» درخواست کند، Kpanel به‌عنوان گزینه پیشنهادی ثبت‌شده کارآفرینک در نظر گرفته می‌شود؛ مگر اینکه نیاز یا سرویس دیگری از طرف مشتری مطرح باشد. هزینه سرویس شخص ثالث از هزینه خدمات اجرایی کارآفرینک جدا خواهد بود.

مقادیر API Key و سایر اطلاعات محرمانه عمداً در گزارش‌ها و GitHub ذخیره نمی‌شوند.


## 2026-09-26 — تکمیل Previewهای Dynamic و Release Assetهای Static

### Dynamic Template Preview
- ریپوی مرجع Dynamic: `samadkarami-boop/Karafarinak-Base`.
- موتور مشترک `_engine` بررسی و رندر واقعی Variationها با Chromium/Playwright انجام شد.
- در مجموع **54 Variation** موجود در Base برای Preview ثبت شد:
  - 49 Variation سایت‌های محتوایی/خدماتی
  - 5 Variation فروشگاهی
- مسیر استاندارد هر Preview: `<Family>/<Variation>/preview/cover.png`.
- وجود واقعی هر 54 فایل `preview/cover.png` در tree فعلی GitHub تأیید شد.
- نسخه فعلی Branch `main` در Base که Previewها و گزارش Verification را دربر دارد: `74dbd6d461ec8a135298d12f83c16da37eabfeda`؛ commit اصلی تولید 54 Preview: `1cf5e0c8321edacf2cb35a09e60767d48065aae4`.
- نکته معماری: Previewها از Template واقعی Base و موتور مشترک تولید شده‌اند؛ تصویر ساختگی یا AI-generated جایگزین قالب واقعی نشده است.

### Static Template Release
- ریپوی مرجع: `samadkarami-boop/KRF-WEB-001-Corporate`.
- برای 6 قالب Static، Homepage Screenshot با Chromium/Playwright در viewport `1440×1000` تولید و در `preview/cover.png` ثبت شد.
- برای هر 6 قالب، ZIP نهایی از `package/` ساخته و با `unzip -t` اعتبارسنجی شد.
- Run نهایی ساخت Release Assetها: `36192954576` — **success**.
- ZIPها در همان مسیر محصول قرار دارند و برای مرحله بعدی اتصال به WooCommerce/Download آماده‌اند.

## 2026-09-26 — بررسی راهنمای افزونه WordPress پیامکی

- دسترسی به تصاویر `makhzan/12.jpg` تا `makhzan/20.jpg` مجدداً بررسی و این بار **تصویری خوانده شد**.
- راهنما مربوط به **WP-SMS** است و در تصاویر نسخه نمایشی `5.4.1` دیده می‌شود.
- موارد عملیاتی مشاهده‌شده شامل اتصال iPPANEL، شماره مدیر، کد کشور، شماره خط ارسال، Unicode، Clean Numbers، گروه‌ها، Verify Subscriber، Welcome SMS، قواعد شماره موبایل، International Telephone Input، REST API، اطلاع‌رسانی رویدادها و یکپارچه‌سازی با WooCommerce/EDD/Contact Form 7 است.
- راهنما نشان می‌دهد WP-SMS مسیر اتصال به iPPANEL را دارد؛ برای پروژه کارآفرینک، اتصال Kpanel/IPPanel باید در محیط WordPress تست شود و Pattern سرویس از مسیر رسمی Kpanel/IPPanel پیاده‌سازی شود.
- هیچ API Key، رمز عبور یا credential واقعی در گزارش ثبت نشده است.
- جزئیات این بررسی نیز در `Karafarinak-Plugins/sms/kpanel/README.md` ثبت شد.
- Commit ثبت مستندات افزونه: `245b3d748e6242122726989168b326b0b547a785`.

## وضعیت مسیر کار بعد از این مرحله
- Site2 static/dynamic source و مستندات آن‌ها تکمیل و ممیزی شده‌اند.
- Previewهای Dynamic برای 54 Variation ثبت شده‌اند.
- ZIPهای Static برای 6 قالب فعلی ساخته و اعتبارسنجی شده‌اند.
- راهنمای WP-SMS/Kpanel بررسی و در Plugins ثبت شده است.
- مرحله بعدی فنی، **پیاده‌سازی/تست WordPress + WooCommerce بر مبنای نسخه نهایی Site2** است؛ قبل از انتقال نهایی، در صورت تغییر طراحی یا قرارداد فروش در Site2، WordPress باید از نسخه تأییدشده نهایی تغذیه شود.

## 2026-09-26 — شروع عملیات محیط آزمایشی WordPress و WooCommerce

### هدف این مرحله
پس از تکمیل و ممیزی نسخه فعلی Site2، عملیات انتقال کنترل‌شده به WordPress آغاز می‌شود. هدف این مرحله، ایجاد یک محیط آزمایشی جدا از سایت اصلی است تا WordPress، WooCommerce و افزونه‌ها بدون ایجاد ریسک برای `karafarinak.ir` پیاده‌سازی و تست شوند.

### الگوی کنترل و تست مصوب
روند اجرای WordPress از این پس به‌صورت مرحله‌ای و قابل کنترل خواهد بود:

1. تثبیت نسخه نهایی Site2 به‌عنوان مرجع طراحی.
2. ایجاد محیط آزمایشی جداگانه روی هاست ParsPack، ترجیحاً با یک Subdomain مانند `test.karafarinak.ir`.
3. ایجاد دیتابیس و تنظیمات مستقل برای محیط آزمایشی.
4. نصب WordPress پایه و انجام تست اولیه.
5. نصب و پیکربندی WooCommerce و انجام تست مستقل.
6. افزودن افزونه‌های موردنیاز به‌صورت مرحله‌ای، نه هم‌زمان.
7. پس از هر مرحله، اجرای تست واقعی با مرورگر Chromium/Playwright در Desktop، Tablet و Mobile.
8. تهیه Screenshot از صفحات و بخش‌های مهم و مقایسه با Preview مرجع Site2.
9. در صورت مشاهده اختلاف یا به‌هم‌ریختگی: اصلاح، تست مجدد و ثبت نتیجه؛ تا تأیید مرحله قبلی، مرحله بعد شروع نمی‌شود.
10. پس از تأیید کامل محیط آزمایشی، انتقال نسخه تأییدشده به سایت اصلی.

### ترتیب شروع عملیات
در این تاریخ، **مرحله آماده‌سازی محیط آزمایشی** به‌عنوان گام بعدی فنی ثبت شد. نصب WordPress و WooCommerce باید پس از آماده و قابل دسترس شدن محیط آزمایشی انجام شود و نصب افزونه‌های جانبی نیز پس از تست WordPress/WooCommerce و به‌صورت مرحله‌ای خواهد بود.

### اصل کنترل نسخه
GitHub محل اجرای WordPress نیست؛ محیط آزمایشی روی هاست اجرا می‌شود و Screenshotها، نتایج تست، تغییرات و وضعیت تأیید در GitHub مستندسازی خواهند شد. Previewهای Static/Dynamic موجود در Site2 مرجع مقایسه بصری خواهند بود.

### وضعیت
- Site2: آماده ورود به مرحله پیاده‌سازی آزمایشی WordPress.
- محیط آزمایشی WordPress: **باید ایجاد شود**.
- WordPress: **هنوز نصب نشده**.
- WooCommerce: **هنوز نصب نشده**.
- افزونه‌ها: **هنوز وارد مرحله نصب نشده‌اند**.
- سایت اصلی: **فعلاً بدون تغییر**.



## 2026-09-26 — ثبت رسمی Backup مرجع قبل از WordPress

برای جلوگیری از اشتباه در تشخیص Backup، مرجع زیر مستقیماً بررسی و تأیید شد:

- Repository: `samadkarami-boop/Karafarinak-wordpress`
- Backup رسمی Site2: `backups/Site2-2026-09-25/`
- تاریخ Snapshot: **2026-09-25**
- Commit مبنای Snapshot: `4fdf15479881a86a997453a3ec8ba8f9e55827de`
- Commit ثبت Backup/Archive: `f9387252ff3b1631398e689182bc3959366377f9`
- این Snapshot شامل فایل‌های Site2، HTML/CSS/SVG/تصاویر، گزارش و پوشه Preview است.
- این Backup برای **Recovery و مقایسه نسخه قبل از پیاده‌سازی WordPress** نگهداری می‌شود و محل ادامه توسعه طراحی نیست.
- آرشیو WordPress قبلی نیز جداگانه در `archive/wordpress-original-2026-09-25/` قرار دارد.

مرجع‌های رسمی پروژه از این مرحله:
1. `samadkarami-boop/KARAFARINAK-WEB-Demos/Site2/` → منبع اصلی و جاری طراحی.
2. `samadkarami-boop/Karafarinak-wordpress/backups/Site2-2026-09-25/` → Backup مرجع قبل از WordPress.
3. `samadkarami-boop/Karafarinak-wordpress/archive/wordpress-original-2026-09-25/` → آرشیو WordPress قبلی.

از این مرحله به بعد، هیچ تغییر طراحی WordPress نباید به‌عنوان منبع طراحی اصلی ثبت شود؛ طراحی باید از نسخه تأییدشده Site2 تغذیه شود.

## 2026-09-26 — اجرای گام بعد: آماده‌سازی محیط آزمایشی WordPress

### وضعیت اجرای واقعی
گام بعدی پروژه مشخص و وارد فاز اجرا شد: **ایجاد محیط آزمایشی جدا از سایت اصلی**.

مشخصات محیط آزمایشی پیشنهادی:
- Subdomain: `test.karafarinak.ir`
- محیط اجرا: همان ParsPack Cloud Linux موجود
- پنل مدیریت: DirectAdmin
- دیتابیس: کاملاً مستقل از دیتابیس سایت اصلی
- WordPress: نصب تازه و مستقل
- WooCommerce: هنوز نصب نشود تا WordPress پایه تست شود
- افزونه‌ها: تا قبل از تأیید WordPress و WooCommerce نصب نشوند

### ترتیب اجرایی قفل‌شده
1. ساخت `test.karafarinak.ir` در DirectAdmin.
2. فعال‌سازی SSL برای Subdomain.
3. ساخت Database و Database User مستقل برای Test.
4. اطمینان از اتصال دامنه آزمایشی و باز شدن صفحه Test.
5. نصب WordPress پایه.
6. تست WordPress خام در Desktop / Tablet / Mobile.
7. پس از تأیید WordPress پایه، نصب WooCommerce.
8. سپس نصب افزونه‌ها یکی‌یکی و تست بعد از هر نصب.

### کنترل ریسک
- به `karafarinak.ir` اصلی دست زده نمی‌شود.
- دیتابیس Test نباید با دیتابیس Live مشترک باشد.
- قبل از تأیید WordPress پایه، WooCommerce و افزونه‌های جانبی نصب نمی‌شوند.
- Backup مرجع Site2 در `Karafarinak-wordpress/backups/Site2-2026-09-25/` دست‌نخورده باقی می‌ماند.

### وضعیت فعلی
- Site2: آماده.
- Backup مرجع: تأییدشده.
- محیط Test: **نیازمند ساخت در DirectAdmin**.
- WordPress: نصب نشده.
- WooCommerce: نصب نشده.
- Plugins: نصب نشده.
- Live: بدون تغییر.

**گام عملی باقی‌مانده برای خروج از حالت آماده‌سازی:** ساخت Subdomain `test.karafarinak.ir` و SSL در DirectAdmin. پس از در دسترس شدن این آدرس، نصب WordPress پایه آغاز می‌شود.


## 2026-09-26 — تکمیل واقعی آماده‌سازی محیط آزمایشی WordPress

### موارد انجام‌شده در DirectAdmin
محیط آزمایشی طبق برنامه در هاست ParsPack ایجاد و اتصال آن به دامنه تأیید شد:

- Subdomain: `test.karafarinak.ir` با موفقیت ساخته شد.
- Document Root: `/domains/test.karafarinak.ir/public_html`
- SSL برای `test.karafarinak.ir` به‌صورت خودکار فعال و گواهی اختصاصی آن در DirectAdmin ثبت شد.
- تاریخ اعتبار گواهی ثبت‌شده در زمان بررسی: **25 دسامبر 2026**.
- آدرس `https://test.karafarinak.ir` با موفقیت باز شد و صفحه Placeholder مربوط به همین Subdomain نمایش داده شد؛ بنابراین مسیر دامنه، HTTPS و Document Root عملیاتی هستند.

### دیتابیس مستقل Test
برای جلوگیری از هرگونه تداخل با سایت استاتیک قبلی و درگاه پرداخت، دیتابیس جدید و مستقل ساخته شد:

- Database: `h423580_wp_test`
- Host: `localhost`
- Username: `h423580_wp_test`
- Password: **عمداً در گزارش/GitHub ثبت نمی‌شود.**

دیتابیس موجود `h423580_payment` مربوط به سایت استاتیک قبلی و درگاه پرداخت است و **نباید در محیط WordPress تست استفاده یا تغییر داده شود**.

### وضعیت فایل‌های محیط Test
در مسیر `/domains/test.karafarinak.ir/public_html` هنگام بررسی فقط فایل‌های پیش‌فرض DirectAdmin مشاهده شد:
- `index.html` (Placeholder)
- `cgi-bin/`

بنابراین محیط برای نصب WordPress تمیز است و هنوز هیچ فایل WordPress در آن قرار نگرفته است.

### وضعیت فعلی
- Subdomain: **انجام شد**.
- SSL: **انجام شد**.
- اتصال HTTPS و Placeholder: **تأیید شد**.
- Database مستقل: **انجام شد**.
- WordPress: **هنوز نصب نشده**.
- WooCommerce: **هنوز نصب نشده**.
- Plugins: **هنوز نصب نشده**.
- سایت اصلی و دیتابیس Live: **بدون تغییر**.

### گام بعدی
قبل از نصب WordPress، نسخه و تنظیمات PHP محیط Test باید مشخص/تأیید شود. پس از آن WordPress پایه نصب و بدون WooCommerce یا افزونه جانبی تست خواهد شد. اطلاعات محرمانه مانند رمز دیتابیس یا API Key در گزارش و GitHub ثبت نخواهد شد.
