# Common Business Scenarios, and their Pegasystems Solutions

This list serves as reference to primary examples of  pega solutions that apply to common business situations

## Refining an Agile Workbench backlog

Stakeholders at GoGoRoad want to develop a new roadside assistance application to streamline operations for customer roadside assistance requests. Using the scope for the Minimum Loveable Product (MLP) and incremental releases, stakeholders want to track the current progress of the Assistance request case type, and determine the next highest priority functionality to develop in the future. To facilitate progress tracking, stakeholders and the Pega team have identified and prioritized a product backlog.

To prepare for development, the business architect (BA) must populate the backlog and update the user stories to include the feature, subfeature, owner, and the due date. GoGoRoad uses Agile Workbench to manage and prioritize the work. The team created the user stories in an Excel spreadsheet specially formatted for Agile Workbench import. Use the Excel spreadsheet to import user stories and populate the backlog.

## Sizing a Pega Platform Project

Prior to beginning work on the Roadside Assistance application, stakeholders have requested an estimate of the project size and scope. The estimate is used to consider staffing models and provide an approximate delivery date. Using the Case Designer, assign releases to the channels and data objects associated with the Assistance Request and Service case types. Then, run the Estimator tool to calculate the sizing estimate for the MLP 1 release.

## Adding optional actions to a workflow

InsCorp wants to ensure that customers can cancel service requests at any time. Add the Cancel request process as a case-wide optional action to cancel assistance requests. Update the process to advance a case to the Cancellation stage if the user elects to cancel their assistance request.

The following table provides the credentials you need to complete the challenge.

## Control the workflow based on business context

When customers submit a request for roadside assistance, a customer service representative (CSR) manually validates whether the customer is enrolled in roadside assistance coverage. To improve efficiency, stakeholders want to automate this step. Replace the existing Approve/Reject step with an automated decision that sends the case to the Approval Rejection stage if the customer is unenrolled.

> This scenario introduces efficient methods of how to quickly add and connect process shapes to each other in the process builder.

## Attaching PDF files to a case

InsCorp wants to ensure that customers receive an email with a receipt of services, including a breakdown of the services provided. Add two automations, Create PDF and Send email, to the service case type to send an email to customers with the service total and an attachment with the breakdown of the service charges.

## Creating a child case

InsCorp is launching a roadside assistance service as a coverage option for automobile insurance policies. Configure the Assistance request case type to create a Service case during the Service stage to perform the selected services.

## Adding a duplicate case type search

InsCorp wants to ensure that only one assistance request case is processed for each request. Customers that send assistance requests might have difficulty determining their exact location. If a customer submits multiple requests for the same vehicle, but for slightly different locations, the application should identify the new case as a duplicate case.

## Skipping a process based on business context

Roadside assistance requests are covered for customers who have opted for the higher membership coverage level. Configure the Enter payment information and Invoice customer processes to start when the customer coverage level is not a Gold membership.

## Pausing and resuming case processing

InsCorp is launching a roadside assistance service as a coverage option for automobile insurance policies. During the Service stage, the customer selects a service provider, and a Service child case is created to collect information from the service provider. To process the Assistance Request case and the Service case correctly, enforce a dependency to pause and resume case processing on the Assistance Request case when the Service case meets the conditions that you define.

## Validating data against business logic

Customers with standard coverage use a credit card to pay for services performed by a service provider. To ensure that credit card transactions are processed correctly, stakeholders have identified that the expiration date must be in the future. Expired cards are rejected, and the process cannot continue until the user provides a valid expiration date.

## Creating a custom business report

Stakeholders would like to know the number of cases that have been requested over the past month. You have been asked to define a report to track the status of Assistance requests over the last 30 days. Create a report category for Assistance request cases, then create a report definition in the Assistance request category that displays the number and status of requests submitted in the past 30 days.

## Setting a visibility condition for form content

