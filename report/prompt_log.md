# Appendix A: Full Prompt Log

This appendix records all AI prompts used during this project, listed in time order. Each entry shows the date, time, tool, and the exact text of the prompt sent by the user.

---

## Session 1

**Date:** 2026-05-26
**Time:** 09:09
**Tool:** Claude Code

### Prompt 1

```
Task: Convert all the job_descrition.txt to job_description.md and format markdown for its content.
```

### Prompt 2

```
Remove the previous .txt file
```

---

## Session 2

**Date:** 2026-05-26
**Time:** 09:38
**Tool:** claude.ai

### Prompt 1

```
Explain why Google Gemini generated racist images in 2024. What internal training data caused the issue?
```

### Prompt 2

```
Which researchers? Which paper? Which statement?
```

---

## Session 3

**Date:** 2026-05-27
**Time:** 10:56
**Tool:** claude.ai

### Prompt 1

```
Task: Find 25 software defects publicised between 2022 and 2026.

Mandatory: ≥ 5 defects related to AI/LLM (hallucination, prompt injection, bias).
Each defect: source link, description, severity, consequences, solution.
Constraints: When you find a source link, please try to open the website through this link, and check
whether the page doesn't have any content. You must remove this source link and website out of the list.
```

---

## Session 4

**Date:** 2026-06-01
**Time:** 03:11
**Tool:** ChatGPT

### Prompt 1

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

---

## Session 5

**Date:** 2026-06-01
**Time:** 08:51
**Tool:** Claude Code

### Prompt 1

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

---

## Session 6

**Date:** 2026-06-01
**Time:** 09:04
**Tool:** Claude Code

### Prompt 1

```
Context: I collected 25 Software Defects 2022–2026 and stored its source link, description,
severity, consequences, solution in
@"assets/Requirement 2 – 20 Software Defects 2022–2026/25_software_defects_2022_2026 (AI Output).md".
Task:
  1. I need you use choose 20 jobs from the list. After that fill content for @report/req2.md.
Constraints:
  1. The software defects related to AI/LLM (hallucination, prompt injection, bias) must be
     prioritized to exist sooner => The order in .md didn't related to to the order in req2.md.
  2. Didn't copy the icons to req2.md.
```

---

## Session 7

**Date:** 2026-06-01
**Time:** 10:18
**Tool:** claude.ai

### Prompt 1

```
Context: I sent you the Device Specification, Test Case Table Specification and Test Cases Sheet
in my Drive.
Task: Please search for information about my "Evaporative Air Cooler" on the Internet and fill
the content in the test cases sheet that follows the specification.
Constraints: I need more than 5 test cases, which their expected output won't rely really much
on the metric. For example: Can reduce the temperature by 2 - 3. Because I need to record at
least 5 video to execute the test cases, I will want to make it easy to test and record.
```

---

*Total sessions: 7 | Total prompts: 9 | Tools used: Claude Code (3 sessions), claude.ai (3 sessions), ChatGPT (1 session)*
