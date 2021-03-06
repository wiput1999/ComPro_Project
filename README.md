![](/Resource/Banner.png)

# ![](/Resource/Home.png) Introduction
สวัสดีครับ วันนี้กลุ่ม POS System เราได้สร้างโปรแกรมที่นำไปใช้กับเครื่องคิดเงิน (หรือที่เรียกว่า ระบบ Point of Sale) อย่างเต็มรูปแบบ และสามารถทำงานได้จริง และรองรับการทำงานได้ในหลายระบบปฎิบัติการที่สร้างขื้นจากระบบ UNIX โดยการใช้เพียงภาษา C ในการเขียน 100%

---

# ![](/Resource/Help.png) How to use
สำหรับวิธีการใช้งาน ให้ไปที่โฟล์เดอร์หลัก แล้วพิมพ์ `make && make run` ผ่าน Command Line เพื่อเป็นการ สร้างไฟล์ Executable (.exe) หลังจากนั้น โปรแกรมจะเปิดโปรแกรมขื้นมาให้ทันทีอัตโนมัติ สามารถใช้ระบบได้เลยทันที

![](/Resource/First%20time%20Loadup.png)

---

# ![](/Resource/Settings.png) Configurations
โปรแกรมของเรา จะรันได้อย่างราบรื่นมากที่สุดโดยผ่านการใช้ระบบปฏิบัติการ MacOS (OSX) เวอร์ชั่นล่าสุด และระบบปฏิบัติการที่มาจาก UNIX (UNIX-based OS) เช่น Linux Ubuntu

เราแนะนำให้ผู้ใช้ปรับความกว้างหน้าจอ Terminal เป็นขนาดอย่างน้อย 140 x 40 pixel

เนื่องจากว่าระบบของเราไม่รองรับหน้าจอขนาดเล็กกว่าที่เราได้กำหนดไว้

![](/Resource/Startup%20Page.png)

---

# ![](/Resource/Fingerprint.png) Log In
ก่อนที่จะใช้งานระบบ POS ลูกค้าจำเป็นที่จะต้อง login เพื่อจะเข้าระบบเสียก่อน โดยการเข้าระบบจากหน้าแรก (หน้าปรับขนาดหน้าจอ)​
1. ให้กด 'Y' แล้วกด ENTER
2. พิมพ์ username (หรือใช้ scanner เช่นตัวยิงบาร์โค้ด) เข้าไปที่ระบบ
3. พิมพ์ password ของผู้ใช้งาน (user) นั้น
4. ระบบจะเช็คหาถึงความถูกต้องของ username / password และนำผู้ใช้ไปที่หน้่าหลัก

![](/Resource/Login%20Interface.gif)

ในการใช้ demo นี้ คุณสามารถใช้

`username : admin`

`password : admin`

เพื่อเข้าระบบได้

---

# ![](/Resource/Dashboard.png) Feature Dashboard
สำหรับการใช้งานระบบ POS ก็จะมีระบบย่อยๆ ต่างๆ เพื่อช่วยในการขาย เช่น

![](/Resource/First%20Page.png)

|Inventory|Sales|Forecast|Personnel|Category|Promotion|Settings|
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
|เช็คสินค้าคงคลัง|เช็คถึงยอดขาย|เช็คถึงยอดขายในอนาคต|เช็คผู้ใช้งานอื่น|เช็คประเภทของสินค้า| เปลี่ยนโปรโมชั่นสำหรับลูกค้า|แก้ไขข้อมูลพื้นฐานของร้านค้า|

โดยทุกระบบที่ได้เกล่ามานั้น ผู้ใช้งานที่เป็น เจ้าของร้าน (ผู้ใช้งานระดับ admin) **สามารถเข้าไปปรับแก้ได้ และ สามารถเปลี่ยน/เพื่ม/ลด ได้ทั้งหมด**

---

# ![](/Resource/Help.png) Common Shortcut Keys
|Q|V|B|ENTER|1 - 9|
|-|-|-|-|-|
|**Quit**<br/>Sign Out และปิดโปรแกรม|**Void**<br/>ยกเลิกการทำการ <br/> (เฉพาะในหน้า POS)|**Back** <br/> กลับไปหน้าที่แล้ว|**Continue** / **Skip** <br/> ทำงานต่อไป หรือ ให้ใช้ค่าเรื่มต้น <br/>  (แตกต่างกันในแต่ละหน้าจอ)|**Selection** <br/> ตัวเลือกในหน้าจอ

