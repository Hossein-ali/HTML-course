# تگ های HTML :

## Basic Tags

| Syntax             | Description |
| -----------        | ----------- |
| `<!DOCTYPE html>`  |را مشخص میکند `html` نوع سند|
| `<html></html>`    |قرار میگیرد `body` و `head`در بین این تگ کد های برنامه نوشته میشود و همچنین دو تگ|
| `<head></head>`    |متا دیتاها قرار میگیرد `head`  در تگ |
| `<meta>`           |برای توضیحات بیشتر در مورد سایت|
| `<title></title>`  |عنوان سایت در صفحه وب|
| `<body></body>`    | تمام آن چیزی که در صفحه سایت میبینیم، داخل این تگ قرار میگیرد |

یک سند ساده `HTML` میتواند حاوی کد زیر باشد :
```html
<!DOCTYPE html>
<html dir="rtl">
  <head>
    <meta charset="UTF-8" />
    <title>Getting Started</title>
  </head>
  <body>
    <h1>سلام!</h1>
  </body>
</html>

 ```

---

## Text Tags

| Syntax             | Description |
| -----------        | ----------- |
| `<h1></h1>`        |برای نمایش یک تیتر بزرگ |
| `<p></p>`          |نمایش‌ دهنده‌ی یک پاراگراف در وب‌سایت|
| `<hr>`             | کشیدن یک خط افقی|
| `<br>`             |  ایجاد یک خط جدید |
| `<span></span>`    |یک تگ بی هویت که ما به آن هویت میدهیم|
| `<b></b>`          | `Bold`نمایش متن یا کلمه خاص بصورت |
| `<strong></strong>`| `b`مانند تگ |
| `<i></i>`          | `italic` نمایش متن یا کلمه بصورت |
| `<em></em>`        | `i` همانند تگ  |

مثال : 

```html
<h1> عنوان </h1> 
<hr>
<p>این یک <span>پاراگراف</span> می باشد.</p>
<br>
<b>یک متن درشت</b>
<i>یک متن مورب</i>

```
** 
توجه : عنوان‌ها در `HTML` با استفاده از تگ `h1 تا h6` براساس اهمیت و اندازه‌ی آن‌ها تعریف می‌شوند. به این ترتیب که تگ `h1` دارای بیش‌ترین اهمیت و بزرگ‌ترین اندازه و تگ `h6` دارای کم‌ترین اهمیت و کوچک‌ترین اندازه است.

---


## Time and date display Tag 


| Syntax              | Description |
| -----------         | ----------- |
| `<time></time>`     |برای درج تاریخ و زمان مورد نظر |
| `attribute datetime`|فرمت استاندارد از زمانی که متن به آن اشاره دارد|

مثال : 

```html
<p>
  Event will start <time datetime="2024-03-12T15:30">Tomorrow at 3:30pm</time>
</p>
```
**
توجه : برای استفاده از تگ `time ` باید درون تگ `p` قرار بگیرد 

---

## Quote display Tag


| Syntax              | Description |
| -----------                | ----------- |
| `<blockquote></blockquote>`|نمایش یک نقل قول که از خط جدید آغاز شود|
| `attribute cite`|مشخص کردن منبع دقیق نقل قول|
| `<q></q>`| `blockquote`همانند تگ|

مثال : 

```html

<p>Here's a quotation:</p>
<blockquote cite="https://www.huxley.net/bnw/four.html">
  <p>
    Words can be like X-rays, if you use them properly—they’ll go through
    anything. You read and you’re pierced.
  </p>
</blockquote>

<!-- ------------------------------------ -->

<p>
  According to Mozilla's website,
  <q cite="https://www.mozilla.org/en-US/about/history/details/">
    Firefox 1.0 was released in 2004 and became a big success.
  </q>
</p>


```
**
توجه : تفاوت تگ `q` با تگ `blockquote` در این است که تگ `p` درون تگ `blockquote` قرار میگیرد ولی تگ `q` درون تگ `p` قرار میگیرد

