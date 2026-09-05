# Exploratory Testing

## Objective

The objective of exploratory testing is to identify unexpected behaviors,
usability issues, validation inconsistencies, and functional risks that may
not be covered by the predefined test cases.

## Approach

Exploratory testing was performed using time-boxed exploratory sessions.

Each session was based on an exploratory charter defining:

- the area to explore
- the main objectives
- the risks to investigate
- the exploration scope

During each session, observations were documented and unexpected behaviors
were investigated further when necessary.

## Exploratory Testing Sessions

| Session | Area | Objective | Status |
|---|---|---|---|
| ET-Session-001 | Customer Banking Flow | Explore the main customer banking journey | Planned |
| ET-Session-002 | Boundary & Negative Testing | Explore invalid and boundary inputs | Planned |
| ET-Session-003 | Manager & Navigation | Explore management functions and navigation | Planned |

## Defect Handling

If an unexpected behavior is identified, it will be:

1. Observed
2. Reproduced
3. Investigated
4. Compared with the expected behavior
5. Confirmed as a potential defect
6. Documented in the Bug Reports section if confirmed

## Evidence

Screenshots and other relevant evidence will be stored in:

`06-Evidence/`

## Scope

Exploratory testing focuses on manual functional behavior and user flows.

API testing, SQL/database testing, automation, performance testing, and
security testing are outside the scope of this project.
