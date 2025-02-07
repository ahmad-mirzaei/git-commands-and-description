<a id="go-to-the-command-list"></a>

# دستورات گیت و توضیحات

## توضیحات
_دستورات [گیت](https://git-scm.com/doc) به همراه توضیحات مختصر آنها در این ریپوزیتوری فهرست می شوند؛ از ترجمه به زبانهای دیگر استفبال می شود_. &nbsp; 

---

- ### **ورژن های ترجمه شده**
    - [Persian Version - فارسی](READMEir.md)

---

<a id="go-to-the-command-list"></a>

### **فهرست دستورات**

| ردیف | عنوان | ردیف | عنوان | ردیف | عنوان |
|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
| 1 | [Init](#git-init) | 11 | [Branch](#git-branch) | 21 |  |
| 2 | [Satus](#git-status) | 12 | [Merge](#git-merge) | 22 |  |
| 3 | [Add](#git-add) | 13 | [Stash](#git-stash) | 23 |  |
| 4 | [Rm](#git-rm) | 14 | [Diff](#git-diff) | 24 |  |
| 5 | [Commit](#git-commit) | 15 | [Checkout](#git-checkout) | 25 |  |
| 6 | [Tag](#git-tag) | 16 | [Restore](#git-restore) | 26 |  |
| 7 | [Log](#git-log) | 17 | [Clean](#git-clean) | 27 |  |
| 8 | [Blame](#git-blame) | 18 | [Reset](#git-reset) | 28 |  |
| 9 | [Show](#git-show) | 19 | [Revert](#git-revert) | 29 |  |
| 10 | [Config](#git-config) | 20 | [Bisect](#git-bisect) | 30 |  |

---

<!-- git init -->
## <a id="create-empty-repository"></a>
![create-an-empty-git-repository](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/3624c3706fd890ef4a8584d9e45f1d1651a27bb3/images/create-an-empty-git-repository.png)

| دستورات | توضیحات |
|-----|-----:|
| `git -v` or `git --version` | مشاهده ی ورژن نصب شده ی گیت |
| `git init` | معرفی کردن پروژه به گیت یا اینیشیالایز کردن آن (ایجاد یک ریپوزیتوری یا مخزن خالی در لوکال شما) |
| `git` or `git help` | نمایش راهنمای کلی گیت |
<br />

👆[برو به فهرست](#go-to-the-command-list)

---

<!-- git status -->
## <a id="git-status"></a>
![git-status](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/09b16830daf385e596a8dbb4cb741334f3a3ec06/images/GIT%20STATUS.png)

| دستورات | توضیحات |
|-----|-----:|
| `git status` | ( working directory - staging area - head ) مشاهده ی موقعیت فعلی فایل های پروژه؛ |
| `git status --short` | مشاهده ی موقعیت فعلی فایل های پروژه به صورت خلاصه شده |
| `git status -s` | مشاهده ی موقعیت فعلی فایل های پروژه به صورت خلاصه شده |
<br />

👆[برو به فهرست](#go-to-the-command-list) &nbsp; | &nbsp; [قبلی](#create-empty-repository)👈 

---

<!-- git add -->
## <a id="git-add"></a>
![git-add](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/731249e7b065c208a7606d7b398ce2bac41d26b1/images/git-add.png)

| دستورات | توضیحات |
|-----|-----:|
| `git add [file-name]` | [staging area] فایل مورد نظر را می برد به مرحله ی |
| `git add .` | [staging area] تمامی فایل ها و تغییرات پروژه را می برد به مرحله ی  |
| `git add -A` |[staging area] همانند دستور قبلی تمامی فایل ها و تغییرات پروژه را می برد به مرحله ی  |
| `git add *.AnExtension` -> `git add *.css` |[staging area] تمامی فایل هایی که پسوند مورد نظر را داشته باشند را می برد به مرحله ی  |
<br />

👆[برو به فهرست](#go-to-the-command-list) &nbsp; | &nbsp; [قبلی](#git-status)👈  

--- 

<!-- git rm -->
## <a id="git-rm"></a>
![git-rm](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/2d029aca4b8234e9bac1727223c84d3c6035a776/images/git-rm.png)

| دستورات | توضیحات |
|-----|-----:|
| `git rm [file name]` or `git rm -r [file name]` | فایل مورد نظر را از پروژه حذف می کند |
| `git rm -- *.AnExtension` -> `git rm -- *.py` | تمامی فایل هایی که پسوند مورد نظر را داشته باشند از پروژه حذف می کند |
| `git rm --cached --ignore-unmatch *.js` | [working directory] تمامی فایل های با پسوند مورد نظر را می برد به مرحله ی  |
| `git rm --cached [file name]` -> `git rm --cached .` | [working directory] تمامی فایل های با پسوند مورد نظر را نادیده گرفته و می برد به  |
| `git rm -rf --cached .` | [working directory] تمامی فایل ها را از `ریپوزیرتوری لوکال` می برد به مرحله ی  |
<br />

👆[برو به فهرست](#go-to-the-command-list) &nbsp; | &nbsp; [قبلی](#git-add)👈

--- 

<!-- git commit -->
## <a id="git-commit"></a>
![git-commit](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/40f6b1ea94378e16c2cb3bf4650311dfe4578c10/images/git-commit.png)

| دستورات | توضیحات |
|-----|-----:|
| `git commit -m [message]` | فایل های پروژه که در مرحله ی استیجینگ قرار دارند را با یک پیغام مرتبط به مرحله ی نهایی یا هد، مخزن یا ریپوزیتوری می برد (From staging area to HEAD or repositories) |
| `git commit -am [message]` or `git commit -a -m [message]` | **فایل هایی که از قبل در پروژه ساخته شده اند** و تغییر پیدا می کنند را مستقیماً به مرحله ی ریپوزیتوری یا هد می برد <br /> new file --> git add "file name" --> git commit -m "message" <br /> modified file --> git commit -am "message" --> git commit -a -m "message" |
| `git commit --amend -m [message]` | تغییر نام آخرین کامیت |
| `git commit --amend -am [message]` or `git commit --amend -a -m [message]` | آخرین تغییرات لوکال یا `working directory` را به آخرین کامیت اضافه می کند  |
<br />

👆[برو به فهرست](#go-to-the-command-list) &nbsp; | &nbsp; [قبلی](#git-rm)👈

--- 

<!-- git tag -->
## <a id="git-tag"></a>
![git-tag](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/9f84915a653decde5acb2d4124e12ad06e610a05/images/git-tag.png)

| دستورات | توضیحات |
|-----|-----:|
| `git tag` or `git tag -l` | تگ برای ورژن بندی پروژه استفاده می شود که این دستور، لیست تگ های درون پروژه را نمایش می دهد و اگر تگی وجود نداشته باشد، خروجی هم نخواهیم داشت |
| `git tag [tag name]` -> `git tag 3.12.0` | اگر یک ورژن یا نام بخصوصی روبروی دستور قرار دهیم آن را برای آخرین کامیت در نظر می گیرد |
| `git tag 3.13.0 [commit-hash]` -> `git tag v5.2.0 6d2ef95` | با قرار دادن ورژن یا نام برای تگ بعلاوه ی کد هش کامیت مورد نظر می توانیم برای کامیت هایمان تگ بگذاریم |
| `git show [tag name]` -> `git show 3.13.2` | برای مشاهده ی تغییرات درون هر تگ استفاده می کنیم |
| `git tag -d [tag name]` -> `git tag -d 3.12.2` | برای حذف تگ از این دستور استفاده می کنیم |
| `git tag -f [tag name] [commit-hash]` -> `git tag -f v2.1.1 6d2ef95` | ک زمانی یک تگی را اشتباهی به یک کامیت دیگر منتسب میکنیم که برای رفع این اشکال از این دستور استفاده میکنیم که می آید نام تگ را از روی کامیت قبلی برداشته و روی کامیت جدید می گذارد |
| `git tag -l '13.*'` - `git tag -l '*.0'` - `git tag -l '*.1.*'` | برای سرچ در تگ ها استفاده می کنیم که در مورد اول گفته ایم تگهایی که ابتدای آنها با فلان مشخصات شروع می شود و بعد از آن هر چیزی باشد در مورد دوم گفته ایم تگ هایی را بیاور که آخر آنها صفر داشته باشد و قبل از آن هر چیزی باشد و در مورد سوم گفته ایم که تگ هایی را بیاور عدد وصط آنها یک باشد و قبل و بعد آن هر چیزی باشد |
<br />

👆[برو به فهرست](#go-to-the-command-list) &nbsp; | &nbsp; [قبلی](#git-commit)👈 

--- 

<!-- ---------------------------------------------------------------------------------------------------------- -->

<!-- git log -->
## <a id="git-log"></a>
![git-log](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/94a989c252f295535c78e677fce6af6b9d2dd0e2/images/git-log.png)

| دستورات | توضیحات |
|-----|-----:|
| `git log` | تغییرات و کامیت های پروژه را بر می گرداند که در خروجی می توان نام و ایمیل نویسنده، تاریخ و ساعت درج کامیت را مشاهده کرد |
| `git log --oneline` | تغییرات و کامیت های پروژه را به صورت **خلاصه شده و کوتاه** بر می گرداند |
| `git log --oneline --all` | [origin] و [head] مشاهده ی تمامی کامیت ها و دیدن موقعیت  |
| `git log --stat` | تغییرات پروژه را به صورت خیلی کاملتری نمایش می دهد؛ به طوری که می توان نام و ایمیل نویسنده، تاریخ و ساعت درج کامیت و همچنین تعداد فایل های تغییر یافته و تعداد خط کدهایی که به فایل تغییر یافته اضافه یا کم شده اند را نمایش می دهد |
| `git log --graph` | اطلاعات کامیت ها را به صورت **گرافیکی** نمایش می دهد |
| `git log --graph --oneline` | اطلاعات کامیت ها را به صورت **گرافیکی ولی جزئی تر و خلاصه تر** برمیگرداند |
| `git log --after="25-10-12"` | کامیت های **بعد از یک تاریخ مشخص** را بر میگرداند |
| `git log --before="25-10-12"` | کامیت های **قبل از یک تاریخ مشخص** را بر میگرداند |
| `git log --author="user-name"` | کامیت های نویسنده یا یوزر مورد نظر به همراه تاریخ و ساعت درج آنها را بر می گرداند  |
<br />

👆[برو به فهرست](#go-to-the-command-list) &nbsp; | &nbsp; [قبلی](#git-tag)👈  

--- 

<!-- git blame -->
## <a id="git-blame"></a>
![git-blame](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/23a05680cf6bd592387e68299797be47dc6add29/images/git-blame.png)

| دستورات | توضیحات |
|-----|-----:|
| `git blame [file name]` | یک زمانی میخواهیم بدانیم که کدهای یک قسمت پروژه، مثلاً در یک فایل خاص، توسط چه کسی نوشته شده اند که برای این کار، از این دستور استفاده می کنیم که نام نویسنده به همراه تاریخ درج و ساعت کامیت را نمایش میدهد |
| `git blame -e [file name]` | یک زمانی میخواهیم بدانیم که کدهای یک قسمت پروژه، مثلاً در یک فایل خاص، توسط چه کسی نوشته شده اند که برای این کار، از این دستور استفاده می کنیم که ایمیل نویسنده به همراه تاریخ درج و ساعت کامیت را نمایش میدهد |
| `git blame [file name] -L [start-line],[end-line]` | زمانی که بخواهیم بفهمیم کدهای مثلا از خط 10 تا 20 را در فلان فایل چه کسی نوشته است از این دستور استفاده می کنیم که در خروجی، نام، تاریخ درج کامیت و ساعت آن را مشاهده خواهیم کرد |
| `git blame -L start-line,end-line [file-name]` | شبیه دستور قبلیست با کمی جابجایی در دستورات |
<br />

👆[برو به فهرست](#go-to-the-command-list) &nbsp; | &nbsp; [قبلی](#git-log)👈 

---

<!-- git show -->
## <a id="git-show"></a>
![git-show](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/42834c805f3cb89302e3e0d94652766b4d0a6087/images/git-show.png)

| دستورات | توضیحات |
|-----|-----:|
| `git show` | تمامی تغییرات در آخرین کامیت را برمی گرداند؛ اینکه چند خط کد اضافه یا کم شده اند یا توسط چه کسی این تغییرات اعمال شده است |
| `git show [commit-hash]` | مشاهده ی تغییرات در کامیت مورد نظر با استفاده از کد هش آن کامیت |
| `git show [commit-hash] --stat` | تغییرات اعمال شده در کامیت مورد نظر را به صورت خلاصه شده به همراه مشخصات نویسنده نمایش می دهد |
| `git show [commit-hash] --path` | این دستور تفاوت های واقعی ایجاد شده در کامیت از جمله خطوط اضافه و حذف شده را نمایش می دهد |
| `git show [tag name]` | برای مشاهده ی تغییرات درون هر تگ استفاده می کنیم |
<br />

👆[برو به فهرست](#go-to-the-command-list) &nbsp; | &nbsp; [قبلی](#git-blame)👈 

---

<!-- git config -->
## <a id="git-config"></a>
![git-config](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/23a93a088f87ae7106cffd3f9f45214ae88ec6fd/images/git-config.png)

| دستورات | توضیحات |
|-----|-----:|
| `git config --list` | لیستی از تمام تنظیمات پیکر بندی که در حال حاضر روی نسخه ی نصبی گیت شما وجود دارد را نمایش می دهد؛ مثل تنظیمات محلی، تنظیمات سراسری و تنظیمات سیستم |
| `git config --local alias.[name] [command-name]` -> `git config --local alias.com commit` | با استفاده از این دستور می توانیم برای دستورات گیت درون لوکال خودمان، اسامی کوتاه تر و خلاصه انتخاب کنیم |
| `git config --global alias.com commit` | اگر بخواهیم از یک نام مستعار در تمامی پروژه هایمان استفاده کنیم به جای کلمه ی لوکال از کلمه ی گلوبال استفاده میکنیم |
| `git config --global user.name [your-name]` & `git config --global user.email [your-email]` | تنظیم نام کاربری و ایمیل کاربری برای تمامی پروژه ها |
| `git config --global user.name` & `git config --global user.email` | مشاهده ی نام یا ایمیل کاربری که برای تمام پروژه ها انتخاب کرده ایم |
| `git config user.name [your-name]` & `git config user.email [your-email]` | تنظیم نام کاربری و یا ایمیل کاربری برای یک پروژه |
| `git config user.name` or `git config user.email` | مشاهده ی نام یا ایمیل کاربری که برای یک پروژه انتخاب کرده ایم |
<br />

👆[برو به فهرست](#go-to-the-command-list) &nbsp; | &nbsp; [قبلی](#git-show)👈 

---

<!-- git branch -->
## <a id="git-branch"></a>
![git-branch](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/6b54be5ba9a395f603ec67c3020dfe950f1c5a49/images/git-branch.png)

| دستورات | توضیحات |
|-----|-----:|
| `git branch` | نام برنچ ها یا شاخه های پروژه، و برنچی که درون آن قرار داریم را بر میگرداند |
| `git branch -a` | لیست **تمام** برنچ ها را اعم از لوکال و ریموت بر می گرداند |
| `git branch origin --delete [branch-name]` | برای حذف برنچ ریموت استفاده می شود |
| `git branch [new-branch]` | ایجاد یک برنچ یا شاخه ی جدید |
| `git switch [branch-name]` | سوئیچ کردن یا جابه جا شدن از یک برنچ به برنچ دیگر |
| `git switch -c [new-branch-name]` | ساخت برنچ جدید و سوئیچ کردن در آن برنچ در لحظه |
| `git branch -d [branch-name]` | برای حذف برنچی استفاده می شود که پس از ساخت هیچ تغییراتی درون آن صورت نگرفته و بلافاصله بخواهیم آن را حذف کنیم. اما اگر فایلی ساخته شد و کامیتی برای آن فایل در نظر گرفته شد، از دستور زیر استفاده می کنیم |
| `git branch -D [branch-name]` | برای حذف شاخه یا برنچ مورد نظر استفاده می شود که در آن برنچ تغییرات و کامیت زده شده است <br /> نباید برای حذف یک برنچ، درون خود آن برنچ باشیم؛ بلکه باید به برنچی دیگر سوئیچ کرده، سپس اقدام به حذف برنچ قبلی نماییم |
| `git branch -m [new-name]` or `git branch -m [branch-name] [new-name]` | تغییر نام برنچ مورد نظر <br /> از روش دوم زمانی استفاده می شود که در یک برنچ دیگر باشیم و بخواهیم نام یک برنچ دیگر را تغییر دهیم که دیگر نیازی به سوئیچ کردن در برنچی که میخواهیم نام آن را تغییر دهیم، نیست |
<br />

👆[برو به فهرست](#go-to-the-command-list) &nbsp; | &nbsp; [قبلی](#git-config)👈 

---

<!-- git merge -->
## <a id="git-merge"></a>
![git-merge](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/6e23a417bd29442ee7d4e34cb5d9894b891adbf3/images/git-merge.png)

| توضیحات | دستورات | 
|-----|-----:|
| `git merge [branch-name]` | الحاق برنچ فرعی به برنچ اصلی <br /> برای مرج کردن باید در برنچ اصلی باشیم؛ و پس از اتمام عملیات باید برنچ فرعی را حذف کنیم |
| `git merge [source-branch] [target-branch]` | از این دستور زمانی استفاده می کنیم که بخواهیم بدون سوئیچ کردن به شاخه ی اصلی عملیات مرج را انجام دهیم |
<br />

👆[برو به فهرست](#go-to-the-command-list) &nbsp; | &nbsp; [قبلی](#git-branch)👈 

---

<!-- git stash -->
## <a id="git-stash"></a>
![git-stash](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/b2073a1db16d850b1ba9047c91852903b9134911/images/git-stash.png)

| توضیحات | دستورات | 
|-----|-----:|
| `git stash` or `git stash save` | یک زمانی نیاز است که در برنچ فرعی یا اصلی یک سری تغییراتی ایجاد کنیم که بخواهیم بعدا آن تغییرات را به پروژه اضافه یا اعمال کنیم؛ برای این کار نیاز به یک چرک نویس یا یک جعبه یا لیست است که تغییرات را درون خود نگه داری کند تا زمانی که بخواهیم از آنها استفاده کنیم |
| `git stash save [message]` | هنگام استفاده از **استش**، می توانید یک نام یا پیام برای توصیف تغییرات ذخیره شده ارائه دهید |
| `git stash show` | اطلاعات کلی در مورد فایلی که استش روی آن صورت گرفته را برمی گرداند |
| `git stash list` | لیست استش ها را بر می گرداند |
| `git stash show stash@{index}` | نمایش تغییرات کامل هر استش با استفاده از اندیس آن |
| `git stash show -p stash@{index}` | دیدن تغییرات روی استش مورد نظر با جزئیات بیشتر |
| `git stash pop` | آخرین آیتم درون استش را بر می گرداند |
| `git stash apply` | تغییرات **استش** انتخاب‌ شده را به پروژه اعمال می‌کند بدون اینکه آن را از لیست استش‌ها حذف کند | 
| `git stash drop stash@{index}` | برای حذف استش مورد نظر استفاده می شود |
| `git stash clear` | حذف تمامی استش ها به صورت یکجا |
<br />

👆[برو به فهرست](#go-to-the-command-list) &nbsp; | &nbsp; [قبلی](#git-merge)👈 

---

<!-- git diff -->
## <a id="git-diff"></a>
![git-diff](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/eb735e7ac6b7f4d16fab33342ca3296072d8f8cc/images/git-diff.png)

| توضیحات | دستورات | 
|-----|-----:|
| `git diff` | مشاهده یا مقایسه ی تغییرات ورکینگ دایرکتوری با استیجینگ |
| `git diff --name-only [branch-name]` | مشاهده ی **نام** فایل هایی که پس از یک کامیت خاص، تغییر کرده اند |
| `git diff --staged` | مشاهده یا مقایسه ی آخرین کامیت به همراه تغییرات در مرحله ی استیجینگ |
| `git diff head or [HEAD]` | مقایسه ی آخرین کامیت با ورکینگ دایرکتوری |
| `git diff [first-hash-commit] [second-hash-commit]` -> `git diff 28344dc 85d9a5b` or `git diff 28344dc..85d9a5b` | مشاهده یا مقایسه ی تغییرات دو کامیت با یک دیگر |
| `git diff 28344dc..85d9a5b [file-name]` | مشاهده یا مقایسه ی دو کامیت در یک فایل |
| `git diff [first-branch] [second-branch]` or `git diff [first-branch]..[second-branch]` | مشاهده یا مقایسه ی تغییرات دو برنچ قبل از مرج شدن با هم |
| `git diff HEAD^ HEAD` | مشاهده ی تفاوت بین نسخه ی فعلی و آخرین نسخه |
<br />

👆[برو به فهرست](#go-to-the-command-list) &nbsp; | &nbsp; [قبلی](#git-stash)👈 

---

<!-- git checkout -->
## <a id="git-checkout"></a>
![git-checkout](https://github.com/ahmad-mirzaei/git-commands-and-description/blob/168ba498fb4fe7ff88a4d5cfc6dd530e7fdea94d/images/git-checkout.png)

| توضیحات | دستورات | 
|-----|-----:|
| `git checkout [branch-name]` | به برنچی که مشخص کرده اید سوئیچ می شوید| 
| `git switch [branch-name]` | به برنچی که مشخص کرده اید سوئیچ می شوید |
| `git checkout [hash-commit]` | زمانی که بخواهیم تغییرات پروژه را به یک کامیت در گذشته ببریم از این دستور استفاده می شود که در این صورت می گوییم **هد دیتچ یا جابجا** شده است |
| `git checkout -- [file-name]` | این دستور تغییرات اعمال‌شده روی فایل‌ها را در ورکینگ دایرکتوری لغو می‌کند و آن‌ها را به آخرین وضعیت کامیت باز می‌گرداند |
| `git checkout [hash-commit] [file-name]` |  برگرداندن تغییرات یک فایل بخصوص به یک کامیت با هش  کد آن کامیت  |
| `git checkout HEAD~[number]` -> `git checkout HEAD~5` | برگشتن به چند کامیت قبل تر با وارد کردن تعداد حرکت از هد به کامیت های پایین تر |
| `git checkout HEAD [file-name]` | بازگرداندن تغییرات فعلی فایل، به آخرین کامیت زده شده <br /> Discard working directory changes |
| `git checkout HEAD .` | زمانی که در ورکینگ دایرکتوری روی چند فایل تغییرات ایجاد کرده ایم ولی نمی خواهیم که آن تغییرات اعمال  شوند، از این دستور استفاده می کنیم که در این حالت، همه ی تغییرات را دیسکارد کرده ایم <br /> Discarding all changes in the working directory|
| `git checkout -- .` | دور انداختن همه تغییرات در ورکینگ دایرکتوری و بازگرداندن آن به وضعیت آخرین کامیت |
| `git checkout -b [new-branch-name]` | ایجاد یک برنچ و سوئیچ کردن در آن |
<br />

👆[برو به فهرست](#go-to-the-command-list) &nbsp; | &nbsp; [قبلی](#git-diff)👈 

---

<!-- git restore -->
## <a id="git-restore"></a>
![git-restore](https://github.com/ahmad-mirzaei/git-commands-and-description/blob/a06c7e6cef5de9b7ea8f69c03fe4c42ed1ebb29a/images/git-restore.png)

| توضیحات | دستورات | 
|-----|-----:|
| `git restore [file-name]` | زمانی که در ورکینگ دایرکتوری در یک فایلی تغییراتی ایجاد میکنیم یا به اصطلاح مادیفای می کنیم، با اجرای این دستور، تغییرات دیسکارد می شوند یا تغییرات بر می گردند به آخرین کامیت یا هد که دقیقاً کار دستور زیر را انجام می دهد <br /> `git checkout HEAD`  |
| `git restore --staged [file-name]` | زمانی که یک فایل جدید ساخته ایم و به مرحله ی استیجینگ برده ایم، با اجرای این دستور به حالت **آنترکد** در می آید <br /> `untracked` |
| `git restore --source [hash-commit] [file-name] ` | این دستور شبیه دستور زیر است <br />  git checkout [hash-commit] [file-name] <br /> ولی با این تفاوت که، **هد** جابجا یا **دیتچ** نمی شود. یعنی داریم میگوییم که فایل مورد نظر را برگردان به فلان کد هش یا سورس  مورد نظر|
| `git restore --source HEAD python.py` | برگرداندن تغییرات به **آخرین کامیت یا هد**  |
| `git restore --source HEAD~5 [file-name]` | بردن **هد** به پنج کامیت قبل (تغییرات پروژه را به **5** کامیت قبل بر می گرداند) |
<br />

👆[برو به فهرست](#go-to-the-command-list) &nbsp; | &nbsp; [قبلی](#git-checkout)👈 

---

<!-- git clean -->
## <a id="git-clean"></a>
![git-clean](https://github.com/ahmad-mirzaei/git-commands-and-description/blob/d5904c7c8fd3305b856323ada458be9ebe993811/images/git-clean.png)

| توضیحات | دستورات | 
|-----|-----:|
| `git clean -h` | [clean] مشاهده ی راهنمای دستورات  |
| `git clean -f -d [file-name]` |حذف فایلی که ساخته شده و هنوز به مرحله ی استیجینگ نرفته و کامیتی هم برای آن در نظر گرفته نشده است |
<br />

👆[برو به فهرست](#go-to-the-command-list) &nbsp; | &nbsp; [قبلی](#git-restore)👈 

---

<!-- git reset -->
## <a id="git-reset"></a>
![git-reset](https://github.com/ahmad-mirzaei/git-commands-and-description/blob/4e57ac4c22cc2883a89145e68793fff34cc5ed42/images/git-reset.png)

| توضیحات | دستورات | 
|-----|-----:|
| `git reset --soft [hash-commit]` | با اجرای این دستور اگر مثلاً کد هش مربوط به 4 کامیت پایینتر باشد، برمیگردیم به 4 کامیت قبل و تمامی کامیت های بالایی از ریپوزیتوری حذف می شوند اما فایل ها و تغییراتی که در پروژه صورت گرفته حذف نمی شوند بلکه به یک مرحله قبل تر یعنی استیجینگ می برد تا دوباره نسبت به آنها تصمیم گیری شود |
| `git reset [hash-commit]` or `git reset --mixed [hash-commit]` | همانند دستور قبلی عمل می کند یعنی بر میگردد به کامیت قبلی و کامیت های بالایی را از ریپوزیتوری حذف می کند اما با این تفاوت که تغییرات را اگر در مرحله ی استیجینگ باشند، به مرحله ی ورکینگ دایرکتوری می برد و اگر در مرحله ی ورکینگ دایرکتوری باشند، آنها را **آنترکد** میکند |
| `git reset --hard [hash-commit]` | تمام پروژه را می برد به همان کامیتی که میخواهیم و حتی مرحله ی ورکینگ دایرکتوری را هم تغییر می دهد.. یعنی تغییرات هم بر می گردند به همان کامیتی که خواسته ایم <br /> نکته: فایل هایی که **آنترکد** بودند با اجرای این دستور از بین نمی روند چون گیت این فایلها را به دلیل **آنترکد** بودن نمی شناسد و به همین دلیل تغییری روی این فایل ها اعمال نمی شود|
<br />

👆[برو به فهرست](#go-to-the-command-list) &nbsp; | &nbsp; [قبلی](#git-clean)👈 

---

<!-- git revert -->
## <a id="git-revert"></a>
![git-revert](https://github.com/ahmad-mirzaei/git-commands-and-description/blob/04c5cfd16d1504c2889d1e2aaaa3649d4d85b366/images/git-revert.png)

| توضیحات | دستورات | 
|-----|-----:|
| `git revert [hash-commit]` | از این دستور زمانی استفاده می شود که، به فرض مثال یک زمانی یک کامیتی ایجاد کرده ایم و حال متوجه می شویم که آن کامیت به درد پروژه نمی خورد؛ مثلاً میخواهیم هر کدی که قبلاً در فایل مورد نظر بوده پاک شود و کدهایی که قبلاً پاک کرده بودیم برگردند<br /> نکته ی مهم اینکه، اگر یک کامیتی را **ریورت** کنیم که به یک کامیت دیگر وابسته باشد، به  **کانفلیکت یا تداخل** میخوریم و برای حل این مشکل باید از دستور **ریست** استفاده کنیم |
<br />

👆[برو به فهرست](#go-to-the-command-list) &nbsp; | &nbsp; [قبلی](#git-reset)👈 

---

<!-- git bisect -->
## <a id="git-bisect"></a>
![git-bisect](https://github.com/ahmad-mirzaei/git-commands-and-description/blob/4c0c7fe81e7bc86124b703e4913e58d05be31f48/images/git-bisect.png)

| توضیحات | دستورات | 
|-----|-----:|
| `git bisect start` | زمانی که تعداد کایمت های پروژه زیاد هستند و در یک جایی به باگی بر می خوریم از این دستور استفاده می کنیم تا به باگ مورد نظر رسیده و آن را فیکس کنیم؛ این دستور به صورت باینری در کامیت ها سرچ انجام می دهد تا به باگ برسد |
| `` |  |
| `` |  |
| `` |  |
<br />

👆[برو به فهرست](#go-to-the-command-list) &nbsp; | &nbsp; [قبلی](#git-revert)👈 

---

![updating](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/2c6daafcb71ea5808ce52360a5c333d34733048c/images/updating-coming-soon.gif)



