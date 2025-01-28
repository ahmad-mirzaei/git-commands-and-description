<!-- description -->
<h2 align="center">
  دستورات <a href="https://git-scm.com/doc">گیت</a> به همراه توضیحات مختصر آنها در اینجا قرار خواهند گرفت
</h2>
<br>
<hr>

<!-- ---------------------------------------------------------------------------------------------------------- -->

<!-- git logo -->
<!-- <div align="center">
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/2100aca18de101af32ed35f314d8c462dfd8dd29/git-logo-gif.gif">
</div>
<br> -->

<!-- ---------------------------------------------------------------------------------------------------------- -->

<!-- read-line -->
<!-- <div align="center">
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/ae35ec9426f4bb320eefac7d94961e33acc729ff/red-line.gif">
</div>
<br> -->

<!-- ---------------------------------------------------------------------------------------------------------- -->

<div align="center">
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/3624c3706fd890ef4a8584d9e45f1d1651a27bb3/images/create-an-empty-git-repository.png" alt="git-init">
</div>

<!-- git init -->
<table align="center">
    <thead>
        <tr>
            <th>دستورات</th>
            <th>توضیحات</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td align="left"><code>git init</code></td>
            <td align="right">معرفی کردن پروژه به گیت یا اینیشیالایز کردن آن (ایجاد یک ریپوزیتوری یا مخزن خالی در لوکال شما)</td>
        </tr>
        <tr>
            <td align="left"><code>git</code></td>
            <td align="right">مشاهده ی دستورات گیت</td>
        </tr>
    </tbody>
</table>
<br>
<hr

<!-- ---------------------------------------------------------------------------------------------------------- -->

<!-- git status -->
<div align="center" >
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/09b16830daf385e596a8dbb4cb741334f3a3ec06/images/GIT%20STATUS.png">
</div>

<table align="center">
    <thead>
        <tr>
            <th>دستورات</th>
            <th>توضیحات</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td align="left"><code>git status</code></td>
            <td align="right">( working directory - staging area - head ) مشاهده ی موقعیت فعلی فایل های پروژه؛ </td>
        </tr>
        <tr>
            <td align="left"><code>git status --short</code></td>
            <td align="right">مشاهده ی موقعیت فعلی فایل های پروژه به صورت <b>خلاصه شده</b></td>
        </tr>
        <tr>
            <td align="left"><code>git status -s</code></td>
            <td align="right"> مشاهده ی موقعیت فعلی فایل های پروژه به صورت <b>خلاصه شده</b></td>
        </tr>
    </tbody>
</table>
<br>
<hr>

<!-- ---------------------------------------------------------------------------------------------------------- -->

<!-- git add  -->
<div align="center" >
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/731249e7b065c208a7606d7b398ce2bac41d26b1/images/git-add.png">
</div>

<table align="center">
    <thead>
        <tr>
            <th>دستورات</th>
            <th>توضیحات</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td align="left"><code>git add [file-name]</code></td>
            <td align="right">[staging area] فایل مورد نظر را می برد به مرحله ی </td>
        </tr>
        <tr>
            <td align="left"><code>git add .</code></td>
            <td align="right">[staging area] تمامی فایل ها و تغییرات پروژه را می برد به مرحله ی </td>
        </tr>
        <tr>
            <td align="left"><code>git add -A</code></td>
            <td align="right">همانند دستور قبلی تمامی فایل ها و تغییرات پروژه را می برد به مرحله ی [staging area]</td>
        </tr>
        <tr>
            <td align="left"><code>git add *.AnExtension</code> -> <code>git add *.css</code></td>
            <td align="right">تمامی فایل هایی که پسوند مورد نظر را داشته باشند را می برد به مرحله ی [staging area]</td>
        </tr>
    </tbody>
</table>
<br>
<hr>

<!-- ---------------------------------------------------------------------------------------------------------- -->

<!-- git rm -->
<div align="center" >
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/2d029aca4b8234e9bac1727223c84d3c6035a776/images/git-rm.png" alt="git-rm">
</div>

