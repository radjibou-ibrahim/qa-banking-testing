# Test Summary Report — XYZ Bank

## 1. Document Information

| Field | Details |
|---|---|
| Application | XYZ Bank |
| Application Type | Web Banking Application |
| Test Type | Manual Functional Testing & Exploratory Testing |
| Test Level | System Testing |
| Tester | QA Manual Tester |
| Test Status | Completed |
| Report Status | Final |

---

# 2. Executive Summary

This report summarizes the manual testing activities performed on the
XYZ Bank web application.

The testing activities included requirements analysis, test planning,
test scenario design, test case design, test data preparation, test
execution, exploratory testing, and test evidence collection.

A total of 40 predefined test cases were executed.

Exploratory testing was also performed to investigate the main customer
banking workflow, boundary values, negative inputs, repeated operations,
and navigation behavior.

No confirmed functional defects were identified during the testing
activities performed within the defined project scope.

---

# 3. Application Under Test

### Application

XYZ Bank — Banking Project

### Application URL

https://www.globalsqa.com/angularJs-protractor/BankingProject/#/login

### Application Type

Web Banking Application

### Main Functional Areas Tested

- Customer Authentication
- Manager Authentication
- Customer Dashboard
- Account Information
- Account Balance
- Transaction History
- Deposit
- Withdrawal
- Customer Management
- Account Management
- Navigation
- Logout

---

# 4. Test Scope

## In Scope

The following functionalities were included in the testing scope:

- Customer login
- Manager login
- Customer dashboard
- Account selection
- Account information
- Account balance
- Transaction history
- Deposit
- Withdrawal
- Customer creation
- Account creation
- Navigation
- Logout
- Boundary and negative input exploration

## Out of Scope

The following areas were not tested:

- API testing
- SQL/database testing
- Test automation
- Performance testing
- Mobile testing
- Inter-account fund transfers
- Beneficiary management
- Account statements
- Notifications
- Advanced security testing

---

# 5. Test Activities Performed

The following QA activities were completed:

| Activity | Status |
|---|---|
| Requirements Analysis | Completed |
| Test Planning | Completed |
| Test Scenario Design | Completed |
| Test Case Design | Completed |
| Test Data Preparation | Completed |
| Test Execution | Completed |
| Exploratory Testing | Completed |
| Evidence Collection | Completed |
| Defect Reporting | No confirmed defects |
| Test Summary | Completed |

---

# 6. Test Execution Summary

A total of **40 test cases** were executed.

| Status | Count | Percentage |
|---|---:|---:|
| PASS | 40 | 100% |
| FAIL | 0 | 0% |
| BLOCKED | 0 | 0% |
| NOT EXECUTED | 0 | 0% |
| **TOTAL** | **40** | **100%** |

### Pass Rate

**100%**

All 40 executed test cases produced results consistent with their
defined expected results.

---

# 7. Functional Coverage

The executed test cases covered the following requirements:

| Requirement | Functional Area | Test Cases | Result |
|---|---|---:|---|
| FR-001 | Customer Authentication | 4 | PASS |
| FR-002 | Manager Authentication | 3 | PASS |
| FR-003 | Customer Dashboard | 4 | PASS |
| FR-004 | Account Information | 4 | PASS |
| FR-005 | Account Balance | 4 | PASS |
| FR-006 | Transaction History | 5 | PASS |
| FR-007 | Deposit | 5 | PASS |
| FR-008 | Withdrawal | 5 | PASS |
| FR-009 | Customer and Account Management | 4 | PASS |
| FR-010 | Logout and Application Navigation | 2 | PASS |

---

# 8. Exploratory Testing Summary

Two exploratory testing sessions were completed.

## ET-SESSION-001 — Customer Banking Flow

The session explored:

- Customer Login
- Customer Dashboard
- Account Switching
- Deposit
- Withdrawal
- Transaction History
- Navigation
- Logout
- Session behavior

### Result

The explored customer banking workflow behaved consistently during the
session.

No confirmed functional defects were identified.

An additional observation related to session timeout was recorded for
further investigation.

---

## ET-SESSION-002 — Boundary and Negative Testing

The session explored:

- Deposit boundary values
- Withdrawal boundary values
- Numeric input
- Repeated operations
- Invalid operations followed by valid operations

### Result

The application displayed validation, success, or failure behavior
according to the inputs observed during the session.

No confirmed functional defects were identified.

---

# 9. Defect Summary

No confirmed defects were identified during the testing activities.

| Severity | Confirmed Defects |
|---|---:|
| Critical | 0 |
| High | 0 |
| Medium | 0 |
| Low | 0 |
| **Total** | **0** |

The `04-Bug-Reports/` folder therefore does not contain confirmed defect
reports for this test cycle.

---

# 10. Test Evidence

Test evidence was collected during the execution and exploratory testing
activities.

