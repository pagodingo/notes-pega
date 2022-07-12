# mod_ans

## [x]

### -

#### A business process requirement states that users should be able to modify the shipping address at any time without interrupting the primary path of the case. Which of the following options is the best way to design for this requirement?

Add a step in a process.
Add a process to an alternate stage.
Add a process in a stage.
> Add an optional action to the case type.

Correct answer.
Adding an optional action to the case type allows end users to choose when they want to modify the address and keep the case on the primary path.

#### Which requirement could be satisfied with an optional action?

An application randomly sends a survey to customers once their case is resolved.
> Allow a user to transfer a case to another employee at any stage of the case.

Correct answer.
Because the decision to transfer the case is left to the user, the requirement can be implemented as an optional action.
Reassign any task that remains open after three days to another user.
Require a separate approval process whenever an order exceeds USD10,000.

#### Automating decisions based on business logic enables ____________________

architects to spend less time building the application

> application users to focus on decisions that require **human/business** expertise

Correct answer.
Recording and automating decisions based on business logic allows users to focus on decisions that require human expertise
application users to mark a specific location for business exceptions that may arise in the process flow
architects to improve the performance of the application

#### Drag the term from the left to the appropriate business case on the right

`[1]`A medical insurance claims case for a flu shot or annual exam are automatically approved. All other medical claims, such as visits to a specialist or alternative practitioners, require additional review by a claims agent

`[1]`A home appraisal case requires a house older than 40 years to be tested for asbestos. If the home is 40 years old or greater, additional information is required. If the home is less than 40 years old, the appraisal case moves forward.

`[0]`A car insurance claims case always requires a claims agent to assess the claims report. If the claim includes images of the damages to the vehicle, the claim report must include those as well

`[0]`An onboarding case requires that new employees receive an assigned seating location. If an employee is remote, it is unnecessary to assign a seating location or office equipment. The Facilities Setup process starts if the employee is not remote. Otherwise, the process does not execute

#### The UCom shopping website decides to share an update on order acceptance and the expected delivery time of the product. Which automation step is most suitable to achieve this objective?

Update case
Push notification
Post to pulse
> Send notification

Correct.
The Send notification step can be used to send notification over multiple channels.

#### UPlus Bank offers new mortgage loans to eligible customers. The bank creates a loan request form to collect the loan requests and decides not to consider the loan request if a customer already applied for a loan. To achieve the business use case, which of the following automation shapes is best suitable?

Persist case
Create case
> Search duplicate cases

Correct.
The Search duplicate cases shape can be used to find potential duplicate cases.
Send email

#### Which of the following statements is true about automation shapes?

An Automation shape can be used to configure the service-level agreements for a case type.
An Automation shape can be used to create views.
An Automation shape can be used to delete a case.
> An Automation shape can be used to change the stage of a case.

Correct.
You can use the change to the next stage automation shape to move the case to the desired stage.

#### In a mortgage application, the user creates a loan request. Before approving the loan request, the loan officer must receive the appraisal results. How can you configure the case types to reflect the loan request and appraisal relationship?

Make appraisal a parent case type and loan request a child case type.
Make mortgage a parent case type. Make loan request and appraisal child case types.
Make both loan request and appraisal parent case types.
> Make loan request a parent case type and appraisal a child case type.

Correct.
A loan request case must be created before an appraisal case can be created.

#### In an online shopping application, the primary case type PurchaseOrder has two child case types: Payment and Packaging. In processing PurchaseOrder case PO-11, the Payment case Pay-37 and Packaging case Pac-56 are created. Which statement about the processing of PO-11, Pay-37, and Pac-56 is correct?

> Both Pay-37 and Pac-56 must be resolved before PO-11 can be resolved.

Correct.
By definition, child cases represent work that must be completed to resolve the parent case. Therefore, both Pay-37 and Pac-56 must be resolved before PO-11 is resolved. 
PO-11 can be resolved when either Pay-37 or Pac-56 is resolved.
Pac-56 must be resolved before Pay-37 is resolved.
PO-11 must be resolved before either Pay-37 and Pac-56 is resolved.

#### In an online banking application, a Transaction inquiry case is created when a suspicious transaction is detected. If the customer verifies that the transaction was unauthorized, Pega Platform creates a Fraud investigation case, which can be spun off into investigations as appropriate. Details about the transaction are collected in the Transaction inquiry case. Those details are populated in the Fraud investigation case. What two actions do you perform to achieve this configuration in App Studio? (Choose Two)

> Propagate the transaction data from the parent case to the child case.

