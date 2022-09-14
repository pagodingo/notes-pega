# Processes & Flows

## Set the value of one property to another (without DTs)

- In Case Lifecycle Designer, first open the assignment that contains the property (that is going to be set to another), and check `Set Properties` on the flow action leading away from the assignment shape.

This process is simpler than creating a DT to pass data from property-to-property, and it performs exactly the same.

### Use Case

Say you have a form, 'create account', which will at some point be saved as a new account (as the name suggests). But, the actual submission (saving the field group of account details), is a few case stages or steps down in a step called "Submit account information" (before submission), and the group of account properties is labeled "Account Information"

Using this technique, your entire configuration is this >

<img src="./images/process-connector-set-properties.png" alt="connector pannel in Process Map: Set Properties Section" />

Where **Name** defines the target property to be set, and **Value** determines the source property value used.

The screenshot above is cropped pporly, hoewever, **there is an option to add more properties** just beneath the cancel button.

**Further Discussion** --

Account Information in theory, could be an aggregate of multiple fields (multiple groups), that could all be persisted at once.
