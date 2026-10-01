<p align="center"><img src="logo.svg" width="160" alt="Parasitology Contest logo"></p>

# Parasitology Contest

เว็บฝึกทำข้อสอบ Parasitology Contest จากข้อสอบที่รวบรวมได้ปี 2021–2025 เป็นไฟล์ HTML ไฟล์เดียว ไม่ต้องติดตั้งอะไร

## เปิดใช้

- เปิด `index.html` ในเบราว์เซอร์ได้เลย
- หรือเปิด GitHub Pages: Settings → Pages → Source: `main` / root แล้วเข้าที่ลิงก์ที่ได้ (ถ้า repo เป็น private ต้องใช้แพ็กเกจ GitHub ที่รองรับ Pages แบบ private)

## มีอะไรบ้าง

- **ฝึกพิมพ์ตอบ** 178 ข้อ แบ่ง 7 บท มีเฉลยและคำอธิบาย บอกว่าข้อไหนออกปีไหน กรองตามปีได้
  - Basic Parasitology · General knowledge · Protozoa · Cestode/Acanthocephalans · Trematode · Nematode · Arthropods
- **Extended (โจทย์คาดการณ์)** 92 ข้อ: หัวข้อที่ยังไม่เคยออกแต่มีโอกาสออก (วิเคราะห์จากรูปแบบข้อสอบ 5 ปีและบริบทมาเลเซีย/อาเซียน) และชุด **แยกคู่สับสน** 20 ข้อ เปิดด้วยปุ่ม Extended ในหน้าฝึกทำข้อสอบ หรือกล่อง Extended content ในหน้าสรุป (ไม่ใช่ข้อสอบจริง และไม่นับรวมใน Flashcard)
- **Flashcards** ทบทวนแบบ spaced repetition (แบบ Anki)
- **ทายภาพ (spot diagnosis)** 94 ภาพ: ไข่พยาธิ, มาลาเรียทั้ง 4 ชนิดทุกระยะ, Babesia, Leishmania, T. cruzi, ยุง 3 สกุล และโจทย์ภาพจากข้อสอบจริง สุ่มภาพที่ยังไม่เคยทำหรือเคยตอบผิดขึ้นก่อน
- **สอบจำลองแบบจับเวลา** เลือกจำนวนข้อ เวลาต่อข้อ ชุดโจทย์ และเฉพาะโจทย์ภาพได้ ทำจบแล้วตรวจและให้คะแนนทีเดียว บันทึกผลกลับไปที่โหมดฝึกได้
- **สรุปเนื้อหา** รายบท พร้อมรายการข้อที่ออกซ้ำหลายปี
  - ภาพจุลทรรศน์จริง 39 รูป: มาลาเรียทั้ง 4 ชนิด, Babesia, Leishmania, T. cruzi, ไข่พยาธิที่ออกสอบ, ยุง 3 สกุล
  - แผนภาพ 5 ภาพ: วิธีตรวจ, ขนาดไข่ตามสเกลจริง, scolex/proglottid ของ Taenia, หางไมโครฟิลาเรีย, ท่าเกาะของยุง
  - รายการ **ข้อที่เฉลยยังไม่แน่นอน** พร้อมปุ่มคัดลอกไปให้อาจารย์ตรวจ

ความคืบหน้าเก็บไว้ในเบราว์เซอร์ของแต่ละเครื่อง (localStorage) ย้ายข้ามเครื่องได้ด้วยปุ่ม **ย้ายความคืบหน้าไปอีกเครื่อง** ท้ายหน้า: คัดลอกรหัสจากเครื่องหนึ่ง แล้ววางในอีกเครื่อง

## ไฟล์

| ไฟล์ | คืออะไร |
|---|---|
| `index.html` | ตัวเว็บทั้งหมด (ข้อสอบ ภาพ และโค้ดฝังอยู่ในไฟล์นี้) |
| `data/questions.json` | ข้อสอบทั้งหมดในรูป JSON ไว้อ่านหรือแก้ไข (`ch` บท, `y` ปีที่ออก, `q` คำถาม, `a` เฉลย, `ex` คำอธิบาย) |
| `data/extended.json` | โจทย์และสรุป Extended (คาดการณ์) |

## หมายเหตุ

- ข้อสอบมาจากการ recall ของนักศึกษา บางข้อมีกล่องเตือนว่าเฉลยยังไม่แน่นอน ควรตรวจกับเฉลยจริงถ้ามี
- เฉลยทุกข้อ (ข้อสอบจริง, Extended) และหน้าสรุปผ่านการตรวจทานซ้ำกับ CDC DPDx, WHO และตำรามาตรฐานแล้ว (ต.ค. 2026)
- ที่มาของภาพ: [Microscopic-Medical-Parasitology-Classification](https://github.com/sayedgamal99/Microscopic-Medical-Parasitology-Classification), [MP-IDB](https://github.com/andrealoddo/MP-IDB-The-Malaria-Parasite-Image-Database-for-Image-Processing-and-Analysis), [csbl-br/chagas_detection](https://github.com/csbl-br/chagas_detection), [mosquito-monitoring](https://github.com/mosquito-boys/mosquito-monitoring), CDC PHIL / James Gathany (public domain) และ Wikimedia Commons ใช้เพื่อการศึกษา
