# Work Class *

    Explain about Work Object?

A work object is the primary unit of work completion in an application and the primary collection of data that a flow operates on.
When an application is used, work objects are created, updated, and eventually closed (resolved).
Every work object has a unique ID (property pyID), an urgency value, and a status (property pyStatusWork).

    What is meant by pyWorkPage and pyWorkCover?

When you have an active work object, **pyWorkPage** is meant as reference to that current work object's data.

If the current work object has another work object it inherits from,**pyWorkCover** is in reference to that object. This can be considered the current work object's parent.

