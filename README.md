<div dir="rtl">

# 🔎 Arabic OSINT Awesome

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Check Links](https://github.com/YOUR_USERNAME/arabic-osint-awesome/actions/workflows/links.yml/badge.svg)](https://github.com/YOUR_USERNAME/arabic-osint-awesome/actions/workflows/links.yml)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![License: CC0](https://img.shields.io/badge/License-CC0-lightgrey.svg)](LICENSE)

> قائمة منتقاة لأدوات ومصادر **الاستخبارات مفتوحة المصدر (OSINT)** بشرح عربي لكل أداة: بتعمل إيه، إمتى تستخدمها، وإيه حدودها.
> مش مجرد روابط متكدّسة. كل أداة معاها سطر أو اتنين عن قيمتها الفعلية.

**الرموز:** 🆓 مجاني · 💰 مدفوع · 🔑 مجاني بحساب · 🧰 مفتوح المصدر / سطر أوامر

## المحتويات

1. [محركات البحث و Dorking](#search)
2. [البحث عن اليوزرنيم والإيميل](#username-email)
3. [الدومين والـ IP والبنية التحتية](#infra)
4. [السوشيال ميديا (بيانات عامة فقط)](#social)
5. [تحليل الصور والتحديد الجغرافي](#image-geo)
6. [الخرائط وصور الأقمار الصناعية](#maps)
7. [فحص التسريبات والاختراقات](#leaks)
8. [مصادر عربية وخاصة بالمنطقة (MENA)](#mena)
9. [التعلم: كورسات، CTF، كتب، قنوات](#learning)
10. [الأخلاقيات والقانون](#ethics)
11. [المساهمة](#contributing)

---

<a id="search"></a>
## 1. محركات البحث و Dorking

- [Google Advanced Search](https://www.google.com/advanced_search) 🆓 - واجهة جاهزة لفلاتر الموقع والنوع والتاريخ واللغة. مناسبة للبداية، لكن كتابة الـ operators يدويًا أسرع وأدق.
- [Google Hacking Database](https://www.exploit-db.com/google-hacking-database) 🆓 - أرشيف ضخم لـ dorks جاهزة. مفيد كإلهام، لكن أغلبه موجّه للأمن مش للتحقيق العام.
- [DorkSearch](https://dorksearch.com) 🆓💰 - بيبني استعلامات dorks بواجهة بسيطة. النسخة المجانية محدودة.
- [Yandex](https://yandex.com) 🆓 - فهرس مختلف عن جوجل، وممتاز في البحث بالصور والمحتوى الروسي وشرق أوروبا.
- [Bing](https://www.bing.com) 🆓 - فهرس مستقل أحيانًا بيطلّع نتائج مش موجودة في جوجل. الـ operators فيه أقل.
- [Brave Search](https://search.brave.com) 🆓 - فهرس مستقل وخصوصية أعلى. مفيد كمصدر تاني للمقارنة.
- [DuckDuckGo](https://duckduckgo.com) 🆓 - مناسب للخصوصية وبحث الـ bangs. العمق أقل من جوجل.
- [Wayback Machine](https://web.archive.org) 🆓 - بيعرض نسخ قديمة من المواقع. مش كل الصفحات مؤرشفة، وممكن صاحب الموقع يمنع الأرشفة.
- [archive.today](https://archive.ph) 🆓 - بيحفظ لقطة فورية للصفحة قبل ما تتحذف، وبيتحفظ بيها دليل. الوصول له ممكن يتحجب في بعض الشبكات.
- [Google Alerts](https://www.google.com/alerts) 🆓 - تنبيهات إيميل لأي ذكر جديد لاسم أو كلمة. بسيط ومفيد للمتابعة المستمرة.

<a id="username-email"></a>
## 2. البحث عن اليوزرنيم والإيميل

- [Sherlock](https://github.com/sherlock-project/sherlock) 🧰 - بيدوّر على يوزرنيم في مئات المواقع. فيه نتائج كاذبة (false positives) فراجع كل نتيجة يدويًا.
- [Maigret](https://github.com/soxoj/maigret) 🧰 - زي Sherlock لكن بيجمع معلومات من الحسابات اللي يلاقيها ويعمل تقرير. أبطأ لكن أغنى.
- [WhatsMyName](https://whatsmyname.app) 🆓 - نسخة ويب من قاعدة بيانات مجتمعية لمواقع اليوزرنيم. مفيدة لو مش عايز تنصّب حاجة.
- [Namechk](https://namechk.com) 🆓 - بيتأكد إن كان اسم معين محجوز على المنصات. أسرع للفحص الأولي.
- [Holehe](https://github.com/megadose/holehe) 🧰 - بيفحص إذا كان إيميل مسجّل على مواقع معروفة. الموقع ممكن يغيّر السلوك فتبطل الأداة تشتغل مع بعضها.
- [Epieos](https://epieos.com) 🆓💰 - بيربط إيميل أو رقم بحسابات عامة (زي حساب جوجل). مفيد لكن النتائج بتعتمد على إعدادات خصوصية صاحب الحساب.
- [Hunter](https://hunter.io) 🔑💰 - بيطلّع صيغة إيميلات شركة وإيميلات منشورة. النسخة المجانية بعدد بحث محدود.

<a id="infra"></a>
## 3. الدومين والـ IP والبنية التحتية

- [ICANN Lookup](https://lookup.icann.org) 🆓 - WHOIS رسمي. أغلب البيانات الشخصية دلوقتي مخفية بسبب الخصوصية.
- [crt.sh](https://crt.sh) 🆓 - بيبحث في شهادات SSL المنشورة، وبيكشف subdomains ما كنتش تعرفها. من أفضل المصادر المجانية.
- [DNSDumpster](https://dnsdumpster.com) 🆓 - خريطة DNS سريعة للدومين. النتائج محدودة مقارنة بالأدوات المدفوعة.
- [SecurityTrails](https://securitytrails.com) 🔑💰 - تاريخ DNS وWHOIS. الخطة المجانية محدودة.
- [ViewDNS.info](https://viewdns.info) 🆓 - مجموعة أدوات DNS وreverse IP في مكان واحد. الواجهة قديمة لكنها عملية.
- [Shodan](https://www.shodan.io) 🔑💰 - محرك بحث للأجهزة المتصلة بالإنترنت. استخدمه للاستكشاف فقط، ومتتصلش بأجهزة مش بتاعتك.
- [Censys](https://search.censys.io) 🔑💰 - بديل Shodan بتركيز على الشهادات والخدمات. الحد المجاني قليل.
- [urlscan.io](https://urlscan.io) 🆓🔑 - بيفحص صفحة ويطلّع لقطة شاشة وكل الطلبات اللي عملتها. ممتاز للروابط المشبوهة.
- [VirusTotal](https://www.virustotal.com) 🆓🔑 - بيفحص ملفات وروابط بمحركات متعددة، وبيربط الدومينات والـ IPs. أي حاجة ترفعها بتبقى متاحة للباحثين، فمترفعش ملفات حساسة.
- [BuiltWith](https://builtwith.com) 🆓💰 - بيعرف التقنيات اللي موقع بيستخدمها. التفاصيل الكاملة مدفوعة.
- [Wappalyzer](https://www.wappalyzer.com) 🆓💰 - إضافة متصفح لكشف تقنيات الموقع. أسرع للفحص اليومي.
- [BGPView](https://bgpview.io) 🆓 - بيعرف ASN ونطاقات الـ IP لأي منظمة. مفيد لمعرفة مين مالك الشبكة.
- [Hurricane Electric BGP Toolkit](https://bgp.he.net) 🆓 - بيانات BGP وASN ونطاقات تفصيلية. مناسب للتعمق في بنية شبكة.
- [IPinfo](https://ipinfo.io) 🆓💰 - موقع تقريبي ومزوّد خدمة للـ IP. الموقع الجغرافي تقريبي مش دقيق.
- [Subfinder](https://github.com/projectdiscovery/subfinder) 🧰 - أداة لاكتشاف subdomains بشكل سلبي (passive). أحسن مع مفاتيح API لمصادر إضافية.
- [Amass](https://github.com/owasp-amass/amass) 🧰 - رسم خريطة شاملة للنطاقات. أثقل وأبطأ لكن أشمل.
- [theHarvester](https://github.com/laramies/theHarvester) 🧰 - بيجمع إيميلات ودومينات من مصادر عامة. أغلب المصادر محتاجة مفاتيح API.
- [SpiderFoot](https://github.com/smicallef/spiderfoot) 🧰 - أتمتة جمع المعلومات من مصادر كتير بواجهة ويب. بيدي كمية بيانات كبيرة، فاحتاج تفرزها.

<a id="social"></a>
## 4. السوشيال ميديا (بيانات عامة فقط)

- [X Advanced Search](https://x.com/search-advanced) 🔑 - بحث متقدم بالتاريخ واللغة والحساب. مهم جدًا في العربي: استخدم فلتر اللغة `lang:ar`.
- [Social Searcher](https://www.social-searcher.com) 🆓💰 - بحث في المنشورات العامة على منصات متعددة. التغطية محدودة والنسخة المجانية قليلة.
- [TGStat](https://tgstat.com) 🆓💰 - إحصائيات وبحث في قنوات تيليجرام العامة. مفيد لقنوات المنطقة، لكن التغطية غير كاملة.
- [Telepathy](https://github.com/jordanwildon/Telepathy) 🧰 - أرشفة وتحليل قنوات ومجموعات تيليجرام العامة. محتاج حساب API من تيليجرام.
- [Instaloader](https://github.com/instaloader/instaloader) 🧰 - تنزيل بيانات حسابات إنستجرام العامة. إنستجرام بيحجب الاستخدام الكثيف.
- [InVID-WeVerify](https://www.invid-project.eu/tools-and-services/invid-verification-plugin/) 🆓 - إضافة متصفح للتحقق من الفيديوهات: لقطات مفتاحية وبحث عكسي. أساسية لأي تحقق من فيديو منتشر.
- [YouTube DataViewer](https://citizenevidence.amnestyusa.org) 🆓 - بيطلّع وقت الرفع الدقيق وصور مصغرة لفيديو يوتيوب، وبيساعد في البحث العكسي.

<a id="image-geo"></a>
## 5. تحليل الصور والتحديد الجغرافي

- [Google Lens](https://lens.google.com) 🆓 - بحث عكسي ممتاز في الأماكن والأشياء والنصوص داخل الصور.
- [TinEye](https://tineye.com) 🆓💰 - بيدوّر على أقدم ظهور للصورة. ممتاز لتتبّع الأصل.
- [Yandex Images](https://yandex.com/images) 🆓 - أفضل بحث عكسي في أماكن كتير، وأحيانًا بيتعرف على المباني والشوارع.
- [ExifTool](https://exiftool.org) 🧰 - بيقرا بيانات EXIF بالكامل. أغلب المنصات بتمسح EXIF عند الرفع، فمتتوقعش دايمًا تلاقي حاجة.
- [FotoForensics](https://fotoforensics.com) 🆓 - تحليل ELA لكشف التعديل. النتائج تحتاج خبرة ومش دليل قاطع لوحدها.
- [Forensically](https://29a.ch/photo-forensics) 🆓 - مجموعة أدوات تحليل صور في المتصفح: clone detection وغيرها.
- [SunCalc](https://www.suncalc.org) 🆓 - بيحسب اتجاه الشمس وطول الظل. أداة أساسية لتحديد الوقت والمكان من الظلال.
- [GeoGuessr](https://www.geoguessr.com) 🆓💰 - لعبة ممتازة لتدريب عينك على علامات الدول: الطرق، اللوحات، النباتات.
- [Overpass Turbo](https://overpass-turbo.eu) 🆓 - استعلامات على بيانات OpenStreetMap (مثلًا: كل محطة وقود جنب مسجد). قوية لكن محتاجة تتعلم الصيغة.
- [Mapillary](https://www.mapillary.com) 🆓 - صور شوارع مجتمعية، بتغطي أماكن مش موجودة في Street View.
- [PeakFinder](https://www.peakfinder.com) 🆓💰 - بيتعرف على الجبال من الأفق. مفيد لصور الطبيعة.
- [Wikimapia](https://wikimapia.org) 🆓 - خريطة مجتمعية بتوسيم المباني والمنشآت. الدقة بتختلف حسب المنطقة.

<a id="maps"></a>
## 6. الخرائط وصور الأقمار الصناعية

- [Google Earth](https://earth.google.com) 🆓 - صور تاريخية وعرض ثلاثي الأبعاد. شريط الزمن بيساعد في مقارنة التغيرات.
- [OpenStreetMap](https://www.openstreetmap.org) 🆓 - خريطة مفتوحة بتفاصيل أحيانًا أحسن من جوجل. التغطية بتعتمد على المتطوعين.
- [Copernicus Browser](https://browser.dataspace.copernicus.eu) 🆓🔑 - صور Sentinel المجانية. الدقة 10 متر تقريبًا، فمش مناسبة للتفاصيل الصغيرة.
- [Sentinel Hub EO Browser](https://apps.sentinel-hub.com/eo-browser/) 🆓🔑 - تصفح ومقارنة صور الأقمار الصناعية بتواريخ مختلفة وطبقات تحليل.
- [NASA FIRMS](https://firms.modaps.eosdis.nasa.gov/map/) 🆓 - خريطة الحرائق النشطة شبه لحظية. مفيدة للتحقق من حرائق وأحداث كبيرة.
- [Zoom Earth](https://zoom.earth) 🆓 - صور أقمار صناعية شبه حية وتتبّع الأعاصير. الدقة منخفضة.
- [FlightRadar24](https://www.flightradar24.com) 🆓💰 - تتبّع الطيران. السجل التاريخي الطويل مدفوع.
- [ADS-B Exchange](https://globe.adsbexchange.com) 🆓 - تتبّع طيران بدون حجب، بما فيها بعض الطائرات اللي مش بتظهر في مواقع تانية.
- [MarineTraffic](https://www.marinetraffic.com) 🆓💰 - تتبّع السفن. التغطية ضعيفة لو السفينة قفلت الـ AIS.
- [VesselFinder](https://www.vesselfinder.com) 🆓💰 - بديل لـ MarineTraffic لتتبّع السفن. فيه تفاصيل أساسية مجانية.

<a id="leaks"></a>
## 7. فحص التسريبات والاختراقات

> للاطمئنان على حساباتك وللتحقيق المشروع. متستخدمش بيانات مسرّبة للأذى أو الابتزاز أو الدخول لحسابات حد.

- [Have I Been Pwned](https://haveibeenpwned.com) 🆓 - بيقولك إيميلك ظهر في أي تسريب معروف. أشهر أداة وبتحترم الخصوصية.
- [Intelligence X](https://intelx.io) 🔑💰 - محرك بحث في بيانات التسريبات والـ darknet والأرشيفات. الوصول الكامل مدفوع.
- [DeHashed](https://dehashed.com) 💰 - فهرس لبيانات مسرّبة. مدفوع. افحص الوضع القانوني في بلدك قبل الاستخدام.
- [TruffleHog](https://github.com/trufflesecurity/trufflehog) 🧰 - بيدوّر على أسرار (مفاتيح API وكلمات سر) متسرّبة في الكود. مفيد لفحص ريبوهاتك.
- [GitHub Search](https://github.com/search) 🆓 - البحث في الكود العام بيكشف مفاتيح ومعلومات داخلية بالغلط. استخدم الـ qualifiers زي `org:` و`filename:`.

<a id="mena"></a>
## 8. مصادر عربية وخاصة بالمنطقة (MENA)

### سجلات ومصادر مفتوحة

- [OpenCorporates](https://opencorporates.com) 🆓💰 - أكبر قاعدة بيانات مفتوحة للشركات. تغطية دول المنطقة متفاوتة، فاعتبرها نقطة بداية مش مصدر نهائي.
- [ICIJ Offshore Leaks Database](https://offshoreleaks.icij.org) 🆓 - بيانات Panama وPandora Papers وغيرها. فيها أسماء وشركات من المنطقة، لكن الظهور فيها مش دليل على مخالفة بالضرورة.
- [OCCRP Aleph](https://aleph.occrp.org) 🔑 - منصة وثائق وسجلات للصحفيين الاستقصائيين. مفيدة جدًا لو بتحقق في شبكات شركات.
- [Humanitarian Data Exchange](https://data.humdata.org) 🆓 - بيانات إنسانية وحدود إدارية ومؤشرات لدول المنطقة. مفيدة للسياق الجغرافي والسكاني.
- [World Bank Open Data](https://data.worldbank.org) 🆓 - مؤشرات اقتصادية واجتماعية لكل دولة. للسياق العام.
- [Wathq (السعودية)](https://wathq.sa) 🆓💰 - خدمات التحقق من بيانات السجل التجاري السعودي. بعض الخدمات للجهات المسجّلة فقط.
- [SaudiNIC](https://nic.sa) 🆓 - سجل نطاقات `.sa`. مفيد للتحقق من مالك نطاق سعودي.

> 🛠️ **محتاجين مساهمات:** سجلات تجارية، بوابات نشر رسمية (الجريدة الرسمية)، وسجلات دومينات لباقي الدول (`.eg` `.ae` `.iq` `.ma` `.dz` `.tn` `.jo` `.lb` وغيرها). لو تعرف مصدر موثوق، افتح PR.

### مصادر تحقق وأرشفة وتوثيق

- [Misbar (مسبار)](https://misbar.com) 🆓 - منصة عربية لتدقيق المعلومات. تفيد لمعرفة هل الادعاء اتفحص قبل كده.
- [Fatabyyano (فتبينوا)](https://fatabyyano.net) 🆓 - تدقيق معلومات عربي. استخدمها قبل ما تبدأ تحقق من الصفر.
- [Matsda2sh (متصدقش)](https://matsda2sh.com) 🆓 - تدقيق معلومات بتركيز على المحتوى المصري.
- [Akhbarmeter (أخبارميتر)](https://akhbarmeter.org) 🆓 - تدقيق معلومات في الأردن ودول الجوار.
- [Verify-Sy](https://verify-sy.com) 🆓 - تدقيق معلومات متخصص في الشأن السوري.
- [Syrian Archive](https://syrianarchive.org) 🆓 - أرشيف موثّق لمحتوى مفتوح المصدر عن الصراع في سوريا. نموذج ممتاز لمنهجية الأرشفة والتوثيق.
- [ACLED](https://acleddata.com) 🆓🔑 - بيانات أحداث نزاع وعنف سياسي مصنفة جغرافيًا وزمنيًا. أساسية لأي تحليل أمني إقليمي.
- [Airwars](https://airwars.org) 🆓 - توثيق ضحايا الغارات الجوية. فيها منهجية مفتوحة قابلة للتعلم.
- [Liveuamap](https://liveuamap.com) 🆓💰 - خريطة أحداث لحظية. المصادر متنوعة فتحتاج التحقق من كل حدث بنفسك.
- [SMEX](https://smex.org) 🆓 - تقارير عن الحقوق الرقمية في المنطقة العربية. مفيدة لفهم سياق الرقابة والحجب.
- [ARIJ](https://arij.net) 🆓 - شبكة صحفيين استقصائيين عرب. فيها أدلة ومواد تدريبية.

### نصائح البحث بالعربي

هنا الميزة اللي أغلب القوايم الإنجليزي مفيهاش:

1. **اكتب كل صيغ الاسم.** `محمد` و`محمّد` و`مُحَمَّد`. وكمان `أحمد` و`احمد` و`إحمد`. الألف المهموزة والتاء المربوطة (`ة`/`ه`) والياء (`ى`/`ي`) بتغيّر النتائج.
2. **جرّب كل تهجئات الاسم باللاتيني.** `Mohamed` `Mohammed` `Muhammad` `Mohamad`. وكمان `Abdelrahman` `Abdul Rahman` `Abd al-Rahman`.
3. **الأرقام والـ Arabizi.** الناس بتكتب `7abibi` `3amr` `5aled` `9alah`. الأرقام بتمثل حروف: 2=ء 3=ع 5=خ 7=ح 9=ص. دوّر بالشكلين.
4. **قيّد النتائج بالدولة.** مثال: `site:.eg` `site:.sa` `site:.ae` `site:.iq`. بيضيّق البحث على المواقع المحلية.
5. **استخدم فلتر اللغة.** في X: `lang:ar`. في جوجل: الإعدادات المتقدمة أو `&lr=lang_ar`.
6. **اللهجات بتغيّر الكلمات.** نفس الحدث بيتوصف بكلمات مختلفة في مصر والخليج والشام والمغرب. جرّب مرادفات من أكتر من لهجة.
7. **جرّب مع التشكيل وبدونه.** وكمان ابحث بعبارة كاملة بين علامتي تنصيص `" "` لو الكلمات مجاورة.
8. **أسماء الأماكن ليها أكتر من صيغة.** `القاهرة` / `Cairo` / `Al-Qahira`، و`الدار البيضاء` / `Casablanca` / `Casa`. تحقّق من الأسماء القديمة كمان.
9. **تيليجرام هو المصدر العربي الأكبر.** كتير من الأخبار بتظهر فيه الأول. ابحث بـ TGStat وبمحركات خارجية، واحتفظ بلقطات وأرشيف لأن القنوات بتتحذف.
10. **خد لقطات واحفظ روابط أرشيف.** المحتوى العربي المتداول في الأحداث بيتحذف بسرعة.

<a id="learning"></a>
## 9. التعلم: كورسات، CTF، كتب، قنوات

- [OSINT Framework](https://osintframework.com) 🆓 - شجرة تصنيفية ضخمة للأدوات. ممتازة للاستكشاف، لكن مش بتشرح الأدوات ولا بتتحقق من الروابط.
- [Bellingcat Online Investigations Toolkit](https://bellingcat.gitbook.io/toolkit) 🆓 - قايمة أدوات منتقاة بشروح من فريق Bellingcat. مرجع أساسي.
- [Trace Labs](https://www.tracelabs.org) 🆓 - مسابقات CTF للبحث عن أشخاص مفقودين بالتعاون مع الجهات المختصة. تطبيق عملي ذو أثر حقيقي.
- [Gralhix](https://gralhix.com) 🆓 - تحديات OSINT وتحديد جغرافي بحلول مفصّلة. ممتازة للتدريب.
- [Sector035 - Week in OSINT](https://sector035.nl) 🆓 - نشرة أسبوعية بأحدث الأدوات والتقنيات. بالإنجليزي.
- [OSINT Curious](https://osintcurio.us) 🆓 - مقالات وبودكاست وفيديوهات عن المنهجية والأدوات.
- [IntelTechniques](https://inteltechniques.com) 🆓💰 - أدوات ومواد Michael Bazzell، ومؤلف كتاب Open Source Intelligence Techniques. الكتاب مدفوع.
- [TryHackMe](https://tryhackme.com) 🔑💰 - غرف تدريب عملية في OSINT ضمن مسارات الأمن. مناسب للمبتدئين.

> 🛠️ **محتاجين مساهمات:** قنوات يوتيوب وتيليجرام ومجتمعات عربية نشطة في OSINT. اقترح اللي جربته فعلًا.

<a id="ethics"></a>
## 10. الأخلاقيات والقانون

OSINT معناه جمع معلومات **متاحة للعامة**، لكن "متاحة" مش معناها "مسموح بأي استخدام".

- **اعرف قانون بلدك.** قوانين الجرائم الإلكترونية والخصوصية بتختلف، وبعضها صارم في المنطقة.
- **بيانات عامة فقط.** متدخلش حسابات، ومتتخطاش حماية، ومتنتحلش هوية لخداع حد.
- **متسرّبش بيانات الناس.** جمع معلومات شخص عادي وتجميعها (doxxing) ممكن يسبب ضرر حقيقي.
- **التسريبات:** فحص حساباتك أو التحقيق المشروع مختلف تمامًا عن استخدام بيانات مسروقة ضد أفراد.
- **وثّق منهجيتك واحفظ مصادرك،** وفرّق بين الحقيقة المؤكدة والاستنتاج.
- **قيّم الضرر المحتمل** قبل نشر أي نتيجة، خصوصًا لو فيها ناس في خطر.

الأدوات هنا للتعلم والتحقق والصحافة والبحث الأمني المشروع. المسؤولية على اللي بيستخدمها.

<a id="contributing"></a>
## 11. المساهمة

عايزين مساهمات، خصوصًا في **قسم MENA**. اقرأ [CONTRIBUTING.md](CONTRIBUTING.md) الأول. باختصار: أداة جرّبتها بنفسك، وصف في سطر أو اتنين، ذكر إنها مجانية ولا مدفوعة، وملاحظة عن القيود.

## الرخصة

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](LICENSE)

</div>
