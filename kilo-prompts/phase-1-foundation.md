# فاز ۱ — پایه پروژه، RTL، Layout و سیستم رسانه موقت

فایل `PROJECT_BRIEF.md` را بخوان (به‌ویژه بخش‌های ۲، ۴، ۸ و ۱۳). فاز ۰ تأیید شده است و می‌توانی کدنویسی را شروع کنی. **فقط کارهای همین فاز را انجام بده.**

## کارها

1. راه‌اندازی پروژه: Next.js (App Router) + TypeScript strict + Tailwind + shadcn/ui + ESLint + Prettier + pnpm. اسکریپت‌های `lint`، `typecheck`، `build`.
2. تنظیم RTL: `<html lang="fa" dir="rtl">`، استفاده از logical properties، شامل ایجاد کامپوننت‌های پایه shadcn با رفتار RTL درست (آیکن‌های جهت‌دار برعکس).
3. فونت Vazirmatn به صورت **self-host** (در `public/fonts` با `next/font/local`)، وزن‌های لازم، `font-display: swap`.
4. توکن‌های طراحی (رنگ، فاصله، شعاع گوشه، سایه) در `tailwind.config` طبق پالت تأییدشده.
5. Layout اصلی: هدر کامل (منوی خدمات با زیرمنو، دکمه رزرو سریع)، منوی موبایل، نوار ثابت پایین موبایل (تماس + رزرو)، فوتر طبق بخش ۵.
6. فایل `content/site.json` با اطلاعات placeholder کلینیک (نام، تلفن، آدرس، شبکه‌های اجتماعی) و یک helper برای خواندن آن.
7. **سیستم رسانه موقت** دقیقاً طبق بخش ۱۳:
   - کامپوننت‌های `MediaSlot`، `VideoSlot`، `BeforeAfter`
   - `content/media.json` با همه اسلات‌های اولیه
   - اسکریپت‌های `media:placeholders`، `media:sync`، `media:report`، `media:check`
   - تولید SVG های موقت برای همه اسلات‌ها و اجرای `media:report`
   - یک صفحه `/_dev/media` (فقط در development) که همه اسلات‌ها را به صورت شبکه نشان دهد
8. فایل‌های `.env.example`، `DECISIONS.md`، `TODO_CONTENT.md` و `README.md` اولیه.
9. `Dockerfile` و `docker-compose.dev.yml` برای توسعه (app + postgres).

## معیار پذیرش

- ناوبری کامل روی موبایل و دسکتاپ، RTL درست و بدون به‌هم‌ریختگی.
- `/_dev/media` همه placeholder ها را با ابعاد درست نشان می‌دهد.
- جایگزین‌کردن یک فایل مثل `public/media/hero-main.webp` و اجرای `pnpm media:sync` آن را بدون تغییر کد جایگزین می‌کند (با یک تصویر تست نشان بده).
- `lint`، `typecheck` و `build` بدون خطا.

## پایان کار

گزارش با فرمت بخش ۱۴ و منتظر تأیید بمان.