<table align="center">
    <thead>
        <tr>
            <th>دستورات</th>
            <th>توضیحات</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td align="left"><code>git rm [file name]</code> or <code>git rm -r [file name]</code></td>
            <td align="right">فایل مورد نظر را از پروژه حذف می کند</td>
        </tr> 
        <tr>
            <td align="left"><code>git rm -- *.AnExtension</code> -> <code>git rm -- *.py</code></td>
            <td align="right">تمامی فایل هایی که پسوند مورد نظر را داشته باشند از پروژه حذف می کند</td>
        </tr>
        <tr>
            <td align="left"><code>git rm --cached --ignore-unmatch *.js</code></td>
            <td align="right"> تمامی فایل های با پسوند مورد نظر را نادیده گرفته و می برد به مرحله ی [working directory] </td>
        </tr>      
        <tr>
            <td align="left"><code>git rm --cached [file name]</code><code>git rm --cached .</code></td>
            <td align="right">[working directory] فایلی که به استیج رفته را می برد به مرحله ی </td>
        </tr>
        <tr>
            <td align="left"><code>git rm -rf --cached .</code></td>
            <td align="right">
                <p>
                    اگر مدتی پس از ایجاد پروژه بخواهیم فایلهایی را در <b>gitignore.</b> قرار دهیم و این کار انجام نشود، به این دلیل است که آن فایل ها در حال حاضر در مخزن یا ریپوزیتوری هستند و باید ابتدا آنها را با این دستور به <b>working directory</b> برده، و سپس دوباره به <b>staging area</b> ببریم
                </p>
            </td>
        </tr>
    </tbody>
</table>
<br>
<hr>
<!-- ---------------------------------------------------------------------------------------------------------- -->

<div align="center" >
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/40f6b1ea94378e16c2cb3bf4650311dfe4578c10/images/git-commit.png" alt="git-commit">
</div>

<table align="center">
    <thead>
        <tr>
            <th>دستورات</th>
            <th>توضیحات</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td align="left"><code>git commit -m [message]</code></td>
            <td align="right">(From staging area to HEAD or repositories) فایل های پروژه که در مرحله ی استیجینگ قرار دارند را به یک پیغام مرتبط به مرحله ی نهایی یا هد، مخزن یا ریپوزیتوری می برد</td>
        </tr>
        <tr>
            <td align="left"><code>git commit -am [message]</code> or <code>git commit -a -m [message]</code></td>
            <td align="right"> <p>فایل هایی که از قبل در پروژه ساخته شده اند و تغییر پیدا می کنند را مستقیماً به مرحله ی ریپوزیتوری یا هد می برد؛ اما اگر فایلی تازه ایجاد شده باشد ابتدا باید به استیج اضافه شود و سپس با کامیت مناسب به ریپوزیتوری اضافه شود</p>
                <p align="left"> new file --> git add "file name" --> git commit -m "message" </p>
                <p align="left"> modified file --> git commit -am "message" --> git commit -a -m "message" </p>
            </td>
        </tr>
        <tr>
            <td align="left"><code>git commit --amend -m [message]</code></td>
            <td align="right">تغییر نام آخرین کامیت</td>
        </tr>
        <tr>
            <td align="left"><code>git commit --amend -am [message]</code> or <code>git commit --amend -a -m [message]</code></td>
            <td align="right"><p>آخرین تغییرات لوکال یا <b>working directory</b> را به آخرین کامیت اضافه می کند </p></td>
        </tr>
    </tbody>
</table>
<br>
<hr>
<!-- ---------------------------------------------------------------------------------------------------------- -->

<div align="center" >
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/9f84915a653decde5acb2d4124e12ad06e610a05/images/git-tag.png" alt="git-tag">
</div>

