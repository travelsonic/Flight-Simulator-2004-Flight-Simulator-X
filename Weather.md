# Weather Related Notes:
## Altitude:
Altitude is entered by the user as an integer representing the altitude in feet.

The altitude is also represented as in integer, and in feet, for the purposes of
displaying altitudes on the chart where you can line up weather layers, and the like.

Internally, this value is stored as a 32-bit float representing the altitude in meters.


## Temperature:
Temperature is entered by the user as an integer value representing the temperature in Fahrenheit.

Internally the value is stored as a 32-bit float that represents the temperature in Celsius.


## Wind 
### Sustained and Gust-To Wind Speeds:
Wind is entered by the user as an integer value, representing the wind speed and wind gust speed
in knots.

Internally, this value is stored as a 32-bit float.

You can easily edit the limits that the text box, and adjacent up/down control to have a value range 
of -2,147,483,648 <= X <= 2,147,483,647.  This value, however, is only for what input the user
enters, and doesn't get used to validate that the value is in the correct range.

### Wind Shear Strength
This value is a simple integer that has a value of 0 <= X <= 3, with one value representing
each of the wind shear strengths for a wind layer (Gradual, Moderate, Steep, and Sharp).

TODO: Learn how this interacts with wind speed - whether it is a multiplier, or whatnot.