Correct.
Transaction data is collected in the Transaction inquiry case, and the data does not change, so it is appropriate to propagate the data from the parent case to the child case.
Reference the transaction data from the parent case in the child case.
> Configure Transaction inquiry as a parent case and Fraud investigation as a child case.

Correct.
A Transaction inquiry case is created before a Fraud investigation case.
Configure Fraud investigation as a parent case and Transaction inquiry as a child case.

#### You want to evaluate cases as potential duplicates when the existing cases and the current case have the same create operator. How can you ensure that only cases with the same create operator are evaluated?

> Add a basic condition where the create operator in an existing case is the same as in the current case.

Correct.

If the basic condition evaluates to true, the current case is eligible as a potential match and is evaluated using weighted conditions.
Add a weighted condition that uses the create operator value, an equals operator, and a weight of 100.
Add a basic condition that uses the create operator value and apply a weight of 100.
Add a weighted condition that uses the create operator value in both condition fields, an equals operation, and a weight of 0.



#### Management reports that a large number of cases are incorrectly identified as potential duplicates. Which two approaches can you use to modify the duplicate case search process to reduce the number of potential duplicates identified? (Choose Two)

Increase the weights for all basic conditions.
Add a second Search duplicate cases step to filter out invalid duplicates.

> Increase the threshold value.

Correct.
Increase the weighted conditions sum threshold value, so that more conditions or conditions with higher weights must evaluate to true.
Do not use a basic condition.

> Adjust the condition weights.

Correct.
Give conditions that frequently produce invalid duplicates lower weights.


#### Drag the words into the correct boxes

On a `stage`, you define a condition with comparators to determine when the `stage` is skipped. On a `process`, you define a condition with comparators to determine when the `process` is executed.

#### In a customer service case type, customers can indicate that they are interested in filling out a survey about their customer service experience. If the customer agrees to complete the survey, they proceed to the Customer Survey stage. Otherwise, the case resolves automatically.

How do you configure this behavior?

Configure the processes in the Customer Survey stage to start if the customer indicates interest in filling out a survey.
Configure the Customer Survey stage never to skip.
> Configure the Customer Survey stage with a custom condition to skip when the customer does not indicate interest in filling out a survey.

Correct answer.
In this configuration, the Customer Survey stage starts if the customer indicates interest in filling out a survey. The Customer Survey stage is skipped if the customer does not indicate interest in filling out a survey.
Configure the Customer Survey stage with a custom condition to start when the customer indicates interest in filling out a survey.


#### Which requirement is best implemented by using a Wait step in a case?

You cannot proceed in an expense report until a manager approves the request.
You need to send an email after a user completes a form.
> You cannot complete a purchase case on a website unless you complete a new account subcase.

Correct answer.
In this scenario, use a Wait step configured as a case dependency.
You must pause a case until a user uploads a signed document.

#### In a mortgage loan case type, applicants enter data in the Credit score, Income, Assets, Liabilities, and Loan amount fields. The data is submitted on different processes in the case type. The system informs applicants that, based on the data they provided in the Financial information stage, there are no loans available, and the case does not enter the Loan stage.

How would you configure the case type to perform the data validation described in this scenario?

Configure business logic validation on each form
Set each field to the appropriate field type to test for valid data
Set the control for each field to allow only valid data
Configure business logic validation on the Financial information stage
> Configure business logic validation on the Loan stage

Correct answer.
Configure the stage entry data validation on the stage to prevent the case from entering the stage.


#### Drag the words into the correct boxes.

In an online shopping application, you use `insights`
 to visualize data about recent returns. From the `explore data landing page`
, you analyze the types of returns and the amount of each return. In the `data tab`
, you select a clustered column, and then you add the Case ID count, Return amount, and Purchase type fields. In the `chart tab`
, you add a tooltip and update the legend.

#### Which two actions can you perform from the Explore Data landing page? (Choose Two)

> Create a pie chart for customer satisfaction data.

Correct.

After selecting an insight from the Explore Data landing page, you can create a chart from the Actions menu.

> Filter, sort, or group data for product inventory.

Correct.

After selecting an insight from the Explore Data landing page, you can filter, sort, or group data to view only the specific information that matches your business needs.
Create a new Sales data field to reference an insight rule.
Edit medical facility data for a health insurance application.

#### A manager has requested a report that shows the purchase requests for each of the regional cost centers. The manager wants to organize the results so that the cost center appears only once on the report and the requests are listed under the cost center. How should you configure the report?

Filter the results so that only cost center and requests are included in the report.

> Use the cost center column to group the results.

Correct answer.
Cases associated with each cost center are grouped beneath each cost center heading. 
Use the requests column to group the results.
Summarize the requests column by count.