<table align="center">
    <thead>
        <tr>
            <th>دستورات</th>
            <th>توضیحات</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td align="left"><code>git tag</code> or <code>git tag -l</code></td>
            <td align="right"><p>تگ برای <b>ورژن بندی</b> پروژه استفاده می شود که این دستور، لیست تگ های درون پروژه را نمایش می دهد و اگر تگی وجود نداشته باشد، خروجی هم نخواهیم داشت</p>
        </td>
        </tr>
        <tr>
            <td align="left"><code>git tag [tag name]</code> -> <code>git tag 3.12.0</code></td>
            <td align="right"><p>اگر یک ورژن یا نام بخصوصی روبروی دستور قرار دهیم آن را <b>برای آخرین کامیت</b> در نظر می گیرد</p></td>
        </tr>
        <tr>
            <td align="left"><code>git tag 3.13.0 [commit-hash]</code> -> <code>git tag v5.2.0 6d2ef95</code></td>
            <td align="right"><p>با قرار دادن <b>ورژن یا نام برای تگ</b> بعلاوه ی <b>کد هش کامیت مورد نظر</b> می توانیم برای کامیت هایمان تگ بگذاریم</p></td>
        </tr>
        <tr>
            <td align="left"><code>git show [tag name]</code> -> <code>git show 3.13.2</code></td>
            <td align="right"><p>برای مشاهده ی تغییرات درون هر تگ استفاده می کنیم</p></td>
        </tr>
        <tr>
            <td align="left"><code>git tag -d [tag name]</code> -> <code>git tag -d 3.12.2</code></td>
            <td align="right"><p>برای <b>حذف تگ</b> از این دستور استفاده می کنیم</p></td>
        </tr>
        <tr>
            <td align="left"><code>git tag -f [tag name] [commit-hash]</code> -> <code>git tag -f v2.1.1 6d2ef95</code></td>
            <td align="right"><p>یک زمانی یک تگی را اشتباهی به یک کامیت دیگر منتسب میکنیم که برای رفع این اشکال از این دستور استفاده میکنیم که می آید <b>نام تگ را از روی کامیت قبلی برداشته و روی کامیت جدید می گذارد</b></p></td>
        </tr>        
        <tr>
            <td align="left"><code>git tag -l '13.*' - git tag -l '*.0' - git tag -l '*.1.*'</code></td>
            <td align="right">
                <p>برای سرچ در تگ ها استفاده می کنیم که در مورد اول گفته ایم تگهایی که ابتدای آنها با فلان مشخصات شروع می شود و بعد از آن هر چیزی باشد
                در مورد دوم گفته ایم تگ هایی را بیاور که آخر آنها صفر داشته باشد و قبل از آن هر چیزی باشد
                و در مورد سوم گفته ایم که تگ هایی را بیاور عدد وصط آنها یک باشد و قبل و بعد آن هر چیزی باشد
                </p>
            </td>
        </tr>
    </tbody>
</table>
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

### `git config --global user.name <your-name>` and `git config --global user.email <your-email>` :
<p align="right">تنظیم نام کاربری و یا ایمیل کاربری برای <b>تمامی پروژه ها</b></p>
<br>

### `git config --global user.name` or `git config --global user.email` :
<p align="right">مشاهده ی نام یا ایمیل کاربری که برای تمام پروژه ها انتخاب کرده ایم</p>
<br>

### `git config user.name <your-name>` and `git config user.email <your-email>` :
<p align="right">تنظیم نام کاربری و یا ایمیل کاربری برای <b>یک پروژه</b></p>
<br>

### `git config user.name` or `git config user.email` :
<p align="right">مشاهده ی نام یا ایمیل کاربری که برای یک پروژه انتخاب کرده ایم</p>
<br>
<hr>

<!-- ---------------------------------------------------------------------------------------------------------- -->

<div align="center">
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/6b54be5ba9a395f603ec67c3020dfe950f1c5a49/images/git-branch.png">
</div>

### `git branch` :
<p align="right">نام <b>برنچ ها یا شاخه های پروژه</b>، <b>و برنچی که درون آن قرار داریم</b> را بر میگرداند</p>
<br>

### `git branch -a` :
<p align="right">لیست <b>تمام برنچ ها را اعم از لوکال و ریموت</b> بر می گرداند</p>
<br>

### `git branch origin --delete <branch-name>` :
<p align="right">برای حذف برنچ ریموت استفاده می شود</p>
<br>

