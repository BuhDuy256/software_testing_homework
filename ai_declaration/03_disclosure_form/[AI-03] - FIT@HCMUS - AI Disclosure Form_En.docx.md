# Faculty of Information Technology (FIT) – Ho Chi Minh City University of Science (HCMUS)

## CS423 / CSC13003 – Software Testing (AI-augmented · 2026)

### AI POLICY · TEMPLATES - 2026 v1.0

# AI Use Disclosure Form

*Attach to assignments where AI was used in any permitted capacity.*

*Adapted from Med Kharbach, PhD (2026) - AI Use Policy Templates for Higher Education. CC BY-NC-SA 4.0. This adaptation is prepared for FIT@HCMUS – CS423 / CSC15003 Software Testing course.*

---

## 1. Course & Student Info

| Field | Value |
|---|---|
| **Course:** | CS423 / CSC13003 – Software Testing |
| **Assignment ID:** | HW01 |
| **Assignment Title:** |  QA/QC Jobs · 20 Defects · Test a Physical Product |
| **AI Use Category (1–5):** | 1 + 3 |
| **Date:** | Monday - 06/01/2026 |
| **Student name:** | Nguyễn Bảo Duy |
| **Student ID:** | 23127179 |

---

## 2. Disclosure Questions

### 1. AI tool(s) used:

*List every AI tool used for this assignment (e.g., AI Tool (e.g., ChatGPT, Claude, Gemini), ChatGPT, GitHub Copilot, Cursor, Gemini).*

CLAUDE, CHATGPT

---

### 2. Stage(s) of the assignment where AI was used:

*Tick all that apply:*

- [X] brainstorming
- [ ] outlining
- [X] drafting
- [ ] feedback
- [ ] revision
- [ ] coding
- [X] data analysis
- [ ] visual design
- [ ] other (specify): ________________

*(Additional notes here.)*

---

### 3. Main prompts or tasks given to the AI:

*Paste the 2–3 most impactful prompts verbatim. For the full transcript, attach Appendix A (prompt_log.md).*

**Prompt 1 - ChatGPT (Session 4 · 2026-06-01):** QA/QC Role Mindmap

```
You are an ISTQB Foundation Level expert and a QA/QC career consultant.
Create a comprehensive QA/QC Role Mindmap for the Software Testing industry in 2026.
Requirements:
Output in Markdown mindmap format.
The root node must be "QA/QC Roles 2026".
Include at least 20 nodes.
Cover both traditional and AI-augmented QA/QC roles.
For each role, include:
  Main responsibilities
  Required skills
  Common tools
  Career path
The mindmap should include, but not be limited to:
  QA Engineer
  QC Engineer
  Manual Tester
  Automation Tester
  Performance Tester
  Security Tester
  Mobile Tester
  Test Analyst
  Test Lead
  QA Manager
  SDET
  AI Testing Engineer
  LLM Evaluator
  Prompt Testing Specialist
  Test Architect
Also include:
  Relationships between roles
  Differences between QA and QC
  AI impact on each role in 2026
  Which tasks can be replaced, assisted, or cannot be replaced by AI
Format: Markdown mindmap only. Use clear hierarchy with indentation. Add brief explanations for each node.
Follow ISTQB terminology whenever possible.
Intentionally include exactly THREE subtle mistakes in the mindmap related to QA/QC roles,
responsibilities, or ISTQB concepts, but do NOT reveal where the mistakes are.
```

**Prompt 2 - Claude Code (Session 5 · 2026-06-01):** Requirement 1 – QA/QC Job Market Report

```
Context: I collected and stored 10 QA/QC related job in
@"assets/Requirement 1 – QA QC Job Market 2026+\". Each subfolder job_[n] contains its
job_description.md which shows the description in website.
Task: I need you write content for @report/req1.md follows these steps:
  1. Use heading 3 for job title => For example: ### Job 1 - [Title]
  2. Use heading 4 and write content for these parts: link, dated screenshot
     (Monday, 01/06/2027), job description, required skills, salary, AI impact Analysis.
  3. Especially, with "AI Impact Analysis" sections: Please use maximum 2 sentences to write
     contents => This section must shows how a job is required more than before AI era.
Constraints:
  1. Use 5.5 IELTS Vocabs to write content.
  2. Don't read .png file.
  3. With the jd's section such as "job description", "required skills", ... (the section was
     already existed in JD) => Copy paste content exactly, the only thing you analyze and write
     by yourself is AI Impact Analysis.
  4. Job link in link.txt.
```

