# Todoist – Manual Testing Portfolio

**Type:** Personal QA / Manual Testing practice project  
**Application under test:** Todoist (task management application)  
**Tools:** Microsoft Excel, Jira  
**Focus:** Functional test design, test execution, issue tracking and test reporting

## Project overview

This portfolio documents manual testing of core Todoist task-management scenarios, including task creation, editing, deletion, completion and selected exceptional conditions (offline behavior, unusual inputs and page refresh).

## Test execution results

| Result | Count |
| --- | ---: |
| Total recorded test cases | 20 |
| Passed | 15 |
| Failed | 5 |
| Recorded pass rate | 75% |

These are the outcomes recorded in the testing worksheet. They do not by themselves establish that all five failing scenarios are confirmed application defects.

## Test artifacts

- [`test-cases/Todoist_Test_Cases.xlsx`](test-cases/Todoist_Test_Cases.xlsx) – test-case spreadsheet.
- [`jira-issues/Issue_Summary.csv`](jira-issues/Issue_Summary.csv) – selected Jira issue IDs and scenarios, without personal/account metadata.
- [`reports/Todoist_Test_Summary_Report.docx`](reports/Todoist_Test_Summary_Report.docx) – summary report.

## Issues recorded

| Jira issue | Test case | Area |
| --- | --- | --- |
| SCRUM-5 | TC02 | Empty title during task creation |
| SCRUM-6 | TC05 | Past due date |
| SCRUM-7 | TC07 | Empty title during editing |
| SCRUM-8 | TC10 | Editing while offline |
| SCRUM-9 | TC20 | Refresh during task entry |

The issue records were reported as **Medium** priority and **In Progress** at the time of the exported data. Verify Jira for their current state.

## Testing approach

1. Identify functional scenarios and expected results.
2. Design positive, negative and edge-case tests.
3. Execute tests and record Pass/Fail.
4. Track observations in Jira.
5. Summarize execution results, limitations and follow-up actions.

## Caveats and next steps

- Verify ambiguous expected behavior against the actual product specification before calling an observation a defect.
- In particular, recheck whether a past due date is allowed, and whether unsaved input is expected to survive a refresh.
- TC20 was marked Fail even though the worksheet's expected result appears to describe loss of unsaved data on refresh. Reconcile this inconsistency.
- TC03 has inconsistent title/input lengths (101 versus 501 characters). Align its test data.
- Add actual result descriptions, screenshots, OS/browser/app version, and dates when available.
- The exported Jira issue type/workflow does not establish a fix or a successful retest.

## Portfolio note

This is an independent learning project, **not** an official Todoist QA engagement. No claim is made that Todoist defects have been independently confirmed.

## How to present this project in an interview

Explain how you translated requirements into test cases, selected edge cases, investigated mismatches between expected and actual results, and documented limitations rather than overstating findings.
