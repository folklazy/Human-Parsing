# Scope & deliverables — Human Parsing

## Purpose
งานวิจัยและชุดส่งมอบของ Human Parsing ที่คัดเลือกจากการทดลองหลายโมเดล/weights และประเมินกับชุดข้อมูลสาธารณะและ CCTV

## Deliverables
- จัดทำ roster ของ parser/checkpoint ที่เทสจริงเทียบกับตัวที่ศึกษาแต่ไม่รัน; อธิบาย native full-frame vs YOLO-conditioned person-crop.
- บันทึก provenance ของ MHP-v2/CIHP/CCIHP หรือ dataset อื่นที่ใช้จริง รวม taxonomy/native instance ownership, leakage risks และ exclusion policy.
- ตรวจ class mapping ระหว่าง parser output กับ body/clothing labels ที่ระบบสุดท้ายต้องการ.
- ประเมิน per-class IoU/mIoU, missed person, neighbor contamination, speed ms/person และ integrated ms/frame ตาม evaluator ที่ใช้จริง.
- เลือก parser model/weight/configuration พร้อม evidence, qualitative failures และข้อจำกัดจาก CCTV.
- ส่งมอบ parser adapter, mask alignment contract และ checkpoint manifest เฉพาะตัวที่ยืนยันใช้งานจริง.

## Out of scope / risks
- ไม่เพิ่ม parser ใหม่หรือ benchmark ใหม่โดยไม่มีคำสั่ง
- ไม่ยก Stage-0 blocked findings เป็นผลการทดสอบจริง
- ไม่อ้าง published benchmark parity โดยไม่มี reproduction

## Definition of done
- ยืนยัน actual checkpoint inference และ selected weight ไม่ใช่ metadata-only
- GT format/person ownership/class mappings ถูกต้องกับ evaluation population
- แยก oracle parsing, native full frame และ YOLO-conditioned อย่างชัด
- รักษารายงาน Stage0/audit/data provenance ของเดิม

## Interface to the final project
Only export the minimal verified runtime module, configuration, schema, model/checkpoint manifest, test fixtures and documentation needed by [Final End-to-End Project](https://github.com/folklazy/A-Comparative-Study-of-YOLO-Based-Instance-Segmentation). Archive research outputs stay in their original repos unless there is a clear and approved reason to bundle them.

Before release, register exact source commits, package/API versions and rights in the [Project Hub](https://github.com/folklazy/Human-Body-Extraction).
