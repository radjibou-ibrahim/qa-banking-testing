# Exploratory Testing Session 001 — Customer Banking Flow

## 1. Session Information

| Field | Details |
|---|---|
| Session ID | ET-SESSION-001 |
| Application | XYZ Bank |
| Application Type | Web Banking Application |
| Test Type | Manual Exploratory Testing |
| Tester | QA Manual Tester |
| Status | Completed |

---

## 2. Test Environment

| Item | Details |
|---|---|
| Application | XYZ Bank |
| Environment | Public Demo Web Application |
| Application URL | https://www.globalsqa.com/angularJs-protractor/BankingProject/#/login |
| Platform | Web |
| Browser | chrome|
| Browser Version | 152.0.7977.64 (iOS)|
| Network | Internet connection |

---

## 3. Exploratory Charter

### Objective

Explore the main customer banking journey to identify unexpected behaviors,
functional inconsistencies, usability issues, and risks that may not have
been covered by the predefined test cases.

### Mission

Explore the application from the perspective of an authenticated customer,
starting from customer login and continuing through the main banking
functions until logout.

The exploration focuses on how the different customer functions work
together rather than only verifying individual requirements.

---

# 4. Exploration Results

## Exploration 1 — Customer Login

### Actions

- Select a registered customer
- Log in
- Observe login behavior after customer selection
- Navigate after login
- Return to the login area
- Perform a repeated login attempt

### Observation

Navigation is smooth, and each opened page corresponds to the selected
action. The authenticated customer corresponds to the selected customer.

### Status

**PASS**

---

## Exploration 2 — Customer Dashboard

### Actions

- Customer name
- Account selector
- Account Number
- Balance
- Currency
- Transactions button
- Deposit button
- Withdrawal button
- Logout button

### Observation

All expected elements are displayed. The buttons are functional and are
associated with their corresponding actions.

### Status

**PASS**

---

## Exploration 3 — Account Switching

### Actions

1. Select the first account.
2. Record the displayed Account Number, Balance, and Currency.
3. Switch to another account.
4. Compare the displayed information.
5. Switch back to the first account.
6. Verify whether the information remains consistent.

### Observation

The Account Number, Balance, Currency, and transaction information
correspond to the selected account. The information is automatically
updated when switching between accounts.

### Status

**PASS**

---

## Exploration 4 — Deposit and Withdrawal

### Actions

The following input types were explored for deposit and withdrawal:

- Normal positive amount
- `0`
- Negative amount
- Empty value
- Decimal value
- Relatively large positive amount

### Observation

The balance increases after a successful deposit and decreases after a
successful withdrawal according to the transaction amount.

Invalid or unsupported inputs, including negative amounts, amounts
exceeding the available balance, empty values, and decimal values where
not accepted, are rejected. Appropriate validation or transaction
messages are displayed depending on the input.

### Status

**PASS**

---

## Exploration 5 — Transaction History

### Actions

- Open transaction history
- Review existing transactions
- Verify Date-Time
- Verify Amount
- Verify Transaction Type
- Review Credit transactions
- Review Debit transactions
- Apply date filtering
- Use Reset
- Explore pagination

### Observation

The transaction history is displayed correctly with the transaction date
and time, amount, and transaction type. Date filtering is available, and
the transaction history can be navigated using the available controls.

### Status

**PASS**

---

## Exploration 6 — Navigation

### Actions

- Dashboard
- Transactions
- Deposit
- Withdrawal
- Customer Login
- Logout

### Observation

The customer can navigate between the available banking functions without
unexpected behavior. The selected account context is correctly maintained
during navigation.

### Status

**PASS**

---

## Exploration 7 — Logout and Session Behavior

### Actions

1. Log in as a customer.
2. Navigate through several customer functions.
3. Click **Logout**.
4. Observe the resulting page.
5. Attempt to access the customer dashboard again without logging in.

### Observation

After clicking **Logout**, the customer is returned to the appropriate
page and the session ends correctly. The customer cannot access the
banking dashboard without logging in again.

### Status

**PASS**

---

## Additional Observation — Session Timeout

During the exploratory session, an automatic session timeout behavior was
observed after a period of inactivity.

The exact timeout duration was not measured during this session.

### Status

**Observation — Further Investigation**

This behavior was not included in the predefined test cases and was
therefore recorded as an exploratory observation.

The exact inactivity timeout should be verified before documenting a
specific duration.

---

# 5. Observation Summary

| Exploration | Area | Result |
|---|---|---|
| Exploration 1 | Customer Login | PASS |
| Exploration 2 | Customer Dashboard | PASS |
| Exploration 3 | Account Switching | PASS |
| Exploration 4 | Deposit & Withdrawal | PASS |
| Exploration 5 | Transaction History | PASS |
| Exploration 6 | Navigation | PASS |
| Exploration 7 | Logout & Session Behavior | PASS |
| Additional Observation | Session Timeout | Further Investigation |

---

# 6. Unexpected Behaviors

No confirmed functional defects were identified during this exploratory
session.

An additional observation related to session timeout was identified and
recorded for further investigation.

---

# 7. Defect Assessment

No defect was created in the `04-Bug-Reports/` section based on the
observations from this session.

The session timeout behavior was not classified as a defect because no
specific requirement defining the expected inactivity timeout was
available.

---

# 8. Evidence

Relevant screenshots and test evidence can be stored in:

`06-Evidence/`

Evidence should be referenced when it provides useful support for an
observation or unexpected behavior.

---

# 9. Conclusion

The main customer banking journey was explored, including authentication,
dashboard navigation, account switching, deposits, withdrawals,
transaction history, navigation, and logout.

The explored functionalities behaved consistently with the expected
customer banking workflow.

No confirmed functional defects were identified during the session.

An additional observation concerning session inactivity was identified
and should be investigated further if session timeout behavior is within
the application's requirements or expected behavior.

---

## 10. QA Notes

Exploratory testing results are based on observations made during the
session.

Unexpected behavior is not automatically considered a defect. Any
potential defect should be reproduced and compared with the expected
behavior before being documented as a confirmed defect.
