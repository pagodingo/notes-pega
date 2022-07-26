# Processes & Flows

## Set the value of one property to another (without DTs)

- In Process Map, open the step that contains the property that is to be set to another, and checkmark `Set Properties` for this step's purpose instead of `Apply Data Transform.`

- It's simpler than creating a DT to pass the data to another prop, and works in the same.

**Example:**

Say you have a `Create Account` Form, which will at some point be saved as a new account as the form name suggests. But, the field group that will be persisted, is a few case stages or steps down, in perhaps a step called "Review Information" (before submission), and the final field group to be persisted is called "Account Information"

Using this technique of passing data to another prop without creating a DT is then as simple as this:

<img src="./images/process-connector-set-properties.png" alt="connector pannel in Process Map: Set Properties Section" />

Where the Name column identifies the target property to be set, and the value column identifies the source property value to use.

The screen shot is cropped, but there is an option to additional properties below the cancel button.

In the last step, Review Information, there is an `Account Information` field group.

Account Information in theory, could be an aggregate of multiple fields (groups), to be persisted at once.
