# Banking Application — Functional Requirements

## 1. Document Information

| Item | Description |
|---|---|
| Project | Banking Application Testing |
| Application Under Test | XYZ Bank |
| Application Type | Web Banking Application |
| Environment | Demo / Training Environment |
| Testing Type | Manual Functional Testing |
| Document | Functional Requirements |
| Version | 1.0 |
| Status | Draft for Test Design |

---

# 2. Project Overview

This document defines the functional requirements identified for the XYZ Bank web application selected for the Manual QA Portfolio project.

The purpose of this document is to establish a clear and testable functional baseline for the following QA activities:

- Requirements Analysis
- Test Scenario Design
- Test Case Design
- Test Data Preparation
- Manual Test Execution
- Defect Reporting
- Exploratory Testing
- Test Summary Reporting

The requirements are based on the functionality available in the selected demo application and on the behaviors observed during the initial application reconnaissance.

The project focuses on Manual Functional Testing and Exploratory Testing.

---

# 3. Application Under Test

**Application:** XYZ Bank

**Application URL:**

https://www.globalsqa.com/angularJs-protractor/BankingProject/#/login

The application provides two main user roles:

- Customer
- Bank Manager

The customer area provides access to account-related operations such as:

- Account information
- Account balance
- Transaction history
- Deposits
- Withdrawals
- Account selection
- Logout

The bank manager area provides access to:

- Customer creation
- Account opening
- Customer list

---

# 4. Functional Scope

The following functional areas are included in the project scope:

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

---

# 5. Requirements

## FR-001 — Customer Authentication

### Description

The application shall provide a Customer Login functionality allowing registered customers to access their banking area.

### Functional Requirements

The system shall:

- provide access to the Customer Login functionality;
- display a list of available registered customers;
- allow a customer to be selected from the available list;
- display the Login button after a customer has been selected;
- allow the selected customer to log in;
- redirect the authenticated customer to the customer banking area.

### Acceptance Criteria

| ID | Acceptance Criterion |
|---|---|
| AC-001-01 | The Customer Login option is available from the application entry point. |
| AC-001-02 | A list of available customers is displayed. |
| AC-001-03 | The Login button is not displayed before a customer is selected. |
| AC-001-04 | Selecting a customer makes the Login button available. |
| AC-001-05 | A selected customer can access the customer banking area through Login. |

### Priority

**High**

---

# FR-002 — Bank Manager Authentication

### Description

The application shall provide a Bank Manager Login functionality allowing an authorized bank manager to access customer and account management functions.

### Functional Requirements

The system shall:

- provide access to the Bank Manager Login functionality;
- allow the bank manager to access the management area;
- provide access to customer management functions after successful access.

### Acceptance Criteria

| ID | Acceptance Criterion |
|---|---|
| AC-002-01 | The Bank Manager Login option is available from the application entry point. |
| AC-002-02 | A bank manager can access the manager area. |
| AC-002-03 | The manager area provides access to customer and account management functions. |

### Priority

**High**

---

# FR-003 — Customer Dashboard

### Description

The application shall provide an authenticated customer with a dashboard containing information and actions related to the selected bank account.

### Functional Requirements

The customer dashboard shall provide access to:

- customer identification;
- account selection;
- account number;
- account balance;
- account currency;
- Transactions;
- Deposit;
- Withdrawal;
- Logout.

### Acceptance Criteria

| ID | Acceptance Criterion |
|---|---|
| AC-003-01 | The authenticated customer's name is displayed. |
| AC-003-02 | An account selection control is available when applicable. |
| AC-003-03 | The selected account number is displayed. |
| AC-003-04 | The selected account balance is displayed. |
| AC-003-05 | The account currency is displayed. |
| AC-003-06 | Transactions, Deposit and Withdrawal actions are available. |
| AC-003-07 | The Logout option is available to the authenticated customer. |

### Priority

**High**

---

# FR-004 — Account Information

### Description

The application shall display the main information associated with the customer's selected bank account.

### Functional Requirements

For the selected account, the application shall display:

- Account Number;
- Balance;
- Currency.

When a customer has access to more than one account, the customer shall be able to select an available account.

### Acceptance Criteria

| ID | Acceptance Criterion |
|---|---|
| AC-004-01 | The account number displayed corresponds to the selected account. |
| AC-004-02 | The account balance displayed corresponds to the selected account. |
| AC-004-03 | The account currency is displayed. |
| AC-004-04 | Selecting another available account updates the displayed account information accordingly. |

### Priority

**High**

---

# FR-005 — Account Balance

### Description

The application shall display the current balance of the selected customer account and update the balance following successful account transactions.

### Functional Requirements

The system shall:

- display the current account balance;
- maintain the balance associated with the selected account;
- update the balance following a successful deposit;
- update the balance following a successful withdrawal.

### Acceptance Criteria

