<h2 align="center">
  دستورات <a href="https://git-scm.com/doc">گیت</a> به همراه توضیحات مختصر آنها در اینجا قرار خواهند گرفت
<h2>

<div align="center">
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/2100aca18de101af32ed35f314d8c462dfd8dd29/git-logo-gif.gif">
</div>

---

<div align="center">
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/ae35ec9426f4bb320eefac7d94961e33acc729ff/red-line.gif">
</div>

### `git` : 
<p align="right">مشاهده ی دستورات گیت</p>
<hr>
<br>

### `git init`:  
<p align="right">معرفی کردن پروژه به گیت یا اینیشیالایز کردن آن</p>
<hr>
<br>

<div align="center" >
  <img height="200" src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/3d81633e1a8ab8c354b2fa2a0d4e68e408f84c56/images/git-status.png">
</div>

### `git status`:   
<p align="right">برای فهمیدن موقعیت فعلی فایل های پروژه که مثلا در کدام مرحله هستند</p>
<p align="right">(working directory | staging area | head)</p>
<br>

### `git status --short` or `git status -s`: 
<p align="right">برای فهمیدن موقعیت فعلی فایل های پروژه به صورت <b>خلاصه شده</b> که مثلا در کدام مرحله هستند</p>
<hr>
<br>

### `git add <file name>` : 
<p align="right"><b>فایل</b> مورد نظر را به مرحله ی <b>استیجینگ</b> می برد</p>
<p align="right">staging area</p>
<br>

### `git add .` : 
<p align="right"><b>تمامی</b> فایل ها و تغییرات پروژه را به مرحله ی استیجینگ می برد</p>
<hr>
<br>

### `git rm --cached <file name>` : 
<p align="right"><b>فایلی</b> که به مرحله ی استیجینگ اضافه شده را به مرحله ی <b>ورکینگ دایرکتوری</b> بر می گرداند </p>
<p align="right">(From staging area to working directory)</p>
<hr>
<br>

### `git commit -m <message>` :
<p align="right">فایل های پروژه که در مرحله ی استیجینگ قرار دارند را به یک پیغام مرتبط به مرحله ی نهایی یا هد، مخزن یا ریپوزیتوری می برد</p>
<p align="right">(From staging area to HEAD or repositories)</p>
<br>

### `git commit -am <message>` or `git commit -a -m <message>` :
<p align="right">فایل هایی که <b>از قبل</b> در پروژه ساخته شده اند و<b> تغییر پیدا می کنند</b> را مستقیماً به مرحله ی ریپوزیتوری یا هد می برد؛ اما اگر فایلی تازه ایجاد شده باشد ابتدا باید به استیج اضافه شود و سپس با کامیت مناسب به ریپوزیتوری اضافه شود</p>
<p align="left"> new file --> git add "file name" --> git commit -m "message" </p>
<p align="left"> modified file --> git commit -am "message" --> git commit -a -m "message" </p>
<hr>
<br>

### `git log` : 
<p align="right">تغییرات و کامیت های پروژه را بر می گرداند که در خروجی می توان نام و ایمیل نویسنده، تاریخ و ساعت درج کامیت را مشاهده کرد</p>
<br>
<br>

### `git log --oneline` :
<p align="right">تغییرات و کامیت های پروژه را به صورت <b>خلاصه شده و کوتاه</b>  بر می گرداند</p>
<br>

### `git log --oneline --all` :
<p align="right">برای مشاهده ی تمامی کامیت ها استفاده می شود</p>
<br>

### `git log --stat` : 
<p align="right">تغییرات پروژه را به صورت خیلی کاملتری نمایش می دهد؛ به طوری که می توان نام و ایمیل نویسنده، تاریخ و ساعت درج کامیت و همچنین تعداد فایل های تغییر یافته و تعداد خط کدهایی که به فایل تغییر یافته اضافه یا کم شده اند را نمایش می دهد</p>
<br>

### `git log --graph` :
<p align="right">اطلاعات کامیت ها را به صورت گرافیکی نمایش می دهد</p>
<br>

### `git log --graph --oneline` :
<p align="right">اطلاعات کامیت ها را به صورت گرافیکی ولی جزئی تر و خلاصه تر برمیگرداند</p>
<br>

### `git log --after="25-10-12"` :
<p align="right">کامیت های <b>بعد</b> از یک تاریخ مشخص را بر میگرداند</p>
<br>

### `git log --before="25-10-12"` :
<p align="right">کامیت های <b>قبل</b> از یک تاریخ مشخص را بر میگرداند</p>
<br>

### `git log --author="User Name"` :
<p align="right">کامیت های نویسنده یا یوزر مورد نظر به همراه تاریخ و ساعت درج آنها را بر می گرداند</p>
<br>
<hr>

<div align="center">
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/facb8d8134ca9be4c997d5ab0497281c742df536/images/stack-data-structure.png">
</div>

<!-- <p align="right"></p> -->
