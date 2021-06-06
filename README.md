# android-number-to-date
python script to transform saved timestamps in android to a human readable date format

example android time
from Android Developers Docs Reference

Time
public class Time
extends Date
java.lang.Object
   ↳ 	java.util.Date
  	   ↳ 	java.sql.Time 

A thin wrapper around the java.util.Date class that allows the JDBC API to identify this as an SQL TIME value. 
The Time class adds formatting and parsing operations to support the JDBC escape syntax for time values.

The date components should be set to the "zero epoch" value of January 1, 1970 and should not be accessed.

public Timestamp (long time)
Constructs a Timestamp object using a milliseconds time value. The integral seconds are stored in the underlying date value; the fractional seconds are stored in the nanos field of the Timestamp object.

long 	getTime()
Returns the number of milliseconds since January 1, 1970, 00:00:00 GMT represented by this Timestamp object

void 	setTime(long time)
Sets this Timestamp object to represent a point in time that is time milliseconds after January 1, 1970 00:00:00 GMT

Parameters
year 	  int: the year minus 1900
month 	int: 0 to 11
date 	  int: 1 to 31
hour 	  int: 0 to 23
minute 	int: 0 to 59
second 	int: 0 to 59
nano 	  int: 0 to 999,999,999


toString
public String toString ()
Formats a time in JDBC time escape format.
Returns
String 	a String in hh:mm:ss format


valueOf
public static Time valueOf (String s)
Converts a string in JDBC time escape format to a Time value.
Parameters
s 	String: time in format "hh:mm:ss"
Returns
Time 	a corresponding Time object


Android forensics: Interpretation of timestamps
https://www.sciencedirect.com/science/article/abs/pii/S1742287614000449
