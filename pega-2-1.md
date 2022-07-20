# <u>Pega 2-1</u>

## What is BPM?

### Case Management

Applications should function the same way users think about and describe their work and follow a business view of work, so that we model business transaction as a casetype.

* We need to identify the major milestones we call them stages
* Each stage can have single / multiple process based on requirement
* A process contains a series of tasks / steps that users complete as they work in the case.
* After identifying the process we need to identify the tasks, we call it as steps.
* Steps: A user completes the steps required by each process or stage.

---

### Other notes

* Whenever you want to execute multiple processes - add a Parallel Process.
* Steps you want the user to complete - user action steps. Steps that should be completed automatically - automated steps.
* * Look for "when all processes in this stage are complete" ... "automatically move to next stage."

### Data propegation

Whenever you want to send data from one case to another - data propegation.

From Field | To Field
---- | ----
Parent properties | Child properties

### Case Status

Case status is how users identify the state of each case.
