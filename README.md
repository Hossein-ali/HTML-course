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


برای فهم بیشتر تگ های `bloukqoute , q ` به این [تمرین](https://github.com/Hossein-ali/HTML-course/tree/master/quote) مراجعه بفرمایید.


برای فهم بیشتر تگ های `address ` به این [تمرین](https://github.com/Hossein-ali/HTML-course/tree/master/simple-invitation) مراجعه بفرمایید.


---
