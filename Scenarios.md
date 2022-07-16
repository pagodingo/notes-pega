# Common Business Scenarios, and their Pega  Applicative Solutions

The reason for listing each of these scenarios (from Pega Academy Exercises), is because I know I won't be able to remember all of the other information given - **I can't retain all of it.**

My primary focus is to first **finish** the work that's required. Then, **revise and practice** what I've marked as important. For example, **<u>these scenarios:</u>**

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
