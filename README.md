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
---

برای فهم بیشتر تگ های `img` به این [تمرین](https://github.com/Hossein-ali/HTML-course/tree/master/invitation-logo) مراجعه بفرمایید.

برای فهم بیشتر تگ های `video` به این [تمرین](https://github.com/Hossein-ali/HTML-course/tree/master/ad-video) مراجعه بفرمایید.

برای فهم بیشتر تگ های `audio` به این [تمرین](https://github.com/Hossein-ali/HTML-course/tree/master/spanish-learning) مراجعه بفرمایید.

---