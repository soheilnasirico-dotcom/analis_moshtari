# Knowledge Base: آناتومی وب‌سایت (Page → Section → Component → Content)

> **نوع سند:** مرجع Requirement طراحی برای AI Agent متخصص استراتژی/طراحی وب‌سایت
> **کاربرد:** تجزیهٔ سلسله‌مراتبی هر صفحه به اجزای قابل‌اجرا، برای استفاده در تولید Wireframe، Brief طراحی، یا تخصیص کار به تیم محتوا/طراحی/توسعه.
> **سلسله‌مراتب مرجع:**
> `Page (صفحه) → Section (بخش) → Component (مؤلفهٔ رابط کاربری) → Content (نوع محتوای موردنیاز)`

---

## بخش صفر: منطق ساختاری کلی

**Page (صفحه):** یک واحد ناوبری مستقل با URL خاص خودش و هدف کاربری واحد (مثلاً «متقاعدکردن» در Homepage، «اثبات صلاحیت» در About).

**Section (بخش):** بلوک عمودی داخل یک صفحه که یک پیام/کارکرد واحد را حمل می‌کند. هر Section باید به‌تنهایی قابل‌فهم باشد حتی اگر کاربر فقط تا آن نقطه اسکرول کند.

**Component (مؤلفه):** واحد قابل‌استفادهٔ مجدد رابط کاربری داخل یک Section (کارت، اسلایدر، آکاردئون، فرم، دکمه). یک Component می‌تواند در چند Section مختلف تکرار شود.

**Content (محتوا):** داده‌های واقعی/متنی/تصویری/عملکردی که داخل هر Component قرار می‌گیرد — چیزی که تیم کپی‌رایتینگ یا مشتری باید تأمین کند.

**قاعدهٔ AI برای تولید Brief:** هر خروجی طراحی باید این چهار سطح را جدا نگه دارد؛ ترکیب کردن Section و Component باعث ابهام در تخصیص کار می‌شود.

---

## بخش یک: ساختار استاندارد یک وب‌سایت مدرن (نقشهٔ سایت پایه)

```
Website
├── Homepage (/)
├── About (/about)
├── Services or Products (/services یا /shop)
│   └── Service/Product Detail Pages (/services/[slug])
├── Portfolio / Case Studies (/work)
│   └── Case Study Detail (/work/[slug])
├── Blog (/blog) [اختیاری بسته به نوع سایت]
│   └── Article Detail (/blog/[slug])
├── Pricing (/pricing) [عمدتاً SaaS/Membership]
├── FAQ (/faq) [یا به‌صورت Section در صفحات دیگر]
├── Contact (/contact)
└── صفحات پشتیبان: Privacy Policy, Terms, 404
```

این ۵ صفحه (Homepage، About، Service، Portfolio، Contact) در اکثر انواع سایت (Corporate، Portfolio Website، SaaS Marketing، Ecommerce برندی) مشترک‌اند و به همین دلیل کانون تمرکز این سند هستند.

---

## بخش دو: تجزیهٔ کامل صفحات

### 2.1 Homepage

**هدف صفحه:** در کمترین زمان ممکن به بازدیدکننده بگوید «این سایت چیست، برای چه کسی است، و چرا باید ادامه دهد».

| # | Section | هدف Section |
|---|---|---|
| 1 | Hero | جلب توجه فوری + بیان پیشنهاد ارزش |
| 2 | Trust Section | اثبات اعتبار در همان نگاه اول |
| 3 | Services | معرفی خدمات/محصولات اصلی |
| 4 | Features | برجسته‌کردن مزیت‌های رقابتی |
| 5 | Portfolio | نمایش نمونه‌کار/نتیجهٔ واقعی |
| 6 | Testimonials | اثبات اجتماعی از زبان مشتری |
| 7 | CTA | دعوت نهایی به اقدام |
| 8 | FAQ | رفع اعتراض/ابهام باقی‌مانده |
| 9 | Footer | ناوبری ثانویه + اطلاعات پایانی |