---

# ![](/Resource/Help.png) How to use POS Sales System
![](/Resource/POS%20Landing%20Page.png)

|Step 1|Step 2|Step 3|Step 4|
|:-|:-|:-|:-|
|กรอก รหัสบัตรสมาชิก (หากไม่มี สามารถกด Skip ขั้นตอนนี้ได้)|สแกนสินค้าที่ต้องการจ่าย <br/>(หากสินค้าที่สแกน ไม่ได้อยู่ในระบบ หรือของคงคลังหมด ระบบจะแจ้งว่าสินค้านั้นไม่สามารถจ่ายได้)|หากลูกค้าอยากใช้คะแนนเป็นส่วนลด หรือใช้ Voucher เงินสด ก็สามารถสแกนเข้าไปได้|ยอดการใช้จ่ายครั้งนี้ และ ยอดคะแนนสะสมของลูกค้า จะถูกแสดงในขั้นตอนนี้|

---

# ![](/Resource/Help.png) How to use Inventory Dashboard
![](/Resource/Inventory%20Landing%20Page.png)

|พิมพ์|เพื่อ|วิธีการใช้งาน|
|:-:|:---|----------|
|1|เช็คสินค้าคงคลัง|สามารถดูฐานข้อมูลได้ทันที <br/> หากต้องการเปลี่ยนหน้าสามารถพิมพ์เลขหน้าที่อยากจะไปได้ในทันที|
|2|เพื่มรายการ|กรอกรายละเอียดของสินค้า <br/> เช่นชื่อสินค้า รหัสบาร์โค้ด รายได้ที่จะได้รับ ราคา และปริมาณสินค้าคงคลัง โดยหลังจากเพื่มลงในระบบแล้ว ข้อมูลนี้จะเข้าไปอยู่ในฐานข้อมูลและสามารถใช้งานได้ทันที|
|3|เปลี่ยนข้อมูลในฐานข้อมูล|เปลี่ยนข้อมูลโดยการกรอกใหม่ทั้งหมด <br/> หากไม่ต้องการเปลี่ยน สามารถใช้ข้อมูลเก่าได้|
|4|ลบสินค้าในฐานข้อมูล|ลบข้อมูลในฐานข้อมูล <br/> โดยการพิมพ์รหัสสินค้า และกดยืนยัน หากยืนยันแล้ว ระบบจะลบข้อมูลของสินค้านั้นออก และไม่สามารถกู้กลับคืนได้|
|5|เช็คประเภทสินค้่า|สามารถดูฐานข้อมูลได้ทันที <br/>  หากต้องการเปลี่ยนหน้าสามารถพิมพ์เลขหน้าที่อยากจะไปได้ในทันที|
|6|เพื่มประเภทสืนค้า|เพื่มชื่อประเภทสินค้่าโดยการพิมพ์ชื่อประเภทที่เราต้องการ <br/> (หากมีชื่อนั้นอยู่แล้ว จะไม่สามารถตั้งซ้ำได้) <br/> และระบบจะสร้าง ไอดี เพื่อนำไปติดกับสินค้าได้|
|7|เปลี่ยนชื่อของประเภทสืนค้า|เปลี่ยนชื่อประเภทสินค้าโดยการพิมพ์ชื่อประเภทเก่าที่ต้องการเปลี่ยน และพิมพ์ชื่อใหม่เข้าไป ระบบจะเปลี่ยนชื่อในทันที (ไอดีจะคงเหมือนเดิม ดังนั้นระบบจะยังสามารถทำงานต่อได้อย่างปกติ)|

### Inventory Database Interface
![](/Resource/Inventory%20List.png)

### Category Database Interface
![](/Resource/Category%20List.png)

### Reporting Interface
![](/Resource/Report%20List.png)

---

# ![](/Resource/Help.png) How to use Settings Dashboard
![](/Resource/Settings%20Landing%20Page.png)

