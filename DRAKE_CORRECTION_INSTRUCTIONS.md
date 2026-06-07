# DRAKE CORRECTION INSTRUCTIONS
## ELIANA MACHADO DE ALMEIDA — 2024 FORM 1040-X
## Prepared for: Eliana Machado de Almeida | Date: June 7, 2026

---

## PART 1 — YOUR QUESTIONS ANSWERED

### Q1: Can I file an amended return (Form 1040-X) DURING an active IRS audit?

**YES. You can and should file Form 1040-X now, before the IRS issues a proposed adjustment.**

Here is exactly how it works under U.S. tax procedure:

**Stage of this audit:** IRS Letter 566-T is a "correspondence examination" at the earliest stage. No deficiency has been proposed yet. The IRS is simply asking for documentation.

**What you can do right now:**
1. Respond to Letter 566-T with the audit defense package (already prepared).
2. In the cover letter, inform the examiner that you are conceding the overstatement and have corrected the return in Drake.
3. Include the completed Form 14900 with the response.
4. File (or offer to file) Form 1040-X showing the corrected figures.

**You do NOT need to wait** for the IRS to complete their review. In fact, filing proactively:
- Shows voluntary compliance and good faith
- May result in reduced penalties
- Often causes the examiner to close the case faster
- Avoids having the IRS issue a formal proposed adjustment (which triggers a more formal process)

---

### Q2: What happens if you wait vs. act now?

| Action | What Happens |
|--------|-------------|
| **Act now (file 1040-X + respond to 566-T)** | IRS examiner may accept concessions and close the case. Faster resolution. |
| **Wait for IRS review** | IRS issues an examination report (30-day letter) proposing the adjustment. Eliana then has 30 days to agree or dispute. More formal and slower. |
| **Don't respond at all** | IRS disallows the entire deduction and issues a tax bill. Worst outcome. |

**Recommendation:** Respond to Letter 566-T by June 17, 2026 with the audit package. State clearly in the cover letter that you concede the overstatement and include the corrected Form 14900.

---

### Q3: Procedure in Drake — Should you correct in Drake and prepare a 1040-X?

**Yes.** Here is the process:
1. Make the corrections in Drake (instructions below).
2. Drake will generate the corrected Form 1040 figures automatically.
3. Open the **Form 1040-X** module in Drake and it will pull the original and corrected figures.
4. Print the 1040-X for my signature.
5. The 1040-X must be **mailed** (paper filing) — it cannot be e-filed in this situation because the original was e-filed and a 1040-X during an active audit examination is typically mailed directly to the examining office, not the normal 1040-X service center, unless the examiner instructs otherwise.

**Note:** Attach the Form 14900 to the 1040-X as a supporting document.

---

---

## PART 2 — DRAKE CORRECTION INSTRUCTIONS

### WHAT CHANGED AND WHY

Upon review, two discrepancies were identified in the original return:

| Error | Original | Corrected | Authority |
|-------|----------|-----------|-----------|
| IRC §163(h) loan limit not applied | $114,034 deducted | $77,409 deductible | IRC §163(h)(3)(B) / Form 14900 |
| Radius points treated as fully deductible | $18,900 in 2024 | ~$67 in 2024 (amortized) | IRC §461(g)(2) / Pub. 936 |
| Radius interest ($1,870) excluded from Sch A | $0 included | Included in Form 14900 | Forms 1098 |

---

### STEP 1 — OPEN ELIANA'S 2024 DRAKE RETURN
File: MACHADO DE ALMEIDA, ELIANA | SSN: 697-75-6336

---

### STEP 2 — FIX THE RADIUS FORM 1098 ENTRY
**Drake path:** Data Entry → Form 1098 → Record 2 of 2 (Radius Financial Group)

**Problem found:** The "Deductible amount, if different" field next to Box 1 shows **0**.
This zero overrides the $1,869.86 interest and tells Drake to flow $0 to Schedule A.

**Action required:**

| Field | Current Value | Change To |
|-------|--------------|-----------|
| Box 1 — Mortgage interest received | 1870 | Leave as-is (correct) |
| **"Deductible amount, if different" (next to Box 1)** | **0** | **DELETE THE ZERO — leave BLANK** |
| Box 2 — Outstanding principal | 840000 | Leave as-is |
| Box 3 — Origination date | 11-13-2024 | Leave as-is |
| Box 6 — Points | 18900 | Leave as-is (correct amount) |

