<h2 align="center">
  دستورات <a href="https://git-scm.com/doc">گیت</a> به همراه توضیحات مختصر آنها در اینجا قرار خواهند گرفت
<h2>

<div align="center">
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/2100aca18de101af32ed35f314d8c462dfd8dd29/git-logo-gif.gif">
</div>

<br>

<div align="center">
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/ae35ec9426f4bb320eefac7d94961e33acc729ff/red-line.gif">
</div>

### `git` : 
<p align="right">مشاهده ی دستورات گیت</p>
<br>
<hr>

<!-- ---------------------------------------------------------------------------------------------------------- -->

### `git init`:  
<p align="right">معرفی کردن پروژه به گیت یا اینیشیالایز کردن آن</p>
<br>
<hr>

<!-- ---------------------------------------------------------------------------------------------------------- -->

<div align="center" >
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/09b16830daf385e596a8dbb4cb741334f3a3ec06/images/GIT%20STATUS.png">
</div>

### `git status`:   
<p align="right">برای فهمیدن موقعیت فعلی فایل های پروژه که مثلا در کدام مرحله هستند</p>
<p align="right">(working directory | staging area | head)</p>
<br>

### `git status --short` or `git status -s`: 
<p align="right">برای فهمیدن موقعیت فعلی فایل های پروژه به صورت <b>خلاصه شده</b> که مثلا در کدام مرحله هستند</p>
<br>
<hr>

<!-- ---------------------------------------------------------------------------------------------------------- -->

<div align="center" >
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/731249e7b065c208a7606d7b398ce2bac41d26b1/images/git-add.png">
</div>

### `git add <file name>` : 
<p align="right"><b>فایل</b> مورد نظر را به مرحله ی <b>استیجینگ</b> می برد</p>
<p align="right">staging area</p>
<br>

### `git add .` : 
<p align="right"><b>تمامی</b> فایل ها و تغییرات پروژه را به مرحله ی استیجینگ می برد</p>
<br>

### `git add *.AnExtension` example `git add *.css` : 
<p align="right">تمامی فایلهایی که پسوند مورد نظر را  داشته باشند به مرحله ی استیجینگ می برد که در اینجا گفته ایم تمامی فایلهای با پسوند css را به استیج ببر</p>
<br>
<hr>

<!-- ---------------------------------------------------------------------------------------------------------- -->

<div align="center" >
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/2d029aca4b8234e9bac1727223c84d3c6035a776/images/git-rm.png">
</div>

### `git rm <file name>` or `git rm -r <fale name>` :
<p align="right">فایل مورد نظر را از پروژه <b>حذف</b> می کند</p>
<br>

### `git rm -- *.AnExtension` for example `git rm -- *.py` :
<p align="right">تمامی فایل هایی که <b>پسوند</b> مورد نظر را داشته باشند حذف می کند</p>
<br>

### `git rm --cached --ignore-unmatch *.js` :
<p align="right">تمامی فایل های با پسوند مورد نظر را <b>نادیده</b> گرفته و <b>به مرحله ی ورکینگ دایرکتوری می برد</b></p>
<br>

### `git rm --cached <file name>` : 
<p align="right"><b>فایلی</b> که به مرحله ی استیجینگ اضافه شده را به مرحله ی <b>ورکینگ دایرکتوری</b> بر می گرداند </p>
<p align="right">(From staging area to working directory)</p>
<br>
<hr>

<!-- ---------------------------------------------------------------------------------------------------------- -->

<div align="center" >
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/40f6b1ea94378e16c2cb3bf4650311dfe4578c10/images/git-commit.png">
</div>

### `git commit -m <message>` :
<p align="right">فایل های پروژه که در مرحله ی استیجینگ قرار دارند را به یک پیغام مرتبط به مرحله ی نهایی یا هد، مخزن یا ریپوزیتوری می برد</p>
<p align="right">(From staging area to HEAD or repositories)</p>
<br>