#### Section 1: Hero

| Component | نوع محتوای لازم |
|---|---|
| Headline (تیتر اصلی) | یک جملهٔ پیشنهاد ارزش (Value Proposition) — نه شعار مبهم، بلکه نتیجهٔ ملموس |
| Subheadline | یک یا دو جمله توضیح تکمیلی: برای چه کسی، چگونه |
| Primary CTA Button | متن اقدام (مثل «شروع کنید»، «مشاورهٔ رایگان») + لینک مقصد |
| Secondary CTA (اختیاری) | اقدام کم‌ریسک‌تر (مثل «مشاهدهٔ نمونه‌کارها») |
| Hero Visual | تصویر/ویدیو/انیمیشن/Illustration مرتبط با محصول یا نتیجه |
| Trust Micro-signal (اختیاری) | یک خط کوچک زیر CTA (مثل «بیش از ۵۰۰ مشتری راضی») |

#### Section 2: Trust Section

| Component | نوع محتوای لازم |
|---|---|
| Logo Strip | لوگوی مشتریان/شرکای شناخته‌شده |
| Stat Counters | اعداد کلیدی (سال‌های فعالیت، تعداد پروژه، رضایت مشتری) |
| Badge/Certification | نمادهای اعتماد (نماد اعتماد الکترونیک، گواهینامه‌ها) |

#### Section 3: Services

| Component | نوع محتوای لازم |
|---|---|
| Section Heading | تیتر معرفی خدمات (مثل «چه کاری برایتان انجام می‌دهیم») |
| Service Card (تکرارشونده) | آیکون/تصویر + عنوان خدمت + توضیح ۱-۲ خطی + لینک «بیشتر بدانید» |
| Grid/Layout Container | چیدمان کارت‌ها (معمولاً ۳ یا ۴ ستونه) |

#### Section 4: Features

| Component | نوع محتوای لازم |
|---|---|
| Feature Item (آیکون + متن) | آیکون بصری + عنوان ویژگی + توضیح کوتاه ارزش‌محور (نه صرفاً فنی) |
| Comparison Highlight (اختیاری) | ویژگی متمایزکننده نسبت به رقبا |
| Supporting Visual | اسکرین‌شات/موکاپ/دیاگرام که ویژگی را نشان می‌دهد |

#### Section 5: Portfolio (در Homepage به‌صورت خلاصه)

| Component | نوع محتوای لازم |
|---|---|
| Project Thumbnail Card | تصویر شاخص پروژه + عنوان + دسته‌بندی |
| Filter Tabs (اختیاری) | دسته‌بندی پروژه‌ها بر اساس نوع/صنعت |
| "View All" Link | لینک به صفحهٔ کامل Portfolio |

#### Section 6: Testimonials

| Component | نوع محتوای لازم |
|---|---|
| Testimonial Card | نقل‌قول مشتری + نام + سمت/شرکت + عکس (در صورت وجود) |
| Rating Indicator (اختیاری) | امتیاز ستاره‌ای |
| Carousel/Slider Control | دکمه‌های جابه‌جایی بین نظرات متعدد |

#### Section 7: CTA (Call To Action نهایی)

| Component | نوع محتوای لازم |
|---|---|
| Closing Headline | جملهٔ انگیزشی نهایی برای اقدام |
| CTA Button | متن اقدام واضح و مشخص |
| Risk Reducer (اختیاری) | متن کاهش‌دهندهٔ ریسک (مثل «بدون نیاز به کارت اعتباری») |

#### Section 8: FAQ

| Component | نوع محتوای لازم |
|---|---|
| Accordion Item | سؤال + پاسخ (۳ تا ۸ مورد معمول) |
| "سؤال دیگری دارید؟" Link | لینک به صفحهٔ تماس یا چت پشتیبانی |

