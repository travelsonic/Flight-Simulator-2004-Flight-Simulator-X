# Weather Related Notes:
## Wind - Sustained and Gust Speeds:
Wind is entered by the user as an integer value, representing the wind speed and wind gust speed
in knots.

Internally, this value is stored as a 32-bit float.

You can easily edit the limits that the text box, and adjacent up/down control to have a value range 
of -2,147,483,648 <= X <= 2,147,483,647.  This value, however, is only for what input the user
enters, and doesn't get used to validate that the value is in the correct range.

## Temperature:
### Input vs Storage
Temperature is entered by the user as an integer value representing the temperature in Fahrenheit.

Internally the value is stored as a 32-bit float that represents the temperature in Celsius.