**Prompt 3 - claude.ai (Session 7 · 2026-06-01):** Requirement 3 – Physical Product Test Cases

```
Context: I sent you the Device Specification, Test Case Table Specification and Test Cases Sheet
in my Drive.
Task: Please search for information about my "Evaporative Air Cooler" on the Internet and fill
the content in the test cases sheet that follows the specification.
Constraints: I need more than 5 test cases, which their expected output won't rely really much
on the metric. For example: Can reduce the temperature by 2 - 3. Because I need to record at
least 5 video to execute the test cases, I will want to make it easy to test and record.
```

*For the full prompt list, see Appendix A: `report/prompt_log.md`.*

---

### 4. Specific parts of the work AI contributed to:

*Be specific. Example: 'AI generated TC01–TC15 in Section 3.2; I rewrote TC04 and TC11; AI did NOT contribute to Sections 1, 2, 4, or the AI Critique.'*

- **Requirement 1 (QA/QC Job Market):** AI wrote the "AI Impact Analysis" paragraph for each of the 10 job listings in `report/req1.md`. All other sections (job description, required skills, salary) were copied directly from the original job postings without any change.
- **Requirement 2 (20 Software Defects):** AI selected 20 defects from a prepared list of 25 and formatted the content into `report/req2.md`. I decided the priority order, placing AI/LLM-related defects first as required.
- **Requirement 3 (Physical Product Testing):** AI generated the initial set of test cases for the Evaporative Air Cooler based on the device specification. I reviewed each test case and removed those whose expected outputs depended too heavily on exact measurements.
- **QA/QC Role Mindmap:** AI produced the full mindmap structure in `report/req4.md`. I then identified and corrected the three intentional mistakes that were embedded by the AI.
- **AI did NOT contribute to:** the collection of job postings, the selection of the physical product, the recording of test execution videos, the AI Audit Report, or this disclosure form.

---

### 5. How I reviewed, revised, or verified the AI output:

*Describe your verification method (ran the test, checked the spec, asked the TA, looked up RFC, cross-checked with the ISTQB syllabus, etc.).*

My main method was mental review. Because I knew what context I had given the AI and what I had left out, I could predict its output before reading it. Each prompt also included a short reasoning guide, which kept the output close to what I expected. If something looked wrong, it was easy to spot.

For most parts, one read-through was enough. I checked Requirement 1 for verbatim copying and sentence limits, and Requirement 2 for correct ordering and no leftover icons. For the QA/QC Mindmap, I used the ISTQB FL Syllabus (§1.2) to find the three intentional mistakes.

Requirement 3 needed the most checking. The AI assumed the device had push-buttons, but the real product uses rotary knobs. I corrected the affected test cases after comparing them against the device specification (ISTQB FL §4.1), and added three more test cases from my own observation of the product.

---

### 6. Citation (if required by course style guide):

*Software Testing uses the IEEE style. Example: Anthropic. (2026). AI Tool (e.g., ChatGPT, Claude, Gemini) [Large language model]. https://claude.ai*

1. Anthropic. (2026). Claude [Claude - Sonnet 4.6 - Medium]. https://claude.ai / Claude Code
2. OpenAI. (2026). ChatGPT [ChatGPT 5.5 for Teacher - Instance]. https://chatgpt.com

---

## 3. Statement of Honesty

*By signing below, I confirm that the disclosure above is accurate and complete. I understand that undisclosed or false disclosure of AI use is treated as academic misconduct and may result in a 0 grade for the assignment and disciplinary referral.*

### Signature

| Field | Value |
|---|---|
| **Student name (printed):** | Nguyễn Bảo Duy|
| **Student ID:** | 23127179 |
| **Class / Cohort:** | 23KTPM2 |
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
