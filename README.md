# หาเพื่อนร่วมทีม Opendream 2022.01

[โอเพ่นดรีม][1] กำลังหา developer มาเป็นเพื่อนร่วมทีม โจทย์ทดสอบนี้หวังว่าจะทำให้เรารู้จักฝีมือกันมากขึ้น

# ลักษณะโจทย์

โจทย์จะมีทั้งหมด 3 ข้อ ดังนี้
## 01 - FizzBuzz

เขียนโปรแกรมที่รับ `input` เป็นชุดตัวเลข `1` ถึง `100` และแสดง `output` ตามเงื่อนไขดังนี้
- ถ้า `input` หารด้วย 3 ลงตัว แสดง `output` เป็น `Fizz`
- ถ้า `input` หารด้วย 5 ลงตัว แสดง `output` เป็น `Buzz`
- ถ้า `input` หารด้วย 3 และ 5 ลงตัว แสดง `output` เป็น `FizzBuzz`
- ถ้า `input` ไม่อยู่ในเงื่อนไขข้างต้น แสดง `output` เป็น `input`

## 02 - เรียงลำดับ string ภาษาไทย

เขียน function ให้เรียงลำดับอักขระตามลำดับของอักขระไทยตามมาตรฐาน [Unicode][4] โดย มีเงื่อนไขดังนี้

![Thai Unicode Order](/images/thai-unicode-order.png "Thai Unicode Order")

- string ที่ขึ้นต้นด้วยพยัญชนะ ให้เรียงตามลำดับพยัญชนะ
- string ที่ขึ้นต้นสระ ให้เรียงตามพยัญชนะแรกหลังสระนั้น เช่น [`ช้าง` , `เชียงใหม่`, `ช่าง`] เรียงเป็น [`ช่าง`, `ช้าง`, `เชียงใหม่`]
- string ที่ขึ้นตันด้วยอักษรนำ `ห` `อ` ให้เรียงตาม อักษรนำ เช่น [`อย่า`, `อ้าง`, `อยาก`] เรียงเป็น [`อย่า`, `อยาก`, `อ้าง`]
- string ที่ขึ้นต้นด้วยสระและอักษรนำ `ห` `อ` ให้เรียงตาม พยัญชนะและอักษรนำ เช่น [`หญิง`, `ยักษ์`, `ใหญ่`] เรียงเป็น [`ยักษ์`, `หญิง` , `ใหญ่`]

### ตัวอย่างที่ 1

```
input = ["ไก่", "กา", "ขา", "แก", "แขวน", "เกีย"]
output = ["กา", "เกีย", "แก", "ไก่",  "ขา", "แขวน"]
```

### ตัวอย่างที่ 2

```
input = ["ขอ,"ให้","เจริญ","นะ","จ๊ะ","หนุ่ม","สาว","ทั้ง","หลาย"]
output = ["ขอ,"จ๊ะ","เจริญ","ทั้ง","นะ","สาว","หนุ่ม","หลาย","ให้"]
```
### ตัวอย่างที่ 3

```
input = ["เสือ","สาว","ใส่","แว่น","แวว","วาว"]
output = ["วาว", "แว่น", "แวว",  "สาว", "เสื้อ","ใส่"]
```
## 03 - นับอักขระใน string

เขียน function รับ `input` เป็น string และ return เป็นอีก string ที่นับจำนวนตัวอักษรใน `input` ดังตัวอย่าง

```
Input: GOOGLE
Output: G2O2L1E1
```
```
Input: SCHOOL
Output: S1C1H1O2L1
```
```
Input: HELLOWORLD
Output: H1E1L3O2W1R1D1
```


# เงื่อนไขการทำโจทย์

ณ วันที่ 10 กุมภาพันธ์ 2565 เป็นต้นไป ผู้ทำโจทย์ สามารถเลือกทำโจทย์ด้วยภาษาโปรแกรมหรือเครื่องมือที่ตนเองถนัดได้ดังนี้

- โจทย์ที่ `01` `02` และ `03` ใช้ภาษา `PHP` `Python` หรือ `JavaScript`

# วิธีส่งคำตอบ  

1. Fork repository นี้ไปยัง Github ของตัวเอง
2. สร้าง directory เป็น `ชื่อ account Github` ของตัวเอง เช่น `kengggg` ไว้ใน `/solutions`
3. ตั้งชื่อไฟล์ตามลำดับโจทย์ เช่น `01.py`, `02.php` และ `03.js`
4. สร้าง [Pull Request][2] มาที่ branch `main` ของ repository นี้
5. เมื่อทีมโอเพ่นดรีมได้รับแจ้ง Pull Request จะทำการ review เพื่อทำการดำเนินการสัมภาษณ์ต่อไป

[1]: https://www.opendream.co.th
[2]: https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request
[3]: https://raw.githubusercontent.com/opendream/openteam/main/posts.json
[4]: http://www.unicode.org/charts/PDF/U0E00.pdf