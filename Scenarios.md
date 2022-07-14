# Common Business Scenarios, and their Pega  Applicative Solutions


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

