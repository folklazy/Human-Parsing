# AGENTS.md — Human Parsing

## Mission
งานวิจัยและชุดส่งมอบของ Human Parsing ที่คัดเลือกจากการทดลองหลายโมเดล/weights และประเมินกับชุดข้อมูลสาธารณะและ CCTV

## Read before any change
1. `README.md`
2. `docs/SCOPE_AND_DELIVERABLES.md`
3. `docs/SOURCE_INVENTORY.md`
4. `docs/QUALITY_GATES.md`
5. `tasks/ACTIVE_TASK.md` if present
6. Corresponding source repos' own `AGENTS.md` and exact workspace files.

## Scientific and source integrity
- Confirm source file paths, git status, commit hashes, actual selected implementation, checkpoint/version and report provenance before claiming anything is final.
- Treat old experiments as **read-only evidence**. Preserve canonical metrics, raw annotations, source hashes, logs and model artifacts; do not delete or silently regenerate them.
- Do not assume the newest-named folder is what the final app runs. Verify actual imports/config/checkpoints in the running project.
- Preserve prior git histories; use links/evidence manifests rather than bulk-duplicating research data.
- Separate confirmed facts, derived analysis, inference and TODO/NOT_VERIFIED.

## Scope and permissions
- ไม่เพิ่ม parser ใหม่หรือ benchmark ใหม่โดยไม่มีคำสั่ง
- ไม่ยก Stage-0 blocked findings เป็นผลการทดสอบจริง
- ไม่อ้าง published benchmark parity โดยไม่มี reproduction
- Do not edit the Hub, Final repo or any other repository without a separate scoped task.
- Do not download large models/datasets, install packages, run full benchmarks/training, move/delete originals or change repository visibility without authorization.
- No API keys, passwords, tokens, DB credentials or company imagery in public commits. **PUBLIC — metadata and approved code/docs only.** Never publish restricted company footage or secrets.

## Required work product
- ตรวจ scripts, weights registry, report ล่าสุด และ branch จริงใน Human_Parsing_Study
- ค้นผลทดลองสุดท้ายและตัดสินใจ checkpoint ที่ใช้งานจริงจาก evidence
- จัดเอกสาร visual comparison, failure analysis, taxonomy และ API interface
- จัด clean code adapter พร้อม tests หากมี source ใช้งานจริง

## Done means
- ยืนยัน actual checkpoint inference และ selected weight ไม่ใช่ metadata-only
- GT format/person ownership/class mappings ถูกต้องกับ evaluation population
- แยก oracle parsing, native full frame และ YOLO-conditioned อย่างชัด
- รักษารายงาน Stage0/audit/data provenance ของเดิม
- Preserve a durable summary of findings, source SHAs, changed paths, test results, known issues and a reproducibility note.
- Record relevant decisions/limitations in docs and the Project Hub if authorized.
- Remove **only** `tasks/ACTIVE_TASK.md` after owner acceptance and saved evidence; never remove permanent `AGENTS.md`, provenance or historical artifacts.
