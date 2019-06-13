---
layout: post
title: CSS Box Model
date: 2018-11-07 06:52:02.000000000 +07:00
type: post
categories: [ html, coding ]
image: assets/images/box-model.png
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


![CSS Box model](/assets/box-model.png)
{: .text-center}
<h3>ความแตกต่างระหว่าง content-box กับ border-box</h3>
<p><img class="aligncenter size-full wp-image-1704" src="{{ site.baseurl }}/assets/c7oir.png" alt="" width="744" height="409" /></p>
<p>จากภาพตัวอย่างข้างบน จะเห็นว่าเรากำหนดค่า width: 300px; ไว้</p>
<p>การกำหนด width ของ<strong> content-box</strong>  จะหมายถึงความกว้างของ <strong>content area</strong> อย่างเดียว ส่วน <strong>border-box</strong> จะหมายถึงความกว้างภายใน <strong>border (content area + padding + border)</strong></p>
<p><strong>content-box<br />
</strong>width = content-area<br />
300 = 300</p>
<p><strong>border-box</strong><br />
width = content area + padding + border<br />
300 = 260 + (15x2) + (5x2)<br />
300 = 260 + (padding ซ้ายและขวา) + (border ซ้ายและขวา)</p>
<p><a href="//codepen.io/nemopear/embed/KrdodP/?height=265&amp;theme-id=0&amp;default-tab=html,result">//codepen.io/nemopear/embed/KrdodP/?height=265&amp;theme-id=0&amp;default-tab=html,result</a></p>
<p><strong>Image credit : </strong></p>
<ol>
<li><em><a href="https://stackoverflow.com/questions/44453391/what-is-the-difference-between-border-box-and-content-box-in-css">https://stackoverflow.com/questions/44453391/what-is-the-difference-between-border-box-and-content-box-in-css</a></em></li>
<li><em><a href="http://ictacademy.com.ng/css-box-model/">http://ictacademy.com.ng/css-box-model/</a></em></li>
</ol>
<p>&nbsp;</p>
