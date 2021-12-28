# bitkub-tbl
Cryptocurrency Trailing Buy Stop for BitKub exchange.
โปรแกรมช่วยซื้อเหรียญคริปโตอัตโนมัติบน BitKub Exchange โปรแกรมพัฒนาด้วย python และเรียกใช้งาน BitKub Official API (https://github.com/bitkub/bitkub-official-api-docs)

## How to use
โปรแกรมประกอบด้วย 3 ไฟล์
- cPandaBitKubTBL.exe  <-- Program TBL
- API.txt <-- ไฟล์สำหรับเก็บค่า KEY ส่วนตัวสำหรับการเข้าถึง Account ของเราใน BitKub
- BUY_XXX.txt <-- ไฟล์สำหรับตั้งค่าเหรียญต่างๆ ที่เราต้องการซื้อ

## สร้าง API & KEY บน BitKub

![image](https://user-images.githubusercontent.com/56244402/147461471-7f83da7a-84f6-42fb-bcb2-205f6e59edb2.png)

กดสร้าง API KEY & SECRET แล้วนำไปใส่ในไฟล์ API.txt

![image](https://user-images.githubusercontent.com/56244402/147462137-06d94cdb-046d-4312-bdbf-11fe4b3215e6.png)

![image](https://user-images.githubusercontent.com/56244402/147461646-150a486e-ad72-4a27-8945-9a5fb97bc2da.png)

** ห้ามส่ง API KEY & SECRET ให้ใครรู้เป็นอันขาด !!! 

## การตั้งค่าในไฟล์ BUY_XXX.txt (แทนที่ XXX ด้วยชื่อเหรียญที่เราต้องการ)

![image](https://user-images.githubusercontent.com/56244402/147552622-b332a9b5-b6ec-4ae0-804d-9397a77caef9.png)

`Symbol` - ชื่อคู่เหรียญกับเงินบาทกับชื่อเหรียญ ตัวอย่าง THB_GALA

`gridsize` - ระยะห่างจากราคาปัจจุบันของเหรียญนั้นๆ เช่น ราคา GALA ปัจจุบันอยู่ที่ 17 บ. แล้วเราอยากจะวาง Stoploss เริ่มต้นที่ 17.5 บ. ก็ให้ใส่ค่า gridsize=0.5 

`buyamount` - จำนวนเงิน (บาท) ที่ต้องการใช้ซื้อเหรียญ

## วิธีการใช้งาน

เข้า Command Prompt ไปที่ folder ที่เราเก็บโปรแกรมไว้ แล้วพิมพ์คำสั่ง

`cPandaBitKubTBL.exe -f BUY_GALA.txt`

(สามารถสร้างไฟล์ config คู่เงินหลายๆ ไฟล์ แล้วสั่งทำงานหลายจอได้)

![image](https://user-images.githubusercontent.com/56244402/147553141-150f8f0b-5a1a-406a-a8b7-54da25c872f4.png)

** วิธีหยุดการทำงานของโปรแกรมให้กด Ctrl + C

## Note
- ทดสอบดาวน์โหลดจาก GitHub มาเครื่องตัวเอง เจอ antivirus ฟ้องว่าเป็นไวรัสนะครับ สำหรับคนรู้จักผมขอไฟล์ทาง LINE ได้นะครับ ส่วนถ้าท่านใดผ่านมาเจอแล้วไม่แน่ใจก็ผ่านเลยนะครับ

![image](https://user-images.githubusercontent.com/56244402/147465738-c3c0d68f-d60b-4425-b051-bd8b07ec6eaa.png)


## Support
หากพบปัญหาหรือต้องการฟีเจอร์เพิ่มเติม สามารถโพสไว้ในหัวข้อ issue ได้เลยครับ 

ถ้าเห็นว่าโปรแกรมมีประโยชน์ สามารถช่วยกดติดตามเป็นกำลังใจช่องเกมของผมได้ที่ 

[![Youtube_Badge](https://img.shields.io/badge/Youtube-CrazypandaGaming-red)](https://www.youtube.com/channel/UC9PgjH7Bc0_P4tbc8c6K25Q)
[![Facebook Badge](https://img.shields.io/badge/Facebook-CrazypandaGaming-blue)](https://fb.com/crazypandagaming)

หรือช่วยสนับสนุนค่ากาแฟก็ยินดีนะครับ 

BTC : bc1qtczemkkmqdle9n838la3sk407jgzqx2ap03dtg

ETH : 0x08cb7F954aAC9710cc5D5cCd3DBaE86ab972A391

BNB (Smart Chain) : 0x5a60f4f993837F637a868Fb0A4789d6F861E5eCA
