# <u>Pega 2-2</u>

## Properties and Data Models

### What are Data Models and Properties in Pega?

`Every application accesses data`

Data Models, properties such as First Name, Last Name, these are different types of data models. Data Models define the data structure of case types.

All properties belonging to a case type live inside of the Data Model tab of said case type.

Single element properties are reffered to as data elements.

Properties with multiple elements are considered Data Objects or Data Types.

### Field Groups

One-to-one, one-to-many. 1-1 are represented using Field Groups. 1-many are stored using Field Group Lists.

### Reading Properties

Properties names in Pega stored with no spaces, and begin with a ".".

`Example, a property with the name Shop Details, will be stored as
.ShopDetails.`

### Page Mode

- Single Page
  - Storing a single value in a property is (PersonalDetails). Access is done by using dot notation (PersonalDetails.)
- Page List
  - Storing multiple values (ExperienceDetails).
    can only be accessed by specifying the index first. (ExperienceDetails(1).YearsOfExperience).

- Page Group
  - Address. (Address(Shipping), Address(Billing))

Page Mode properties

### Value Mode

- Single Value
  - (FN,LN)
- Value List
  - List of Values (Multiple), example, list of best friends. (.BestFriend(1).Daniel)
- Value Group
  - BestFriend

Page Lists vs. Value Lists = Data Objects | Data Elements.

score of Top in class = Value List
Multi Value Multi records = Page List
Multi value Single Record = Value List

## Data relationships

### Relationships between data objects

A data object is a template for describing an entity through fields, such as name and address. A data relationship is a container in which you associate a set of related fields. You can use data relationships to create relationships between data objects and also between cases. A data relationship does not store data itself but instead relates data.

For example, when customers sign up for a video streaming account, they provide basic information such as first name, last name, and email. The value provided in the email field must be associated with the customer's first and last name because that email belongs to the customer. The system can capture the three associated values in a Customer data relationship.

In the Customer data relationship example, the data relationship establishes a common context for the first name, last name, and email fields. These fields all contain data that describe a customer, as shown in the following image.

### Data relationships with multiple records

You can configure data relationships to reference a single record or multiple records. The difference is that a multiple record data relationship references a list of grouped values. A single record data relationship references only a single set of values. **The Customer data relationship example in the previous section demonstrates a single record data relationship.**

Data Reference = Database
Case Reference = Case fields or state

### Predefined Pega properties

pX, pY, pZ

- **px**- Properties with prefix px are Read Only and cannot be overridden or extended by your application. These are generally used to support your application.

- **py**- Properties with prefix py are Read/Write so can be overridden in your application.

- **pz**- Properties with prefix pz are Read Only and cannot be overridden or extended by - your application.

Pega properties have access controls.

pX Example - Date time property.

You want to create a list of products and their attributes to use as reference data in an application. Which method do you use to create the reference data?

> Configure a Products data object with a local system of record and add your data records to the Products data object.

### Data pages and the Visual Data Model

[^1] In App Studio, data pages show how your application uses data and defines the data associated with a data object. Data pages provide links between data records and your application. The Visual Data Model is a diagram that shows these links by providing visibility into the application's data model and how the entities are related. You can update, add, and delete fields while viewing the Visual Data Model.

 **Note: In previous versions of Pega Platform™, data pages were called data views.**

Data pages are very reminiscent of Database Schematics

In App Studio, data pages identify how to obtain data from a system of record.

### Integration Designer

The Integration Designer provides a single location in App Studio for viewing all the data objects, data pages, object dependencies, and external systems in an application. The Integration Designer also provides insight into how these entities are connected.

### Integration Map

The Integration Map is a diagram of the data objects, cases, and systems of record in the application and where they are sourced. The Integration Map can optionally be displayed above the Integration Designer.

The Integration Designer helps you understand how the data objects, data pages, case types, and systems of record relate to one another.

### Data Pages Review

Data stored in Pega = System of Records

External data = External Systems of records

No data storage = no system of records.

Data pages is to access and review Data Types

Process -> Create data type -> Field -> Add record.

Single, List and Saveable.

All data pages will start with "D_".
