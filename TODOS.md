# TODOs

## Legal and claims review for India pilot

What: Review product claims, disclaimers, consent language, and reviewer boundaries before any public launch.

Why: The Doctor Visit Optimizer must not imply diagnosis, treatment, emergency triage, or medicine stop/start authority without qualified clinical review.

Pros: Reduces legal, clinical, and trust risk before the product handles real family health data.

Cons: Requires outside expertise and may slow public launch if claims need to be narrowed.

Context: The approved plan limits V1 to organizing information, extracting medicine lists, flagging overlap or ambiguity, preparing doctor questions, and routing clinical judgment to qualified reviewers. This TODO should validate that those boundaries are safe for an India pilot and that the landing-page/product language stays inside them.

Depends on / blocked by: Identify a clinician, pharmacist, or healthcare/legal advisor who can review the pilot workflow and claims.

## Secure pilot data store

What: Choose and document the restricted non-git storage location for real pilot prescriptions, reports, packets, consent records, and reviewer notes.

Why: The repo is only for blank templates and synthetic examples. Real health data needs restricted access, no public links, retention rules, and a deletion path before the first real family case.

Pros: Prevents accidental commits or loose sharing of sensitive health documents.

Cons: Adds a small operations step before pilots and requires disciplined handling by anyone reviewing cases.

Context: The approved plan requires a 30-day retention default, family-requested deletion path, no reuse for demos/training without explicit permission, and access limited to the founder/operator plus named case reviewer.

Depends on / blocked by: Decide the actual storage tool and folder structure before accepting real patient documents.

## Clinician and pharmacist reviewer bench

What: Recruit at least one pharmacist and one doctor or nurse reviewer for cases that cross the founder/admin boundary.

Why: The pilot can organize information without clinical review, but it cannot make medicine safety claims, dosage judgments, symptom urgency assessments, or care-setting recommendations without qualified review.

Pros: Enables safer handling of medicine ambiguity, chronic-condition risk, and urgent symptom cases.

Cons: Adds coordination work, turnaround-time constraints, and likely cost per reviewed case.

Context: The approved plan separates founder/admin work from pharmacist review and doctor/nurse review. Urgent red flags bypass normal review and tell the family to seek urgent medical care.

Depends on / blocked by: Define reviewer availability, scope, payment, response time, and signoff language before accepting cases that need review.

## ABDM / health locker compatibility research

What: Research whether Ayukiz should later integrate with ABHA/ABDM health lockers or remain a manual packet workflow.

Why: ABDM already supports consent-based health-record sharing and health lockers in India. Ayukiz should not accidentally rebuild a long-term health-record system if the right future path is to generate packets from user-controlled records.

Pros: Keeps future architecture aligned with India's health-data ecosystem and avoids wasting an innovation token on generic record storage.

Cons: Not needed for the first manual pilot and could distract from proving packet demand.

Context: The approved V1 explicitly avoids a broad health wallet, but the product may later need to import or link records from ABDM-compatible health lockers after repeat demand is proven.

Depends on / blocked by: Complete 5-10 manual packet pilots first, then evaluate if repeated use justifies integration research.
