<div dir='rtl'>

# تقسیمات کشوری ایران
[مرکز آمار ایران](https://www.amar.org.ir/) فایل‌هایی شامل اطلاعات تقسیمات کشوری را در وب سایت خود منتشر می‌کند. آخرین فایل منتشر شده مربوط به سال ۱۳۹۷ است که در قالب اکسل 
از [این آدرس](https://www.amar.org.ir/Portals/0/Geo/GEO97.xlsx) قابل دریافت است.

این مخزن، تمام اطلاعات فایل اکسل تقسیمات کشوری از جمله آبادی‌ها را شامل می‌شود. از آنجایی که اطلاعات فایل اکسل مرکز آمار، نرمال نیست در این مخزن در حال حاضر در دو قالب `json` و `sql` اطلاعات به صورت نرمال شده با `relation` درج شده است.

:warning: اطلاعات فایل اکسل مرکز آمار، از نظر حروف فارسی صحیح نیست و در این مخزن، یکسان‌سازی و تبدیل کاراکترها به کاراکترهای استاندارد فارسی هم انجام شده است.

### تعاریف

- **استان** : واحدی از تقسیمات كشوری است با محدوده جفرافیایی معین، كه از به هم پیوستن چند شهرستان همجوار با توجه به موقعیت سیاسی، اجتماعی، فرهنگی، اقتصادی و طبیعی تشكیل می‌شود


- **شهرستان**: واحدی از تقسیمات كشوری است با محدوده جغرافیایی معین كه ار بهم پیوستن چند بخش همجوار كه از نظر عوامل طبیعی، اجتماعی، اقتصادی، سیاسی و فرهنگی واحد متناسب و همگنی را به وجود آورده‌اند.

- **بخش**: واحدی است از تقسیمات كشوری كه دارای محدوه جغرافیایی معین بوده و از به هم پیوستن چند دهستان همجوار مشتمل بر چندین مزرعه، مكان، روستا و احیاناً شهر كه در آن عوامل طبیعی و اوضاع اجتماعی، فرهنگی، اقتصادی و سیاسی واحد همگنی را به وجود می‌آورد به نحوی كه با در نظر گرفتن تناسب، وسعت، جمعیت، ارتباطات و دسترسی و سایر موقعیت‌ها، نیل به اهداف و برنامه‌ریزی‌های دولت در جهت احیاء امكانات طبیعی و استعدادهای اجتماعی و توسعه امور رفاهی و اقتصادی آن تسهیل گردد.

- **ذعسالت**: كوچك‌ترین واحد تقسیمات كشوری است كه دارای محدوده جغرافیایی معین بوده و از به هم پیوستن چند روستا، مكان، مزرعه همجوار تشكیل می‌شود كه از لحاظ محیط طبیعی، فرهنگی، اقتصادی و اجتماعی همگن بوده و امكان خدمات رسانی و برنامه‌ریزی در سیستم و شبكه واحدی را فراهم می‌نماید.

- **شهر**: شهر محلی است با حدود قانونی كه در محدوده جغرافیایی بخش واقع شده و از نظر بافت ساختمانی، اشتغال و سایر عوامل، دارای سیمائی با ویژگی‌های خاص خود بوده به طوری كه اكثریت ساكنان دائمی آن در مشاغل كسب، تجارت، صنعت، كشاورزی، خدمات و فعالیت‌های اداری اشتغال داشته و در زمینه خدمات شهری از خودكفایی نسبی برخوردار و كانون مبالات اجتماعی، اقتصادی، فرهنگی و سیاسی حوزه جذب و نفوذ پیرامون خود بوده و حداقل دارای ده هزار نفر جمعیت باشد.


### فرمت داده‌ها

هر ردیف از داده‌ها شامل ستون‌های زیر می‌باشد:

- `id`: شناسه ردیف 
- `parentCountryDivisionId`: شناسه پدر بر اساس تعاریف. به عنوان مثال، پدر یک ردیف از نوع «شهرستان»، ردیفی از نوع «استان» می‌باشد.
- `name`: نام محل
- `code`: کد محل بر اساس کدگذاری فایل اکسل مرکز آمار ایران
- `divisionType`: نوع ردیف شامل یکی از موارد زیر:
  - `0`: کشور
  - `1`: استان
  - `2`: شهرستان
  - `3`: بخش
  - `4`: دهستان
  - `5`: شهر
  - `6`: آبادی

</div>