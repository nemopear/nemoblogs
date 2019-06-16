---
layout: post
title: CSS Box Model
date: 2018-11-07 06:52:02.000000000 +07:00
type: post
categories: [ html, coding ]
image: assets/images/box-model.jpg
permalink: "/2018/11/07/css-box-model/"
comments: true
status: publish
published: true
---

CSS box model เป็น box ที่คลุมทุกๆ element ของ HTML ไว้ การจะสร้าง Layout ที่ดี ให้กับเว็บไซต์ เราจำเป็นต้องเข้าใจถึง CSS box model
**CSS box model ประกอบด้วยส่วนต่างๆ ดังนี้**
1. **content area** : ส่วนที่แสดง text หรือ รูปภาพ
2. **padding** : เป็นช่องว่างที่อยู่ภายใน border ซึ่งคั่นระหว่าง **border** กับ **content** ถัดไป
3. **border** :  อยู่รอบ content area และ padding ถ้าสามารถเห็น border ได้ เราจะเห็นการแยกชัดเจนระหว่าง padding กับ margin
4. **margin** : เป็นช่องว่างที่อยู่ภายนอก border ซึ่งคั่นระหว่าง **border** กับ **element** ถัดไป

### ความแตกต่างระหว่าง content-box กับ border-box

![What is the difference between border-box and content-box in CSS?](/assets/images/contentbox-borderbox.png){:class="img-responsive"}

จากภาพตัวอย่างข้างบน จะเห็นว่าเรากำหนดค่า width: 300px; ไว้
การกำหนด width ของ `content-box` จะหมายถึงความกว้างของ `content area` อย่างเดียว ส่วน `border-box` จะหมายถึงความกว้างภายใน `border` (content area + padding + border)

**content-box**
<br>
width = content-area
<br>
300 = 300

**border-box**
<br>
width = content area + padding + border
<br>
300 = 260 + (15x2) + (5x2)<br>
300 = 260 + (padding ซ้ายและขวา) + (border ซ้ายและขวา)
<iframe height="594" style="width: 100%;" scrolling="no" title="Box Model" src="//codepen.io/nemopear/embed/KrdodP/?height=594&theme-id=light&default-tab=html,result" frameborder="no" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/nemopear/pen/KrdodP/'>Box Model</a> by nemopear
  (<a href='https://codepen.io/nemopear'>@nemopear</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>
<br>
**Image credit :**

1. <a href="https://stackoverflow.com/questions/44453391/what-is-the-difference-between-border-box-and-content-box-in-css">https://stackoverflow.com/questions/44453391/what-is-the-difference-between-border-box-and-content-box-in-css</a>
2. <a href="http://ictacademy.com.ng/css-box-model/">http://ictacademy.com.ng/css-box-model/</a>

