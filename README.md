# Human Parsing

> **Curated delivery repository — content migration pending verification.** The project owner reports that implementation/research work was completed in older VS Code/SSH workspaces and source repos, but this new repository does not yet claim a fully packaged release.

งานวิจัยและชุดส่งมอบของ Human Parsing ที่คัดเลือกจากการทดลองหลายโมเดล/weights และประเมินกับชุดข้อมูลสาธารณะและ CCTV

**PUBLIC — metadata and approved code/docs only.** Never publish restricted company footage or secrets.

## เป้าหมายการส่งมอบ

- จัดทำ roster ของ parser/checkpoint ที่เทสจริงเทียบกับตัวที่ศึกษาแต่ไม่รัน; อธิบาย native full-frame vs YOLO-conditioned person-crop.
- บันทึก provenance ของ MHP-v2/CIHP/CCIHP หรือ dataset อื่นที่ใช้จริง รวม taxonomy/native instance ownership, leakage risks และ exclusion policy.
- ตรวจ class mapping ระหว่าง parser output กับ body/clothing labels ที่ระบบสุดท้ายต้องการ.
- ประเมิน per-class IoU/mIoU, missed person, neighbor contamination, speed ms/person และ integrated ms/frame ตาม evaluator ที่ใช้จริง.
- เลือก parser model/weight/configuration พร้อม evidence, qualitative failures และข้อจำกัดจาก CCTV.
- ส่งมอบ parser adapter, mask alignment contract และ checkpoint manifest เฉพาะตัวที่ยืนยันใช้งานจริง.

## Existing sources (read-only starting points)

- [Human Parsing Study](https://github.com/folklazy/Human_Parsing_Study)
- [Human Parsing CCTV600 Benchmark](https://github.com/folklazy/Human_Parsing_CCTV600_Benchmark)

**Important:** these references are candidates, not proof that all content is current, supported or safe to move. Agent must verify files and commits before copying.

## เอกสารสำคัญ

- [AGENTS.md](AGENTS.md) — read first; permanent agent rules
- [Scope & deliverables](docs/SCOPE_AND_DELIVERABLES.md) — exact responsibilities and exclusions
- [Source inventory](docs/SOURCE_INVENTORY.md) — existing source pointers and audit template
- [Quality gates](docs/QUALITY_GATES.md) — acceptance checklist
- [Active task](tasks/ACTIVE_TASK.md) — first-pass work brief; delete **only after** verified completion and durable handoff
- [Project Hub](https://github.com/folklazy/Human-Body-Extraction)
- [Final End-to-End Repository](https://github.com/folklazy/A-Comparative-Study-of-YOLO-Based-Instance-Segmentation)

## Release status

| Stage | Status |
|---|---|
| Historical experiments / implementation | Reported complete by project owner; specific commits to be audited |
| Clean delivery repository | Initialized |
| Source migration and code/package verification | **Pending** |
| Actual tests and release evidence in this repository | **Not verified yet** |

Only claim numbers and performance backed by linked canonical files. Do not make up final file counts, model parameters or deployment commands.
