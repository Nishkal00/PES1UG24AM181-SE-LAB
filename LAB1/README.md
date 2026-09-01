# Alumni Mentorship & Mock Interview Platform — Test Case Suite

Testing artifacts for **Problem Statement #06 — Alumni Mentorship & Mock Interview Platform** (PES University, Requirements Engineering & UML Use-Case Modelling, Lab 1).

The platform connects **Student Mentees** with **Alumni Mentors** through domain-based recommendations, slot-based session booking, and structured post-interview scorecards, while enforcing privacy and soft-deletion guarantees on user data.

## Requirements Covered

| ID | Type | Priority | Summary |
|---|---|---|---|
| FR-001 | Functional | High | Recommend alumni mentors based on domain matching |
| FR-002 | Functional | High | Mentor availability calendar — students view open slots |
| FR-003 | Functional | High | Student books a session in an available slot |
| FR-004 | Functional | High | Confirmed session synced to both calendars with meeting link |
| FR-005 | Functional | Medium | Post-interview scorecard recording |
| NFR-001 | Performance & Security | High | Data privacy and soft-deletion within 24 hours |
| NFR-002 | Performance | High | Response time under simulated peak load |

Full details: [`Requrirements.xlsx`](./Requrirements.xlsx).

## Test Cases

| Test Case | Title | Requirement(s) | Owner | Report |
|---|---|---|---|---|
| TC-01 | Mentor Matching & Booking | FR-001, FR-002, FR-003, FR-004 | Owner 1 | `TC-01_Mentor_Matching_Booking_Test_Case_Report.docx` |
| TC-02 | Double-Booking Prevention | FR-003 | Owner 2 | `TC-02_Double_Booking_Prevention_Test_Case_Report.docx` |
| TC-03 | Post-Interview Scorecard Recording | FR-005 | Owner 3 | `TC-03_Scorecard_Recording_Test_Case_Report.docx` |
| TC-04 | Privacy / Soft-Deletion | NFR-001 | Owner 4 | `TC-04_Privacy_Soft_Deletion_Test_Case_Report.docx` |

Each report follows a common structure:

1. Test Case Identification
2. Requirement Under Test
3. Test Objective
4. Test Scope (In / Out)
5. Preconditions
6. Test Data
7. Test Procedure
8. Expected Results
9. Acceptance / Pass-Fail Criteria
10. Test Status
11. Notes

## Repository Structure

```
.
├── README.md
├── Requrirements.xlsx                  # FR/NFR requirements table
├── 6_SE_Lab1_SE_Problem_Statements.pdf  # Problem statement #06
├── TC-01_Mentor_Matching_Booking_Test_Case_Report.docx
├── TC-02_Double_Booking_Prevention_Test_Case_Report.docx
├── TC-03_Scorecard_Recording_Test_Case_Report.docx
├── TC-04_Privacy_Soft_Deletion_Test_Case_Report.docx
└── diagrams/
    ├── use-case-diagram.*        # UML use-case diagram (actors, «include», «extend»)
    └── use-case-flow-spec.*      # 1-page flow spec for one core use case
```

## Status

All test cases are currently **specifications only** — documented ahead of implementation. Execution status, evidence, and PASS/FAIL outcomes will be filled in once the corresponding system functionality is built and testable.
