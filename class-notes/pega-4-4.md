# <u>Pega 4-4</u>

## Guardrails

Guardrails: Rules that should be followed, so that the application works as expected.

Example: Number of stages should be no more than 7-9.

In Pega, warnings will appear as red or orange banners above areas in which errors are present.

In total, there are <a href="https://docs.pega.com/implementation-methodology-and-dco/ten-guardrails-success?check_logged_in=1">10 predefined guardrails.</a>

### 1. Adopt an iterative approach
- Define an initial project scope (with intent to design-and-complete within 60-90 days).
- Document five concrete use case scenarios up front.
- Storyboard your scenarios. This ensures that each  delivers a measurable business benefit.
### 2. Establish a robust foundation
- Design your class structure. It should be understandable, easy to extend, and utilize the standard work and data classes appropriately.
- Use your organization's entities as a starting pattern, and then proceed with class groups.
- Lead with work objects. Create the class structure and work objects early.
- Position rules correctly by class and ruleset.
- Actively use inheritance to prevent rule redundancy.
### 3. Do nothing that is hard
- Use out-of-the-box functionality as much as possible, especially in the initial project release.
- Avoid creating custom HTML screens or adding buttons.
- Always use the “Auto Generated HTML” feature for harness sections and flow actions.
- Always use the standard rules, objects, and properties. Reporting, urgency, work status, and other built-in behaviors rely on standard properties.
- Never add a property to control typical work or to manage the status or timing of work.
### 4. Limit custom Java
- Avoid Java steps in activities when standard rule types, library functions, or activity methods are available.
- Reserve your valuable time and Java skills for implementing things that do not already exist.
### 5. Build for Change
- Identify and define 10 to 100 specific rules that business users own and will maintain.
- <u>Do not include activities</u> - use other rule types for business-maintained logic.
### 6. Design intent-driven processes
- Design your application control structure to consist of flows and declarative rules, calling activities only as needed.
- Use flow actions to prompt a user for input.
Present fewer than five connector flow actions for any individual assignment. If you need more than that, you need to redesign the process.
- Create activity rules that implement only a single purpose to maximize reuse.
### 7. Create easy-to-read flows
- Design your flows to fit on one page. Flows must not contain more than 15 smart shapes per page, excluding routers, notify shapes, and connectors.
- Redesign a flow if it has more than 15 smart shapes. You can:
Create a subflow.
- Use parallel flows to perform additional functions.
8. Monitor performance regularly
- Evaluate and tune application performance at least weekly by using the Performance tool to check rule and activity efficiency.
- Use PAL early to establish benchmarks. Compare these readings to later readings and correct the application as required.
### 9. Calculate and edit declaratively, not procedurally
- Whenever the value of a property is calculated or validated, use declarative rules wherever appropriate.
- Create a Declare Expressions rule instead of using a Property-Set method in an activity.
- Use a Declare Constraints rule instead of a Validation rule.
### 10. Keep security object-oriented, too
- Implement a security design that is rule-based and role-driven, based on who should have access to each type of work.
- Never code security controls in an activity.
- Use the standard access roles that are provided with PRPC or the Pega 7 Platform only as a starting point.
- Use rulesets to segment related work for the purpose of introducing rule changes to the business, not as a security measure.
___

To display your application's guardail compliance score:

Guardrail compliance is scored (%).

To view: Configure > Application > Quality > Dashboard

:two_hearts:

To raise guardrail compliance score:

[^1] Dashboard > Guardrail (**View details**) > Rules with Warnings.

[^1]: This action provides additional information regarding current rule warnings.
