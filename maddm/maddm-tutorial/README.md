# Running MadDM “out of the box”

وارد شدن به محیط MadDM
```
./bin/maddm.py
```
شروع آموزش MadDM
```
tutorial
```
وارد کردن مدل ماده تاریک ساده‌شده (DMsimp)
```
import model DMsimp_s_spin0_MD
```
 تعریف ذره ماده تاریک
 ```
define darkmatter ~xd
```
تولید فرایند محاسبه‌ی چگالی مانده (relic density)
```
generate relic_density
```
خروجی گرفتن پروژه
```
output my_dm_project
```
اجرای پروژه و مشاهده‌ی نتایج
```
launch my_dm_project
```

ویرایش پارامترها در فایل param_card.dat با زدن شماره 7 سپس خروج از ویرایشگر ظاهر شده با دستورات زیر :
 اگر تغییرات دادی و می‌خوای ذخیره کنی: Esc سپس ‍‍```wq:``` و Enter
  اگر اشتباهی کردی و می‌خوای بدون ذخیره خارج شی:  Esc سپس ‍‍```!q:``` و Enter
  فقط ذخیره بدون خروج : ‍‍```w:```
  فقط خروج : ‍‍‍``` q:```
  قبل از زدن این دستورها باید با Esc از حالت ویرایش (insert mode) خارج بشی.

   لیستی از فرآیندهایی که در مدل محاسبه شده‌اند را مشاهده کنید:
 ```
MadDM> display processes
```
 دیاگرام‌های فاینمن مربوط به فرآیندهای محاسبه شده را مشاهده کنید:
```
MadDM> display diagrams
```

برای مشاهده لیست مدل‌ها، می‌توانید از دستور زیر در MadDM استفاده کنید:
```
MadDM> display modellist
```
برای وارد کردن مدل دلخواه به MadDM، کافی است از دستور زیر استفاده کنید:
```
MadDM> import model <model_name>
```

 ذراتی که با ماده تاریک کوآنیهیلات می‌شوند را مشخص می‌کند:
```
define coannihilator <particle_names>
```





























 