|พิมพ์|เพื่อ|วิธีการใช้งาน|
|:-:|---|----------|
|1|เปลี่ยนพาสเวิร์ด|สามารถเปลี่ยนรหัสเพื่อเข้าระบบของตนเองได้ <br/> โดยการกรอกรหัสเก่า แล้วจึงสามารถเปลี่ยนรหัสใหม่ได้ โดยต้องพิมพ์ยืนยันอีกครั้งหนึ่ง <br/> (หากพิมพ์ยืนยันผิด จะต้องเข้าไปทำการแก้ใหม่อีกครั้งตั้งแต่แรก)|
|2|เปลี่ยนชื่อหน้าร้าน|ชื่อร้านจะปรากฎในหน้าแรก และ หน้าการชำระเงิน โดยสามารถแก้ได้โดยการพิมพ์ชื่อใหม่เข้าไปในระบบ|
|3|เปลี่ยนที่อยู่ร้าน|ที่อยู่ร้านจะปรากฎในหน้าแรก และ หน้าการชำระเงิน โดยสามารถแก้ได้โดยการพิมพ์ชื่อใหม่เข้าไปในระบบ|
|4|เปลี่ยนค่าคะแนนที่จะได้รับจากการใช้จ่าย|โดยที่ การใช้จ่ายทุกๆ x บาท จะได้ 1 คะแนน <br/> โดยเจ้าของร้านสามารถแก้ไขค่า x ได้ และจะเรื่มใช้งานด้วยเรทใหม่กับการทำรายการหลังจากการเปลี่ยนเท่านั้น (ไม่แก้ไขย้อนหลัง)|
|5|เปลี่ยนค่าคะแนนเป็นส่วนสดเงินสด|โดยที่ การใช้ x คะแนน สามารถแลกเป็นส่วนลดได้ 1 บาท <br/> โดยเจ้าของร้านสามารถแก้ไขค่า x ได้ และจะเรื่มใช้งานด้วยเรทใหม่กับการทำรายการหลังจากการเปลี่ยนเท่านั้น (ไม่แก้ไขย้อนหลัง)|

### Price to Point Interface
![](/Resource/Point%20to%20Price%20List.png)

### Terminate Interface
![](/Resource/Terminate.png)
---

# ![](/Resource/Help.png) How to use Forecast Dashboard
![](/Resource/Forecast%20Landing%20Page.png)

|พิมพ์|เพื่อ|
|:-:|:--:|
|1|ดูการคาดเดารายวัน (ตามประเภทสินค้า)|
|2|ดูการคาดเดารายเดือน (ตามประเภทสินค้า)|

สำหรับวิธีการคาดคะเนนั้น ทางเราใช้ Exponential Smoothing ในการคาดเดา

Exponential Smoothing เป็นรูปแบบหนึ่งของการพยากรณ์ท่ีให้ความสําคัญกับข้อมูลเก่าทุกค่า โดยให้ความสําคัญแก่ค่าท่ีใกล้ปัจจุบันมากท่ีสุด ลดหลั่นลงไปจนถึงค่าที่ 1 และถ่วงน้ําหนักข้อมูล โดยใช้สัมประสิทธิ์การปรับเรียบ (alpha)

![](/Resource/Exponential%20Smoothing.png)

Sum of squared errors (SSE) คือ การหาค่าความคลาดเคลื่อนของข้อมูลที่ได้จากการทำนาย กับข้อมูลที่เกิดขึ้นจริง

![](/Resource/Sum%20of%20Square%20Error.png)

โปรแกรม Point of Sales (POS) Systems สามารถพยากรณ์ยอดขายให้ผู้ใช้ระบบ สามารถดูการพยากรณ์ยอดขายของวันถัดไป และเดือนถัดไปได้ โดยใช้หลักการของ Exponential Smoothing ร่วมกับค่า Sum of squared errors (SSE)

จากหลักการพยากรณ์ของ Exponential Smoothing จะต้องมีการเลือกค่าสัมประสิทธิ์การปรับเรียบ
(alpha) ที่เหมาะสม ซึ่งโปรแกรม POS จะทำการเลือกค่า  ที่เหมาะสมจากการคำนวนค่า Sum of squared errors โดยจะเลือกค่า alpha ที่มีค่า Sum of squared errors ที่น้อยที่สุด


### Daily Forecast Interface
![](/Resource/Forecast%20List.png)

---

