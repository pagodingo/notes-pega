# All Things Data

**1. Activities Save Data**

Setting up an activity:

- Method: Page-new

- Step Page: {Page Name} (create a new Page reference in Pages & Classes. Source the property's data class like this: )

> OOO-AAA-Data-{Data-Object}

**2. For whichever step contains the data to be persisted, open its flow action rule**

**3. Create an Activity in its Post Processing Section**

Activity Methods:

1. Page New
2. Property Set
3. Object Save

I'm going to write this down for a third time because this is so hard to remember.

~~**Only an activity can save data.**~~

To save data, create whatever data model you're trying to save. A single property, field group. Whatever.

Next, you have to get into the flow action of that data model's or property's case step. The step you input new data in? Click on the connector that leads away from that. In the process viewer or diagram thing.

Open the action tab and look for the Post Processing section. There you'll call an activity to save your data. It's also the easiest place to create a new one.

Once you're in there, You head to Pages & Classes first and create a new "Page"

Really a "New Page" is like a "New Record." I don't know why they call it a page in this context. 

For its class, you'll look for the one that matches this pattern.


Organization name - Application Name - Data - Your Data Model.

So that's the page stuff.

Next, head back to the steps tab to finish fleshing out this activity.

Here the methods you need to create:

1. Page New
2. Property Set
3. Obj Save

The requirements for these methods look something like this:

|Method|StepPage|
|-|-|
|Page new|The "record" page we just created.|
|Property Set|Hit the arrow to the left of this label {**Left Box:** NewRecordPage.Property#1, **Right Box:** Primary.Property#1|
|Obj Save|The record page we just created.|

That's it.

#### Displaying Saved Data

You don't ***save*** data references. You ***view*** data references.

You ***save*** Embedded Data.

If you define a new data object through view, you can't change its pyGUID easily. I'm sure you can, but it's not easy. So, if you want to set something like the `Account number` of an Account as the GUID, you'll have to define the model in your data types first.