#### Section 9: Footer

| Component | نوع محتوای لازم |
|---|---|
| Sitemap Columns | لینک‌های دسته‌بندی‌شده به صفحات اصلی |
| Contact Snippet | آدرس/ایمیل/تلفن خلاصه |
| Social Icons | لینک شبکه‌های اجتماعی |
| Newsletter Signup (اختیاری) | فیلد ایمیل + دکمهٔ عضویت |
| Legal Line | کپی‌رایت + لینک حریم خصوصی/قوانین |

---

### 2.2 About Page

**هدف صفحه:** ایجاد ارتباط انسانی و اعتماد از طریق روایت، ارزش‌ها و افراد پشت برند.

| # | Section | هدف Section |
|---|---|---|
| 1 | Story | روایت شکل‌گیری برند/کسب‌وکار |
| 2 | Mission | بیان چشم‌انداز و دلیل وجودی |
| 3 | Team | معرفی افراد کلیدی |
| 4 | Values | ارزش‌های بنیادین که رفتار برند را شکل می‌دهد |

#### Section: Story

| Component | نوع محتوای لازم |
|---|---|
| Narrative Text Block | متن روایی (چرا شروع شد، چه مشکلی حل می‌کند، مسیر رشد) |
| Timeline (اختیاری) | نقاط عطف زمانی به‌صورت بصری |
| Founder Quote (اختیاری) | نقل‌قول شخصی از بنیان‌گذار |

#### Section: Mission

| Component | نوع محتوای لازم |
|---|---|
| Mission Statement | یک جملهٔ مأموریت شفاف و به‌یادماندنی |
| Vision Statement (اختیاری) | جملهٔ چشم‌انداز بلندمدت |

#### Section: Team

| Component | نوع محتوای لازم |
|---|---|
| Team Member Card | عکس + نام + سمت + توضیح کوتاه/تخصص |
| Social Link (اختیاری) | لینک لینکدین/شبکهٔ حرفه‌ای هر عضو |

#### Section: Values

| Component | نوع محتوای لازم |
|---|---|
| Value Card | آیکون + عنوان ارزش (مثل «شفافیت») + توضیح یک‌خطی |
| Layout Grid | چیدمان ۳ تا ۶ کارت ارزش |

---

### 2.3 Service Page (صفحهٔ خدمت/محصول)

**هدف صفحه:** متقاعدسازی عمیق دربارهٔ یک خدمت خاص با جزئیات کافی برای تصمیم‌گیری خرید.

| # | Section | هدف Section |
|---|---|---|
| 1 | Overview | معرفی خدمت و مخاطب هدف آن |
| 2 | Benefits | نتایج و منافع ملموس برای مشتری |
| 3 | Process | نحوهٔ ارائهٔ خدمت گام‌به‌گام |
| 4 | Proof | اثبات کارایی (نمونه‌کار/آمار/نظرات مرتبط) |
| 5 | CTA | دعوت به اقدام مرتبط با همان خدمت |

#### Section: Overview

| Component | نوع محتوای لازم |
|---|---|
| Service Headline | عنوان خدمت + جملهٔ توضیح‌دهندهٔ ارزش |
| Target Audience Line | مشخص‌کردن اینکه این خدمت برای چه کسب‌وکار/فردی است |
| Overview Visual | تصویر/آیکون نمایندهٔ خدمت |

#### Section: Benefits

| Component | نوع محتوای لازم |
|---|---|
| Benefit Item | عنوان منفعت + توضیح کوتاه نتیجه‌محور (نه فقط ویژگی فنی) |
| Before/After Comparison (اختیاری) | مقایسهٔ وضعیت قبل و بعد از استفاده از خدمت |

#### Section: Process

| Component | نوع محتوای لازم |
|---|---|
| Step Item (شماره‌گذاری‌شده) | شمارهٔ گام + عنوان + توضیح کوتاه |
| Timeline/Stepper Visual | نمایش بصری توالی گام‌ها |
| Estimated Duration (اختیاری) | بازهٔ زمانی تقریبی هر مرحله یا کل فرآیند |

