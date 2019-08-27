---
layout: post
title:  "ทดสอบ Email Template โดยใช้ Putsmail"
type: post
categories: [ html, coding ]
image: assets/images/email-client.jpg
permalink: "/2019-08-27/email-test-with-putsmail/"
date: 2019-05-10 14:18:08.000000000 +07:00
comments: true
status: publish
published: true

---
เวลาเราสร้าง Email Template มาแล้ว เราก็อยากจะเช็คว่า Email Template ของเรา เป็นยังไงบ้าง ไปอยู่ใน Email Clients แต่ละเจ้า แสดงผลออกมายังไง Tool ที่เราจะมานำเสนอวันนี้ คือ [Putsmail](https://putsmail.com/)

Putsmail ช่วยส่ง Email ไปยัง email address ที่เราต้องการ ทำให้เราสามารถ Test design  และ debugging ได้ง่ายขึ้น

### วิธีการใช้ Putsmail 
1. เลือกเมนู [New Test](https://putsmail.com/tests/new) หรือ คลิกที่ปุ่ม [“Create a New Test Email”](https://putsmail.com/tests/new)
2. กรอกอีเมลผู้รับ (Recipients)
3. กรอกหัวข้อ Email (Subject Line)
4. Copy HTML ของ Email Template ที่เราต้องการเช็คมาไว้ใน Body(HTML)

<img src="../../assets/images/putsmail.png">

การส่งไปครั้งแรกจะมี Email ส่งไปยัง Email ผู้รับเพื่อให้ Confirm ก่อน
เมื่อ Confirm แล้ว Email ที่เราต้องการ Test จะถูกส่งตามมา

**Credit Image**

* [Unsplash image](https://unsplash.com/photos/3Mhgvrk4tjM)

