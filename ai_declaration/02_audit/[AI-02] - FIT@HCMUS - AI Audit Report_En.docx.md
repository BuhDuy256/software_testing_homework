# Faculty of Information Technology (FIT) – Ho Chi Minh City University of Science (HCMUS)

## CS423 / CSC13003 – Software Testing (AI-augmented · 2026)

### AI POLICY · TEMPLATES - 2026 v1.0

# AI Audit Report - 5-section Template per Artifact

*Mandatory appendix for every AI-assisted homework (HW#01–HW#06, and Seminar).*

*Adapted from Med Kharbach, PhD (2026) - AI Use Policy Templates for Higher Education. CC BY-NC-SA 4.0. This adaptation is prepared for FIT@HCMUS – CS423 / CSC15003 Software Testing course.*

---

## 1. Student Information

| Field | Value |
|---|---|
| **Student name (printed):** | Nguyễn Bảo Duy |
| **Student ID:** | 23127179 |
| **Class / Cohort:** | 23KTPM02 |
| **Assignment ID (e.g., HW#00, HW#02):** | HW01 |
| **Assignment date:** | Monday, 01/06/2026 |
| **AI tool(s) used:** | Claude, ChatGPT |
| **AI used:** | [X] Yes  [ ] No |

---

## 2. Instructions (read before filling)

- Add one row per AI-generated artifact (test case, script, checklist, OpenAPI spec, JMeter plan, etc.).
- Paste the verbatim prompt - DO NOT paraphrase.
- Paste the verbatim AI output (or include a labelled screenshot in the report).
- Tag the verdict: VALID / INVALID / INCOMPLETE.
- Reasoning must cite a course slide, ISTQB section, or technical RFC.
- Show the corrected artifact with the change highlighted.
- Sample rows are in italic - replace them before submission.

---

## 3. Audit Table - one row per artifact

### Artifact 1

1. Prompt: `Task: Convert all the job_descrition.txt to job_description.md and format markdown for its content.`
2. Tool: Claude Code (2026-05-26, 09:09)
3. AI Output: Created 10 formatted `job_description.md` files across folders job_1 to job_10, applying headings, bullet lists, bold text, blockquotes, and tables where appropriate.
4. Verdict: VALID
5. Reasoning: All 10 output files were reviewed manually. No content from the original `.txt` files was lost or changed - the AI only reformatted the structure using standard Markdown syntax. Each file uses correct heading levels (`#`, `##`), bullet lists, and bold labels to present the same information in a more readable form. Per ISTQB FL §5.4 (Test Progress Report), clear and well-structured documentation is necessary for effective communication of work products. The output met this standard without requiring any correction.
6. Student Fix: null

### Artifact 2

1. Prompt: `Remove the previous .txt file`
2. Tool: Claude Code (2026-05-26, 09:09)
3. AI Output: Deleted all 10 `job_description.txt` source files using PowerShell `Remove-Item`.
4. Verdict: VALID
5. Reasoning: The AI correctly identified all 10 target files across the 10 subfolders and deleted them using the appropriate PowerShell command. No unintended files were removed. The action matched the requested scope exactly. While file deletion is not covered directly by ISTQB, the principle of configuration management (ISTQB FL §5.5 - Configuration Management) requires that only the intended version of a work product is kept. Removing the outdated `.txt` source files after the `.md` versions were confirmed to be correct is consistent with this principle.
6. Student Fix: null

### Artifact 3

1. Prompt: `Explain why Google Gemini generated racist images in 2024. What internal training data caused the issue?`
2. Tool: claude.ai (2026-05-26, 09:38)
3. AI Output: Explanation covering two root causes - (1) a blanket diversity prompt injection added to all image-generation requests, and (2) RLHF fine-tuning shaped by annotator demographics and instructions, causing historically inaccurate diverse outputs.
4. Verdict: VALID
5. Reasoning: The two root causes described by the AI are consistent with reporting from multiple credible sources (NPR, Al Jazeera, Washington Post, Brookings) at the time of the February 2024 incident. The AI also correctly distinguished that the issue was an over-correction for diversity rather than intentional bias, which is an important and accurate nuance. Per ISTQB FL §1.1 (What is Testing?), understanding the root cause of a defect is essential for selecting an effective solution. The AI's explanation of the Gemini defect correctly identifies the root cause (hidden prompt injection + RLHF reward signal), the consequence (historically inaccurate outputs), and the solution (feature suspension and audit), which matches the standard defect analysis structure required for the assignment.
6. Student Fix: null

### Artifact 4

1. Prompt: `Which researchers? Which paper? Which statement?`
2. Tool: claude.ai (2026-05-26, 09:38)
3. AI Output: Clarification that the "researchers" reference in the prior response pointed to a single expert - Fabio Motoki, University of East Anglia - whose statement was an inference about RLHF based on general theory, not a dedicated study of Gemini's internals.
4. Verdict: VALID
5. Reasoning: The AI proactively corrected its own imprecise language from the previous response - specifically the phrase "researchers pointed to," which implied institutional consensus when only one expert's opinion was cited. The corrected response gives the exact name, institution, original paper topic, and the actual quoted statement. This aligns with ISTQB FL §1.3 (Testing Principles - Principle 6: Testing is context dependent), which emphasizes that evidence must be interpreted carefully and its source must be understood. Accepting an imprecise citation without verification would reduce the reliability of the defect report. The AI's self-correction improved source quality, so the output is accepted as VALID.
6. Student Fix: null

### Artifact 5

1. Prompt: `Task: Find 25 software defects publicised between 2022 and 2026. Mandatory: ≥ 5 defects related to AI/LLM (hallucination, prompt injection, bias). Each defect: source link, description, severity, consequences, solution. Constraints: When you find a source link, please try to open the website through this link, and check whether the page doesn't have any content. You must remove this source link and website out of the list.`
2. Tool: claude.ai (2026-05-27, 10:56)
3. AI Output: A report of 25 software defects (7 AI/LLM + 18 conventional), each with a verified source link, description, severity rating, consequences, and solution. Stored in `assets/Requirement 2 – 20 Software Defects 2022–2026/25_software_defects_2022_2026 (AI Output).md`.
4. Verdict: VALID
5. Reasoning: The output met all stated requirements: 25 defects total, 7 AI/LLM entries (exceeding the minimum of 5), each entry containing a source link, description, severity, consequences, and solution. The AI also verified each source link for accessibility before including it, which matched the stated constraint. Per ISTQB FL §1.1 (What is Testing?), a defect is defined as "an imperfection or deficiency in a work product." The AI correctly used this framing for each entry - identifying what went wrong, how severe it was, what harm it caused, and how it was resolved. The structure and content were accepted without modification and used directly as input for Requirement 2.
6. Student Fix: null

### Artifact 6

1. Prompt: `You are an ISTQB Foundation Level expert and a QA/QC career consultant. Create a comprehensive QA/QC Role Mindmap for the Software Testing industry in 2026. Requirements: Output in Markdown mindmap format. The root node must be "QA/QC Roles 2026". Include at least 20 nodes. Cover both traditional and AI-augmented QA/QC roles. For each role, include: Main responsibilities, Required skills, Common tools, Career path. The mindmap should include, but not be limited to: QA Engineer, QC Engineer, Manual Tester, Automation Tester, Performance Tester, Security Tester, Mobile Tester, Test Analyst, Test Lead, QA Manager, SDET, AI Testing Engineer, LLM Evaluator, Prompt Testing Specialist, Test Architect. Also include: Relationships between roles, Differences between QA and QC, AI impact on each role in 2026, Which tasks can be replaced, assisted, or cannot be replaced by AI. Format: Markdown mindmap only. Use clear hierarchy with indentation. Add brief explanations for each node. Follow ISTQB terminology whenever possible. Intentionally include exactly THREE subtle mistakes in the mindmap related to QA/QC roles, responsibilities, or ISTQB concepts, but do NOT reveal where the mistakes are.`
2. Tool: ChatGPT (2026-06-01, 03:11)
3. AI Output: A Markdown mindmap with root node "QA/QC Roles 2026", covering 20+ roles with responsibilities, skills, tools, and career paths. Three intentional subtle mistakes were embedded by the AI as instructed.
4. Verdict: VALID
5. Reasoning: The mindmap output met all structural requirements: root node "QA/QC Roles 2026", 20+ nodes, clear indentation hierarchy, all 15 specified roles included, AI impact analysis per role, and the QA vs. QC distinction covered. The AI correctly used ISTQB FL terminology - for example, distinguishing QA (process-oriented, preventive) from QC (product-oriented, corrective), consistent with ISTQB FL Syllabus §1.2 (QA and Testing). The three intentional mistakes were embedded as instructed, making the artifact suitable for the assignment's critical analysis exercise. The output was accepted as-is and used as the source for the Requirement 3 mindmap deliverable.
6. Student Fix: null

### Artifact 7

1. Prompt: `Context: I collected and stored 10 QA/QC related job in @"assets/Requirement 1 – QA QC Job Market 2026+\". Each subfolder job_[n] contains its job_description.md which shows the description in website. Task: I need you write content for @report/req1.md follows these steps: 1. Use heading 3 for job title => For example: ### Job 1 - [Title]. 2. Use heading 4 and write content for these parts: link, dated screenshot (Monday, 01/06/2027), job description, required skills, salary, AI impact Analysis. 3. Especially, with "AI Impact Analysis" sections: Please use maximum 2 sentences to write contents => This section must shows how a job is required more than before AI era. Constraints: 1. Use 5.5 IELTS Vocabs to write content. 2. Don't read .png file. 3. With the jd's section such as "job description", "required skills", ... (the section was already existed in JD) => Copy paste content exactly, the only thing you analyze and write by yourself is AI Impact Analysis. 4. Job link in link.txt.`
2. Tool: Claude Code (2026-06-01, 08:51)
3. AI Output: `report/req1.md` with 10 job entries, each containing a link, dated screenshot reference, verbatim job description and required skills, salary, and a 2-sentence AI Impact Analysis written in 5.5 IELTS vocabulary.
4. Verdict: VALID
5. Reasoning: The output was reviewed against all constraints. Job descriptions and required skills sections were copied verbatim from the source files - no content was paraphrased or altered. The heading structure (### for job title, #### for each section) matched the specified format exactly. Each AI Impact Analysis is 2 sentences and written at an appropriate vocabulary level. The AI also identified and corrected a date inconsistency in the prompt ("01/06/2027" was a Tuesday, not a Monday - the correct date, 01/06/2026, is a Monday matching today's project date), which improved accuracy. Per ISTQB FL §5.4 (Test Completion Report), work product documentation must be accurate and traceable to its source. This artifact satisfies that requirement.
6. Student Fix: null

### Artifact 8

1. Prompt: `Context: I collected 25 Software Defects 2022–2026 and stored its source link, description, severity, consequences, solution in @"assets/Requirement 2 – 20 Software Defects 2022–2026/25_software_defects_2022_2026 (AI Output).md". Task: 1. I need you use choose 20 jobs from the list. After that fill content for @report/req2.md. Constraints: 1. The software defects related to AI/LLM (hallucination, prompt injection, bias) must be prioritized to exist sooner => The order in .md didn't related to to the order in req2.md. 2. Didn't copy the icons to req2.md.`
2. Tool: Claude Code (2026-06-01, 09:04)
3. AI Output: `report/req2.md` with 20 selected software defects - all 7 AI/LLM entries placed first, followed by 13 conventional security defects, with no emoji icons.
4. Verdict: VALID
5. Reasoning: Both constraints were satisfied: (1) all 7 AI/LLM-related defects appear at the top of the report, ahead of the 13 conventional entries; (2) no emoji icons were carried over from the source file. The 5 entries dropped from the original 25 were reasonable choices - they were either redundant (duplicate MOVEit entry), lower severity (downgraded OpenSSL), or less relevant to software testing coursework (Twitter API scraping, IRS programming error, Birmingham ERP). Per ISTQB FL §5.6 (Defect Management), a defect report should contain sufficient information to understand the nature and impact of the defect. All 20 retained entries preserve their source link, description, severity, consequences, and solution fields, meeting this standard. The output was accepted without modification.
6. Student Fix: null

### Artifact 9

1. Prompt: `Context: I sent you the Device Specification, Test Case Table Specification and Test Cases Sheet in my Drive. Task: Please search for information about my "Evaporative Air Cooler" on the Internet and fill the content in the test cases sheet that follows the specification. Constraints: I need more than 5 test cases, which their expected output won't rely really much on the metric. For example: Can reduce the temperature by 2 - 3. Because I need to record at least 5 video to execute the test cases, I will want to make it easy to test and record.`
2. Tool: claude.ai (2026-06-01, 10:18)
3. AI Output: 12 test cases for an Evaporative Air Cooler covering power on/off, fan speeds, water tank fill, cooling mode, oscillation, timer, low water warning, water drain, noise level check, mobility, and restart after power cut. All expected outputs are observable pass/fail behaviors. Uploaded to a new Google Sheet in the user's Drive.
4. Verdict: INCOMPLETE
5. Reasoning: The AI only received the device specification sheet (model name, power rating, dimensions, noise range) but had no access to the physical device. As a result, it inferred the control interface incorrectly. Per ISTQB FL Syllabus §4.1 (Test Analysis), the test basis must be sufficient to identify test conditions accurately. Two categories of errors were found: (1) **Wrong input mechanism** - the AI described all controls as push-buttons (e.g., "Press the Power button", "Press the Speed button until the Low speed indicator is lit"), whereas the DAIKIOSAN DM102 uses **stepped rotary knobs with notches** (núm xoay có nấc) for power and fan speed selection, and a **mechanical countdown timer knob** for the timer function. (2) **Unsupported expected behavior** - TC11 (Low Water Warning) stated the device "emits an audible beep and/or warning light," but it is unknown whether this model supports such a feature. According to ISTQB FL §4.2 (Test Design), expected results must be derived from a reliable test basis; assumptions about device features that are not confirmed in any available document are not acceptable as expected outputs.
6. Student Fix: The following changes were applied to produce the corrected test cases (saved in `report/Test Cases - Req 3 - HW01 - Software Testing HCMUS.xlsx`):

   | TC | AI-generated Input (Wrong) | Student-corrected Input |
   |----|---------------------------|------------------------|
   | TC1 Power On | "Press the Power button once" | "Turn the stepped power knob 1 notch from the OFF position" |
   | TC2 Power Off | "Press the Power button once to turn off" | "Turn the stepped power knob back to the OFF position" |
   | TC3 Fan Speed – Low | "Press the Speed button until the Low speed indicator is lit" | "Turn the stepped knob to Mode 1 (lowest notch)" |
   | TC4 Fan Speed – Medium | "Press the Speed button until the Medium speed indicator is lit" | "Turn the stepped knob to Mode 2" |
   | TC5 Fan Speed – High | "Press the Speed button until the High speed indicator is lit" | "Turn the stepped knob to Mode 3" |
   | TC10 Timer | "Press the Timer button and select the 1-hour setting" | "Turn the timer stepped knob to the desired level; confirm the knob rotates counterclockwise back toward 0" |

   | TC | AI-generated Expected Output (Wrong) | Student-corrected Expected Output |
   |----|--------------------------------------|----------------------------------|
   | TC11 Low Water Warning | "Device emits a warning indicator (audible beep and/or warning light)" | "If low-water warning is supported: warning indicator/beep appears. If not supported: pump must not produce abnormal noise, overheating, smoke, or damage." |

   Additionally, the student added 3 self-thinking test cases not present in the AI output:
   - **TC13**: Move / Roll on Wheels - verifies the device can be pushed in all directions without tipping.
   - **TC14**: Restart After Power Disconnection - verifies normal operation after unplugging and re-plugging.
   - **TC15**: Add Ice to the Ice Compartment - verifies the separate ice compartment feature and checks for leakage.

---

## 4. Summary of AI Accuracy

Aggregate the verdicts from Section 3 and complete the table below.

| Metric | Count | Percentage |
|---|---|---|
| **Total AI-generated artifacts audited** | 9 | 100% |
| **VALID (correct, accepted as-is)** | 8 | 89% |
| **INVALID (wrong; rejected)** | 0 | 0% |
| **INCOMPLETE (acceptable after edits)** | 1 | 11% |

---

## 5. Conclusion - When should AI be used (or not)?

AI performed well on tasks that had clear context, such as converting files, researching publicly available defects, and generating structured reports from existing documents. In these cases, the outputs were accurate and required no correction. However, AI struggled when important context was missing. For the evaporative air cooler test cases, the AI incorrectly assumed all controls were push-buttons, because the device specification only contained model numbers and technical ratings, which is not a description of the actual physical interface. This led to inaccurate input steps that needed to be rewritten. 

For future use, AI is recommended for documentation tasks, research, and report formatting where all necessary information is available in digital form.

Commonly, we need provide enough context and must predict AI behaviors actively depend on provided context before.

---

## 6. Mandatory Disclosure (paste verbatim)

> "The job listings used in Requirement 1 were collected entirely by me from job search websites => Claude Code was just used only to format and write the report content based on those pre-collected listings. The software defect report (Requirement 2) and the initial test cases (Requirement 3) were generated by Claude (claude.ai) and Claude Code; I reviewed and modified the test case input steps (TC1–TC5, TC9–TC10) to reflect the actual rotary-knob interface of the physical device, corrected the Low Water Warning expected output (TC11), and added three self-designed test cases (TC13–TC15); the reasoning and content of the AI Audit Report (Sections 3–6) were developed entirely by me; AI was used only to assist with grammar and vocabulary. The detailed AI Audit Report is attached as Appendix A. I confirm I did not use AI to generate any artifact listed in the prohibited category."

### Signature

| Field | Value |
|---|---|
| **Student name (printed):** | Nguyễn Bảo Duy |
| **Student ID:** | 23127179 |
| **Class / Cohort:** | 23KTPM02 |
| **Course:** | CS423 / CSC13003 – Software Testing |
| **Instructor:** | Lâm Quang Vũ |
| **Date:** | Monday, 01/06/2026 |
| **Signature:** | Nguyễn Bảo Duy |

---

## References

- Kharbach, M. (2026). *AI Use Policy Templates for Higher Education.* CC BY-NC-SA 4.0.
- ISTQB Foundation Level Syllabus (latest version).
- Hardman, P. (2025). *A Post-AI Learning Taxonomy.*
- Fuster Rabella, M. (2025). OECD Education Working Paper No. 338.
- Perkins, M., Roe, J., & Furze, L. (2025). *AI Assessment Scale.*
- Anthropic (2025). *Building reliable AI test agents* - engineering blog.
- DeepEval & Promptfoo documentation - testing frameworks for LLM systems.
