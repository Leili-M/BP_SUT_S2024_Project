![logo](starstore.png)
<img align="left" src="https://user-images.githubusercontent.com/65187002/144930161-2f783401-8d27-4fdf-a2f7-cc0ba32f1f1f.gif" width="21%" style="display:inline;"><img align="right" src="https://user-images.githubusercontent.com/65187002/144930161-2f783401-8d27-4fdf-a2f7-cc0ba32f1f1f.gif" width="21%" style="display:inline;">
<h1 align="center">پروژه مبانی برنامه سازی پایتون</h1>
<h2 align="center">بهار 1403</h2>
<h3 align="center">StarStore</h3>
<p align="center">فروشگاه StarStore به تازگی آغاز به کار کرده است. در این پروژه، قصد داریم با استفاده از مفاهیم شی‌گرایی و پایگاه داده، یک رابط کاربری خط فرمان (CLI) طراحی کنیم که امکاناتی چون ورود کاربران، ثبت نام، مدیریت سفارشات، و نظارت بر محصولات را برای این فروشگاه فراهم آورد.</p>
<div align="center">
  <img src="https://techstack-generator.vercel.app/python-icon.svg" alt="icon" width="50" height="50" />
 <img src="https://techstack-generator.vercel.app/mysql-icon.svg" alt="icon" width="50" height="50" />
</div>
<br>
<img src="https://i.imgur.com/dBaSKWF.gif" height="20" width="100%">
<h3 align="right">صفحه اصلی</h3>
<p align="right">در ورودی این سیستم، ابتدا باید تعیین شود که کاربر ورود کننده ادمین است یا مشتری</p>
<br>
<h3 align="right">ورود ادمین</h3>
<p align="right">
 <ul align="right">
  <li>ادمین باید نام کاربری و رمز عبور خود را وارد نماید.</li>
  <li>سیستم صحت نام کاربری و رمز عبور را بررسی کرده و در صورت احراز هویت، ادمین به پنل مدیریتی دسترسی پیدا می‌کند.</li>
 </ul>
</p>
<br>
<h3 align="right">ورود مشتری</h3>
<p align="right">•مشتری دو گزینه پیش رو دارد: ثبت نام یا ورود به حساب کاربری</p>
<p align="right">
 <ul align="right">
  <li align="right">ورود به حساب کاربری: مشتری باید نام کاربری و رمز عبور خود را وارد کند. سیستم صحت اطلاعات را بررسی کرده و در صورت تأیید، به حساب کاربری وارد می‌شود.</li>
  <li align="right">ثبت نام
    <ul align="right">
      <li align="right">مشتری باید اطلاعات لازم را وارد نماید</li>
      <li align="right">یک نام کاربری انتخاب کند که پیش از این در سیستم ثبت نشده باشد.</li>
      <li align="right">سپس باید رمز عبوری انتخاب کند که شامل حداقل 8 کاراکتر، یک کاراکتر بزرگ، و ترکیبی از اعداد و حروف باشد.</li>
    </ul>
  </li>
 </ul>
</p>
<p>این مراحل اولیه اطمینان می‌دهند که تمامی کاربران به طور مناسبی شناسایی و مدیریت شوند و به بخش‌های مربوط به نقش خود در سیستم دسترسی پیدا کنند.</p>
<h3 align="right">پس از ورود به پنل مشتری</h3>
<h4 align="right">نمایش اعتبار کیف پول</p>
<p align="right">به محض ورود مشتری به پنل خود، مقدار اعتبار کیف پول او نمایش داده می‌شود.</p>
<h4 align="right">منوی مشتری شامل</p>
<p align="right">
 <ol align="right">
  <li align="right">ثبت سفارش جدید
    <ul align="right">
      <li align="right">o	نمایش لیست کالاها به همراه قیمت‌ها.(هر کالا شامل یک کد منحصر به فرد است می تواند برای انتخاب کالا ها توسط مشتری از کد آن ها استفاده نمایید.)</li>
      <li align="right">مشتری می‌تواند کالاهای مورد نظر خود را به همراه تعداد مشخص کند.</li>
      <li align="right">اگر تعداد درخواستی بیشتر از موجودی باشد، به مشتری اطلاع داده می‌شود که تنها تعداد محدودی از کالا موجود است.(موجودی در انبار را به او نشان داده تا مجدد تعداد مورد نظر را وارد کند)</li>
      <li align="right">پس از تأیید تعداد و کالا، مجموع بهای خرید به مشتری نشان داده می‌شود.</li>
      <li align="right">از مشتری پرسیده می‌شود که آیا مایل به استفاده از اعتبار کیف پول خود برای پرداخت است یا خیر. در صورت تأیید، مبلغ اعتبار از کل خرید کسر می‌گردد.</li>
      <li align="right">مشتری می تواند در صورت داشتن کد تخفیف ان را وارد کرده و از ان استفاده کند. هر کد شامل یک درصد تخفیف و تاریخ انقضاست که پس از گذشت از این تاریخ امکان استفاده از ان میسر نیست</li>
      <li align="right">این کد ها به صورت یک فایل جیسون در اختیار شما قرار داده شده است.</li>
      <li align="right">پس از هر خرید 5 درصد مبلغ خریداری شده به عنوان اعتبار به کیف پول اون  اضافه خواهد شد.</li>
    </ul>
  </li>
  <li align="right">تاریخچه سفارشات:نمایش تمام سفارشات گذشته مشتری به همراه مبلغ پرداخت شده و تاریخ</li>
  <li align="right">تغییر رمز عبور:امکان تغییر رمز عبور برای تأمین امنیت بیشتر حساب کاربری.رمز عبور جدید باید شامل حداقل 8 کاراکتر باشد و ترکیبی از اعداد و حروف را دارا باشد و حداقل شامل یک کاراکتر بزرگ باشد</li>
 </ol>
</p>
<img src="https://i.imgur.com/dBaSKWF.gif" height="20" width="100%">



<img src="https://i.imgur.com/dBaSKWF.gif" height="20" width="100%">



<img src="https://i.imgur.com/dBaSKWF.gif" height="20" width="100%">




<img src="https://i.imgur.com/dBaSKWF.gif" height="20" width="100%">


<img src="https://i.imgur.com/dBaSKWF.gif" height="20" width="100%">

<br>
<p align="right" > Created with 🧡 by <a href="http://supun.traditionalme.life">Supun Nanayakkara</a></p>
