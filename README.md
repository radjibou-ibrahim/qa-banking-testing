# Banking Application Testing

## 📌 Project Overview

This project is a Manual QA testing project based on a demo web banking application.

The objective is to simulate a realistic software testing lifecycle and demonstrate practical skills required for a Junior QA Manual Tester position.

The project covers the complete testing process, from requirements analysis to test execution, defect reporting, exploratory testing, and final test reporting.

---

## 🎯 Project Objectives

The main objectives of this project are to demonstrate the ability to:

- Analyze functional requirements
- Identify testable conditions
- Design test scenarios
- Design detailed test cases
- Prepare structured test data
- Execute manual functional tests
- Record actual test results
- Investigate unexpected behaviors
- Report confirmed defects using Jira
- Perform defect retesting
- Conduct exploratory testing
- Collect test evidence
- Maintain test traceability
- Prepare a professional test summary report

---

## 🏦 Application Under Test

**Application:** XYZ Bank

**Application Type:** Demo Web Banking Application

**URL:**

https://www.globalsqa.com/angularJs-protractor/BankingProject/#/login

The application provides two main user roles:

- Customer
- Bank Manager

### Customer Features

The customer area provides access to:

- Customer login
- Account selection
- Account information
- Account balance
- Transaction history
- Deposit
- Withdrawal
- Logout

### Bank Manager Features

The bank manager area provides access to:

- Add Customer
- Open Account
- View Customers

---

## 🧪 Testing Scope

This project focuses primarily on:

- Manual Functional Testing
- Exploratory Testing
- Positive Testing
- Negative Testing
- Boundary Value Analysis
- Equivalence Partitioning
- Basic regression testing
- Defect verification and retesting

### In Scope

The following functional areas are included:

1. Customer Authentication
2. Bank Manager Authentication
3. Customer Dashboard
4. Account Information
5. Account Balance
6. Transaction History
7. Deposit
8. Withdrawal
9. Customer and Account Management
10. Logout and Application Navigation

### Out of Scope

The following areas are excluded from this project:

- API Testing
- SQL / Database Testing
- Test Automation
- Performance Testing
- Security Testing
- Mobile Application Testing
- Inter-account Fund Transfer
- Beneficiary Management
- Notifications
- Account Statements

The out-of-scope features were excluded because they are not available in the selected demo application or are outside the current project objectives.

---

## 📋 Project Requirements

The project contains **10 functional requirements**.

| ID | Requirement | Priority |
|---|---|---|
| FR-001 | Customer Authentication | High |
| FR-002 | Bank Manager Authentication | High |
| FR-003 | Customer Dashboard | High |
| FR-004 | Account Information | High |
| FR-005 | Account Balance | Critical |
| FR-006 | Transaction History | High |
| FR-007 | Deposit | Critical |
| FR-008 | Withdrawal | Critical |
| FR-009 | Customer and Account Management | High |
| FR-010 | Logout and Application Navigation | High |

Detailed requirements are available in:

`00-Requirements/Requirements.md`

---

## 🧩 Test Design

The test design phase will include:

- **30 Test Scenarios**
- **40 Test Cases**
- Test Data

The following identification conventions are used:

| Artifact | ID Format |
|---|---|
| Requirement | FR-XXX |
| Test Scenario | SC-XXX |
| Test Case | TC-XXX |
| Exploratory Session | ET-XXX |
| Jira Defect | Real Jira Issue ID |

---

## 🔗 Traceability

Traceability is maintained throughout the testing lifecycle.

```text
Requirement
     ↓
Test Scenario
     ↓
Test Case
     ↓
Test Data
     ↓
Test Execution
     ↓
Defect
     ↓
Retest
     ↓
Regression
```

---

## 🧪 Test Execution Approach

Test execution will be performed manually against the live demo application.

For each test case, the following information will be recorded:

Test Case ID
Requirement ID
Test Scenario ID
Preconditions
Test Data
Test Steps
Expected Result
Actual Result
Status
Evidence
Defect ID, if applicable

---


## Test Statuses

| Status  | Meaning                                                     |
| ------- | ----------------------------------------------------------- |
| PASS    | Actual result matches the expected result                   |
| FAIL    | Actual result does not match the expected result            |
| BLOCKED | The test cannot be executed because of a blocking condition |

---

## 🐞 Defect Management

Unexpected behavior will not automatically be classified as a defect.

The following investigation process will be used:
``` text
Observation
     ↓
Reproduction
     ↓
Analysis
     ↓
Expected vs Actual Comparison
     ↓
Defect Confirmation
     ↓
Jira Bug
```
If the defect still exists:
RETEST
   ↓
REOPENED

---

## 🔍 Banking-Specific Testing Considerations

Special attention will be given to areas where incorrect behavior could affect account information or financial transactions.

Testing will include:

- Account balance consistency
- Deposit calculations
- Withdrawal calculations
- Withdrawal amount greater than balance
- Zero transaction amounts
- Negative transaction amounts
- Decimal transaction amounts
- Empty transaction amounts
- Transaction history updates
- Credit and Debit transaction types
- Account selection
- Customer selection
- Transaction date filtering
- Logout behavior
- Navigation between application areas

The application behavior will be verified through actual test execution rather than assumptions.

---

## 🧭 Exploratory Testing

Exploratory testing will be performed using structured testing charters.

Each exploratory session will contain:

Exploratory Session ID
Charter
Objective
Areas to Explore
Test Notes
Observations
Potential Anomalies
Investigation
Defect Confirmation
Jira Defect ID, if applicable
Evidence
Session Summary

Exploratory testing results will only contain observations from actual testing sessions.

---

## 📁 Project Structure
```
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
│   └── exploratory testing reports
│
├── 06-Evidence/
│   └── screenshots and test evidence
│
└── 07-Test-Summary/
    └── Test-Summary-Report.md
```

---

## 📸 Test Evidence

Screenshots and other test evidence collected during actual test execution will be stored in:

06-Evidence/

Evidence will be linked to the relevant test cases or defects whenever applicable.

---

## 🛠️ Tools

The project may use the following tools:

- Web Browser — Application testing
- Microsoft Excel / Google Sheets — Test scenarios, test cases, test data and execution
- Jira — Defect management
- GitHub — Version control and portfolio documentation
- Screenshots — Test evidence

---

## 🎓 Portfolio Purpose

This project is part of my QA Manual Testing portfolio.

It demonstrates my practical understanding of a complete software testing lifecycle.

---

⚠️ Disclaimer

XYZ Bank is a demo/training application used for educational and portfolio purposes.

No real financial transactions or sensitive banking information are used in this project.

All test results, defects, screenshots and execution evidence documented in this repository should be based on actual testing performed against the demo application.














