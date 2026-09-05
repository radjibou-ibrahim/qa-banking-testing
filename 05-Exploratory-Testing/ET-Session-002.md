# Exploratory Testing Session 002 — Boundary and Negative Testing

## 1. Session Information

| Field | Details |
|---|---|
| Session ID | ET-SESSION-002 |
| Application | XYZ Bank |
| Application Type | Web Banking Application |
| Test Type | Manual Exploratory Testing |
| Tester | QA Manual Tester |
| Status | Planned |

---

## 2. Test Environment

| Item | Details |
|---|---|
| Application | XYZ Bank |
| Environment | Public Demo Web Application |
| Application URL | https://www.globalsqa.com/angularJs-protractor/BankingProject/#/login |
| Platform | Web |
| Browser | Chrome |
| Browser Version | 152.0.7977.64 (iOS)|
| Network | Internet connection |

---

## 3. Exploratory Charter

### Objective

Explore the application using boundary values, invalid inputs, unusual
values, and unexpected user actions in order to identify validation
inconsistencies, unexpected transactions, incorrect balance updates, or
other functional issues.

### Mission

Challenge the Deposit and Withdrawal functionalities with invalid,
boundary, and unusual inputs.

The exploration will also verify whether invalid operations affect the
customer's balance or transaction history.

---

# 4. Exploration Areas

## Exploration 1 — Deposit Boundary Values

### Actions

Using the Deposit functionality, test:

- Empty value
- `0`
- Negative value such as `-1`
- Small positive value such as `0.01`
- Normal positive value such as `10`
- Large positive value
- Very large positive value

### Observe

For each input, verify:

- Validation message
- Success or failure message
- Balance before the operation
- Balance after the operation
- Transaction history
- Transaction type
- Whether an unexpected transaction is created

### Questions

- Can a zero amount be deposited?
- Can a negative amount be deposited?
- Are decimal values accepted?
- What happens with a very large amount?
- Does the balance change only when the deposit is actually processed?
- Is an invalid deposit recorded in the transaction history?

---

## Exploration 2 — Withdrawal Boundary Values

### Actions

Using the Withdrawal functionality, test:

- Empty value
- `0`
- Negative value such as `-1`
- Small positive value
- Amount below the available balance
- Amount exactly equal to the available balance
- Amount greater than the available balance
- Very large amount

### Observe

For each input, verify:

- Validation message
- Success or failure message
- Balance before the operation
- Balance after the operation
- Transaction history
- Transaction type
- Whether an unexpected transaction is created

### Questions

- Can zero be withdrawn?
- Can a negative amount be withdrawn?
- Can the exact available balance be withdrawn?
- Is a withdrawal greater than the available balance rejected?
- Does a rejected withdrawal leave the balance unchanged?
- Is an invalid withdrawal recorded in the transaction history?

---

## Exploration 3 — Numeric Input Exploration

### Actions

Explore unusual numeric inputs where the application allows them:

- Decimal values
- Leading zeros
- Very large numbers
- Multiple digits
- Negative values
- Zero
- Empty input

### Observe

- Browser validation
- Application validation
- Error messages
- Whether the operation is processed
- Balance changes
- Transaction history changes

### Questions

- Does the input field accept the value?
- Is the value rejected by the browser or by the application?
- Is the validation behavior consistent?
- Can an unusual value result in an unintended transaction?

---

## Exploration 4 — Repeated Operations

### Actions

Perform several operations consecutively:

1. Make a valid deposit.
2. Make another valid deposit.
3. Perform a valid withdrawal.
4. Perform another valid withdrawal.
5. Open the transaction history.
6. Compare the operations with the displayed transactions.

### Observe

- Balance updates
- Number of transactions
- Transaction amounts
- Transaction types
- Transaction order
- Consistency between balance and transaction history

### Questions

- Is every successful operation recorded?
- Are transactions duplicated?
- Is the balance updated after each operation?
- Does the transaction history reflect the operations correctly?

---

## Exploration 5 — Invalid Operation Followed by Valid Operation

### Actions

1. Attempt an invalid deposit.
2. Verify the balance.
3. Verify the transaction history.
4. Perform a valid deposit.
5. Verify the balance again.
6. Verify the transaction history.

Repeat a similar sequence for withdrawal.

### Observe

- Whether the invalid operation has any side effect
- Whether the valid operation is processed correctly
- Whether transaction history remains consistent

### Questions

- Does an invalid operation affect the following valid operation?
- Is an invalid transaction accidentally recorded?
- Does the balance remain consistent?

---

# 5. Observation Guidelines

Do not classify an unexpected behavior as a defect immediately.

Use the following process:

**Observation → Reproduction → Investigation → Expected vs Actual → Defect Decision**

For each interesting behavior, record:

- Input used
- Initial balance
- Action performed
- Message displayed
- Final balance
- Transaction history result
- Whether the behavior can be reproduced
- Evidence available

---

# 6. Observation Log

| ID | Area | Input / Action | Observation | Result | Evidence |
|---|---|---|---|---|---|
| OBS-001 | Deposit | | | | |
| OBS-002 | Deposit | | | | |
| OBS-003 | Deposit | | | | |
| OBS-004 | Deposit | | | | |
| OBS-005 | Withdrawal | | | | |
| OBS-006 | Withdrawal | | | | |
| OBS-007 | Withdrawal | | | | |
| OBS-008 | Withdrawal | | | | |
| OBS-009 | Numeric Input | | | | |
| OBS-010 | Repeated Operations | | | | |
| OBS-011 | Invalid → Valid Operation | | | | |
| OBS-012 | Invalid → Valid Operation | | | | |

---

# 7. Potential Defects

Potential defects identified during exploration should be documented here
after reproduction and investigation.

| ID | Area | Potential Issue | Reproduced? | Confirmed Defect? | Bug ID |
|---|---|---|---|---|---|
| DEF-001 | | | | | |
| DEF-002 | | | | | |

---

# 8. Evidence

Relevant screenshots should be stored in:

`06-Evidence/`

Evidence should be captured when it helps demonstrate:

- Validation behavior
- Unexpected messages
- Balance changes
- Transaction history changes
- Unexpected transactions
- Other unexpected application behavior

---

# 9. Session Summary

### Areas Explored

_To be completed after the session._

### Key Observations

_To be completed after the session._

### Unexpected Behaviors

_To be completed after the session._

### Confirmed Defects

_To be completed after the session._

### Risks Identified

_To be completed after the session._

---

# 10. Conclusion

_To be completed after the exploratory session._

The conclusion will summarize the boundary and negative testing performed,
the main observations, and any confirmed defects identified during the
session.
