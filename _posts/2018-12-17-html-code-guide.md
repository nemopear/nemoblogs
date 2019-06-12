---
layout: post
title: HTML Code Guide
date: 2018-12-17 03:56:54.000000000 +07:00
type: post
categories: [ html, coding ]
image: assets/images/html-css-book.jpg
permalink: "/2018/12/17/html-code-guide/"
comments: true
status: publish
published: true
---

### Syntax
* tag element เป็น lowercase เช่น `<html>` `<p>`
* attribute name เป็น lowercase
* ใช้ double-quote สำหรับ attribute value
* ใช้ double quote เวลาประกาศ attribute ใน HTML Element
* tag ที่ต้องการ closing tag ห้ามลืมปิด closing tag `</li>` or `</body>`
* กรณีที่เป็น void element หรือ Element ที่ไม่ต้องการ closing tag ก็ไม่ต้องเพิ่ม slash ได้แก่ `area`, `base`, `br`, `col`, `embed`, `hr`, `img`, `input`, `link`, `meta`, `param`, `source`, `track`, `wbr`

---
### HTML5 doctype

ต้องประกาศไว้ทุกๆหน้าของ HTML page เพื่อการให้เป็นมาตรฐานเดียวกันในการแสดงผลของแต่ละ Browser เท่าที่จะเป็นไปได้

---
### Language Attribute

ระบุ lang=”en-us” เพื่อช่วยในการออกเสียง สำเนียง สำหรับเครื่องมืออ่าน หรือแปลภาษา

---
### IE Compatibility mode

`<meta>` จะช่วยระบุเครื่องมือ render page ของ IE
{% highlight html %}
<meta> http-equiv="x-ua-compatible" content="ie=edge"
{% endhighlight %}

---

### Character encoding

ช่วยตรวจสอบการแสดงผลเนื้อหาได้อย่างรวดเร็ว จากการตรวจสอบจาก encoding โดยทั่วไป default จะตั้งค่าเป็น UTF-8
{% highlight html %}
<head>   
  <meta charset="UTF-8">
</head>
{% endhighlight %}

---

### Attribute order

การเขียน Attribute ใน Tag ควรเรียงจาม alphabet แต่ยกเว้น `class` ให้เอาไว้แรกสุด เพราะสามารถ reuse ได้ เพราะเป็นส่วนที่ developer ใช้บ่อยสุด ถ้าเป็นพวก data-* ควรรวมกลุ่มกันไว้ เพื่อให้อ่านง่ายๆ

มีข้อยกเว้นสำหรับ attribute `type` กรณีที่มี `type` ให้ประกาศ `type` ไว้อันดับแรกสุด เพราะ `type` มีผลต่อการเปลี่ยนแปลงพฤติกรรมของ Element

{% highlight html %}
<!-- Put "type" first because it changes the element's behavior. --> 
<button type="" class=""></button>
{% endhighlight %}

---

### Boolean attributes

Element ที่ต้องแสดง boolean attribute (`true` หรือ `false`) ไม่จำเป็นต้องมี attribute value

{% highlight html %}
<input type="text" disabled>
{% endhighlight %}

---

### Attribute overload

ถ้ามีการกำหนด attribute ใน Element นั้นเป็นจำนวนมาก ก็จะยากต่อการอ่าน ควรจัดการ Pattern ให้อ่านง่าย
* บรรทัดแรกเป็น element
* 1 attribute ต่อ 1 บรรทัด
* ไม่ต้อง indent attribute
* บรรทัดสุดท้ายเป็น closing tag

{% highlight html %}
<input  
type="text"  
class=""  
disabled  
id=""  
name=""  
placeholder=""  
readonly  
value="">
{% endhighlight %}

---

### HTML Convention
**การใช้ Class**
* Classไม่มีผลต่อ semantics.
* Class สามารถ reuse ได้ มีประโยชน์ต่อการทำเป็น module ได้
* Class เป็น case sensitive เราควรตั้งชื่อ class เป็น lowercase
* การเรียก CSS selector ถ้าใช้ Class จะเร็วกว่าการเรียกผ่าน Element

**การใช้ ID**
* ID ต้องเป็น Unique / 1 document. ไม่สามารถ reuse ได้
* ID ดีต่อการใช้ใน JS

**Reference**

* [https://manuals.gravitydept.com](https://manuals.gravitydept.com/code/html/style-guide)
* [http://codeguide.co](http://codeguide.co/#html)


**Credit Image**

* [Unsplash image](https://unsplash.com/@grakozy?utm_medium=referral&amp;utm_campaign=photographer-credit&amp;utm_content=creditBadge)