| ID | Acceptance Criterion |
|---|---|
| AC-005-01 | The current account balance is displayed on the customer dashboard. |
| AC-005-02 | The displayed balance corresponds to the selected account. |
| AC-005-03 | A successful deposit increases the account balance by the deposited amount. |
| AC-005-04 | A successful withdrawal decreases the account balance by the withdrawn amount. |
| AC-005-05 | A rejected withdrawal does not reduce the account balance. |

### Priority

**Critical**

---

# FR-006 — Transaction History

### Description

The application shall allow customers to view transactions associated with their selected account.

### Functional Requirements

The transaction history shall provide transaction information including:

- Date-Time;
- Amount;
- Transaction Type.

The transaction type shall identify the transaction as a credit or debit where applicable.

The transaction history shall provide date filtering functionality.

### Acceptance Criteria

| ID | Acceptance Criterion |
|---|---|
| AC-006-01 | The Transactions functionality is available to the customer. |
| AC-006-02 | The transaction history displays the Date-Time of transactions. |
| AC-006-03 | The transaction history displays the transaction Amount. |
| AC-006-04 | The transaction history displays the Transaction Type. |
| AC-006-05 | Credit transactions are identifiable as Credit. |
| AC-006-06 | Debit transactions are identifiable as Debit. |
| AC-006-07 | The customer can specify a date range for transaction filtering. |
| AC-006-08 | A Reset option is available for the transaction filter. |
| AC-006-09 | Transactions resulting from successful account operations are reflected in the transaction history. |

### Priority

**High**

---

# FR-007 — Deposit

### Description

The application shall allow an authenticated customer to deposit an amount into the selected bank account.

### Functional Requirements

The Deposit functionality shall provide:

- an amount input field;
- a Deposit action;
- confirmation of a successful deposit.

A successful deposit shall update the account balance and transaction history accordingly.

### Acceptance Criteria

| ID | Acceptance Criterion |
|---|---|
| AC-007-01 | The Deposit functionality is available from the customer dashboard. |
| AC-007-02 | An amount input field is displayed. |
| AC-007-03 | A Deposit action is available. |
| AC-007-04 | A valid deposit can be submitted. |
| AC-007-05 | A successful deposit displays a success confirmation. |
| AC-007-06 | A successful deposit updates the account balance accordingly. |
| AC-007-07 | A successful deposit is recorded in the transaction history as a credit transaction. |
| AC-007-08 | The application prevents submission when the required amount field is empty. |

### Priority

**Critical**

---

# FR-008 — Withdrawal

### Description

The application shall allow an authenticated customer to withdraw an amount from the selected bank account, subject to available account balance.

### Functional Requirements

The Withdrawal functionality shall provide:

- an amount input field;
- a Withdraw action;
- confirmation of a successful withdrawal;
- validation preventing a withdrawal greater than the available account balance.

### Business Rules

| ID | Business Rule |
|---|---|
| BR-008-01 | A customer cannot withdraw an amount greater than the available account balance. |
| BR-008-02 | A successful withdrawal decreases the account balance by the withdrawn amount. |
| BR-008-03 | A successful withdrawal is recorded as a debit transaction. |

### Acceptance Criteria

| ID | Acceptance Criterion |
|---|---|
| AC-008-01 | The Withdrawal functionality is available from the customer dashboard. |
| AC-008-02 | An amount input field is displayed. |
| AC-008-03 | A Withdraw action is available. |
| AC-008-04 | A valid withdrawal can be submitted. |
| AC-008-05 | A successful withdrawal displays a success confirmation. |
| AC-008-06 | A successful withdrawal updates the account balance accordingly. |
| AC-008-07 | A withdrawal greater than the available balance is rejected. |
| AC-008-08 | The application displays an appropriate message when a withdrawal exceeds the available balance. |
| AC-008-09 | A rejected withdrawal does not reduce the account balance. |
| AC-008-10 | The application prevents submission when the required amount field is empty. |

### Priority

**Critical**

---

# FR-009 — Customer and Account Management

### Description

The application shall provide bank managers with functions to manage customers and their bank accounts.

### Functional Requirements

The Bank Manager area shall provide access to:

- Add Customer;
- Open Account;
- Customers.

The manager shall be able to:

- create a customer;
- open an account for a customer;
- view available customer information.

### Acceptance Criteria

| ID | Acceptance Criterion |
|---|---|
| AC-009-01 | The Add Customer functionality is available to the bank manager. |
| AC-009-02 | The manager can enter customer information required by the application. |
| AC-009-03 | The manager can submit a new customer record. |
| AC-009-04 | The Open Account functionality is available to the bank manager. |
| AC-009-05 | The manager can select a customer when opening an account. |
| AC-009-06 | The manager can select an available currency when applicable. |
| AC-009-07 | The Customers functionality is available. |
| AC-009-08 | Customer information can be viewed from the Customers area. |

### Priority

**High**

---

# FR-010 — Logout and Application Navigation

### Description

The application shall provide navigation controls that allow users to move between available application areas and terminate an authenticated customer session.