**Why:** By clearing the 0, Drake will use the actual Box 1 amount ($1,870) and include it in the Schedule A calculation.

**Also required — tell Drake the Radius loan is a REFINANCE:**
In Drake's Form 1098 entry for Radius, look for a field or checkbox that asks about the nature of the loan. The label on Box 6 says "Points paid on purchase of principal residence" — but this is a REFINANCE, not a purchase. You need to indicate that in Drake so it amortizes the points instead of deducting them in full.

In Drake 2024, look for:
- A radio button or checkbox near Box 6 that says "Refinance" or asks if this is a purchase loan
- OR the "Loan Limit Worksheet" link at the top right of the Form 1098 entry screen — click it to open the Deductible Mortgage Interest worksheet

If Drake does not have a direct "refinance points" checkbox, you will handle this in Step 3 below.

---

### STEP 3 — COMPLETE THE DEDUCTIBLE MORTGAGE INTEREST WORKSHEET IN DRAKE
**Drake path:** From either Form 1098 screen → Click "Loan Limit Worksheet" (top right) — OR — 
**Data Entry → Deductible Mortgage Interest (the screen that was blank)**

This is the screen that was left completely blank on the original return. **All fields must be filled in.**

**Enter the following values:**

| Drake Field | Value to Enter | Explanation |
|-------------|---------------|-------------|
| Line 1 — Average balance, grandfathered debt (pre-10/14/1987) | **0** | No pre-1987 debt |
| Line 2 — Average balance, pre-12/16/2017 acquisition debt | **0** | No pre-TCJA debt |
| Line 7 — Average balance, post-12/15/2017 acquisition debt | **939,744** | AmWest $519,744 + Radius $420,000 |
| Line 12 — Total average balances (Drake may auto-fill) | **939,744** | Same as Line 7 |
| Line 13 — Total interest paid (NO points) | **97,004** | AmWest $95,134 + Radius $1,870 |
| Line 17 — Points reported on 1098 | **18,900** | Radius Box 6 |
| Points NOT reported on 1098 | **0** | |

**After entering Line 7 = 939,744:**
Drake will automatically calculate:
- Line 8: $750,000
- Line 9: $750,000
- Line 10: $939,744
- Line 11: **$750,000** ← Qualified loan limit
- Line 14: $750,000 ÷ $939,744 = **0.798**
- Line 15: $97,004 × 0.798 = **$77,409** ← Deductible home mortgage interest

**Verify that Drake flows $77,409 to Schedule A.**

---

### STEP 4 — HANDLE RADIUS REFINANCE POINTS ($18,900)

The $18,900 in Radius points must be amortized over the loan term — NOT deducted in full in 2024.

**Drake path:** The points amortization is typically set up through the Form 1098 entry or through a separate points amortization screen.

**You need the Radius Mortgage Note to confirm the loan term.** Assuming 30 years (360 months):

| Calculation | Amount |
|-------------|--------|
| Total points | $18,900 |
| Loan term | 360 months (30 years) — CONFIRM FROM MORTGAGE NOTE |
| Monthly amortization | $18,900 ÷ 360 = $52.50 |
| Loan origination date | 11/13/2024 |
| Months in 2024 (11/13 to 12/31) | 1.57 months |
| 2024 gross deductible points | $52.50 × 1.57 = $82.43 |
| After loan limit ratio (× 0.798) | $82.43 × 0.798 = **$65.78 → $66** |
| 2024 deductible points | **$66** |
| Future annual deduction (years 2025–2054) | $52.50 × 12 × 0.798 = **$502/year** |
| Final year (2054, partial) | Remaining balance |

**In Drake:**
- Look for a "Points Amortization" or "Unamortized Points" screen
- Enter: Loan origination date 11/13/2024, total points $18,900, loan term (360 months)
- Confirm Drake limits the 2024 deduction to the prorated amount (approximately $66)
- Drake will carry forward the remaining unamortized points to future years automatically

**If Drake applies the loan limit ratio to the points automatically through the Deductible Mortgage Interest worksheet, verify the output. If not, manually enter the 2024 deductible points as approximately $66 on Schedule A line 8c (Points not reported on Form 1098 — the amortized portion).**

---

### STEP 5 — VERIFY CORRECTED SCHEDULE A

After completing Steps 2–4, Drake's Schedule A should show:

