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