### Functional Requirements

The application shall provide:

- Home navigation;
- Customer Login navigation;
- Bank Manager Login navigation;
- Logout functionality for authenticated customers.

### Acceptance Criteria

| ID | Acceptance Criterion |
|---|---|
| AC-010-01 | The Home navigation is available where applicable. |
| AC-010-02 | The Customer Login area can be accessed from the application navigation. |
| AC-010-03 | The Bank Manager Login area can be accessed from the application navigation. |
| AC-010-04 | The Logout option is available to authenticated customers. |
| AC-010-05 | Selecting Logout returns the customer to an unauthenticated application area. |
| AC-010-06 | After logout, the customer dashboard is no longer displayed as the active authenticated area. |

### Priority

**High**

---

# 6. Observed Behaviors from Initial Reconnaissance

The following behaviors were observed during the initial application exploration.

These observations are recorded as **test observations**, not confirmed defects.

| Area | Observation |
|---|---|
| Customer Login | A list of available customers is displayed. |
| Customer Login | The Login button appears after selecting a customer. |
| Customer Login | The Login button is not displayed before selecting a customer. |
| Deposit | The Deposit page contains an amount field and a Deposit button. |
| Deposit | A successful deposit displays "Deposit Successful". |
| Deposit | An empty deposit field triggers a required-field browser validation. |
| Deposit | No error message was observed when entering `0`. |
| Deposit | No error message was observed when entering a negative value. |
| Withdrawal | The Withdrawal page contains an amount field and a Withdraw button. |
| Withdrawal | A successful withdrawal displays "Transaction successful". |
| Withdrawal | A withdrawal greater than the available balance is rejected. |
| Withdrawal | The application displays a message indicating that the withdrawal cannot exceed the balance. |
| Withdrawal | An empty withdrawal field triggers a required-field browser validation. |
| Withdrawal | Decimal input was rejected by the browser's numeric input validation in the tested environment. |
| Withdrawal | No error message was observed when entering `0`. |
| Withdrawal | No error message was observed when entering a negative value. |
| Transactions | Transaction history displays Date-Time, Amount and Transaction Type. |
| Transactions | Credit and Debit transaction types were observed. |
| Transactions | A date range filter is available. |
| Transactions | A Reset option is available. |

These observations will be used to guide Test Scenario and Test Case design.

They must not be interpreted as final PASS/FAIL results.

---

# 7. Known Business Rules

The following business rule was explicitly observed during reconnaissance:

### BR-008-01 — Withdrawal Balance Restriction

A customer cannot withdraw an amount greater than the available account balance.

The application displays the following observed message when this condition occurs:

> "Transaction Failed. You can not withdraw amount more than the balance."

Additional business rules concerning:

- zero amounts;
- negative amounts;
- decimal amounts;
- minimum transaction amounts;
- maximum transaction amounts;

have not yet been formally established and will be investigated during test design and execution.

---

# 8. Out of Scope

The following functionalities are outside the scope of this project because they are not available or have not been identified in the selected application:

- Inter-account fund transfers;
- Beneficiary management;
- Notifications;
- Account statements;
- API testing;
- SQL/database testing;
- Automation testing;
- Performance testing;
- Security testing;
- Mobile application testing.

These areas may be considered in a future project if the application or project scope is expanded.

---

# 9. Assumptions

The following assumptions apply to this project:

1. The application is a training/demo banking application and does not process real financial transactions.
2. Test accounts and customer data available in the application may be used for testing purposes.
3. The application behavior may differ from a production banking system.
4. Business rules not explicitly documented or observed will not be assumed to be defects.
5. Browser-level validation will be distinguished from application-level business validation where possible.
6. Test results will only be recorded after the corresponding test has been manually executed.
7. Defects will only be reported in Jira after reproduction and confirmation.
8. Actual Jira issue IDs will be recorded only after Jira generates them.

---

# 10. Requirement Priorities

The requirements are prioritized according to their functional and business impact within the demo banking application.

| Priority | Meaning |
|---|---|
| Critical | Failure may affect financial account information or financial transactions. |
| High | Important functionality required for normal application usage. |
| Medium | Supporting functionality with limited business impact. |
| Low | Minor functionality or usability-related functionality. |

Current requirement priorities:

| Requirement | Priority |
|---|---|
| FR-001 — Customer Authentication | High |
| FR-002 — Bank Manager Authentication | High |
| FR-003 — Customer Dashboard | High |
| FR-004 — Account Information | High |
| FR-005 — Account Balance | Critical |
| FR-006 — Transaction History | High |
| FR-007 — Deposit | Critical |
| FR-008 — Withdrawal | Critical |
| FR-009 — Customer and Account Management | High |
| FR-010 — Logout and Application Navigation | High |

---

# 11. Requirements Traceability

Requirements will be linked to the corresponding test scenarios and test cases during the Test Design phase.

The planned traceability structure is:

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
