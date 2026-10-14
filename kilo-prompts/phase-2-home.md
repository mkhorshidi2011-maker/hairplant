# فاز ۲ — صفحه اصلی و کامپوننت‌های مشترک

فایل `PROJECT_BRIEF.md` را بخوان (بخش‌های ۶، ۸ و ۱۳). فاز ۱ تأیید شده است. **فقط کارهای همین فاز را انجام بده.**

## کارها

1. صفحه اصلی را با **۱۲ بخش** بخش ۶ بساز، به ترتیب و ریسپانسیو.
2. همه تصویرها و ویدیوها فقط از طریق `MediaSlot`، `VideoSlot` و `BeforeAfter` و اسلات‌های `content/media.json` باشند. اگر اسلات جدیدی لازم شد، به مانیفست اضافه کن و `media:placeholders` و `media:report` را دوباره اجرا کن.
3. کامپوننت‌های قابل استفاده مجدد در `components/sections` و `components/ui`:
   - `HeroSection`، `TrustCard`، `ServiceCard`، `StatsStrip`، `TestimonialSlider`، `CtaBanner`، `WhyUsList`
   - `BeforeAfterSlider` (مقایسه کشویی با پشتیبانی کیبورد و لمس)
   - `ArticleCard`، `MapBlock` (Neshan/Balad با fallback)، `VipFeatures`، `SocialLinks`
4. محتوای متنی صفحه اصلی در `content/home.json` یا MDX تا قابل ویرایش بدون کد باشد. متن‌ها اصیل، محتاطانه و بدون آمار جعلی باشند. بخش‌های آمار و نظرات فقط وقتی داده واقعی هست نمایش داده شوند و در غیر این صورت با placeholder واضح «نمونه» نشان داده شوند (فقط در development).
5. انیمیشن ملایم با احترام به `prefers-reduced-motion`.

## معیار پذیرش

- صفحه اصلی کامل و بدون layout shift، همه تصویرها placeholder محلی هستند و هیچ درخواست شبکه خارجی نمی‌رود.
- Lighthouse موبایل ≥ 85 (گزارش را بیاور).
- `lint`، `typecheck` و `build` بدون خطا.

## پایان کار

گزارش با فرمت بخش ۱۴ و منتظر تأیید بمان.