| Line | Description | Original | Corrected |
|------|-------------|---------|-----------|
| 5a | State/local income taxes | $5,424 | $5,424 (no change) |
| 5b | Real estate taxes | $2,651 | $2,651 (no change) |
| 5e | Taxes cap | $8,075 | $8,075 (no change) |
| 7 | Total taxes | $8,075 | $8,075 (no change) |
| 8a | Mortgage interest (Form 14900 limited) | $114,034 | **$77,409** |
| 8c | Points (2024 amortized, if on this line) | $0 | **$66** |
| 8e | Total interest | $114,034 | **$77,475** |
| **17** | **Total itemized deductions** | **$122,109** | **$85,550** |

---

### STEP 6 — VERIFY FORM 8995 (QBID) AUTO-RECALCULATION

Drake will automatically recalculate the QBID when Schedule A changes. Verify:

| Form 8995 Line | Original | Corrected |
|----------------|---------|-----------|
| QBI amounts (Lines 1i–1iii) | $75,630 + $42,054 + $30,405 | No change |
| Line 4 — Total QBI | $148,089 | No change |
| Line 5 — 20% of QBI | $29,618 | No change |
| Line 11 — Pre-QBID taxable income | $25,980 | **$62,539** |
| Line 14 — Income limitation (×20%) | $5,196 | **$12,508** |
| **Line 15 — QBID** | **$5,196** | **$12,508** |

---

### STEP 7 — VERIFY CORRECTED FORM 1040

| Line | Description | Original | Corrected |
|------|-------------|---------|-----------|
| 11 | Adjusted gross income | $148,089 | $148,089 (no change) |
| 12 | Schedule A deductions | $122,109 | **$85,550** |
| 13 | QBID | $5,196 | **$12,508** |
| 14 | Total deductions (12+13) | $127,305 | **$98,058** |
| **15** | **Taxable income** | **$20,784** | **$50,031** |
| 16 | Income tax | $2,261 | **$6,060** |
| 23 | SE tax | $11,498 | $11,498 (no change) |
| **24** | **Total tax** | **$13,759** | **$17,558** |
| 25d | Tax withheld | $0 | $0 (no change) |
| **37** | **Amount owed** | **$14,379** | **$17,558** |

**Corrected income tax calculation on $50,031 (single filer, 2024 brackets):**
- 10% bracket ($0–$11,600): $11,600 × 10% = $1,160
- 12% bracket ($11,601–$47,150): $35,550 × 12% = $4,266
- 22% bracket ($47,151–$50,031): $2,881 × 22% = $634
- **Total income tax = $6,060**

**SE tax: $11,498 (unchanged)**
**Total corrected tax: $17,558**

---

### STEP 8 — PREPARE FORM 1040-X IN DRAKE

**Drake path:** Tools → Amended Return → Form 1040-X

Drake will populate three columns automatically:
- **Column A (Original):** Original figures as filed
- **Column B (Net Change):** The difference
- **Column C (Corrected):** New figures

**Key 1040-X lines to verify:**

| 1040-X Line | Description | Col A (Original) | Col B (Change) | Col C (Corrected) |
|-------------|-------------|-----------------|----------------|-------------------|
| 1 | Adjusted gross income | $148,089 | $0 | $148,089 |
| 4 | Itemized deductions | $122,109 | ($36,559) | $85,550 |
| 5 | QBI deduction | $5,196 | $7,312 | $12,508 |
| 7 | Taxable income | $20,784 | $29,247 | $50,031 |
| 10 | Tax | $2,261 | $3,799 | $6,060 |
| 16 | Total tax | $13,759 | $3,799 | $17,558 |
| 20 | Amount previously paid | $0 | — | — |
| 22 | Amount you owe | $13,759 | $3,799 | **$17,558** |

**Part III — Explanation of Changes (required on Form 1040-X):**

Enter the following explanation in Drake's Form 1040-X explanation field:

> "The taxpayer's home mortgage interest deduction on Schedule A is being corrected pursuant to IRC §163(h)(3)(B). Both mortgages (AmWest Funding Corp, originated 10/20/2023; Radius Financial Group, originated 11/13/2024) were incurred after December 15, 2017. The average combined mortgage balance for 2024 was $939,744, exceeding the $750,000 qualified loan limit. Per the completed Form 14900 (attached), the correct deductible interest is $77,409 (vs. $114,034 originally claimed), a ratio of 79.8%. Additionally, the $18,900 in points paid on the Radius refinancing loan must be amortized over the loan term under IRC §461(g)(2); only approximately $66 is deductible in 2024. The corrected Schedule A deduction is $85,550. The QBID under IRC §199A increases from $5,196 to $12,508 as a result of the higher taxable income. The additional tax owed is $3,799. Form 14900 is enclosed."

