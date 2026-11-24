# GradeCalculator — Test Case และ TDD
 
## Test Case
 
| TC ID | Req | Test Scenario | Type | Technique | Priority | Test Data | Test Steps | Expected Result | Actual Result | Status |
|---|---|---|---|---|---|---|---|---|---|---|
| TC01 | R1 | คะแนน 100 ได้เกรด A (ขอบบนสุดของ A) | ขอบเขต | BVA | H | score = 100 | 1. เรียก calc.gradeOf(100)<br>2. assertEquals("A", ผลลัพธ์) | คืนค่า "A" | ตรงตามที่คาดหวัง | Pass |
| TC02 | R1 | คะแนน 90 ได้เกรด A (กลางช่วง A) | ปกติ | EP | M | score = 90 | 1. เรียก calc.gradeOf(90)<br>2. assertEquals("A", ผลลัพธ์) | คืนค่า "A" | ตรงตามที่คาดหวัง | Pass |
| TC03 | R1 | คะแนน 80 ได้เกรด A (ขอบล่างของ A) | ขอบเขต | BVA | H | score = 80 | 1. เรียก calc.gradeOf(80)<br>2. assertEquals("A", ผลลัพธ์) | คืนค่า "A" | ตรงตามที่คาดหวัง | Pass |
| TC04 | R1 | คะแนน 79 ได้เกรด B+ (ขอบบนของ B+ ติดกับ A) | ขอบเขต | BVA | H | score = 79 | 1. เรียก calc.gradeOf(79)<br>2. assertEquals("B+", ผลลัพธ์) | คืนค่า "B+" | ตรงตามที่คาดหวัง | Pass |
| TC05 | R1 | คะแนน 77 ได้เกรด B+ (กลางช่วง B+) | ปกติ | EP | M | score = 77 | 1. เรียก calc.gradeOf(77)<br>2. assertEquals("B+", ผลลัพธ์) | คืนค่า "B+" | ตรงตามที่คาดหวัง | Pass |
| TC06 | R1 | คะแนน 75 ได้เกรด B+ (ขอบล่างของ B+) | ขอบเขต | BVA | H | score = 75 | 1. เรียก calc.gradeOf(75)<br>2. assertEquals("B+", ผลลัพธ์) | คืนค่า "B+" | ตรงตามที่คาดหวัง | Pass |
| TC07 | R1 | คะแนน 74 ได้เกรด B (ขอบบนของ B) | ขอบเขต | BVA | H | score = 74 | 1. เรียก calc.gradeOf(74)<br>2. assertEquals("B", ผลลัพธ์) | คืนค่า "B" | ตรงตามที่คาดหวัง | Pass |
| TC08 | R1 | คะแนน 72 ได้เกรด B (กลางช่วง B) | ปกติ | EP | M | score = 72 | 1. เรียก calc.gradeOf(72)<br>2. assertEquals("B", ผลลัพธ์) | คืนค่า "B" | ตรงตามที่คาดหวัง | Pass |
| TC09 | R1 | คะแนน 70 ได้เกรด B (ขอบล่างของ B) | ขอบเขต | BVA | H | score = 70 | 1. เรียก calc.gradeOf(70)<br>2. assertEquals("B", ผลลัพธ์) | คืนค่า "B" | ตรงตามที่คาดหวัง | Pass |
| TC10 | R1 | คะแนน 69 ได้เกรด C+ (ขอบบนของ C+) | ขอบเขต | BVA | H | score = 69 | 1. เรียก calc.gradeOf(69)<br>2. assertEquals("C+", ผลลัพธ์) | คืนค่า "C+" | ตรงตามที่คาดหวัง | Pass |
| TC11 | R1 | คะแนน 67 ได้เกรด C+ (กลางช่วง C+) | ปกติ | EP | M | score = 67 | 1. เรียก calc.gradeOf(67)<br>2. assertEquals("C+", ผลลัพธ์) | คืนค่า "C+" | ตรงตามที่คาดหวัง | Pass |
| TC12 | R1 | คะแนน 65 ได้เกรด C+ (ขอบล่างของ C+) | ขอบเขต | BVA | H | score = 65 | 1. เรียก calc.gradeOf(65)<br>2. assertEquals("C+", ผลลัพธ์) | คืนค่า "C+" | ตรงตามที่คาดหวัง | Pass |
| TC13 | R2 | คะแนน 64 ได้เกรด C (ขอบบนของ C) | ขอบเขต | BVA | H | score = 64 | 1. เรียก calc.gradeOf(64)<br>2. assertEquals("C", ผลลัพธ์) | คืนค่า "C" | ตรงตามที่คาดหวัง | Pass |
| TC14 | R2 | คะแนน 62 ได้เกรด C (กลางช่วง C) | ปกติ | EP | M | score = 62 | 1. เรียก calc.gradeOf(62)<br>2. assertEquals("C", ผลลัพธ์) | คืนค่า "C" | ตรงตามที่คาดหวัง | Pass |
| TC15 | R2 | คะแนน 60 ได้เกรด C (ขอบล่างของ C) | ขอบเขต | BVA | H | score = 60 | 1. เรียก calc.gradeOf(60)<br>2. assertEquals("C", ผลลัพธ์) | คืนค่า "C" | ตรงตามที่คาดหวัง | Pass |
| TC16 | R2 | คะแนน 59 ได้เกรด D+ (ขอบบนของ D+) | ขอบเขต | BVA | H | score = 59 | 1. เรียก calc.gradeOf(59)<br>2. assertEquals("D+", ผลลัพธ์) | คืนค่า "D+" | ตรงตามที่คาดหวัง | Pass |
| TC17 | R2 | คะแนน 57 ได้เกรด D+ (กลางช่วง D+) | ปกติ | EP | M | score = 57 | 1. เรียก calc.gradeOf(57)<br>2. assertEquals("D+", ผลลัพธ์) | คืนค่า "D+" | ตรงตามที่คาดหวัง | Pass |
| TC18 | R2 | คะแนน 55 ได้เกรด D+ (ขอบล่างของ D+) | ขอบเขต | BVA | H | score = 55 | 1. เรียก calc.gradeOf(55)<br>2. assertEquals("D+", ผลลัพธ์) | คืนค่า "D+" | ตรงตามที่คาดหวัง | Pass |
| TC19 | R2 | คะแนน 54 ได้เกรด D (ขอบบนของ D) | ขอบเขต | BVA | H | score = 54 | 1. เรียก calc.gradeOf(54)<br>2. assertEquals("D", ผลลัพธ์) | คืนค่า "D" | ตรงตามที่คาดหวัง | Pass |
| TC20 | R2 | คะแนน 52 ได้เกรด D (กลางช่วง D) | ปกติ | EP | M | score = 52 | 1. เรียก calc.gradeOf(52)<br>2. assertEquals("D", ผลลัพธ์) | คืนค่า "D" | ตรงตามที่คาดหวัง | Pass |
| TC21 | R2 | คะแนน 50 ได้เกรด D (ขอบล่างของ D) | ขอบเขต | BVA | H | score = 50 | 1. เรียก calc.gradeOf(50)<br>2. assertEquals("D", ผลลัพธ์) | คืนค่า "D" | ตรงตามที่คาดหวัง | Pass |
| TC22 | R2 | คะแนน 49 ได้เกรด F (ขอบบนของ F ติดกับ D) | ขอบเขต | BVA | H | score = 49 | 1. เรียก calc.gradeOf(49)<br>2. assertEquals("F", ผลลัพธ์) | คืนค่า "F" | ตรงตามที่คาดหวัง | Pass |
| TC23 | R2 | คะแนน 25 ได้เกรด F (กลางช่วง F) | ปกติ | EP | M | score = 25 | 1. เรียก calc.gradeOf(25)<br>2. assertEquals("F", ผลลัพธ์) | คืนค่า "F" | ตรงตามที่คาดหวัง | Pass |
| TC24 | R2 | คะแนน 0 ได้เกรด F (ขอบล่างสุดของคะแนนที่ถูกต้อง) | ขอบเขต | BVA | H | score = 0 | 1. เรียก calc.gradeOf(0)<br>2. assertEquals("F", ผลลัพธ์) | คืนค่า "F" | ตรงตามที่คาดหวัง | Pass |
| TC25 | R3 | คะแนน -1 ต้องโยน exception (ต่ำกว่าขอบล่าง 1) | ขอบเขต | BVA | H | score = -1 | 1. เรียก calc.gradeOf(-1) ภายใน assertThrows (หรือ @Test(expected = ...)) | โยน IllegalArgumentException และไม่คืนเกรดใดๆ | ตรงตามที่คาดหวัง | Pass |
| TC26 | R3 | คะแนน 101 ต้องโยน exception (สูงกว่าขอบบน 1) | ขอบเขต | BVA | H | score = 101 | 1. เรียก calc.gradeOf(101) ภายใน assertThrows (หรือ @Test(expected = ...)) | โยน IllegalArgumentException และไม่คืนเกรดใดๆ | ตรงตามที่คาดหวัง | Pass |
| TC27 | R3 | คะแนน -100 ต้องโยน exception (ติดลบมาก) | ผิดปกติ | EP | M | score = -100 | 1. เรียก calc.gradeOf(-100) ภายใน assertThrows (หรือ @Test(expected = ...)) | โยน IllegalArgumentException และไม่คืนเกรดใดๆ | ตรงตามที่คาดหวัง | Pass |
| TC28 | R3 | คะแนน Integer.MIN_VALUE ต้องโยน exception (ค่าต่ำสุดของ int) | ผิดปกติ | Error guessing | M | score = Integer.MIN_VALUE | 1. เรียก calc.gradeOf(Integer.MIN_VALUE) ภายใน assertThrows (หรือ @Test(expected = ...)) | โยน IllegalArgumentException และไม่คืนเกรดใดๆ | ตรงตามที่คาดหวัง | Pass |
| TC29 | R3 | คะแนน Integer.MAX_VALUE ต้องโยน exception (ค่าสูงสุดของ int) | ผิดปกติ | Error guessing | M | score = Integer.MAX_VALUE | 1. เรียก calc.gradeOf(Integer.MAX_VALUE) ภายใน assertThrows (หรือ @Test(expected = ...)) | โยน IllegalArgumentException และไม่คืนเกรดใดๆ | ตรงตามที่คาดหวัง | Pass |
| TC30 | R3 | ข้อความของ exception ตรงตามข้อกำหนด | ผิดปกติ | Use case | L | score = 101 | 1. เรียก calc.gradeOf(101) ใน assertThrows แล้วเก็บ exception<br>2. ตรวจ e.getMessage() | ข้อความเป็น "score must be 0-100" | ตรงตามที่คาดหวัง | Pass |
| TC31 | R4 | ทุกคะแนน 0–100 ได้เกรดที่ไม่ใช่ null และอยู่ในชุดเกรดที่กำหนด | ปกติ | Use case | H | score = 0, 1, 2, …, 100 (วนลูป) | 1. วนลูป score 0–100<br>2. เรียก gradeOf(score)<br>3. ตรวจว่าไม่ null และเป็นหนึ่งใน A, B+, B, C+, C, D+, D, F | ไม่มีคะแนนใดได้ null หรือเกรดนอกชุด | ตรงตามที่คาดหวัง | Pass |
| TC32 | R4 | เมื่อคะแนนเพิ่มขึ้น เกรดต้องไม่แย่ลง | ปกติ | EP | M | score = 0 ถึง 100 ทีละ 1 | 1. วนลูป score 0–100<br>2. เทียบอันดับเกรดของ score กับ score-1 | อันดับเกรดไม่ลดลงเมื่อคะแนนเพิ่ม (ไม่มีช่วงสลับกัน) | ตรงตามที่คาดหวัง | Pass |
| TC33 | R4 | เกรดเปลี่ยนที่ 7 จุดพอดี ไม่มีช่องว่างหรือซ้อน | ขอบเขต | BVA | M | คู่ (49,50), (54,55), (59,60), (64,65), (69,70), (74,75), (79,80) | 1. สำหรับแต่ละคู่ เรียก gradeOf ทั้งสองค่า<br>2. เทียบว่าเกรดต่างกัน | ทั้ง 7 คู่ได้เกรดต่างกัน และคะแนนอื่นที่อยู่ติดกันได้เกรดเดียวกัน | ตรงตามที่คาดหวัง | Pass |
| TC34 | NFR | Fast: เรียก gradeOf 101 ครั้งเสร็จเร็ว | ไม่ใช่เชิงฟังก์ชัน | Performance test | H | score = 0 ถึง 100 | 1. จับเวลา<br>2. เรียก gradeOf ทุกคะแนน 0–100<br>3. หยุดจับเวลา | รวมไม่เกิน 100 ms และไม่ใช้ฐานข้อมูล เครือข่าย หรือ Thread.sleep | ตรงตามที่คาดหวัง | Pass |
| TC35 | NFR | Independent/Repeatable: ผลเหมือนเดิมทุกครั้งและไม่ขึ้นกับลำดับเทสต์ | ไม่ใช่เชิงฟังก์ชัน | EP | M | score = 75 (เรียกซ้ำ) และรันเทสต์ในลำดับสลับกัน | 1. รัน gradeOf(75) 3 ครั้ง<br>2. รันทั้งชุดเทสต์โดยสลับลำดับ<br>3. เปรียบเทียบผล | ได้ "B+" ทุกครั้ง ทุกลำดับ (ไม่มี static state ที่แชร์ระหว่างเทสต์) | ตรงตามที่คาดหวัง | Pass |
 
## TDD (Red → Green → Refactor)
 
| รอบ | Red (commit เทสต์ที่ล้ม) | Green (โค้ดน้อยที่สุดให้ผ่าน) |
|---|---|---|
| 1 | 100 และ 80 ได้ A | `return "A";` (hard-code) |
| 2 | 75 ได้ B+ | เพิ่ม `if (score >= 80) return "A";` |
| 3 | 70 ได้ B | เพิ่มเงื่อนไข B+ |
| 4 | 65 ได้ C+ | เพิ่มเงื่อนไข B |
| 5 | 60 ได้ C | เพิ่มเงื่อนไข C+ |
| 6 | 55 ได้ D+ | เพิ่มเงื่อนไข C |
| 7 | 50 ได้ D | เพิ่มเงื่อนไข D+ |
| 8 | 49 และ 0 ได้ F, ค่าขอบ 79 ได้ B+ | เพิ่มเงื่อนไข D และ `return "F"` |
| 9 | 101 และ -1 โยน exception | ตรวจช่วง 0–100 ไว้บนสุด |
| Refactor | — | เปลี่ยน if 7 ชั้นเป็นตาราง `MIN` / `GRADE` (เทสต์ยังเขียวทุกตัว) |
 
