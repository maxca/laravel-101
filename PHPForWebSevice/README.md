# PHP For Web Service 1 Day
## ไคเอ็นต์ (Client part) 
+ Web service คืออะไร 
+ ทำความเข้าใจเกี่ยวกับ Rest full API 
+ การติดตั้ง Xamp เพื่อสร้าง ENV สำหรับการพัฒนา Project PHP 
+ การใช้งาน composer ร่วมกับ PHP Project 
+ การใช้งาน git ร่วมกับ source tree เพื่อควบคุม code 
+ รู้จักกับ https://packagist.org/ แหล่งรวบรวม package ของ PHP
+ การใช้งาน postman เพื่อทดสอบการทำงานของ Web Service.
+ สร้าง Mocking Server ด้วย postman เพื่อทดสอบการเชื่อมต่อ
+ รู้จักกับ Http standard response [1xx- 5xx] 
+ การจัดการ error ในรูปแบบต่าง ๆ Error handling 
+ การเชื่อมต่อกับ web service ด้วย Curl ของ php 
+ การเชื่อมต่อกับ web service ด้วย guzzle
    + การติดตั้ง guzzle ด้วย composer 
    + การใช้งาน guzzle ในรูแบบต่าง ๆ 
    + การส่งข้อมูลในรูปแบบ JSON 
    + การส่งข้อมูลในรูปแบบ Form Params
    + การแนบ headers ในรูปแบบต่าง ๆ 
+ การใช้งาน web service ที่มีระบบ authentication
    + Basic authentication 
    + JWT (JSON Web token)
+ ทดสอบเชื่อมต่อ public api ของ LINE 
    + line notify

## เซิฟเวอร์ (Server Part)
+ ทำความเข้าใจเกี่ยวกับ webservice ในส่วนของเซิฟเวอร์ 
+ การออกแบบ api response เพื่อการใช้งาน
+ เริ่มต้นการสร้าง Web service api (CURD)
    + ออกแบบโครงสร้างของ code เพื่อสร้างมาตรฐานเดียวกัน
    + ออกแบบฐานข้อมูลเพื่อใช้ในการจัดเก็บข้อมูลของ API
    + สร้างส่วนกลางเพื่อเชื่อมต่อกับฐานข้อมูล 
    + เขียน API เพื่อนำข้อมูลมาบันทึก (Create) 
    + เขียน API เพื่อนำข้อมูลมาแก้ไข (Update) 
    + เขียน API เพื่อนำข้อมูลมาลบ (Delete) 
    + เขียน API เพื่อนำข้อมูลมาใช้ในการสืบค้น (Search)
    + เขียน API เพื่อเรียกใช้ข้อมูลในรูปแบบ ID
 + การออกแบบระบบจัดการความปลอดภัยของ API 
    + สร้าง middleware ในการตรวจสอบการเข้าถึงในรุปแบบ Basic authentication
    + สร้าง middleware ในการตรวจสอบการเข้าถึงในรุปแบบ JWT 
 + การเขียน PHPunit เพื่อทดสอบการทำงานของ code
 + การสร้างเอกสาร (API DOC)อย่างรวดเร็วด้วย POSTMAN 
     + การ public document เพื่อให้เป็นสาธาระณะแบบออนไลน์ 
     
## สรุป 
+ การนำไปประยุกต์ใช้งานจริง
+ ถามตอบ

## เครื่องมือที่ใช้การอบรม Tools
+ xamp กรณีที่เครื่องไหนสามารถใช้ docker ได้จะสอนในรูปแบบ docker ไปพร้อมกัน
+ git sourcetree 
+ composer 
+ mysql + phpmyadmin
+ postman 
+ line account (Line notify alert) 