### `git branch <new-branch-name>` :
<p align="right">از این دستور برای <b>ایجاد</b> یک برنچ یا شاخه ی جدید استفاده میکنیم</p>
<br>

### `git switch <branch-name>` :
<p align="right">سوئیچ کردن یا جابه جا شدن از یک برنچ به برنچ دیگر</p>
<br>

### `git switch -c <new-branch-name>` :
<p align="right">ساخت برنچ جدید و سوئیچ شدن به آن برنچ در لحظه</p>
<br>

### `git branch -d <branch-name>` :
<p align="right">برای حذف برنچی استفاده می شود که پس از ساخت هیچ تغییراتی درون آن صورت نگرفته و بلافاصله بخواهیم آن را حذف کنیم. اما اگر فایلی ساخته شد و کامیتی برای آن فایل در نظر گرفته شد، بعد از اجرای این دستور ما را راهنمایی می کند که برای حذف برنچ، از حرف D بزرگ استفاده کنید </p>
<br>

### `git branch -D <branch-name>` :
<p align="right">برای حذف شاخه یا برنچ مورد نظر استفاده می شود که در آن برنچ تغییرات و کامیت زده شده است</p>
<p align="right">نباید برای حذف  یک برنچ، درون خود آن برنچ باشیم؛ بلکه باید به برنچی دیگر سوئیچ کرده، سپس اقدام به حذف برنچ قبلی نماییم</p>
<br>

### `git branch -m <new-name>` or `git branch -m <branch-name> <new-name>` :
<p align="right">برای تغییر نام برنچ مورد نظر استفاده می شود که حرف -m  مخفف modified است</p>
<p align="right">برای تغییر نام حتماً باید درون همان برنچی باشیم که قصد تغییر نام آن را داریم</p>
<p align="right">از روش دوم زمانی استفاده می شود که در یک برنچ دیگر باشیم (مثلاً master) و بخواهیم نام یک برنچ دیگر (مثلاً second_branch) را تغییر دهیم که دیگر نیازی به سوئیچ کردن در برنچی که میخواهیم نام آن را تغییر دهیم، نیست</p>
<br>
<hr>

<!-- ---------------------------------------------------------------------------------------------------------- -->

<div align="center">
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/6e23a417bd29442ee7d4e34cb5d9894b891adbf3/images/git-merge.png">
</div>

### `git merge <branch-name>` :
<p align="right">الحاق برنچ فرعی به برنچ اصلی</p>
<p align="right">برای مرج کردن باید در برنچ اصلی یا master باشیم؛ و پس از اتمام عملیات باید برنچ فرعی را حذف کنیم</p>
<br>

### `git merge <source-branch> <target-branch>` -> `git merge second main` :
<p align="right">از این دستور زمانی استفاده می کنیم که بخواهیم بدون سوئیچ کردن به شاخه ی اصلی عملیات مرج را انجام دهیم</p>
<br>
<hr>

<!-- ---------------------------------------------------------------------------------------------------------- -->

<div align="center">
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/b2073a1db16d850b1ba9047c91852903b9134911/images/git-stash.png">
</div>

### `git stash` or `git stash save` :
<p align="right">یک زمانی نیاز است که در برنچ فرعی یا اصلی یک سری تغییراتی ایجاد کنیم که بخواهیم بعدا آن تغییرات را به پروژه اضافه یا اعمال کنیم؛ برای این کار نیاز به یک <b>چرک نویس</b> یا <b>یک جعبه یا  لیست</b> است که تغییرات را درون خود <b>نگه داری</b> کند تا زمانی که بخواهیم از آنها استفاده کنیم</p>
<br>

### `git stash save <message>` :
<p align="right"><b>زمانی که چندین استش داریم</b> می توانیم برای مدیریت بهتر، برای آنها نام یا پیامی در نظر بگیریم</p>
<br>

### `git stash show` :
<p align="right"><b>اطلاعات کلی</b> در مورد <b>فایلی که استش روی آن صورت گرفته</b> را برمی گرداند</p>
<br>

### `git stash list` :
<p align="right">لیست استش ها را بر می گرداند</p>
<br>

