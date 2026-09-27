# BITS Digital CodeForge V1.0

## Live Demo

**Vercel:** `https://bits-digital-code-forge-v1.vercel.app/`

## GitHub Repository

**GitHub:** `https://github.com/Vedanthinde/BITS-Digital-CodeForge-V1`

## Project Overview

BITS Digital CodeForge V1.0 is a prototype grading console created for
the CodeForge challenge.

The application allows an instructor to upload an Excel marks file,
validate the data, select a course, review course-level marks analytics,
configure grade ranges, verify calculated student grades, confirm the
final grading operation, and export final grades as a CSV file.

> **Disclaimer:** This is a prototype created for the CodeForge
> challenge. It is not an official BITS Pilani Digital grading system
> and is not intended for actual academic grading.

## Workflow

**Upload → Validate → Review Analytics → Configure Grades → Verify
Students → Finalize → Download CSV**

## Input Format

The application expects an Excel (`.xlsx` or `.xls`) file containing
exactly:

  Column        Requirement
  ------------- ----------------------------
  BITS ID       Student's BITS ID
  Course        Course name
  Total Marks   Whole number from 0 to 100

Students receiving NC because they did not appear for the examination
should not be included.

## Default Grading Scale

  Grade       Marks
  ------- ---------
  A         80--100
  A-         70--79
  B          60--69
  B-         50--59
  C          40--49
  C-         30--39
  D          20--29
  E           0--19

## Key Enhancements

### 1. Professional UI/UX

The original prototype was redesigned into a clean, responsive grading
workflow with clearer hierarchy, consistent controls, analytics cards,
student preview, status feedback and a finalization confirmation step.

### 2. Stronger Validation and Error Handling

Validation was strengthened for required Excel columns, empty files,
whole-number marks, marks outside the 0--100 range, duplicate BITS ID
records within the same course, grade-range consistency and safe
finalization.

### 3. Improved Export and Auditability

The final CSV export was improved to include grading-session context
such as the generated timestamp and the grading scale used for the
export.

## Technology

-   HTML5
-   CSS3
-   JavaScript
-   SheetJS for Excel processing
-   Responsive browser-based UI

## Testing

The application was tested for valid Excel uploads, invalid and missing
columns, empty data, invalid marks, duplicate student records, multiple
courses, grade-range changes, student search, finalization, CSV export
and responsive layout.

## Competition Stages

### Stage 1 --- Debug

Identified and fixed functional and validation issues and documented
them in `BUG_FIX_LOG.md`.

### Stage 2 --- Reimagine

Added meaningful improvements focused on usability, validation, product
workflow and export clarity.

### Stage 3 --- Deploy

The application is deployed publicly using Vercel.

## Project Structure

``` text
BITS-Digital-CodeForge-V1/
├── index.html
├── README.md
└── BUG_FIX_LOG.md
```

## Author

Vedant Hinde
