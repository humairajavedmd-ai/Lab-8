# Defect Taxonomy for Requirements Verification

This taxonomy has 8 categories. Each has a definition and an example, and is used for the defect log in `defect-log.csv`.

| # | Category | Definition | Example (from PSVS) |
|---|---|---|---|
| 1 | Ambiguity | A statement that can be read in more than one way, so different readers reach different conclusions. | 'Year' in S10 could mean calendar or rolling year. |
| 2 | Vagueness | A statement that uses subjective or unquantified terms ('good', 'large', 'safe', 'promptly'). | 'Safe temperature' in S6 has no value. |
| 3 | Incompleteness | Required information is missing: an actor, condition, input, error case or boundary. | S1 says 'registered' but never defines registration. |
| 4 | Contradiction | Two requirements (or parts of one) cannot both be satisfied. | S4 (only the owner may withdraw) vs S5 (any box to any party). |
| 5 | Non-verifiability | No finite, objective test, inspection or proof can show that the requirement is met. | S9 'promptly' has no time limit to test against. |
| 6 | Redundancy | The same requirement is stated more than once, risking inconsistency when one copy changes. | S2 is covered by S3. |
| 7 | Infeasibility | The requirement cannot be achieved with the stated resources, physics or technology. | S7 'never' above -18 degrees C cannot be guaranteed during a power failure. |
| 8 | Untraceability | The requirement has no unique identifier, source, rationale or link to design and tests, so it cannot be traced. | S11 has no link to S9 or any rationale. |

## Severity scale

| Severity | Meaning |
|---|---|
| Critical | Makes the system unimplementable or unsafe as written, or two requirements directly conflict. |
| High | Likely to cause wrong design, safety or compliance failure unless fixed. |
| Medium | Can cause misunderstanding or rework; a workaround exists. |
| Low | Cosmetic or minor; little effect on the design. |