Evidence includes screenshots related to:

- Customer authentication
- Dashboard
- Account information
- Deposits
- Withdrawals
- Transaction history
- Manager functions
- Account management
- Exploratory testing observations

Evidence is stored in:

`06-Evidence/`

---

# 11. Key Observations

The following observations were made during testing:

- Customer authentication worked as expected.
- Manager authentication and management functions were accessible.
- Customer dashboard information corresponded to the selected account.
- Account switching updated the displayed account information.
- Successful deposits updated the balance.
- Successful withdrawals updated the balance.
- Withdrawals exceeding the available balance were rejected.
- Transaction history reflected successful banking operations.
- Invalid inputs were rejected during the explored scenarios.
- Customer and account creation functions worked successfully.
- Logout ended the authenticated customer session.
- No confirmed functional defects were identified.

---

# 12. Additional Observation

During exploratory testing, an automatic session timeout behavior was
observed after a period of inactivity.

The exact timeout duration was not formally measured during the
exploratory session.

Because no specific requirement defining the expected inactivity timeout
was available, this behavior was recorded as an observation rather than
classified as a defect.

Further investigation would be recommended if session timeout behavior
becomes part of the application's defined requirements.

---

# 13. Risks and Limitations

Although the planned functional tests were completed successfully, the
testing campaign has several limitations.

### Testing Scope

The project focused primarily on manual functional testing.

API, database, performance, automation, mobile, and advanced security
testing were outside the defined scope.

### Environment

Testing was performed against a public demo web application.

The behavior of a public demo environment may differ from a production
banking application.

### Security

No dedicated security testing was performed.

Therefore, the absence of identified defects should not be interpreted
as evidence that the application is secure.

### Test Data

Testing used available application data and tester-created data within
the demo environment.

---

# 14. Exit Criteria Assessment

| Exit Criterion | Status |
|---|---|
| Planned test cases executed | Met |
| Test execution results recorded | Met |
| Critical functional defects identified | None |
| High-severity functional defects identified | None |
| Exploratory testing completed | Met |
| Test evidence collected | Met |
| Test summary completed | Met |

---

# 15. Overall Test Assessment

Based on the testing activities performed within the defined scope, the
XYZ Bank application demonstrated consistent behavior across the tested
functional areas.

The 40 planned test cases were executed with:

- 40 PASS
- 0 FAIL
- 0 BLOCKED
- 0 NOT EXECUTED

Exploratory testing did not identify any confirmed functional defects.

The application is therefore considered to have **met the defined
functional test objectives for this portfolio test cycle**.

This conclusion applies only to the tested scope and environment.

---

# 16. Recommendations

The following activities are recommended for a more extensive testing
campaign:

- Perform API testing.
- Perform database validation.
- Perform dedicated security testing.
- Perform performance and load testing.
- Expand boundary value testing.
- Add browser compatibility testing.
- Add responsive/mobile testing.
- Define and test session timeout requirements.
- Perform regression testing after future application changes.
- Expand test coverage for additional banking workflows.

---

# 17. Traceability

The project follows the following QA traceability chain:

**Requirement → Test Scenario → Test Case → Test Data → Test Execution
→ Evidence → Bug / Retest**

This traceability allows each test result to be linked back to the
corresponding functional requirement.

---

# 18. Project Deliverables

The completed project includes:

```text
qa-banking-testing/
│
├── README.md
│
├── 00-Requirements/
│   └── Requirements.md
│
├── 01-Test-Planning/
│   └── Test-Plan.md
│
├── 02-Test-Design/
│   ├── Test-Scenarios.xlsx
│   ├── Test-Cases.xlsx
│   └── Test-Data.xlsx
│
├── 03-Test-Execution/
│   └── Test-Execution.xlsx
│
├── 04-Bug-Reports/
│
├── 05-Exploratory-Testing/
│   ├── README.md
│   ├── ET-Session-001.md
│   └── ET-Session-002.md
│
├── 06-Evidence/
│   └── README.md
│
└── 07-Test-Summary/
    └── Test-Summary-Report.md
```

---

# 19 Final Conclusion

The manual testing cycle for the XYZ Bank demo application was completed
successfully within the defined scope.

The planned functional test cases were executed and all 40 test cases
passed.

Exploratory testing was also performed to investigate additional
functional and boundary conditions.

No confirmed functional defects were identified during this test cycle.

The project demonstrates a complete manual QA workflow covering
requirements analysis, test planning, test design, test data preparation,
test execution, exploratory testing, evidence collection, defect
assessment, and test reporting.

---

# Disclaimer

This project was created for educational and portfolio purposes using a
public demo banking application.

The results and conclusions apply only to the tested application version,
test environment, data, and defined scope.

Successful execution of the tests does not guarantee that the application
is free from defects or suitable for production use. 