### `git commit -am <message>` or `git commit -a -m <message>` :
<p align="right">فایل هایی که <b>از قبل</b> در پروژه ساخته شده اند و<b> تغییر پیدا می کنند</b> را مستقیماً به مرحله ی ریپوزیتوری یا هد می برد؛ اما اگر فایلی تازه ایجاد شده باشد ابتدا باید به استیج اضافه شود و سپس با کامیت مناسب به ریپوزیتوری اضافه شود</p>
<p align="left"> new file --> git add "file name" --> git commit -m "message" </p>
<p align="left"> modified file --> git commit -am "message" --> git commit -a -m "message" </p>
<br>

### `git commit --amend -m <message>` :
<p align="right">برای <b>تغییر نام آخرین کامیت</b> استفاده می شود</p>
<br>

### `git commit --amend -am <message>` or `git commit --amend -a -m <message>` :
<p align="right">آخرین تغییرات لوکال یا <b>working directory</b> را به آخرین کامیت اضافه می کند </p>
<br>
<hr>

<!-- ---------------------------------------------------------------------------------------------------------- -->

<div align="center" >
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/9f84915a653decde5acb2d4124e12ad06e610a05/images/git-tag.png">
</div>

### `git tag` or `git tag -l`: 
<p align="right">تگ برای <b>ورژن بندی</b> پروژه استفاده می شود که این دستور، لیست تگ های درون پروژه را نمایش می دهد و  اگر تگی وجود نداشته باشد، خروجی هم نخواهیم داشت</p>
<br>

### `git tag <tag name>` for example `git tag 3.12.0`: 
<p align="right">اگر یک ورژن یا نام بخصوصی روبروی دستور قرار دهیم آن را <b>برای آخرین کامیت</b> در نظر می گیرد</p>
<br>

### `git tag 3.13.0 <commit-hash>` example `git tag v5.2.0 6d2ef95` :
<p align="right">با قرار دادن <b>ورژن یا نام برای تگ</b> بعلاوه ی <b>کد هش کامیت مورد نظر</b> می توانیم برای کامیت هایمان تگ بگذاریم</p>
<br>

### `git show <tag name>` example `git show 3.13.2` :
<p align="right">برای مشاهده ی تغییرات درون هر تگ استفاده می کنیم</p>
<br>

### `git tag -d <tag name>` example `git tag -d 3.12.2` :
<p align="right">برای <b>حذف تگ</b> از این دستور استفاده می کنیم</p>
<br>

### `git tag -f <tag name> <commit-hash>` example `git tag -f v2.1.1 6d2ef95` :
<p align="right">یک زمانی یک تگی را اشتباهی به یک کامیت دیگر منتسب میکنیم که برای رفع این اشکال از این دستور استفاده میکنیم که می آید <b>نام تگ را از روی کامیت قبلی برداشته و روی کامیت جدید می گذارد</b></p>
<br>

### `git tag -l '13.*'` - `git tag -l '*.0'` - `git tag -l '*.1.*'` :
<p align="right">برای سرچ در تگ ها استفاده می کنیم که در مورد اول گفته ایم تگهایی که ابتدای آنها با فلان مشخصات شروع می شود و بعد از آن هر چیزی باشد
در مورد دوم گفته ایم تگ هایی را بیاور که آخر آنها صفر داشته باشد و قبل از آن هر چیزی باشد
و در مورد سوم گفته ایم که تگ هایی را بیاور عدد وصط آنها یک باشد و قبل و بعد آن هر چیزی باشد
</p>
<br>
<hr>

<!-- ---------------------------------------------------------------------------------------------------------- -->

<div align="center" >
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/94a989c252f295535c78e677fce6af6b9d2dd0e2/images/git-log.png">
</div>

### `git log` : 
<p align="right">تغییرات و کامیت های پروژه را بر می گرداند که در خروجی می توان نام و ایمیل نویسنده، تاریخ و ساعت درج کامیت را مشاهده کرد</p>
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

### `git log --author="user-name"` :
<p align="right">کامیت های نویسنده یا یوزر مورد نظر به همراه تاریخ و ساعت درج آنها را بر می گرداند</p>
<br>
<hr>

<!-- ---------------------------------------------------------------------------------------------------------- -->

<div align="center">
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/23a05680cf6bd592387e68299797be47dc6add29/images/git-blame.png">
</div>

### `git blame <file name>` :
<p align="right">یک زمانی میخواهیم بدانیم که کدهای یک قسمت پروژه، مثلاً در یک فایل خاص، توسط چه کسی نوشته شده اند که برای این کار، از این دستور استفاده می کنیم که <b>نام نویسنده</b> به همراه تاریخ درج و ساعت کامیت را نمایش میدهد</p>
<br>

