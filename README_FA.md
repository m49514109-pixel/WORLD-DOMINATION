# WORLD DOMINATION — Android Edition (V41)

پروژه اندرویدی بازی با رابط نئونی V41 و موسیقی اختصاصی «Rise of Empires».

## ساخت APK با GitHub Actions

1. یک مخزن جدید در GitHub بساز.
2. فایل ZIP را استخراج کن و **محتویات داخل پوشه `WORLD_DOMINATION_ANDROID`** (یعنی پوشه‌های `app` و `.github` و فایل‌های Gradle) را در ریشه مخزن GitHub بارگذاری کن؛ خود پوشه‌ی والد را داخل مخزن نگذار.
3. در GitHub وارد زبانه **Actions** شو.
4. گردش‌کار **Build WORLD DOMINATION APK** را انتخاب و **Run workflow** را بزن. با Push به شاخه `main` یا `master` هم خودکار اجرا می‌شود.
5. پس از پایان موفق، پایین صفحه اجرای Workflow در بخش **Artifacts**، فایل `WORLD-DOMINATION-APK` را دانلود کن.
6. ZIP آرتیفکت را استخراج و `app-debug.apk` را روی گوشی اندرویدی نصب کن.

## ساخت با Android Studio

پوشه `WORLD_DOMINATION_ANDROID` را در Android Studio باز کن، Gradle Sync را انجام بده و از **Build → Build APK(s)** خروجی بگیر.

## مشخصات

- شناسه برنامه: `com.worlddomination.game`
- حداقل نسخه اندروید: Android 6.0 (API 23)
- Compile/Target SDK: 35
- Java: 17
- Gradle: 8.9 / Android Gradle Plugin: 8.7.3
- بازی V41 داخل APK بسته‌بندی شده؛ برای ورود، همگام‌سازی آنلاین و کتابخانه‌های خارجی اینترنت لازم است.

## نکته مهم

این بسته، **پروژه کامل اندروید** است، نه APK آماده نصب. در محیط فعلی Android SDK و Gradle نصب نیست؛ بنابراین امکان کامپایل و تأیید اجرای APK در همین محیط وجود ندارد. گردش‌کار GitHub بالا برای ساخت APK تنظیم شده است.
