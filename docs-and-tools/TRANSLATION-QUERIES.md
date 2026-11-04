# Translation queries — methodica-ar-math-ratio-05 (2026-11-04)

What was found while comparing the Arabic unit with the Hebrew source (`methodica-math-ratio-05` @ `f217369`).
Section 1 was **fixed in code** because it could be checked against the Hebrew (numbers, letters, markup).
Section 2 is **left as delivered** for the translator / content owner to decide.

## 1. Fixed (checked against the Hebrew)

| Where | Was | Now | Hebrew source |
|---|---|---|---|
| 02 `script.js` s3 feedback (correct + wrong) | `3/8 · 120 = °هو 5` | `3/8 · 120 = 45°` | `= 45°` |
| 02 `script.js` s2 feedback (correct + wrong) | `3/10 · 30 = 9</span>9` (stray 9) | `… = 9</span>` | — |
| 02 `script.js` s4 ت feedback (correct + wrong) | Eden's games named `x`, the equation uses `y` | `y` in both | `ב-y` |
| 02 `script.js` s4 ت feedback | `نقس على` | `نقسم على` | `נחלק ב-` |
| 02 `script.js` s4 ت feedback | last `<strong>` never closed (2×) | closed | — |
| 05 `script.js` s2 feedback | `ومساحة هي …· 64 = 16` (triangle missing) | `ومساحة ABD هي` | `ושטח ABD הוא` |
| 05 `script.js` s3 א feedback | one run-on line; `5 + 3 + 2 = 10` without an LTR span (shown mirrored); `2/10` as plain text | the Hebrew's line breaks, LTR span, stacked fraction | — |
| 06 `script.js` s1 feedback (correct + wrong) | `المستطيل ‎ AEDB:  AEDB:` | `المستطيل AEDB:` | `המלבן AEDB:` |
| 06 `index.html` s2, 4th sub-question | `ت.` (same letter as the 3rd) | `ث.` (as part 01's ד) | `ד.` |
| 02, 03, 05 (31 places) | degree before the number: `°180`, `°67.5` — inside the LTR spans this shows `°180` | `180°` — as the Hebrew, as the other 42 places in this unit, and as ar-ratio-01/02 | `180°` |

## 2. For the translator / owner (not changed)

1. **01 s4 step ث explanation** (`methodica-ar-math-ratio-05-01/index.html`, `.s4-step-explain` after "طريقة أخرى"):
   `ترتيب البنانير الكرات` — two words for "marbles" side by side; and `فقط تكوّنت <strong>8 مجموعات…`
   — the `فقط` reads as stray. Wording only; the numbers are right.
2. **Metadata sub-question letters** (as delivered, not learner-facing):
   - `metadata/methodica-ar-math-ratio-05-01.json` uses `د.` for two questions, while the screens use
     `أ ب ت ث` (ד = `ث`).
   - `metadata/methodica-ar-math-ratio-05-06.json` labels both the 3rd and the 4th question `ت.`.
3. **`informationToBot` is still Hebrew** in every `metadata/methodica-ar-math-ratio-05-0N.json` (as delivered).
4. **The report form's "other"** is `أخرى` here. The donor unit methodica-ar-math-ratio-01 has `أخر`, which
   looks like a typo there too.