#### A manager requests a report that contains the following columns: Create Date, Case ID, Create Operator and Work Status. You must sort the Create Date values so that the most recently created cases appear at the top of the list with the remaining cases descending from newest to oldest. How should you design the report to support this requirement?

For the Create Date property, select Count in the Summarize column.

> For the Create Date property, select Highest to Lowest sort type.

Correct answer.
The date with the most recent value is the first row. The other rows descend from newest to oldest.
Add a filter condition where Create Date is greater than one.
Configure the Create Date as the first column in the report.

#### Drag each report category to the correspoding description

`[monitor assignments]`Reports provide information about how long assignments are open.

`[monitor processes]`Reports list or summarize open (unresolved) work items in the application.

`[analyze performance]`Reports provide data based on resolved (completed) work.


#### The payroll manager requests a report on the average length of time required to obtain the various approvals for employee raises and promotions. What type of metric does the report provide?

Business metric
Approval metric
> Process metric

Correct answer.

The requested report will give the payroll manager information on the average duration of the employee raise and promotion approval process. 

#### Drag the appropriate attribute to the use case scenario.

`visible` When a user selects Mobile as their preferred communication method, a Mobile Phone Number field is displayed.

`disabled`A promotion is available when a shopper has spent USD100. The Apply Promotion button is grayed out until there is USD100 in merchandise in the cart.

`required`A customer must fill out their address in order to proceed to the next page.

#### End users can clear selections on a form and view the previous actions on the case. How do you configure the action set on a button to achieve this result?

First, configure a Click event with a Refresh action. Next, configure a Double-click event and a View History action.
First, configure a Refresh event with a Click action. Next, configure a View History event and a Click action.
First, configure a Click event with a View History action. Next, add a Refresh action to the event.
> First, configure a Click event with a Refresh action. Next, add a View History action to the event.

Correct answer.
Clicking the button is the trigger. Clearing the selections on a form and viewing the previous actions on the case are actions.

#### Given that an event is a trigger caused by user activity and an action is a response by the application, which two of the following sets represent action sets (event > action) in Pega Platform™? (Choose Two)

Open mobile app > Focus
> Double-click > Scan barcode/QR code

Correct answer.
Double-click is a trigger. Scanning a barcode is an available response.
Run data transform > Enter
> Tab key > Add new work

Correct answer.
Pressing the tab key is a trigger. Adding new work is an available response.


#### Which two of the following statements are true about user interface elements? (Choose Two)

> Autocomplete is an example of a basic control available out of the box

Correct answer.
Autocomplete is a basic control that is available out of the box.

> The predefined formats for a button include Standard, Simple, and Strong

Correct answer.
Standard, Simple, and Strong are the predefined formats for buttons.
Formats for control types can only be reused across a case type
Within an application each control type can only have one defined style.


#### Drag the words into the correct boxes

A user wants to see the number of service requests that team members perform at different times of a day.

 A developer adds the Reports `custom page`

 to the main menu of the `userportal`

, a default portal. Reports is an out-of-the-box 
`landing page`

#### Drag the terms to the correct placement in the following passage

 `Portals` are web channels that are accessed through a browser, regardless of the access device

`Portals` contain `landing pages`
 that combine information to match the needs of your users. To create new landing pages in App Studio, enter the Design mode to access the `Landing pages`
 menu.
.

#### In which scenario is it appropriate to remove a landing page from an application?

You are developing a landing page that is not available from the main menu by default, but that users can add to the main menu if appropriate.
You are developing a new landing page that is available for all users.
You are developing a landing page that is only relevant for people managers and is not available for individual contributors.

> You are developing a landing page that replaces an existing landing page, which is being deprecated and should not be used by any users.

Correct.
In this situation, it is appropriate to remove the deprecated landing page from the application so that it is no longer available on the Landing pages menu.

<img src="./images/template_ans.png" />

#### Which of the following two statements are true about the dashboard? (Choose Two)

>Each role-based interface includes a dashboard tailored to the role. 

Correct answer.
By default, Pega Platform™ uses role-based interfaces, which includes a dashboard tailored to a role.
The dashboard should contain all available widgets for a specific role to help increase productivity.
Each role-based interface includes an empty dashboard that must be customized with widgets tailored to the user's role.
Role-based interfaces must be created and customized for the roles used in the business.
> The dashboard displays key performance indicators (KPIs) and operational information about your application.

Correct answer.
The dashboard consolidates information from different sources and presents it in an actionable format.

#### Drag the words into the correct place in the sentence.

