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