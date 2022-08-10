# Edit Validate

```java
// Validating a credit card number
Integer integerInput;

try 
{
   integerInput = new Integer(Integer.parseInt(theValue.toString()));
}
catch (java.lang.NumberFormatException ex) 
{
    theProperty.addMessage("Please enter a valid number");
    return false;
}

if (integerInput <= 0) 
{
    theProperty.addMessage("Please enter a valid number greater than 0");
    return false;
}

if (theValue.length() != 10)
{
  theProperty.addMessage("Credit card numbers must be 10 digits long");
  return false;
}

return true;
```

```java
// Date of Birth >= 18

if (theValue.trim().length() == 0) {
    return false;
}
java.util.Date  theDate = tools.getDateTimeUtils().parseDateTimeString(theValue);

if (theDate != null && ! theDate.after(tools.getDateTimeUtils().parseDateTimeString("20040810T001940.553 GMT"))){
  return true;
}

theProperty.addMessage("You must be 18 years or older to purcahse a new mobile plan");
return false;
```