---

### STEP 9 — ATTACH FORM 14900 TO THE 1040-X

In Drake, you can attach the Form 14900 as a PDF attachment to the return.
- The Form 14900 is already completed in the Audit Defense Package (Section 3).
- Print or generate it and attach to both the 1040-X mailing and the IRS Letter 566-T response.

---

### STEP 10 — FILING THE 1040-X

**How to file:**
- Form 1040-X **cannot be e-filed** in this situation (active correspondence examination).
- Print the signed 1040-X.
- Send it WITH the audit response package to:

**IRS Correspondence Examination (audit response):**
Internal Revenue Service
P.O. Box 309011, AMC 8236
Memphis TN 38130-0911
*(Use Form 14817 Reply Cover Sheet on top)*

- OR, include it as an exhibit in the audit response package with a note asking the examiner to process it.
- In the cover letter, state: "I am enclosing a corrected Form 1040-X conceding the overstatement. Please advise whether you will process this adjustment through the examination or whether a separate submission is required."

---

---

## PART 3 — COMPLETE SUMMARY OF ALL CHANGES

### Changes to Make in Drake:

| # | Where in Drake | What to Change |
|---|----------------|----------------|
| 1 | Form 1098 — Radius (Record 2) | Delete the "0" in "Deductible amount, if different" → leave BLANK |
| 2 | Form 1098 — Radius (Record 2) | Mark loan as REFINANCE (not purchase) so points are amortized |
| 3 | Deductible Mortgage Interest Worksheet | Enter Line 7: 939,744 |
| 4 | Deductible Mortgage Interest Worksheet | Enter Line 13: 97,004 |
| 5 | Deductible Mortgage Interest Worksheet | Enter Line 17 (Points on 1098): 18,900 |
| 6 | Points Amortization | Set up $18,900 over loan term; 2024 deductible = ~$66 |
| 7 | Form 1040-X | Complete with corrected figures + explanation |
| 8 | Form 1040-X | Attach Form 14900 as supporting document |

### What Drake Will Auto-Calculate After Changes:

| Form | Line | Will Change To |
|------|------|----------------|
| Form 14900 | Line 11 (Qualified Loan Limit) | $750,000 |
| Form 14900 | Line 14 (Ratio) | 0.798 |
| Form 14900 | Line 15 (Deductible interest) | $77,409 |
| Schedule A | Line 8a | $77,409 |
| Schedule A | Line 8c | $66 (amortized points) |
| Schedule A | Line 17 (Total) | $85,550 |
| Form 8995 | Line 15 (QBID) | $12,508 |
| Form 1040 | Line 15 (Taxable income) | $50,031 |
| Form 1040 | Line 16 (Tax) | $6,060 |
| Form 1040 | Line 24 (Total tax) | $17,558 |

### Net Financial Impact on Eliana:

| Item | Amount |
|------|--------|
| Original total tax | $13,759 |
| Corrected total tax | $17,558 |
| **Additional tax owed** | **$3,799** |
| Estimated interest on $3,799 (from 4/15/2025 to today) | ~$380–450 |
| Underpayment penalty | Will be calculated by IRS |

---

## IMPORTANT NOTES

1. **Radius Mortgage Note:** You need the note to confirm the loan term (30-year vs. 15-year vs. other). This affects the points amortization amount. The difference is small ($66 vs. $132 in 2024) but should be exact.

2. **Points carryforward:** After correcting 2024, Drake will create a "points to be amortized in future years" carryforward. Remember to include this in my 2025, 2026... returns until the points are fully amortized.

3. **My signature:** Form 1040-X requires my signature before it can be submitted.

4. **Payment:** If I have not yet paid the original $14,379, I should pay at least that amount now to stop interest accumulation, and then pay the additional $3,799 when the 1040-X is filed.

5. **Deadline:** The IRS Letter 566-T response is due **June 17, 2026** (30 days from May 18, 2026). Do not miss this deadline.

---

*Drake Correction File prepared: June 7, 2026*
*For: Eliana Machado de Almeida | 7 Briarwood Drive, Edgartown MA 02539*