#### Section: Proof

| Component | نوع محتوای لازم |
|---|---|
| Mini Case Study Card | خلاصهٔ یک پروژهٔ مرتبط + نتیجهٔ کلیدی |
| Client Logo/Quote | نام یا نقل‌قول مشتری مرتبط با همین خدمت |
| Result Stat | عدد/درصد نتیجهٔ قابل‌اندازه‌گیری |

#### Section: CTA

| Component | نوع محتوای لازم |
|---|---|
| Service-specific CTA Text | متن اقدام مرتبط با همان خدمت (نه CTA عمومی سایت) |
| Contact/Booking Trigger | دکمه یا فرم اختصاصی درخواست همین خدمت |

---

### 2.4 Portfolio / Case Study Page

**هدف صفحه:** اثبات توانمندی از طریق روایت کامل یک پروژهٔ واقعی (نه فقط نمایش تصویر).

**صفحهٔ فهرست (Gallery) در مقابل صفحهٔ جزئیات (Project Detail):**

#### صفحهٔ فهرست — Section: Gallery

| Component | نوع محتوای لازم |
|---|---|
| Project Card | تصویر شاخص + عنوان پروژه + دسته‌بندی/صنعت |
| Filter/Category Tabs | فیلتر بر اساس نوع خدمت یا صنعت مشتری |
| Grid Layout | چیدمان کارت‌ها (Masonry یا Grid منظم) |

#### صفحهٔ جزئیات — Section: Project Detail

| Component | نوع محتوای لازم |
|---|---|
| Project Header | نام پروژه + نام مشتری + صنعت + سال انجام |
| Meta Info Block | خدمات ارائه‌شده، مدت پروژه، تیم درگیر |
| Visual Gallery | تصاویر/ویدیوی با کیفیت بالا از نتیجهٔ نهایی |

#### صفحهٔ جزئیات — Section: Challenge

| Component | نوع محتوای لازم |
|---|---|
| Problem Statement | توضیح مشکل/چالش اولیهٔ مشتری پیش از همکاری |
| Context Data (اختیاری) | آمار یا شرایط اولیه‌ای که وضعیت مشکل را نشان می‌دهد |

#### صفحهٔ جزئیات — Section: Solution

| Component | نوع محتوای لازم |
|---|---|
| Approach Description | توضیح رویکرد/استراتژی انتخاب‌شده |
| Process Highlights | نکات کلیدی اجرای پروژه (گام‌های مهم یا تصمیمات کلیدی) |
| Supporting Visual | اسکرین‌شات/دیاگرام از فرآیند اجرا |

#### صفحهٔ جزئیات — Section: Result

| Component | نوع محتوای لازم |
|---|---|
| Result Metric Card | عدد/درصد نتیجهٔ قابل‌اندازه‌گیری (رشد فروش، ترافیک، تبدیل) |
| Client Testimonial | نقل‌قول مستقیم مشتری دربارهٔ نتیجهٔ همکاری |
| Next Project CTA | لینک به پروژهٔ بعدی یا بازگشت به Gallery |

---

### 2.5 Contact Page

**هدف صفحه:** حذف هرگونه اصطکاک بین «تصمیم به تماس» و «انجام واقعی تماس».

| # | Section | هدف Section |
|---|---|---|
| 1 | Form | دریافت ساختاریافتهٔ درخواست |
| 2 | Location | نمایش موقعیت فیزیکی (در صورت وجود دفتر) |
| 3 | CTA | مسیر جایگزین/تکمیلی برای اقدام |
| 4 | Communication Channels | راه‌های ارتباطی مستقیم |

#### Section: Form