---

## Address and contact information display Tag


| Syntax              | Description |
| -----------                | ----------- |
| `<address></address>`|برای نمایش نشانی‌ مکان و اطلاعات تماس مربوط به آن صفحه یا وب‌سایت|

```html
<address>
  <p>
    Azadi<br />
    Tehran<br />
    Tehran<br />
    Iran
  </p>

  <p>Tel: 01234 567 890</p>

  <p>Email: me@quera.org</p>
</address>

```
**
توجه : این تگ هم به همانند تگ `blockqoute`، تگ `p`  درون تگ `address`قرار میگیرد


برای فهم بیشتر تگ های `bloukqoute, q` به این [تمرین](https://github.com/Hossein-ali/HTML-course/tree/master/quote) مراجعه بفرمایید.


برای فهم بیشتر تگ  `address` به این [تمرین](https://github.com/Hossein-ali/HTML-course/tree/master/simple-invitation) مراجعه بفرمایید.


---

## Links Tag
| Syntax              | Description |
| -----------         | ----------- |
| `<a></a>`           |... تگ لینک برای رفتن به دیگر صفحات سایت و |
| `attribute href`    |        مشخص کردن مقصد لینک|
| `attribute target="_blank"`  |     جدید `tab` باز شدن صفحه در |
| `attribute download="Logo"`|     لینک محتوای دانلود  |



مثال : 

```html
<a href="https://www.google.com">سایت گوگل</a>
```

آدرس نسبی یک سند HTML به عنوان مقصد :

فرض کنید که روی سیستم خود سندهای HTML زیر را طبق ساختار درختی زیر ایجاد کرده‌ایم:

```
.
└── MyProject
    ├── src
    │   ├── index.html
    │   ├── contact-us.html
    │   └── products
    │       ├── product1.html
    │       └── details
    │           └── product-detail.html
    └── anotherSite
        └── main.html

```
بعنوان مثال برای رفتن از سند `product-detail.htm`به سند `contant-us.html` :

```html
<a href="../../contact-us.html">صفحه تماس با ما</a>
```
توجه : برای برگشت از پوشه خود `..` استفاده میکنیم و برای اینکه در مثال بالا به سند `contant-us.html ` برویم از `/../..` استفاده کردیم .
چون دو پوشه باید برگردیم

---

از آن‌ جایی که این صفحه‌ طولانی است، بالای صفحه‌ لینک‌هایی ایجاد کرده‌ایم که بتوانیم با کلیک روی آن‌ها به بخش‌های مختلف همین صفحه پَرش کنیم. برای این کار ابتدا باید به المانی که می‌خواهیم به آن پَرش کنیم، attribute ای به نام `id` بدهیم، مانند زیر:

```html
<h2 id="introduction">Introduction</h2>
```
این attribute نمود ظاهری ندارد اما برای پیاده‌سازی این عملکرد به ما کمک می‌کند. حالا برای ایجاد لینکی که به این المان پَرش کند، مانند زیر عمل می‌کنیم:

```html
<a href="#introduction">Introduction</a>
```
برای فهم بیشتر تگ  `a` به این [تمرین](https://github.com/Hossein-ali/HTML-course/tree/master/invitation-link)  , و این [تمرین](https://github.com/Hossein-ali/HTML-course/tree/master/helpful-links) مراجعه بفرمایید.

---

## List Tag 

| Syntax              | Description |
| -----------         | ----------- |
| `<ol></ol>`           |  تگ لیست ترتیبی  |
| `<ul></ul>`           |  تگ لیست غیر ترتیبی  |
| `<dl></dl>`           |  تگ لیست توضیحی |
| `attribute type`    |        به لیست های ترتیبی برای **تغییر نشانگر** آن می توان اضافه کرد|
| `attribute start`    |        به لیست های ترتیبی برای **شروع نقطه** نشانگر آن می توان اضافه کرد|
| `attribute reversed`    |      ترتیب شماره‌دهی به آیتم‌ها را میتوان برعکس کرد   |


مثال : 
```html
<!-- لیست غیر ترتیبی -->

 <ul>
  <li>Apple</li>
  <li>Mango</li>
  <li>Orange</li>
  <li>Banana</li>
</ul>

<!-- لیست ترتیبی -->

<ol type="1" start="0">
  <li>Name</li>
  <li>Address</li>
  <li>Phone Number</li>
</ol> 

<!-- لیست توضیحی -->

<dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language</dd>
  <dt>CSS</dt>
  <dd>Cascading Style Sheets</dd>
</dl>

```

برای فهم بیشتر تگ های `List` به این [تمرین](https://github.com/Hossein-ali/HTML-course/tree/master/todo-list) مراجعه بفرمایید.

---

## Image & Video & Audio Tag

| Syntax              | Description |
| -----------         | ----------- |
| `<img></img>`           |  تگ نمایش عکس   |
| `<video></video>`           |   تگ نمایش ویدیو  |
| `<source></source>`           |   برای انتخاب  فرمت‌های مختلف یک ویدئو یا یک فایل صوتی|
| `<track kind="subtitles" src="subtitles_fa.vtt" srclang="fa" label="Farsi">`           |  می‌توان محتوای متنی (زیرنویس یا caption) برای ویدئوها نمایش داد  |
| `<audio></audio>`           |  تگ نمایش فایل صوتی |
| `attribute src=""`|مشخص کردن منبع عکس، ویدیو و فایل صوتی |
| `attribute type=""`|مشخص کردن فرمت ویدیو وفایل صوتی  |
| `attribute alt="تصویر لوگو "`|     مشخص کردن یک توضیح متنی برای عکس برای زمانی ک عکس به هردلیلی لود نمیشود |
| `attribute   width="500" height="300"`|مشخص کردن عرض و ارتفاع   |
| `attribute  loading = "lazy"`|بارگزاری نشدن عکس زمانی که در دید کاربر **نیست**  |
| `attribute controls`|کنترل‌کننده‌هایی برای کم و زیاد کردن صدای ویدئو یا فایل صوتی، عقب و جلو بردن ویدئو و ایست و ادامه‌|
| `attribute autoplay`|ویدئو یا فایل صوتی موردنظر را به محض بارگذاری نمایش داد|
| `attribute loop`|ویدئو یا فایل صوتی پس از اتمام به صورت خودکار دوباره از ابتدا پخش شود|
| `attribute poster`|تصویری که قبل از پخش شدن ویدئو روی پخش‌کننده‌ قرار می‌گیرد را تعیین کرد|
---
مثال :
```html
<!-- تگ عکس -->

 <img
  src=""
  alt="logo" 
  width="300"
  height="300"
  />

  <!-- تگ ویدیو  -->
   <video controls>
  <source src="" type="video/mp4">
  <source src="" type="video/webm">
  <source src="" type="video/ogg">
  
</video>

<!-- تگ فایل صوتی  -->
 <audio controls autoplay muted loop>
  <source src="" type="audio/mp3">
  مرورگر قادر به پخش فایل صوتی نیست.
</audio>
```

**
توجه : برای تگ های ویدیو و تصویر، `attribute width , height` وجود دارد ولی برای تگ فایل صوتی وجود ندارد

---
برای فهم بیشتر تگ های `img` به این [تمرین](https://github.com/Hossein-ali/HTML-course/tree/master/invitation-logo) مراجعه بفرمایید.

برای فهم بیشتر تگ های `video` به این [تمرین](https://github.com/Hossein-ali/HTML-course/tree/master/ad-video) مراجعه بفرمایید.

برای فهم بیشتر تگ های `audio` به این [تمرین](https://github.com/Hossein-ali/HTML-course/tree/master/spanish-learning) مراجعه بفرمایید.

---

## div Tag

| Syntax              | Description |
| -----------         | ----------- |
| `<div></div>`           |  `body`ایجاد یک تقسیم بندی در   |


مثال :

```html
<div>
    <span>دوره</span>
    <span> HTML و CSS</span>
</div>
<div>
    <span>درسنامه</span>
    <span> DIVISION</span>
</div>

```

تگ inline :تنها به اندازه‌ی عرض محتوای خود، فضا اشغال می‌کنند. برای مثال المان `span, a, b, img`

تگ block :در طرف مقابل المان‌های block قرار دارند. این گونه المان‌ها برای نمایش به خط جدید رفته و همچنین به صورت افقی تمام فضایی که از container خود در اختیار دارند را اشغال می‌کنند. ارتفاع المان‌های block به اندازه‌ی ارتفاع محتوای آن‌ها خواهد بود. برای مثال المان `p, div, ol`

برای فهم بیشتر تگ های `div` به این [تمرین](https://github.com/Hossein-ali/HTML-course/tree/master/initial-projext) مراجعه بفرمایید.

 ----

 ## Table Tag

 | Syntax              | Description |
| -----------          | ----------- |
| `<table></table>`    |  ایجاد یک جدول|
| `<tr></tr>`          |  ایجاد سطر  |
| `<th></th>`          |   داده‌های سطر اول جدول معمولاً مشخص‌کننده‌ی نوع داده‌‌های هر ستون هستند(مشخص کننده عنوان یک ستون)  |
| `<td></td>`           |  برای مشخص کردن داده‌های هر سطر از المان |
| `attribute border="1"`|برای نمایش حاشیه‌ی جداکننده میان خانه‌های جدول |
| `attribute colspan = "2"`|به کمک این ویژگی میتوان تعداد ستون های یک خانه را اشغال کرد|
| `attribute rowspan = "2"`|به کمک این ویژگی میتوان تعداد سطر های یک خانه را اشغال کرد|
| `<caption></caption>`           |  توضیح مختصری (عنوان) به بالای یک جدول اضافه کرد|

مثال : 

```html
<table border="1">
  <tr>
    <th>S.N</th>
    <th>Item</th>
    <th>Quantity</th>
  </tr>
  <tr>
    <td>1</td>
    <td>Apple</td>
    <td>2</td>
  </tr>
  <tr>
    <td>2</td>
    <td>Mango</td>
    <td>2</td>
  </tr>
  <tr>
    <td>3</td>
    <td>Orange</td>
    <td>1</td>
  </tr>
  <tr>
    <td colspan="2">Total</td>
    <td>5</td>
  </tr>
</table>

```
![pi](https://quera.org/qbox/download/fylOFXC4g5/Screenshot%202024-06-24%20120625.png)

### ساختاردهی به جدول :


 | Syntax              | Description |
| -----------          | ----------- |
| `<thead></thead>`    |  است که  اطلاعاتی مربوط به ستون‌های جدول دارد header سطر اول مربوط به|
| `<tbody></tbody>`          | سطر میانی جدول مربوط به داده‌های اصلی جدول است |
| `<tfoot></tfoot>`          |   سطر آخر جدول مربوط به جمع‌بندی داده‌های جدول است

مثال : 

```html
<table border="1" style="border-collapse: collapse">
  <thead>
    <tr>
      <th>S.N</th>
      <th>Item</th>
      <th>Quantity</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>Apple</td>
      <td>2</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Mango</td>
      <td>2</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Orange</td>
      <td>1</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td colspan="2">Total</td>
      <td>5</td>
    </tr>
  </tfoot>
</table>

```
برای فهم بیشتر تگ  `table` به این [تمرین](https://github.com/Hossein-ali/HTML-course/tree/master/invitation-table)  , و این [تمرین](https://github.com/Hossein-ali/HTML-course/tree/master/initial-projext2) مراجعه بفرمایید.


---

## Form Tag

 | Syntax              | Description |
| -----------          | ----------- |
| `<form></form>`    |  اولین قدم برای ایجاد یک وب‌فرم استفاده از این تگ است|
| `<input></input>`          | برای دریافت اطلاعات از کاربر المان |
| `<lable></lable>`          |  یک عنوان یا برچسب مشخص کنیم برای ورودی خود|
| `attribute type = ""`          | نوع ورودی دریافتی از کاربر را مشخص کرد|
| `attribute value = ""`          | مقدار پیش فرض ورودی|
| `attribute name = ""`          | اسم متغییر ورودی|

| `<textarea></textarea>`          | برای دریافت متن‌های طولانی‌|

 ### : attribute type مقادیر

1. `type = "text"`   : مشخص می‌کند که هر نوع متنی قابل قبول است

2. `type = "email"`   : باعث می‌شود تا به کاربر ایمیل‌هایی که قبلاً وارد 
کرده‌است پیشنهاد داده شود
3. `type = "password"` : متن نوشته شده در المان، مخفی نمایش داده می‌شود 

4. `type = "color"` :  این امکان را به کاربر می‌دهد تا رنگ مورد نظر خود را از 
 انتخاب کند ، Color Picker طریق
5. `type = "date"` : می‌توان از کاربر یک تاریخ مشخص دریافت کرد

6. `type = "file"` : برای فراهم کردن امکان انتخاب فایل برای آپلود

7. `type = "range"` : Range Picker ایجاد یک 
 
 ** توجه  : اگر چندتا range picker  داشتیم باید مقدار `attribute name `  آن یکسان باشد !

8. `type = "checkbox"` : برای انتخاب کردن یا انتخاب نکردن یک گزینه

9. `type = "radio"` : انتخاب میان چند گزینه 


---
| Syntax              | Description |
| -----------          | ----------- |
| `<select></select>`    |dropdown یکی از راه‌های اصلی ایجاد |

مثال : 

```html 

<label for="pets">Pets:</label>
<select id="pets">
  <option value="dog">Dog</option>
  <option value="cat">Cat</option>
</select>

```

![pi](https://quera.org/qbox/download/QjResf1q04/html-form-inputs-select-open.png)

---

| Syntax              | Description |
| -----------          | ----------- |
| `<fieldset></fieldset>`    |می‌توان چند المان ورودی که در یک گروه خاص قرار می‌گیرند را دسته بندی کرد|
| `<legend></legend>`    |عنوان یا برچسب جدول|

مثال : 

```html

<fieldset>
  <legend>Name</legend>
  <label for="firstname">First name:</label>
  <br />
  <input type="text" id="firstname" name="firstname">
  <br />
  <label for="lastname">Last name:</label>
  <br />
  <input type="text" id="lastname" name="lastname">
</fieldset>

```
![pi](https://quera.org/qbox/download/DJn08cny6o/html-form-inputs-legend.png)

---
| Syntax              | Description |
| -----------          | ----------- |
| `<datalist></datalist>`    |تنها به کاربر چند گزینه پیشنهاد بدیم اما کاربر بتواند ورودی دلخواه خود را نیز وارد کند|

مثال : 

```html

<label for="country-choice">Choose a country:</label>
<input list="country-options" id="country-choice" name="country-choice">
<datalist id="country-options">
  <option value="Australia"></option>
  <option value="Austria"></option>
  <option value="America"></option>
  <option value="Nepal"></option>
</datalist>

```
![pi](https://quera.org/qbox/download/rETbK7o6SF/html-form-inputs-datalist.png)

برای فهم بیشتر تگ  `form` به این [تمرین](https://github.com/Hossein-ali/HTML-course/tree/master/initial%D9%80project)  , و این [تمرین](https://github.com/Hossein-ali/HTML-course/tree/master/initial-project2) مراجعه بفرمایید.

---