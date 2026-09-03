# Banking Application — Test Plan

## 1. Document Information

| Item | Description |
|---|---|
| Project | Banking Application Testing |
| Application Under Test | XYZ Bank |
| Application Type | Demo Web Banking Application |
| Test Level | System Testing |
| Testing Type | Manual Functional Testing |
| Additional Testing | Exploratory Testing |
| Test Plan Version | 1.0 |
| Status | Draft |
| Requirements | 10 |
| Planned Test Scenarios | 30 |
| Planned Test Cases | 40 |

---

## 2. Test Plan Overview

This Test Plan defines the strategy, scope, objectives, resources, risks and activities required to test the XYZ Bank demo web application.

The purpose of the test campaign is to evaluate whether the main banking functions behave according to the defined functional requirements and expected business rules.

Testing will be performed manually using the selected demo application.

The project will follow a structured testing lifecycle:
```text
Requirements Analysis
        ↓
Test Planning
        ↓
Test Scenario Design
        ↓
Test Case Design
        ↓
Test Data Preparation
        ↓
Test Execution
        ↓
Defect Investigation
        ↓
Defect Reporting
        ↓
Retesting
        ↓
Regression Testing
        ↓
Exploratory Testing
        ↓
Test Summary
```

---

## 3. Test Objectives

The main objectives of this test campaign are to:

verify the main functional requirements of the application;
verify customer authentication;
verify bank manager access;
verify customer account information;
verify account balance behavior;
verify transaction history;
verify deposit functionality;
verify withdrawal functionality;
verify customer and account management;
verify logout and application navigation;
identify functional defects;
verify that confirmed defects are reproducible;
document actual test results;
maintain traceability between requirements, scenarios, test cases and defects.

The project also aims to demonstrate practical Manual QA skills in a realistic banking domain.

---

## 4. Scope

### 4.1 In Scope

The following functional areas are included in the test campaign:

Customer Authentication
Bank Manager Authentication
Customer Dashboard
Account Information
Account Balance
Transaction History
Deposit
Withdrawal
Customer and Account Management
Logout and Application Navigation

Testing will include:

Functional Testing
Positive Testing
Negative Testing
Boundary Value Analysis
Equivalence Partitioning
Data Validation Testing
Integration-oriented functional checks between related UI functions
Regression Testing of corrected defects
Exploratory Testing

### 4.2 Out of Scope

The following areas are explicitly excluded from this project:

API Testing
SQL / Database Testing
Test Automation
Performance Testing
Security Testing
Mobile Application Testing
Inter-account Fund Transfer
Beneficiary Management
Notifications
Account Statements

These areas are excluded because they are either unavailable in the selected demo application or outside the objectives of this portfolio project.

---

## 5. Features to Be Tested
### 5.1 Customer Authentication

Testing will verify:

- Customer Login access;
- customer selection;
- Login button behavior;
- successful customer access;
- navigation to the customer area.

### 5.2 Bank Manager Authentication

Testing will verify:

- Bank Manager Login access;
- access to the manager area;
- availability of management functions.

### 5.3 Customer Dashboard

Testing will verify:

- customer name display;
- account selection;
- account number display;
- balance display;
- currency display;
- availability of Transactions;
- availability of Deposit;
- availability of Withdrawal;
- Logout availability.

### 5.4 Account Information

Testing will verify:

- account number;
- selected account;
- balance;
- currency;
- consistency of displayed account information when changing the selected account.

### 5.5 Account Balance

Testing will verify:

- initial balance display;
- balance consistency;
- balance after successful deposits;
- balance after successful withdrawals;
- balance after rejected transactions.

### 5.6 Transaction History

Testing will verify:

- transaction availability;
- Date-Time;
- Amount;
- Transaction Type;
- Credit transactions;
- Debit transactions;
- date filtering;
- Reset functionality;
- transaction history updates following account operations.

### 5.7 Deposit

Testing will verify:

- Deposit page accessibility;
- amount field;
- valid amounts;
- decimal values;
- zero values;
- negative values;
- empty values;
- successful deposit behavior;
- balance update;
- transaction history update.

### 5.8 Withdrawal

Testing will verify:

- Withdrawal page accessibility;
- amount field;
- valid withdrawal;
- decimal values;
- zero values;
- negative values;
- empty values;
- withdrawal greater than available balance;
- successful withdrawal behavior;
- balance update;
- transaction history update.

### 5.9 Customer and Account Management

Testing will verify:

- Add Customer;
- customer data entry;
- customer creation;
- Open Account;
- customer selection during account creation;
- currency selection where applicable;
- Customers list;
- customer information display.
  
### 5.10 Logout and Navigation

Testing will verify:

- Home navigation;
- Customer Login navigation;
- Bank Manager Login navigation;
- Logout;
- navigation after logout;
- access to the customer area after logout.

  ---
  
## 6. Test Approach

The project will use a risk-based and requirement-driven testing approach.

Testing will start with the highest-risk banking functions, particularly:

1. Account Balance
2. Deposit
3. Withdrawal
4. Transaction History
5. Authentication

Supporting functionality such as navigation and management functions will also be covered.

Test cases will be designed from the identified functional requirements.

---

## 7. Test Design Techniques

The following test design techniques will be used where applicable.

### 7.1 Equivalence Partitioning

Input data will be divided into meaningful classes.

For example, transaction amounts may be divided into:

- valid positive values;
- zero;
- negative values;
- empty values;
- decimal values;
- values exceeding the available balance.
  
### 7.2 Boundary Value Analysis

Boundary values will be considered for transaction-related functionality.

Examples include:

- zero;
- minimum valid amount if identified;
- amount equal to the available balance;
- amount greater than the available balance.

Actual boundaries will only be defined when supported by application behavior or documented business rules.

### 7.3 Negative Testing

Invalid or unexpected input conditions will be tested to evaluate how the application handles them.

Examples include:

- empty amount;
- zero amount;
- negative amount;
- amount greater than available balance;
- invalid input formats.

### 7.4 State-Based Testing
```text
State changes will be considered for functions such as:
Unauthenticated
      ↓
Authenticated
      ↓
Transaction
      ↓
Updated Account State
      ↓
Logout
      ↓
Unauthenticated
```

---

## 8. Test Scenario and Test Case Strategy

The project will contain:

- 30 Test Scenarios
- 40 Test Cases

The test scenarios will describe high-level conditions to be verified.

---

## 10. Test Data Strategy
The test data will include, where applicable:

- customer accounts;
- account numbers;
- customer names;
- currencies;
- valid transaction amounts;
- zero amounts;
- negative amounts;
- decimal amounts;
- amounts greater than available balance;
- customer information required for account creation.

Test data will be selected to support both positive and negative test conditions.

Actual account values observed during testing will be recorded accurately.

---

## 11. Test Environment

Testing will be performed against the XYZ Bank demo web application.

Application: XYZ Bank

URL: https://www.globalsqa.com/angularJs-protractor/BankingProject/#/login

Client Environment:

- Desktop web browser
- Mobile web browser when applicable for exploratory observation

The browser, operating system and relevant environment information will be recorded during test execution when required.

---

## 12. Entry Criteria

Testing may begin when the following conditions are satisfied:

- The application is accessible.
- The main application areas are available.
- Functional requirements have been identified.
- Test scenarios have been designed.
- Test cases have been reviewed.
- Required test data is available.
- The test environment is accessible.

  ---
  
## 13. Exit Criteria

The test cycle may be considered complete when:

- all planned executable test cases have been executed or formally marked as BLOCKED;
- actual results have been recorded;
- failed test cases have been investigated;
- confirmed defects have been reported in Jira;
- applicable defect retesting has been completed;
- regression testing has been performed where necessary;
- test evidence has been collected;
- the final test summary report has been prepared.

The exit criteria may be adjusted if significant blocking issues prevent completion of the planned testing scope.

---

## 14. Test Execution

Test execution will be performed manually.
Each test case will receive one of the following statuses:

### PASS

A test case is considered PASS when:

- The actual result matches the expected result.
- No unexpected behavior is observed.

### FAIL

A test case is considered FAIL when:

- The actual result differs from the expected result.
- The observed behavior violates a defined requirement.

### BLOCKED

A test case is considered BLOCKED when:

- Testing cannot be completed because of another defect, environment issue, missing data, or unavailable functionality.

### NOT RUN

A test case is considered NOT RUN when:

- The test has not yet been executed.

---

## 15. Defect Management

```text
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
A Jira defect will only be created after sufficient investigation and reproduction.

### Defect Lifecycle
```text
OPEN
  ↓
IN PROGRESS
  ↓
FIXED
  ↓
READY FOR RETEST
  ↓
RETEST
  ↓
VERIFIED
```
If the defect is still present:
```text
RETEST
   ↓