| Component | نوع محتوای لازم |
|---|---|
| Form Fields | نام، ایمیل/تلفن، موضوع، پیام (حداقل فیلد ممکن برای کاهش افت نرخ تکمیل) |
| Submit Button | متن دکمهٔ ارسال واضح (نه فقط «ارسال») |
| Confirmation State | پیام یا صفحهٔ تأیید پس از ارسال موفق |
| Privacy Note (اختیاری) | یک خط دربارهٔ نحوهٔ استفاده از اطلاعات |

#### Section: Location

| Component | نوع محتوای لازم |
|---|---|
| Embedded Map | نقشهٔ تعاملی (Google Maps یا مشابه) |
| Address Text | آدرس کامل قابل‌کپی |
| Working Hours | ساعات کاری/پاسخ‌گویی |

#### Section: CTA

| Component | نوع محتوای لازم |
|---|---|
| Alternative Action | مسیر جایگزین (مثل «رزرو مشاورهٔ آنلاین» به‌جای فرم) |
| Urgency/Response Time Note (اختیاری) | زمان تقریبی پاسخ‌گویی (مثل «پاسخ ظرف ۲۴ ساعت») |

#### Section: Communication Channels

| Component | نوع محتوای لازم |
|---|---|
| Channel Icon + Link | تلفن، ایمیل، واتساپ/تلگرام، شبکه‌های اجتماعی — هرکدام با آیکون و لینک مستقیم |
| Live Chat Widget (اختیاری) | ابزار گفتگوی آنلاین در صورت وجود پشتیبانی زنده |

---

## بخش سه: جدول مرجع فشرده (برای استخراج سریع توسط AI)

| Page | Sections (به‌ترتیب) |
|---|---|
| Homepage | Hero → Trust → Services → Features → Portfolio → Testimonials → CTA → FAQ → Footer |
| About | Story → Mission → Team → Values |
| Service | Overview → Benefits → Process → Proof → CTA |
| Portfolio/Case Study | Gallery (لیست) / Project Detail → Challenge → Solution → Result (جزئیات) |
| Contact | Form → Location → CTA → Communication Channels |

---

## بخش چهار: قواعد کاربردی برای AI Agent هنگام تولید Brief

1. **ترتیب Section ثابت نیست، منطق ثابت است:** ترتیب پیشنهادی بالا بر اساس منطق سفر کاربر (توجه → اعتماد → معرفی → اثبات → اقدام) است؛ AI می‌تواند بسته به دادهٔ کسب‌وکار (مثلاً نبود Testimonial واقعی) ترتیب یا حذف Section را تعدیل کند، اما نباید منطق را بشکند (مثلاً CTA نباید قبل از معرفی محصول بیاید).
2. **هر Component باید محتوای خودش را داشته باشد، نه محتوای Section:** هنگام تولید Content Requirement، درخواست باید در سطح Component باشد (مثلاً «۳ نقل‌قول مشتری با نام و سمت» نه «محتوای Testimonials»).
3. **Componentهای تکرارشونده باید حداقل/حداکثر تعداد داشته باشند:** مثل Service Card (۳ تا ۶ مورد)، FAQ Item (۳ تا ۸ مورد)، Team Member Card (بسته به اندازهٔ تیم واقعی).
4. **Section اختیاری باید صریحاً علامت‌گذاری شود:** مواردی مثل Newsletter Signup در Footer یا Before/After در Benefits باید در Brief به‌عنوان «اختیاری/شرطی به تصمیم کسب‌وکار» مشخص شوند تا در فاز تولید محتوا سردرگمی ایجاد نشود.
5. **هر صفحه دقیقاً یک Primary Goal دارد:** Homepage → معرفی و هدایت؛ Service → تبدیل به لید همان خدمت؛ Portfolio → اثبات؛ About → اعتمادسازی؛ Contact → حذف اصطکاک تماس. تمام Sectionهای هر صفحه باید در خدمت همان یک هدف باشند، نه اهداف موازی متعدد.
