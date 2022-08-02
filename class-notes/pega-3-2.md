# <u>Pega 3-2</u>

## Data pages

Data Pages (in clipboard) contains the data received from an external system (database.)

> Clipboard memory is temporary memory.

> Data retrieved from an internal or external system of records (database) is stored and accessible through an active case's clipboard - under "Data Pages"

Storing data is done through Savable Datapages. Pega generates three data page types for you:

- Single Data Page
- List Page (a list of single data pages)
- Savable Data Page

Any data type created in Pega will have these three pages created by default.

## pyWorkPage/WorkCover

Clipboard Data (temporary data) accumulated in a case type are stored in folders labeled pyWorkPage and WorkCover.

The folder `WorkPage` stores data related to the active case (or thread).

The folder `WorkCover` stores data related to the case's parent.

## Automation

Automation has many definitions. There are provided case steps in Pega such as Send Email, Wait, and other steps (robotics) that run without the need of manual activation

Although this may satisfy what can be considered "automation" in Pega, there are other practices that the term refers more to.

In Pega, the primary building block of any application is a case. A case is a user experience (or a user-experienced process).

Cases have lifecyles - which are made up of steps that lead it from beginning to end. These lifecycles can be designed by clicking on Case Types, and creating or selecting the case you wish to design.

Alternatively, inside the same view, you can configure a case's lifecycle through a Process Diagram

> Flow Diagram may be what it's more commonly known as.

Inside of this Flow Diagram, you have the option to configure more readily-provided Pega step types:

One of which, are **Decisions**.

Decisions are Case Steps that that lead a case's lifecycle in a new direction, depending on _some condition_. It can be considered Validation (or conditional branching), in some way, but they are not meant to be mistaken for one another.

Decisions are preferred to be used when a case can flow in more than two directions. Or, when the outcome of some event can have more than two resolves.

Utilizing Decisions in this way aids in automating the flow of cases, by providing a solution for each situation any particular business endeavor requires.
