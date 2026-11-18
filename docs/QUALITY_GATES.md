# Acceptance checklist — Human Parsing

## Content selection
- [ ] Confirm actual source workspace/repo inventories, branches and commits.
- [ ] Classify each candidate artifact: shipping / evidence / exploratory / obsolete / sensitive.
- [ ] Include only reviewed code, tests, configs, results and documentation.
- [ ] Link to original full experiment reports instead of copying large logs/caches.

## Domain gates
- [ ] ยืนยัน actual checkpoint inference และ selected weight ไม่ใช่ metadata-only
- [ ] GT format/person ownership/class mappings ถูกต้องกับ evaluation population
- [ ] แยก oracle parsing, native full frame และ YOLO-conditioned อย่างชัด
- [ ] รักษารายงาน Stage0/audit/data provenance ของเดิม

## Engineering/provenance
- [ ] Ensure README is accurate and all internal/external links work.
- [ ] Record source SHA / release version / environment / license/rights where relevant.
- [ ] Verify all imported code has tests or an evidenced smoke run.
- [ ] No secrets, unauthorized CCTV imagery, unverifiable numbers or silently edited canonical metrics.
- [ ] Preserve originals and record a migration summary with before/after checks.
- [ ] Update status in Project Hub only after evidence exists.
- [ ] Delete temporary `tasks/ACTIVE_TASK.md` **only after** acceptance and durable handoff summary.
