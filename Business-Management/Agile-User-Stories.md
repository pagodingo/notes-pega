# User Stories

Accessible through the App Studio, User Stories contain desired features soon-to-come to apps.

A User story consists of a name, description, associated feature, owner, and other details pertaining to new features and application add-ons. User Stories are the meat-and-potatoes of Agile Environments. It allows teams to keep track of new developments and what is currently being worked on.

## Example User Story

### 1. US-1001: Identify duplicate Open Account cases
As a customer, I want to receive a notification if an Open Account case is a potential duplicate, so I can avoid opening multiple accounts by accident.

***US-1001 Description***
Add a Search duplicate cases step after the Identify owner step. The step should have the following basic and weighted conditions:

Basic condition: Choose account type is the same
Weighted conditions sum to at least 50:
Name in the Account data relationship is equal to .Account.Name. This condition has a weight of 30.
Last Name in the Owner data relationship is equal to .Owner.LastName. This condition has a weight of 25.

***US-1001 Acceptance criteria***
When a user creates two Open account cases with matching account types, account names, and owner last names, the current case is identified as a potential duplicate of the previous case.
