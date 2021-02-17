# PHP command
### ทดสอบ version php
`` php --version``
### ทดสอบ composer ติดตั้งเรียบร้อยหรือไม่ ถ้าไม่มีอะไรผิดพลาดจะไม่แสดง error
# Compser command
`` composer``
### clear cache ของ composer ที่เครื่องตัวเอง
`` coposer clear``
### reload autoload file class ที่เครื่องตัวเองใช้ในกรณี  laravel หาไฟล์ไม่เจอต้อง map path และที่อยู่ของไฟล์ใหม่ 
`` composer dump``
### สร้างโปรเจ็ค laravel ด้วย composer 
`` composer crete-project laravel/laravel  folder_name --prefer-dist``
### ติดตั้ง package ของ php ผ่าน composer 
`` composer require composer require kittinan/php-line-notify``
### ค้นหา package ของ php ผ่าน composer 
`` composer search facebook`` 

# Artisan command
### สร้าง controller class ด้วย artisan
`` php artisan make:controller ControlerName``

### สร้าง reqeust class ด้วย artisan  [ทำเพื่อสร้าง class validation]
`` php artisan make:request RequestName``
### สร้าง middleware class ด้วย artisan 
`` php artisan make:middleware MiddlewareName``

### สร้าง model class ด้วย artisan [class สำหรับติดต่อกับฐานข้อมูล]
`` php artisan make:modle ModelName``

### ทดสอบ route ใน laravel ว่ามี route หรือ url อะไรบ้างที่ใช้งานได้ และเป็นการเช็คด้วยว่า code ที่เราเขียนถูกต้องหรือไม่ 
`` php artisan route:list``
### สร้าง migration file ที่ต้องการ create table ด้วย artisan 
`` php artisan make:migration crete_table_something --create``
### สร้าง migration file ที่ต้องการ alter column ใน table (เพิ่มคอลัมในตาราง)
`` php artisan make:migration add_column_some_column --table=table_name``

### run migration file เพื่อให้สร้างตาราง เพิ่มตาราง
`` php artisan migrate`` 
### rollback migration 
`` php artisan migrate:rollback``
### สร้าง unit test file ด้วย artisan 
`` php artisan make:test TestCaseName``
### run unittest ด้วย artisan 
`` php artisan test``
### สำคัญ ! รันเซิฟเวอร์ด้วย artisan
`` php artisan serve``

### แสดงคำสั่งทั้งหมดของ artisan 
`` php artisan ``

# heroku 
### ทดสอบ heroku ติดตั้งเรียบร้อยหรือไม่ ถ้าไม่มีอะไรผิดพลาดจะไม่ขึ้น errors
`` heroku``
### login เข้าสู่ระบบ heroku (ให้กดคีย์บอร์ดอะไรก็ได้)
`` heroku login``
### สร้าง project ของ heroku  [project-name-some] แล้วแต่จะตั้ง
`` heroku create project-name-some``
### ดู logs error จาก heroku 
`` heroku logs --tail`` 
### set config ของ heroku เพื่อเอาไปใช้ใน app config ที่ set จะกลายเป็นตัวแปร global 
`` heroku set:config APP_URL=https://www`` 
### เปิด app ของตัวเองที่สร้างขึ้นบน heroku 
`` heroku open``
### run คำสั่งบางอย่างบน heroku  เช่น migrate artisan
`` heroku run php artisan:migrate`` 

# Git command
### เพิ่มไฟล์ที่แก้ไขเข้าไปใน git 
`` git add .``  หรือ
`` git add -A``
### commit file ที่เพิ่มเข้าไปจากคำสั่ง add ข้างบน
`` git commit -m "message ที่แก้ไข" ``
### สร้าง brach main ของ git ใน project 
`` git check -B main``
### ตรวจสอบสถานะของไฟล์ที่แก้ไขใน repository ของ git (repositroy คือชื่อที่ใช้เรียกที่เก็บไฟล์ source code project) ถ้ามีอะไรแก้ไขมันจะขึ้นสีแดง ๆ แต่ถ้าไม่มีอะไรจะบอก nothing
`` git status`` 
### push code ขึ้นไปบน server เพื่อ deploy heroku ถ้าไม่มีอะไรผิดพลาดจะขึ้น success
`` git push heroku main``
### ไฟล์ .gitignore คือ config ที่จะบอกว่าไม่ให้ git สนใจไฟล์ไหนหรือ floder อะไร มันจะไม่โดย push ขึ้นไปบนเซิฟเราจะแก้ไขยังไงก็แล้วแต่จะถูกเพิกเฉยจาก  git

