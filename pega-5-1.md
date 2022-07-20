# <u>Pega 5-1</u>

## Declare expressions

Use Declare Expression rules to define automatic computations of property values based on expressions.

> These work hand in hand with Calculated fields.

1. Create case
2. Add fields (num_1, num_2, Both of type Integer)
3. Add field: Sum (type Integer) - set Calculated Read-only > Use expression > .Num1 + .Num2

Calculated Read-only is a default declare expression.

4. App Explorer > {Case Name} >  Decision > To view the Declare expression created by default.

> **Procedural Processing**: Rules that need to be invoked explicitly.
> **Declarative Processing**: Rules that are executed implicitly.

The declare expression above is an example of Declarative Processing

6 types of Declarative rules:

1. Declare constraints
2. Declare expressions
3. Declare onchange (based on some property, internal change happens)
4. Declare trigger (executes activities - ex: case creation, deletion, update)
5. Declare index
6. Data Pages

**Example of Declare Constraint:** "Num 1 must be greater than Num

Creating declare constraints:

Right click class (app explorer), create constraint, when num 1 < 25, require that num 1 >= 25, else add message value must be greater than 25, to target "more" -> pyLabel.

## Using declare tables to fulfill larger calculations

When calculations grow to sizes larger than a few  - use declare table

## Forward chaining & Backward chaining declare expressions

Whenever an input value is changed, and all rules that are related to that input change, this is considered forward chaining.

By default, forward chaining is enabled.

To disable forward chaining.

Open Expression > Use legacy expression > Change Tracking > Change **Calculate Value** to "Whenever used."