# ![](/Resource/Person.png) Team Members
|  |ชื่อ|นามสกุล|GitHub Username|รหัสนักศึกษา|
|:-:|--|------|---------------|---------|
|![https://www.facebook.com/son9912](/Resource/sagelga.png)|Kunanon|Srisuntiroj|[@sagelga](https://github.com/sagelga)|59070022|
|![www.facebook.com/hideokyjima](/Resource/skydddoogg.png)|Thanawat|Laodkaew|[@skydddoogg](https://github.com/skydddoogg)|59070071|
|![https://www.facebook.com/noppanut](/Resource/noppanut15.png)|Noppanut|Ploywong|[@noppanut15](https://github.com/noppanut15)|59070082|
|![https://www.facebook.com/7eay.mask](/Resource/59070156.png)|Vasanchai|Prakobkij|[@59070156](https://github.com/@59070156)|59070156|
|![https://www.facebook.com/momay.weerakorn](/Resource/fablemay.png)|Weerakorn|Pongpum|[@fablemay](https://github.com/@fablemay)|59070163|

# ![](/Resource/Supervisor.png) Assistant Teacher
|ผศ. ดร. กิติ์สุชาติ พสุภา|ผศ. ดร. ปานวิทย์ ธุวะนุติ|
|:-:|:-:|
|![](/Resource/Aj.%20Oong.png)|![](/Resource/Aj.%20Panwit.png)|

รายงานนี้เป็นส่วนหนึ่งของวิชา Computer Programming (รหัส 06016206)

คณะเทคโนโลยีสารสนเทศ สถาบันเทคโนโลยีพระจอมเกล้าเจ้าคุณทหารลาดกระบัง

---

# ![](/Resource/Line%20Chart.png) Status Check
|![](/Resource/TravisCI%20Mascot.png) <br/> Travis-CI|![](/Resource/TravisCI%20Mascot.png) <br/> Travis-CI|
|:-:|:-:|
|Master <br/> [![Build Status](https://travis-ci.org/sagelga/ComPro_Project.svg?branch=master)](https://travis-ci.org/sagelga/ComPro_Project)|Development <br/> [![Build Status](https://travis-ci.org/sagelga/ComPro_Project.svg?branch=development)](https://travis-ci.org/sagelga/ComPro_Project)|

These status checks will check on every `git commit`

---

# ![](/Resource/Line%20Chart.png) Repository Statistics
Over 35.1 MB (and growing) are used to complete this projects.

|Classifiers|Lines|Words|Letters|
|---------|-----|-----|-------|
|**All programming files** <br/> (.c and .h)|6,542|28,745|283,862|
|**All .c files**|5,971|25,539|255,361|
|**All additional files** <br/> (MAKEFILE and .md)|287|734|19,972|
|**All database file**<br/> (including backup)|328|2,704|20,006|

### as a individual files
|File Name|Lines|Words|Letters|
|---------|-----|-----|-------|
|authenticate.c|245|885|8,747|
|category.c|252|1,218|11,857|
|customer.c|622|2,776|27,386|
|decorate.c|190|755|9,315|
|inventory.c|771|3,344|34,779|
|main.c|148|483|5,000|
|main.h|571|3,206|28,501|
|personnel.c|718|3,147|32,314|
|pos.c|412|1,873|18,715|
|promotion.c|521|2,183|21,772|
|purchase.c|35|179|1,707|
|report.c|825|3,784|36,379|
|settings.c|760|2,895|30,100|
|support.c|139|586|4,255|
|systemcall.c|292|1,246|11,171|
|transaction.c|35|179|1,815|
|.gitignore|4|2|24|
|.travis.yml|2|4|25|
|README.md|227|583|18,509|
|Database/Backup/category.db|16|38|193|
|Database/Backup/customer.db|3|21|149|
|Database/Backup/inventory.db|44|378|2,774|
|Database/Backup/personnel.db|3|21|198|
|Database/Backup/promotion.db|4|12|128|
|Database/Backup/purchase.db|6|42|394|
|Database/Backup/setting.db|1|10|76|
|Database/Backup/transaction.db|29|294|2,086|
|Database/category.db|16|38|193|
|Database/inventory.db|48|418|3,029|
|Database/personnel.db|6|42|382|
|Database/promotion.db|16|48|503|
|Database/purchase.db|20|138|1,241|
|Database/setting.db|1|10|76|
|Database/transaction.db|112|1,175|8,431|

Calculated using git commands `git ls-files | xargs wc`