# Node command
### ทดสอบ node ติดตั้งเรียบร้อยหรือไม่ 
`` node --version``
### ติดตั้ง package จาก package.json
`` npm install`` 
### รัน node ในเครื่องตัวเอง
`` npm start``
### รัน node js ใน mode watch เพื่อเช็คไฟล์ที่มีการแก้ไขและ reload auto
`` npm run watch`` 

# Bash command
# bash พื้นฐาน power shell, commandline cli , termimal
### อ่านไฟล์
`` cat filename.txt``
`` cat .env`` 
### เขียนไฟล์ผ่าน bash 
`` echo "web: vendor/bin/heroku-php-apache2 public/" > Procfile``
### tail log เพื่อดู log ข้อมูล
`` tail -f /path/log/file.log`` 
### ping server
`` ping http://localhost:8080``
### curl เรียกใช้ข้อมูลจากเซิฟเวอร์
`` curl http://localhot:8080`` 
### ตรวจสอบหมายเลข ip address ของเครื่อง 
`` ifconfig`` (osx) ``ipconfig`` (windows)
### ตรวจสอบเส้นทาง network ที่วิ่งออกจากเครื่องไปหาเซิฟเวอร์
`` traceroute 8.8.8.8`` (osx) 
`` traceroute google.com`` (osx)
`` tracert 8.8.8.8`` (windows)
`` tracert google.com`` (windows)
### ตรวจสอบว่า server เปิด port อะไรไว้บ้าง
``nmap -A -v google.com``

# Osx mode
### ติดตั้งโปรแกรม brew เพื่อมาใช้จัดการโปรแกรมอีกที
`` /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`` 
### ติดตั้ง php version 7.4 ผ่าน brew 
`` brew install php@7.4`` 
### ติดตั้ง compose ผ่าน brew
`` brew install composer``


### พื้นฐานเรื่อง server 
- ปรกติแล้วโปรแกรมที่จะนำมาสร้างเซิฟเวอร์มีหลายประเภทแต่ที่จะกล่าวถึงคือ web server เช่นของ google, youtube facebook เขาเรียกว่า web server มันมีหน้าที่เปิดให้บริการข้อมูลแก่เครื่องลูกข่าย(client) เมื่อ client เรียกเข้าไปหา (request) เครื่องเซิฟเวอร์จะส่งข้อมูลกลับมา ส่วนใหญ่จะส่งออกมาในลักษณะภาษา html, file (css,js,image),json (javascript object notation) xml อื่น ๆ ซึ่งพวกนี้จะมีโปรแกรมที่ใช้ในการสร้างเซิฟเวอร์เช่น apache, nginx , tomcat ที่นิยมก็มีประมาณนี้ 

### พื้นฐานเรื่อง php 
- php เป็นภาษา script language คล้ายกับ javascript เคยมีคนตั้งคำถามว่า php คือภาษาโปรแกรมด้วยหรือ ?​ เป็น opensource ถูกพัฒนามาจาก c, java และ purl 
- ลักษะของภาษาโปรแกรมมีสองแบบคือ interpreter และ Compiler
    + interpreter คือแปลภาษาทุกครั้งที่มีคนเรียกสคริปต์ 
    + Compiler ต้องนำไปประมวลผลใหม่