Various `templates`
 allow you to organize your `widgets`
 differently. Add or remove `widgets`
 from different `slots`
 to personalize your `dashboard`

#### Your company needs two separate mobile apps: one for customers to place delivery orders and one for couriers to confirm deliveries. The specifications include using a blue header background for the customer app and a green header background for the courier app. Which configuration allows you to complete this task?

> Create two mobile app channel interfaces, one for customers and one for couriers. Set the background color in the **theme** configuration menu for each channel interface.

Correct answer.
Because there are two user personas, you create two channel interfaces. Background colors are set in the theme configuration menu.
Create two mobile app channel interfaces, one for customers and one for couriers. Set the background color in the content configuration menu for each channel interface.
Create one mobile app channel interface. Rename the header elements as customer and courier, and change element background colors, respectively.
Create a single mobile app channel interface, and designate two header background colors that switch depending on who downloads the app.

#### Which of the following options is a valid swipe action? 

Changing the text color of a menu
Returning to the previous screen
Starting an optional process on your case
> Executing an optional action on your case

Correct answer.
Swipe actions are situational or optional actions.

#### Two mobile app channel interfaces are created for the Manager and Employee user personas. The Manager channel interface contains capabilities to run reports and edit orders, while the Employee channel interface does not

Both personas can use either channel interface

True **`False`**
The channel interface for the Employee persona is different than that for the Manager persona, which contains additional application components not required or permitted for the Employee persona

#### Each row of a decision table consists of one or more testable conditions organized into columns. How does Pega Platform™ determine when to return the specified result for a row?

When the last condition in the row is true.

> When all the conditions in the row are true.

Correct.
The decision table returns the result after evaluating all conditions specified in a row as true.
When any one of the conditions in the row is true.
When the first condition in the row is true

#### Battery repair discount

The ECare automobile company uses a decision table to evaluate the Express Gold battery warranty discount off the repair price based on when a customer originally purchased their battery in USD. Alex purchased an Express Gold battery from the ECare company 25 months ago. Due to some minor issues, the battery needs repairing. The total repair cost is USD100. Because the battery is under the warranty period, what is the total due after the applied discount?

USD45
> USD55

Correct.
Alex purchased the battery 25 months ago. As a result, the third row of the decision table evaluates as true and returns a discount of USD45 off 100, resulting in a total of USD55
USD0
USD100



#### Drag each configuration option to the description that would best automate the decision.

`Decision table`Before submitting a purchase order, the shipping cost is calculated based on product availability and the fulfillment warehouse location.

`Expression`In a flight booking application, the airline ticket price includes a base fare, fuel charge, tax, and meals.

`Expression`In a loan processing application, the installment is calculated based on the amount borrowed, annual interest rate, and period opted by the user.

`Decision table`In an online grocery store, customers receive an extra 10 percent discount if the purchase amount exceeds USD300.

#### Credit card decision table

UPlus Bank uses a decision table to recommend a credit card based on customer status. Ryan applies for a credit card. He is an existing customer, is 32 years old, and has a credit score of 600. What type of credit card is recommended?

Standard card
Reward plus card
> Gold rewards card

Correct.
Ryan's age is greater than 25, is an existing customer, and has a credit score that is greater than 500, so the second row of the decision table evaluates to true.
Premier Gold rewards card

#### Identify the use case that requires creating a new role

The permissions for an existing role are too limited for the work to be done.
> An additional combination of channel interface and permissions is necessary.  

Correct answer.
A role allows interaction with a specific channel interface and can grant specific permissions within the channel interface.
An additional person needs to interact with an application.
A new application is created

#### Drag the phrases to the correct placements in the sentences.

To create a role, supply

`name`, and `channel`

To create a user, supply

`role`, and `email address`

#### Drag each step in the order required to invite the auditor as a new user.

- create Auditor web channel
- create auditor role
- add the email address
- assign the auditor role

#### Select two use cases supported by Agile Workbench. (Choose Two)

> The lead developer creates a new application for the development team.
You need to adjust the due date for several user stories.

Correct.

Agile Workbench allows you to establish and modify due dates for user stories, feedback items and bugs.

> During a peer review, the reviewer discovers and records an application bug.

Correct.

You can submit a bug directly in Agile Workbench after finding an issue in an application.
The project team discusses how many application developers are needed and reports back to the stakeholders

#### Which two assets are assigned to a release and used to estimate the project scope and duration? (Choose Two)

Work groups
Processes

> Channels

Correct answer.
Channels are assigned to a release to estimate the duration for each release.

Case types

> Data objects

Correct answer.

Data objects are assigned to a release to estimate the duration for each release.