### `git blame -e <file name>` --> `git blame -e python.py`:
<p align="right">یک زمانی میخواهیم بدانیم که کدهای یک قسمت پروژه، مثلاً در یک فایل خاص، توسط چه کسی نوشته شده اند که برای این کار، از این دستور استفاده می کنیم که <b>ایمیل نویسنده</b> به همراه تاریخ درج و ساعت کامیت را نمایش میدهد</p>
<br>

### `git blame <file name> -L start-line,end-line` --> 
### `git blame python.py -L 10,20`:
<p align="right">زمانی که بخواهیم بفهمیم کدهای مثلا از خط 10 تا 20 را در فلان فایل چه کسی نوشته است از این دستور استفاده می کنیم  که در خروجی، نام، تاریخ درج کامیت و ساعت آن را مشاهده خواهیم کرد</p>
<br>

### `git blame -L start-line,end-line <file-name>` :
<p align="right">زمانی که بخواهیم بفهمیم کدهای مثلا از خط 10 تا 20 را در فلان فایل چه کسی نوشته است از این دستور استفاده می کنیم  که در خروجی، نام، تاریخ درج کامیت و ساعت آن را مشاهده خواهیم کرد</p>
<br>
<hr>

<!-- ---------------------------------------------------------------------------------------------------------- -->

<div align="center">
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/42834c805f3cb89302e3e0d94652766b4d0a6087/images/git-show.png">
</div>

### `git show` :
<p align="right"><b>تمامی تغییرات در آخرین کامیت را برمی گرداند</b>؛ اینکه چند خط کد اضافه یا کم شده اند یا توسط چه کسی این تغییرات اعمال شده است</p>
<br>

### `git show <commit-hash>` :
<p align="right">تغییرات کامیتی که id وارد شده مربوط به آن می باشد را بر می گرداند که برای مشاهده ی این id باید از دستور git log --oneline استفاده کرد</p>
<br>

### `git show <commit-hash> --stat` :
<p align="right">تغییرات اعمال شده در کامیت مورد نظر را به صورت خلاصه شده به همراه مشخصات نویسنده نمایش می دهد</p>
<br>

### `git show <commit-hash> --path` :
<p align="right">این دستور تفاوت های واقعی ایجاد شده در commit از جمله خطوط اضافه و حذف شده را نمایش می دهد</p>
<br>

### `git show <tag name>` example `git show 3.13.2` :
<p align="right">برای مشاهده ی تغییرات درون هر تگ استفاده می کنیم</p>
<br>
<hr>

<!-- ---------------------------------------------------------------------------------------------------------- -->

<div align="center">
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/23a93a088f87ae7106cffd3f9f45214ae88ec6fd/images/git-config.png">
</div>

### `git config --list` :
<p align="right">لیستی از تمام تنظیمات پیکر بندی را که در حال حاضر روی نسخه ی نصبی گیت شما وجود دارد را نمایش می دهد؛ مثل تنظیمات محلی، تنظیمات سراسری و تنظیمات سیستم</p>
<br>

### `git config --local alias.<name> <command-name>` -> `git config --local alias.com commit` :
<p align="right">با استفاده از این دستور می توانیم برای دستورات گیت <b>درون لوکال</b> خودمان، اسامی کوتاه تر و خلاصه انتخاب کنیم که در این دستور، کامند commit را به com خلاصه کرده ایم</p>
<br>

### `git config --global alias.com  commit` :
<p align="right">اگر بخواهیم از یک نام مستعار در <b>تمامی پروژه هایمان</b> استفاده کنیم به جای کلمه ی local از کلمه ی global استفاده میکنیم</p>
<br>

### `git config --global user.name <your-name>` :
<p align="right">تنظیم نام کاربری برای تمامی پروژه ها</p>
<br>

<hr>

<!-- ---------------------------------------------------------------------------------------------------------- -->

<div align="center">
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/36c973fd4e0ed02cf70a5832c59b4c60d132334b/images/loading.gif">
</div>
<p align="center">New updates coming soon...</p>

<!-- <p align="right"></p> -->