The GoGoRoad application allows customers to enter the service address by entering information in fields or selecting the location from a map. To customize the user experience by channel, the UI consultant has requested the following functionality: Users on a non-mobile device use the fields to enter the service address. Users on a mobile device select the location from a map. Configure the Identify location form to hide the redundant content depending on the device that is in use.

## Adding dynamic functionality to a button

After a request for roadside assistance is approved, a service provider is dispatched to the location provided by the customer. To perform this task, customer service representatives (CSRs) request the ability to verify and modify the service address when selecting the service provider.

Add a button to the Select service provider view so that the CSR can verify the service address submitted by the customer.

## Customizing a portal

GoGoRoad provides roadside assistance services through contracted vendors. To ensure customer satisfaction and service consistency across vendors, auditors review common service requests (including vehicle unlock, tire repair, and battery charge). The new auditor role requires a unique interface. As the Director of Vendor Management, create a new Auditor portal and add an existing landing page to view recent Assistance Request cases.

## Customizing a dashboard

During the processing of Assistance Request cases, a customer service representative (CSR) may need to request a credit on the behalf of the customer. Requests for credits are processed and authorized by a manager using a second, legacy system. An integration to the system for credit requests is scheduled for a future release. To ensure the prompt processing of credit requests, stakeholders want to display Pulse notifications on the dashboard so that CSRs can notify managers when a case requires a credit to be issued to the customer.

In addition, stakeholders want to track the user performance on Assistance Request cases on the dashboard using the Average duration per flow task report.

## Designing a mobile app experience

GoGoRoad wants to allow customers to create an assistance request case from their mobile device. Customize the User mobile app channel to design a mobile app experience that lets customers:

Create an assistance request case
Check any notifications sent to the customer
Update details on an assistance request case
Update the location for an assistance request case
Log off
In addition, customize the app branding, including the launch screen and app icon, and configure the app to lock after three minutes of inactivity.


## Calculating fields using decision tables

GoGoRoad stakeholders want to ensure customer satisfaction by allowing the application of discounts based on whether the service provider is on time or late. Customers are offered a greater discount based on how late the service provider arrived. You are directed to add a calculated field to the Review service summary step in the Assistance Request case type. The calculation is based on a decision table.

## Creating users and roles

GoGoRoad provides roadside assistance services through contracted vendors. To ensure customer satisfaction and service consistency across vendors, auditors review common service requests (including unlock vehicle, tire repair, and battery charge). The new auditor role has a unique interface. As the Director of Vendor Management, create a new role, and provide application access for the new auditor.

## Complete application

U-Plus Bank provides people with the financial products needed to achieve their financial goals. As part of its digital transformation, U-Plus Bank is creating a web-based account management application built on Pega Platform™. U-Plus wants to provide potential customers with the ability to open a new checking, savings, or investment account online through this application.

To open an account, the customer completes the following process:

The customer selects one of the financial products offered by U-Plus Bank.
The customer identifies the owner and any co-owners of the account.
The customer commits to funding the account with an initial deposit and identifies accounts at other financial institutions from which funds are transferred to complete the deposit.
To complete the account opening process, the application emails a summary of the transaction to the customer. This email confirms the selections made during the process. 

As part of the development team implementing the account management application, you are tasked with configuring functionality in the account opening and account selection case types. The following user stories describe the work assigned to you, which you must complete before releasing the application. You can access these stories in your exercise environment by using Agile Workbench. As part of this mission challenge, set a due date for each user story and update the status of each story as you meet the acceptance criteria.

## Manipulating Application Data

To ensure that customers are billed for only the services provided, the program manager wants the application to display a list of the services performed by the service provider. The list must include the following information: the name of the service performed, the unit cost of the service, the number of times the service was performed, the total cost for each service, and the total cost of the services performed. On the Perform service flow, configure the CopySelectedServices data transform to copy services provided from a Service case to an Assistance request case.

