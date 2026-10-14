# فاز ۵ — سئو، دسترس‌پذیری و کیفیت

فایل `PROJECT_BRIEF.md` را بخوان (بخش‌های ۸، ۹، ۱۰ و ۱۳). فاز ۴ تأیید شده است. **فقط کارهای همین فاز را انجام بده.**

## کارها

1. `metadata` اختصاصی هر صفحه: title، description، canonical، Open Graph با `og:locale=fa_IR`. استفاده از `og-default` برای صفحاتی که تصویر ندارند.
2. `sitemap.xml` و `robots.txt` پویا (بدون صفحات admin و `/_dev`).
3. **JSON-LD:** `MedicalClinic` (یا `LocalBusiness`)، `BreadcrumbList` در همه صفحات داخلی، `FAQPage`، و `Article` برای مقالات. خروجی را با یک اسکریپت یا تست بررسی کن.
4. دسترس‌پذیری WCAG 2.1 AA: کنتراست، focus visible، ترتیب tab، `aria-label` ها، یک H1 در هر صفحه، کنترل با کیبورد برای منو، آکاردئون، اسلایدر قبل/بعد و لایت‌باکس. از `axe` در تست خودکار استفاده کن.
5. بهینه‌سازی عملکرد: `next/image` با اندازه‌های درست، ویدیو با `preload="none"` و poster، حذف JS اضافی، بررسی CLS.
6. تست E2E با Playwright: مسیر رزرو (موفق و ناموفق)، ناوبری منو، فیلتر مجله، ورود ادمین.
7. بررسی رسانه موقت: `pnpm media:check` درست کار کند، و حالت `MEDIA_STRICT=1` وقتی placeholder باقی است build را fail کند. نشان بده.
8. بررسی لینک‌های شکسته داخلی و اجرای مجدد جستجوی عبارات ممنوع محتوا.

## معیار پذیرش

- Lighthouse موبایل: Performance ≥ 90، SEO ≥ 95، Accessibility ≥ 95 (گزارش عددی بیاور؛ اگر placeholder ها مانع شدند، دلیلش را بنویس).
- تست‌های E2E و axe سبز.
- `lint`، `typecheck` و `build` بدون خطا.

## پایان کار

گزارش با فرمت بخش ۱۴ و منتظر تأیید بمان.
