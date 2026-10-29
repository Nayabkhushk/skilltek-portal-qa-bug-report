# SkillTek Web Portal — Ad-Hoc QA Testing & Defect Audit

# Project Overview
This repository contains the software bug report and defect documentation for ad-hoc and exploratory functional testing performed on the SkillTek Institute of Media Solutions web platform (Admin Portal, Teacher Portal, and Public Website)[cite: 1, 12].

A total of 8 key functional, data validation, and UI defects were discovered, documented with reproduction steps, and mapped to screenshot evidence.

# Summary of Defects Found

# 1. Business Logic & Workflow Defects
BUG-01 (Teacher Portal): System allows creation and publishing of assignments with `0` total marks without any validation error.
BUG-03 (Admin Portal): Attendance module allows administrators to select future calendar dates and successfully record attendance in advance.

# 2. Missing Input Validation & Data Sanitization
BUG-02 (Admin Portal): Student registration form accepts fake phone numbers and repeated/invalid CNIC formats without proper regex validation.
BUG-04 (Admin Portal): Edit Teacher form accepts alphabetic characters inside the Phone Number field and saves invalid data.
BUG-08 (Public Website): Contact/Enquiry form accepts alphabetic inputs in the Phone field and successfully submits the lead.

# 3. Data Integrity & Duplication
BUG-06 (Admin Portal): Allows multiple active student enrollments under the exact same CNIC number in the same course.
BUG-07 (Admin Portal): Add Course form permits duplicate course titles to be created without unique title checks.

# 4. UI/UX Safety Controls
BUG-05 (Admin Portal): Clicking the delete icon on a teacher record immediately deletes it without showing a confirmation popup.

## Repository Contents
`SkillTek_Portal_Bug_Report.pdf` — Complete QA report containing step-by-step reproduction instructions, expected vs. actual results, and visual screenshot evidence.