The following diagram displays the relationships of the Selected services Embedded data type in the Assistance Request case type, and the Services data relationship in the Service case type to the Services offered data type.

## Escalating late work

InsCorp is launching a roadside assistance service as a coverage option for automobile insurance policies. Customers initiate Assistance Request cases. After the service is completed, a customer service representative must review a summary of the service provided within 15 minutes and must complete the review within 30 minutes; otherwise, the assignment is considered late. To encourage assignment completion, configure the passed deadline interval to increase the urgency of the assignment by ten every 15 minutes after the Deadline interval elapses until the urgency reaches a maximum of 100.

## Configuring a cascading approval with a reporting structure

GoGoRoad stakeholders want to allow Territory Managers to add new vendors as service providers as the service grows. If the vendor is The Automobile Association (TAA), which has an existing relationship with GoGoRoad, the Add Vendor case is routed to the Manager of the Territory Manager for approval. If the vendor is not TAA, the Add Vendor case type is then routed to a Director for a second approval. Add an Approval step to the Add Vendor case type to support the described behavior.

The following image displays the reporting structure for the author@gogoroad user.

> `Sending approvals to one user or another`

## Automating decisions with decision tables

An organization is launching an application that facilitates loan requests. Customers initiate a loan request and enter their credit score and loan amount. Configure a decision table and declare expression, so that the loan rate is determined automatically based on the credit score and loan amount the customer enters. Use the values in the following table to configure your decision table:

|Credit score > |Loan amount > |Return |
|-|-|-|
|if	800|	50000	|.0225|
|else if 800|	0|	.0200|
|else if 700|	50000|	.0325 |
|else if	700|	0|	.0275|
|else if	200|	50000	|.045|
|else if	200	|0	|.0425|
|otherwise	| 	 |	.07

## Automating decisions with decision trees

An organization is launching an application that facilitates loan requests. Customers initiate a loan request and enter their credit score, loan amount, and country. Configure a decision tree and declare expression so that the loan rate is determined automatically based on the credit score, loan amount, and country the customer enters. For this challenge, if the customer specifies Canada as the country, the loan amount does not affect the loan rate. Use the values in the following table:

|Country |Credit score > |Loan amount >|	Return|
|-|-|-|-|
|	Canada| 800|	| 	.0200|
|	Canada	|700|	 	|.0275|
|	Canada	|200|	 	|.0425|
|	 |	800	|50000|	.0225|
| |	800	|0	|.0200|
|	 |	700	|50000|	.0325|
|	 |	700	|0	|.0275|
|	 |	200	|50000|	.045|
|	 |	200|	0|	.0425|
otherwise | | |	 	 	 	.07|

## Configuring cascading approvals with an authority matrix

As the repair service grows, GoGoRoad stakeholders want to allow Territory Managers to submit new vendors as service providers for approval. If the vendor is The Automobile Association (TAA), which has an existing relationship with GoGoRoad, the New Vendor case is routed to the Manager of the Territory Manager for approval. The case is then routed to a Compliance Officer, who ensures the request adheres to the agreement between TAA and GoGoRoad. If the vendor is not TAA, the New Vendor case is routed to the Manager, and then the Director for approval. Create a decision table to ensure the approval is routed appropriately. Add an Approval step to the New Vendor case type to support the described behavior.

***Decision Table***

| | Vendor name | Vendor approvals|
|-|-|-| 
|when| | "manager@gogoroad|
|when| !=TAA | "director@gogoroad"
|when| TAA | "compliancedirector@gogoroad"|

> Note: To set `Vendor approvals` specified property: ***.VendorApprovals(`<APPEND>`).ApproverID***

## Creating and managing teams of uers

In Roadside Assistance cases, a customer service representative (CSR) must assign a service provider to the case, review the summary of the services provided, and submit the request. Create a team named CSR@GoGo for customer service representatives and route the Select service provider and Review service summary steps to the work queue for the team.

