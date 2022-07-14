# Common Scenarios And Their Solutions


## Refining an Agile Workbench backlog

Stakeholders at GoGoRoad want to develop a new roadside assistance application to streamline operations for customer roadside assistance requests. Using the scope for the Minimum Loveable Product (MLP) and incremental releases, stakeholders want to track the current progress of the Assistance request case type, and determine the next highest priority functionality to develop in the future. To facilitate progress tracking, stakeholders and the Pega team have identified and prioritized a product backlog.

To prepare for development, the business architect (BA) must populate the backlog and update the user stories to include the feature, subfeature, owner, and the due date. GoGoRoad uses Agile Workbench to manage and prioritize the work. The team created the user stories in an Excel spreadsheet specially formatted for Agile Workbench import. Use the Excel spreadsheet to import user stories and populate the backlog.

## Sizing a Pega Platform Project

Prior to beginning work on the Roadside Assistance application, stakeholders have requested an estimate of the project size and scope. The estimate is used to consider staffing models and provide an approximate delivery date. Using the Case Designer, assign releases to the channels and data objects associated with the Assistance Request and Service case types. Then, run the Estimator tool to calculate the sizing estimate for the MLP 1 release.

## Adding optional actions to a workflow

InsCorp wants to ensure that customers can cancel service requests at any time. Add the Cancel request process as a case-wide optional action to cancel assistance requests. Update the process to advance a case to the Cancellation stage if the user elects to cancel their assistance request.

The following table provides the credentials you need to complete the challenge.

## Control the worlflow based on business context

When customers submit a request for roadside assistance, a customer service representative (CSR) manually validates whether the customer is enrolled in roadside assistance coverage. To improve efficiency, stakeholders want to automate this step. Replace the existing Approve/Reject step with an automated decision that sends the case to the Approval Rejection stage if the customer is unenrolled.