REOPENED
```
Jira issue IDs will only be recorded after the issue is actually created in Jira.

---

## 16. Regression Testing

Regression testing will be performed after confirmed defects have been fixed.

The objective is to verify that:
- the reported defect has been resolved;
- related functionality still works;
- previously working functionality has not been negatively affected.
Regression scope will be determined based on the affected functionality.

## 17. Exploratory Testing

Exploratory Testing will complement scripted functional testing.

Exploratory sessions will use testing charters.

Each session will define:

- Session ID;
- Charter;
- Objective;
- Areas to explore;
- Time/session information;
- Observations;
- Potential anomalies;
- Investigation;
- Confirmed defects;
- Evidence;
- Session summary.

---

## 18. Risk Assessment

| Risk                                          | Impact   | Probability | Mitigation                                                      |
| --------------------------------------------- | -------- | ----------- | --------------------------------------------------------------- |
| Application becomes unavailable               | High     | Medium      | Record the environment issue and mark affected tests as BLOCKED |
| Demo data changes unexpectedly                | Medium   | Medium      | Record the test data used for each execution                    |
| Application behavior differs between sessions | Medium   | Medium      | Capture actual observations and test evidence                   |
| Transaction-related defect                    | Critical | Medium      | Prioritize balance, deposit and withdrawal testing              |
| Incorrect balance calculation                 | Critical | Medium      | Verify balance before and after transactions                    |
| Transaction history inconsistency             | High     | Medium      | Compare successful transactions with transaction history        |
| Browser validation affects test results       | Medium   | Medium      | Distinguish browser validation from application behavior        |
| Insufficient test coverage                    | High     | Low         | Maintain Requirement → Scenario → Test Case traceability        |
| Unconfirmed anomaly reported as a defect      | High     | Low         | Require reproduction and analysis before Jira reporting         |

---

## 19. Traceability

Traceability will be maintained throughout the project.
```text

FR-XXX
   ↓
SC-XXX
   ↓
TC-XXX
   ↓
Test Data
   ↓
Test Execution
   ↓
Jira Defect
   ↓
Retest
   ↓
Regression
```

The following ID conventions will be used:

| Artifact            | ID Convention      |
| ------------------- | ------------------ |
| Requirement         | FR-XXX             |
| Test Scenario       | SC-XXX             |
| Test Case           | TC-XXX             |
| Exploratory Session | ET-XXX             |
| Jira Defect         | Real Jira Issue ID |

---

## 20. Test Evidence

Evidence will be collected during actual test execution.

Evidence may include:

- screenshots;
- relevant application messages;
- transaction information;
- account balance before and after an operation;
- Jira defect evidence.

## 21. Deliverables

The project will produce the following deliverables:
| Deliverable         | Location                                 |
| ------------------- | ---------------------------------------- |
| Requirements        | `00-Requirements/Requirements.md`        |
| Test Plan           | `01-Test-Planning/Test-Plan.md`          |
| Test Scenarios      | `02-Test-Design/Test-Scenarios.xlsx`     |
| Test Cases          | `02-Test-Design/Test-Cases.xlsx`         |
| Test Data           | `02-Test-Design/Test-Data.xlsx`          |
| Test Execution      | `03-Test-Execution/Test-Execution.xlsx`  |
| Bug Reports         | `04-Bug-Reports/`                        |
| Exploratory Testing | `05-Exploratory-Testing/`                |
| Test Evidence       | `06-Evidence/`                           |
| Test Summary        | `07-Test-Summary/Test-Summary-Report.md` |

---

## 22. Roles and Responsibilities

This project is conducted as an individual QA portfolio project.

## QA Tester

Responsibilities include:

- requirements analysis;
- test planning;
- test design;
- test data preparation;
- test execution;
- defect investigation;
- Jira defect reporting;
- retesting;
- regression testing;
- exploratory testing;
- evidence collection;
- test reporting.

---

## 23. Test Schedule

The project will be completed progressively through the following phases:
| Phase | Activity                           |
| ----- | ---------------------------------- |
| 1     | Requirements Analysis              |
| 2     | Test Planning                      |
| 3     | Test Scenario Design               |
| 4     | Test Case Design                   |
| 5     | Test Data Preparation              |
| 6     | Test Execution                     |
| 7     | Defect Investigation and Reporting |
| 8     | Retesting and Regression           |
| 9     | Exploratory Testing                |
| 10    | Test Summary                       |
The exact execution timeline may be adjusted according to the availability of the application and the progress of the testing activities.

---

## 24. Test Completion Criteria

The project will be considered complete when the planned testing activities have been performed and documented.

The final project should provide evidence of:

- requirements-based testing;
- structured test design;
- real manual test execution;
- documented actual results;
- confirmed and reproducible defects where applicable;
- professional Jira defect management;
- retesting;
- exploratory testing;
- traceability;
- final test reporting.

  
## 25. Final QA Principle

The project follows an evidence-based testing approach.

No test result, defect, screenshot, Jira issue or execution outcome will be invented.

All execution results will be based on actual observations made while testing the XYZ Bank application.

Unexpected behavior will be investigated before being classified as a defect.

The objective is to demonstrate a realistic and professional Manual QA workflow.