## Validating data in Dev Studio

GoGoRoad customers with Standard coverage provide credit card information during the Submission stage of an Assistance Request case to pay for services performed by the company. To reduce the chance of an error when processing the credit card information, stakeholders want to validate the credit card information provided by customers.

A senior developer created an edit validate rule named IsDigit to verify that a credit card number contains only numbers. Configure a validate rule for the Enter Payment Information step to validate entries in the Card number field by applying the IsDigit edit validate rule and entries in the Expiration date field by applying the EnterPaymentInformation validate rule.

### Configuring additional Data Transforms to run at case start

***Create Data Transform: Set Day of Week***

|action|target|relation|source|
|-|-|-|-|
|set|.serviceDayofWeek|equal to|@if(.ServiceDay=1,"Sunday", @if(.ServiceDay=2,"Monday", @if(.ServiceDay=3,"Tuesday", @if(.ServiceDay=4,"Wednesday", @if(.ServiceDay=5, "Thursday", @if(.ServiceDay=6, "Friday","Saturday"))))))|

***pyDefault in Case Type***

|action|target|relation|source|
|-|-|-|-|
|Set|pyUrgencyWorkClass|equal to| 10|
|Apply Data Transform| pySetFieldDefaults| | |
|Apply Data Transform| SetDayOfWeek| | | |

## Saving data to a system of record

The program manager for the roadside assistance service wants to provide users with an option to enroll when requesting service rather than automatically rejecting unenrolled users. Configure the Approval Rejection process to update the membership status of a customer record if the customer decides to enroll in the roadside assistance program. Create a data transform to copy the updated membership status and coverage level to the customer record. Then, add the data transform and a Save data page step to the Approval Rejection process to update the customer record in the database.

## Customizing a view at run time

GoGoRoad stakeholders want the Enter customer information view and Identify Location view to be streamlined to display the relevant information with proper validations. To achieve this request, change the coverage information of Enter customer information view to a two-column layout and add the ZIP code property to the Identify Location view with required validations.

## Grouping fields in views

Based on feedback, GoGoRoad's customers are unable to double-check details before submitting an Assistance Request, leading to confusion and additional time spent correcting details. The GoGoRoad management team has decided to implement a final read-only confirmation screen after customers enter all the relevant information. This confirmation screen presents all the information to the customer before allowing them to submit their Assistance Request.

## Display list data in views

The GoGoRoad application presents a list of all available service providers in a table. The UI consultant wants you to make the following changes to the UI: present the relevant service provider information only and configure the on-screen content to accommodate multiple screen sizes. Format the list of providers to present in a non-tabular form, using a layout to organize the display of a single item and then embedding the section in a repeating dynamic layout.

## Localizing a UI form

GoGoRoad stakeholders have a requirement to translate the New vendor case type to Spanish.

Use the Localization wizard to localize the New vendor case type of the GoGoRoad application, export the files, translate properties on a UI form into Spanish, import the files, set the locale settings, and test the translated form. translating. language.

## Enabling accessibility features in an application

To ensure compliance with government regulations on accessibility, GoGoRoad wants to assess the user experience (UX) for users with color vision deficiencies. Run the Accessibility Inspector on each view in the application to preview the display for users with one of the four listed color vision deficiencies.

> Note: As a best practice, use the Accessibility Inspector on a step as you configure the user interface; this allows you to identify and resolve accessibility issues during development. For this challenge, focus on running the Accessibility Inspector and identifying any issues on each view. You do not need to fix any of the issues identified. Disability. Achromatopsia (Absence of color).

## Simulating an external data source

During roadside assistance, a service provider performs minor mechanical repairs. Requests for roadside assistance must identify the vehicle so that the service provider can prepare for the service call. For example, certain vehicles might require a flat-bed tow truck or a higher octane fuel blend.