### `git stash show stash@{1}` :
<p align="right">پس  از مشاهده ی لیست استش ها از id یا اندیس آنها برای دیدن خلاصه تغییرات استفاده می کنیم که در اینجا گفته ایم از لیست اسش ها اندیس یکم را برگردان</p>
<br>

### `git stash show -p stash@{1}` :
<p align="right">دیدن تغییرات روی استش مورد نظر با جزئیات بیشتر</p>
<br>

### `git stash pop` :
<p align="right"><b>آخرین آیتم</b> درون استش را بر می گرداند</p>
<br>

### `git stash drop stash@{1}` :
<p align="right">برای <b>حذف</b> استش مورد نظر استفاده می شود</p>
<br>

### `git stash clear` :
<p align="right">حذف <b>تمامی</b> استش ها به صورت یکجا</p>
<br>

### `git stash apply` :
<p align="right">شاید لازم باشد که <b>از یک استش چندین بار استفاده شود</b> و از آنجایی که پاپ آخرین آیتم را بر می دارد و استش از درون چرک نویس یا لیست حذف می شود، از این دستور استفاده می کنیم تا بتوانیم از استش مورد نظر چندین بار استفاده کنیم و اگر لیستی از استش ها بگیریم، خواهیم دید که استش مورد نظر هنوز وجود دارد</p>
<br>
<hr>

<!-- ---------------------------------------------------------------------------------------------------------- -->

<div align="center">
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/eb735e7ac6b7f4d16fab33342ca3296072d8f8cc/images/git-diff.png">
</div>

<table align="center">
    <thead>
        <tr>
            <th>دستورات</th>
            <th>توضیحات</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td align="left"><code>git diff</code></td>
            <td align="right">مشاهده یا مقایسه ی تغییرات ورکینگ دایرکتوری با استیجینگ</td>
        </tr>
        <tr>
            <td align="left"><code>git diff --name-only [branch-name]</code></td>
            <td align="right">مشاهده ی فایل هایی که پس از یک کامیت خاص، تغییر کرده اند</td>
        </tr>
        <tr>
            <td align="left"><code>git diff --staged</code></td>
            <td align="right"> مشاهده یا مقایسه ی آخرین کامیت به همراه تغییرات در مرحله ی استیجینگ</td>
        </tr>
        <tr>
            <td align="left"><code>git diff head</code> or <code>[HEAD]</code></td>
            <td align="right">مقایسه ی آخرین کامیت با ورکینگ دایرکتوری</td>
        </tr>
        <tr>
            <td align="left"><code>git diff [first-hash-commit] [second-hash-commit]</code> -> <code>git diff 28344dc 85d9a5b</code> or <code>git diff 28344dc..85d9a5b</code></td>
            <td align="right">مشاهده یا مقایسه ی تغییرات دو کامیت با یک دیگر</td>
        </tr> 
        <tr>
            <td align="left"><code>git diff 28344dc..85d9a5b [file-name]</code></td>
            <td align="right">مشاهده یا مقایسه ی دو کامیت در یک فایل</td>
        </tr> 
        <tr>
            <td align="left"><code>git diff [first-branch] [second-branch]</code> or <code>git diff [first-branch]..[second-branch]</code></td>
            <td align="right">مشاهده یا مقایسه ی تغییرات دو برنچ <b>قبل از مرج شدن</b> با هم</td>
        </tr>
        <tr>
            <td align="left"><code>git diff HEAD^ HEAD</code></td>
            <td align="right">مشاهده ی تفاوت بین نسخه ی فعلی و آخرین نسخه</td>
        </tr>
    </tbody>
</table>
<br>
<hr>
<!-- ---------------------------------------------------------------------------------------------------------- -->

<div align="center">
  <img src="https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/36c973fd4e0ed02cf70a5832c59b4c60d132334b/images/loading.gif">
</div>
<p align="center">New updates coming soon...</p>

<!-- <p align="right"></p> -->

<!-- 
        <tr>
            <td align="left"><code></code></td>
            <td align="right"></td>
        </tr> 
-->