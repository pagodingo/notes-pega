# <u>Pega 3-3</u>

1. Create Data Type: ProductsCatalog
    - Add fields: Product(name,id,price,etc.)
    - Set ID as P Key
2. Configure Data Type Source -> Under Sources
3. Create Case Type: Product Something
4. New Stage -> Create Step -> Configure view -> New Property (new property - emb data) -> Data obj Product catalog (default view)
5. Go to Data Types -> Savable Products Catalog
6. Change source to Data Transform -> DT: "SaveProduct" -> Open Target -> Save (create/open)
7. Under Pages Classes -> Add pyWorkPage -> Class name is Case Type Class. Org-App-Work-CaseType
8. In DT Definition -> Set Target as .{fieldToSave} -> Set Source as pyWorkPage.{FieldGroup-embdata}.ProductId.
9. The DT will handle saving data, therefore the target can just be .{fieldToStore}.

We're using Data Transformations to copy data from one class to another. In our example, data is moving from the Work class  to Data.

Source: Data Transform (Savable Products Catalog).

Save Type: DB Save - Class name (Products Catalog).

10. Back in our case type - add our next stage step - Save Data (Automation) -> under settings add Data Page D_ProductsCatalogSavable
11. Save your work!

12. There should be no parameters in your 'Save Data Page' Step.

13. Create and run your case to see if everything checks out.

## Decisions

1. Create Case -> DemoDecisions
2. Create Step -> User Documents
    - Fields -> Name, Email, Mobile
    - Boolean Field -> SSN?, Drivers License? Passport?

> If you mess up, fields can be deleted from under 'Data Model' inside of your casetype.

3. Add three more steps to our case:
    - Upload SSN
    - Passport
    - Upload License
4. Open Flow Process
5. Right click empty space in diagram - "Add Decision"
6. Save Decision type as fork.
7. Feed the user documents step into the decision (using flow diagram arrows).
8. Under Connector Properties, Create a When inside of your connector (between Decision and next step). We're configuring first our "when SSN" condition.
9. *When "checkSSN" is true*
10. Repeat for your other documents
     - Drivers license
     - Passport
     - *When "x" is true*, *When "passport" is true*
11. Your decision should flow into three different steps. All corresponding to which documents the user has present.
12. Change the likelihood for the three:
    - SSN = 100
    - Drivers license = 70
    - Passport = 40
13. Ensure your steps do not connect to eachother. They should all be connected to your Decision independently from one another.


## Decision Tables

1. In prev case type - create stage Product Catalog
2. Create Step -> Choices
    - Fields (Place (PL), Price(Cur), # Passengers(Int))
3. Based on # of Passengers, we want to change price.
4. Whenever the place or # of passengers - price should be updated.
5. Open App Explr
6. Expand your case type -> Data Model -> Property (right click) -> Declare Expression
7. In Declare Expression - Price -> build Expressions -> Set Price = Result of Decision table
8. Create a Decision Table: **Price Decision** -> Open Target
9. Create & Open

| place | # of passengers|Return |
|---|---|--|
|Columbia| 2|  300.00|
|Columbia| 4|  500.00|
|Peru| 2|  500.00|
|Argentina| 2|  700.00|

<u>otherwise -> 0</u>

Decision Table property Chooser:

Property: ".OfPassengers

10. In your case type -> Stages & Steps -> Save & run

To find Declare Expressions: Data model -> Right click property -> Create Define Expression

## SQL In Pega: Tables

Where to find (all tables):

- Data Model: Classes and Properties (Landing Page) in Recents: Class Categories (work)

The Work table contains all properties belonging to your particular app.

|Term|Definition|
|-|-|
|Exposed/Mapped|User Accessible Properties|