To allow service providers to prepare for a service call, stakeholders want to ensure that users enter only a valid combination of make, model, and year for a vehicle. As part of the initial application release, a listing of vehicle models is sourced from an external system. Before the external source is configured and tested, stakeholders want to simulate the process of providing the year, make, and model of a vehicle.

Configure a simulated data source for vehicle model data to validate the Identify vehicle view. A separate developer has configured the layout and behavior of the view. You create a simulated data source for the drop-down list of vehicle models to use until the external system with the data source is configured and tested.

> Note: For this exercise, two models of vehicles are sufficient to test the view. The list of models is filtered based on the year and make.
---
> Important info: In Preview (of an Assistance Request case), after creating two simulated sources, we configure the model dropdown (in view) to have a Type of `Data Page` and a Source of one of the data pages we created (D_VehicleModelsList) and `group elements` by `.VehicleType`

The result is that our Dropdown shows two records (that were manually added) to the simulated sources mentioned.

## Adding an external data source

Requests for roadside assistance must identify the vehicle so that a service provider can prepare for the service call. For example, certain vehicles may require a flat-bed tow truck or a higher octane blend of fuel. To better prepare service providers for a service call, stakeholders want to ensure that users only enter a valid combination of make, model, and model year for a vehicle. After evaluating several possible sources for vehicle models, stakeholders decided to source this information from a US National Highway Traffic Safety Administration (NHTSA) web service available at https://vpic.nhtsa.dot.gov/api.

Replace the current simulated data source with an integration to source the model information for passenger cars and trucks using a Representational State Transfer (REST) service provided by the NHTSA. Populate the D_VehiclemodelsList data page with NHTSA response data, based on the model year and make entered by the user.

> Configuring: Data > New > (give name) > System: Create New > endpoint URL (some.json.api.endpoint) > match api parts to pega model properties

---

> Successful external data source confirmation:
"Results returned successfully"
---

> Map return results (wizard provided)
---
> Tags: Example external data source, datasource, json, api

## Configuring security policies

GogoRoad is experiencing a large number of failed login attempts. Management suspects that the attempts are malicious attacks by an internet bot. Management has asked you to implement a new security requirement. After the first failed login attempt, the user cannot make additional attempts without further verification. After each attempt, the user must wait for a progressively longer period before making another attempt. The first failed attempt is delayed by five seconds.

After the first failed login attempt, display a CAPTCHA on the login page to verify that the user is a human and not an automated bot. After two failed attempts, enable a lockout penalty to delay further login attempts in five-second increments.

## Managing application access

GoGoRoad product managers want to restrict access to development on the New Vendor case type so that only approved roles perform updates. Configure permissions on the New Vendor case type to prevent anyone with the User role from performing any actions on the case type.

> Restrict user access to certain features of an application. Restrict Modify. Restrict View History.

## Debugging application errors

As part of processing an assistance request case, the Roadside Assistance application copies the services performed from the child Services case to the Assistance Request case. While testing the configuration of this feature, you notice that Assistance Request cases include service items not indicated on the child case, as shown in the following screenshot. Use the Tracer tool to debug the issue and resolve it.

> Note: To reduce the number of irrelevant events the Tracer records, play the Tracer before you encounter the error.

## Unit testing rules

For an Assistance Request case, when users enter the vehicle make, one or more associated models display in the Model drop-down. Intermittently, users report that during the Submit request process, when entering the vehicle information, some car makes do not have an associated model name in the drop-down. Stakeholders need to easily identify the vehicle makes without at least one associated model.

In addition, stakeholders are concerned about application performance. To ensure customers can complete assistance request cases efficiently, stakeholders require that the vehicle model list is generated within 200 milliseconds.

> Configure > Application > Quality > Automated Testing > Unit testing > Test cases

## Creating a new scenario test case

GoGoRoad wants to create a standard scenario test to automate testing for the Assistance Request case type. Create an automated test for the Submit request process to ensure that the user interface and end-to-end process flow function correctly.
