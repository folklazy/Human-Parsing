# ACTIVE TASK — Initial curated handoff for Human Parsing

**Status:** OPEN (temporary task brief; do not delete until validation + acceptance).

## Objective
Build the clean delivery package for Human Parsing from the owner's completed but mixed historical VS Code/SSH workspaces and GitHub evidence. This repo was newly created and is **not** proof that the original work has migrated.

## Sources to inspect
- [Human Parsing Study](https://github.com/folklazy/Human_Parsing_Study)
- [Human Parsing CCTV600 Benchmark](https://github.com/folklazy/Human_Parsing_CCTV600_Benchmark)

The owner may also have local-only files on the SSH machine. Find paths only by read-only inspection; do not assume or invent them.

## Work sequence
1. ตรวจ scripts, weights registry, report ล่าสุด และ branch จริงใน Human_Parsing_Study
2. ค้นผลทดลองสุดท้ายและตัดสินใจ checkpoint ที่ใช้งานจริงจาก evidence
3. จัดเอกสาร visual comparison, failure analysis, taxonomy และ API interface
4. จัด clean code adapter พร้อม tests หากมี source ใช้งานจริง

## Mandatory restrictions
- ไม่เพิ่ม parser ใหม่หรือ benchmark ใหม่โดยไม่มีคำสั่ง
- ไม่ยก Stage-0 blocked findings เป็นผลการทดสอบจริง
- ไม่อ้าง published benchmark parity โดยไม่มี reproduction
- This task does not authorize deleting experiment directories, modifying original benchmark values, uploading restricted company CCTV, changing visibility, full retraining or large downloads.
- If a choice changes the selected model, interface, source-of-truth or rights exposure, stop and get owner approval.

## Final evidence to leave behind
- `docs/SOURCE_INVENTORY.md` completed with exact paths/commits/hashes
- Updated curated README/scope/quality checklist
- Relevant source files/tests/evidence index with verified links
- Short handoff summary: changed files, verifications, limitations, unresolved tasks
- Update Hub if separately authorized

## Cleanup after verified completion
After owner acceptance, preserve findings in permanent documents and delete **this task file only**. Do not delete `AGENTS.md`, results, provenance or audit files.
