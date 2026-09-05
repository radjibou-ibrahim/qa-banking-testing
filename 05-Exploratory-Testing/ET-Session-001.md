# Exploratory Testing Session 001 — Customer Banking Flow

## Session Information

| Field | Details |
|---|---|
| Session ID | ET-SESSION-001 |
| Application | XYZ Bank |
| Application Type | Web Banking Application |
| Test Type | Exploratory Testing |
| Area | Customer Banking Flow |
| Tester | QA Manual Tester |
| Status | Planned |

---

## Test Environment

| Item | Details |
|---|---|
| Application | XYZ Bank |
| Environment | Public Demo Web Application |
| Application URL | https://www.globalsqa.com/angularJs-protractor/BankingProject/#/login |
| Test Type | Manual Exploratory Testing |
| Platform | Web |
| Browser | To be recorded during execution |
| Browser Version | To be recorded during execution |
| Operating System | To be recorded during execution |
| Network | Internet connection |
| Test Data | Application-provided and tester-created data |

---

## 1. Exploratory Charter

### Objective

Explore the main customer banking journey to identify unexpected behaviors,
functional inconsistencies, usability issues, and risks that may not have
been covered by the predefined test cases.

### Mission

Explore the application from the perspective of an authenticated customer,
starting from customer login and continuing through the main banking
functions until logout.

The exploration should focus on how the different customer functions
work together rather than only verifying individual requirements.

---

## 2. Scope

The following areas will be explored:

- Customer Login
- Customer Dashboard
- Account Selection
- Account Information
- Balance
- Transactions
- Deposit
- Withdrawal
- Navigation between customer functions
- Logout

---

## 3. Exploration Areas

### 3.1 Customer Login

Explore:

- Selecting a registered customer
- Logging in
- Login behavior after customer selection
- Navigation after login
- Returning to the login area
- Repeated login attempts

Questions to consider:

- Is the selected customer correctly identified?
- Does the application always redirect to the correct dashboard?
- Is any unexpected information displayed?
- Does navigation behave consistently?

---

### 3.2 Customer Dashboard

Explore:

- Customer name
- Account selector
- Account Number
- Balance
- Currency
- Transactions button
- Deposit button
- Withdrawal button
- Logout button

Questions to consider:

- Are all expected elements displayed?
- Are the elements accessible?
- Does the displayed information correspond to the selected account?
- What happens when switching between accounts?
- Does the dashboard remain consistent after performing an operation?

---

### 3.3 Account Switching

If the customer has more than one account, explore:

1. Select the first account.
2. Record the displayed Account Number, Balance, and Currency.
3. Switch to another account.
4. Compare the displayed information.
5. Switch back to the first account.
6. Verify whether the information remains consistent.

Questions to consider:

- Does the account information update immediately?
- Does the balance correspond to the selected account?
- Does the currency correspond to the selected account?
- Is any information from the previous account incorrectly retained?

---

### 3.4 Deposit

Explore the Deposit functionality using different inputs.

Test at least:

- A normal positive amount
- `0`
- A negative amount
- An empty value
- A decimal value, if accepted by the field
- A relatively large positive amount

For each input, observe:

- Message displayed
- Balance
- Transaction history
- Transaction type
- Application behavior after returning to the dashboard

Questions to consider:

- Is the transaction processed correctly?
- Is the balance updated correctly?
- Is a transaction recorded when expected?
- Is an appropriate validation message displayed?
- Does the application behave consistently for unusual values?

---

### 3.5 Withdrawal

Explore the Withdrawal functionality using different inputs.

Test at least:

- A valid amount below the available balance
- An amount equal to the available balance
- An amount greater than the available balance
- `0`
- A negative amount
- An empty value
- A decimal value, if accepted by the field

For each input, observe:

- Message displayed
- Balance
- Transaction history
- Transaction type
- Application behavior after the operation

Questions to consider:

- Is a valid withdrawal processed correctly?
- Is an excessive withdrawal rejected?
- Does the balance remain unchanged when the withdrawal is rejected?
- Are invalid values prevented from creating transactions?

---

### 3.6 Transaction History

Explore:

- Opening transaction history
- Existing transactions
- Date-Time
- Amount
- Transaction Type
- Credit transactions
- Debit transactions
- Date filtering
- Reset
- Pagination

Questions to consider:

- Are newly created transactions displayed?
- Are Credit and Debit transactions represented correctly?
- Does filtering return the expected transactions?
- Does Reset restore the expected state?
- Does pagination behave correctly?
- Is any transaction missing or duplicated?

---

### 3.7 Navigation

Explore navigation between:

- Dashboard
- Transactions
- Deposit
- Withdrawal
- Customer Login
- Logout

Questions to consider:

- Can the customer navigate back and forth without unexpected behavior?
- Is the correct account context maintained?
- Are pages loaded correctly?
- Does the application lose information unexpectedly?

---

### 3.8 Logout

Explore:

1. Log in as a customer.
2. Navigate through several customer functions.
3. Click Logout.
4. Observe the resulting page.
5. Attempt to access customer banking functions again through normal navigation.

Questions to consider:

- Does the session end correctly?
- Is the customer returned to the appropriate page?
- Can the customer still access authenticated functions unexpectedly?
- Is any previous customer information still displayed?

---

# 4. Observation Guidelines

During the session, do not immediately classify an unexpected behavior
as a defect.

Use the following process:

**Observation → Reproduction → Investigation → Expected vs Actual → Defect Decision**

For every unexpected behavior, record:

- What was tested?
- What input was used?
- What happened?
- Can the behavior be reproduced?
- What was expected?
- What was actually observed?
- Is the behavior really a defect?

---

# 5. Evidence

Screenshots should be captured when they provide useful evidence.

Recommended evidence includes:

- Unexpected messages
- Validation behavior
- Transaction results
- Balance changes
- Transaction history changes
- Navigation problems
- Unexpected application states

Evidence will be stored in:

`06-Evidence/`

---

# 6. Defect Handling

If an unexpected behavior is identified:

1. Reproduce the behavior.
2. Verify whether it occurs consistently.
3. Compare the actual behavior with the expected behavior.
4. Determine whether it represents a defect.
5. Record the observation.
6. If confirmed, create a bug report in:

`04-Bug-Reports/`

Do not create a bug report based only on an assumption.

---

# 7. Session Notes

The following information should be recorded during the exploration:

| ID | Area | Action / Input | Observation | Result | Evidence |
|---|---|---|---|---|---|
| OBS-001 | | | | | |
| OBS-002 | | | | | |
| OBS-003 | | | | | |
| OBS-004 | | | | | |
| OBS-005 | | | | | |
| OBS-006 | | | | | |
| OBS-007 | | | | | |
| OBS-008 | | | | | |

---

# 8. Session Conclusion

### Summary

_To be completed after the exploratory session._

### Areas Explored

_To be completed after the exploratory session._

### Unexpected Behaviors

_To be completed after the exploratory session._

### Confirmed Defects

_To be completed after the exploratory session._

### Risks / Observations

_To be completed after the exploratory session._

### Final Assessment

_To be completed after the exploratory session._

---

## Important Note

Exploratory testing results must be based on actual observations made
during the session.

No defect, result, or application behavior should be added to this report
without evidence from the exploratory session.