- script language คือภาษาที่ไม่ต้อง Compiler ใหม่เราจะรู้ error ก็ต่อเมื่่อเรารันโปรแกรม
- ตัวอย่าง
``` php 
<?php
    
    // ตัวแปรจะขึนต้นด้วย $ เช่น ตัวอักษรจะถูกครอบด้วย "" ฟันหนู !
    // และปิดคำสั่งด้วย ; semicolon อันนี้สำคัญ
    $name = "samark";
    // echo หรือ print , printf คือการแสดงข้อมูลเช่น 
    echo $name;
    echo "samark";
    // number
    echo 1112;
    // boolean 
    echo true;
    // ตัวอย่าง array 
    $arrayData = []; 
    // หรือ
    $arrayData = array();
    // การใส่ข้อมูลลงใน array (กรณีอาเรย์หนึ่งมิติ)
    $arrayData["key"] = "value";
    // การเรียกใช้ข่้อมูล array 
    echo $$arrayData["key"];
    // if condition 
    if($i == true) {
        // process
    }else {
        // process
    }
    // switch case 
    switch($name) {
        case "max" :
            return true;
            break;
        default:
            return "xxx";
            break;
    }
    // for loop
    for($i=0;$i <20; $i++ ) {
        echo $i
    }
    // foreach ใช้การณีที่เป็น object หรือ array
    foreach($arrayData as $key => $value) {
        // ตัวอย่างการต่อ string (ข้อความ)
        echo $key ." - ". $value;
    }
    // ยัง function สำเร็จรูปอื่น ๆ  อีกมากมายเช่นการ เรียกไปหา server เรียกข้อมูล ตัดข้อความ จัดการวันที่ น่าจะครบทุกอย่างที่เราจะต้องการนำมาเขียนโปรแกรม 
    // เข้าไปดูเพิ่มเติมได้ที่ https://www.php.net/manual/en/funcref.php

    // ตัวอย่าง class 
    class SimplePhp {
        // ตัวอย่าง attribute public
        public $version = "7.4";
        // ตัวอย่าง attribute private 
        private $baseline = "5.6";
        // ตัวอย่าง attribute protected 
        protected $subVersion = "7.4.4.x";
        // construct 
        // function นี้จะถูกทำงานเสมอเมื่อ class ถูก load
        public function __construct($version) {
            // ตัวอย่างการ assigned value to attribute
            $this->version = $version;
        }
        // ตัวอย่างการ return ค่าใน function 
        public function cal(int $x,int $y) {
            return $x**$y;
        }
        // ตัวอย่างการเรียกใช้ attriube value ใน funtion 
        public function displayVersion() {
            echo $this->version;
        }
    }
    //ตัวอย่างการเขียนใช้ class และการส่งค่าผ่าน __construct method 
    // __construct มีอีกชื่อว่า magic method 
    // ถ้าขึ้นต้นด้วย __ สองมักจะเป็น magic method ของ php แต่ต้องดูคู่กับ เอกสารด้วย 
    $simplePhp = new SimplePhp("8.0.x");
    
    // ตัวอย่างเรียกใช้ function จาก object simple php 
    // ส่งค่า 5 และ 40 เข้าไปใน funtion cal
    // function cal คืค่าที่คำนวณได้กลับมา
    // echo แสดงผลลัพธ์ที่ได้ 
    echo $simplePhp->cal(5,40);

    // ตัวอย่างเรียกใช้ function displayVersion
    // ต้องเป็น public function เท่านั้นถึงจะเรียกจากข้างนอกได้
    // ตามหลักการ OOP ที่เราเรียกันมา
    $simplePhp->displayVersion();


    // namespace คือที่อยู่ของไฟล์ไม่มีอะไรมากแค่ต้องตั้งชื่อ namespace ให้ต้องกับ folder ที่ไฟล์มันอยู่แค่นั้นเอง
    namespace App\Http\Controller;
    // ลักษณะนี้จะบอกว่าไฟล์นี้อยู่ใน folder app\http\controller นะ 
    // ทำไมถึงเป็นตัวเล็ก เพราะ laravel มันทำ class mapping แล้ว convert จาก ตัวใหญ่ให้เป็นตัวเล็ก คือมันทำการ mapping ต้นทางกับปลายทางให้แล้วผ่าน composer autoload นั้นเอง 
    

?>
```