# QA Case Study: Registration Flow (Email Verification)

## Overview
This case study demonstrates a process-aware QA approach to testing
a user registration flow. Test scenarios are derived from business
process logic rather than UI behavior.

## Scope
- User registration
- Data validation
- Email verification
- Pending account state
- Reminder flow

## Start Events
- User clicks "Register"
- User is redirected from failed login attempt

## Key Process Steps
1. Display registration form
2. User submits registration data
3. System validates data (format, business rules, database)
4. Account is created in pending state
5. Verification email is sent
6. System waits for user action

## End State Definition
Registration is considered complete only after email verification.
Before verification, the account remains inactive.

## Key Risks Identified
### Business Risk
- User drop-off during email verification

### Security Risk
- Abuse through fake or automated registrations

## QA Insight
QA highlights the trade-off between conversion rate and security
and supports decision-making through risk visibility.

