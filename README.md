# Regex Date/Time

## Due: Tue 2/28 at 11:59 PM

- Create a program called `RegexDateTime.java`
- Prompt the user for a filename containing dates
- Prompt the user for a filename containing times
- Prompt the user for a filename containing datetimes
- Read in all the lines from the dates file into an ArrayList
- Read in all the lines from the times file into another ArrayList
- Read in all the lines from the datetimes file into another ArrayList
- Print whether each date is a valid date or not
  - A date is valid if it follows any of the following formats where months and days can have leading zeroes or not and each number is valid for that field
    - MM-DD-YYYY
    - MM/DD/YYYY
    - MM-DD-YY
    - MM/DD/YY
- Print whether each time is a valid time or not
  - A time is valid if it follows any of the following formats where # is a digit, follows either military time or standard time, and each number is valid for that field (hours can have a leading zero or not)
    - ##:##
    - ##:## AM (not valid if time is in military time)
    - ##:## PM (not valid if time is in military time)
- Print whether each datetime is a valid datetime or not
  - A datetime is valid if it follows the format for date and time
    - A datetime can have the date then the time or the time then the date

***Example Input:***\
date1.txt\
time1.txt\
datetime1.txt\
***Example Output:***\
AABBCC is a valid hex color code\
ZZ9900 is not a valid hex color code\
001122 is a valid hex color code\
00HH33 is not a valid hex color code\
AA99FF is a valid hex color code\
123456 is a valid hex color code\
#$!@%& is not a valid hex color code\
ABCDEF is a valid hex color code\
ABCDHH is not a valid hex color code\
ABCDE is not a valid hex color code\
0-1+2/ is not a valid hex color code\
\
(123) 456-7890 is a valid phone number\
123 456 7890 is not a valid phone number\
(123) 45-7890 is not a valid phone number\
1234567890 is a valid phone number\
123456789 is not a valid phone number\
(123) 456 7890 is not a valid phone number\
123-456-7890 is a valid phone number\
23-456-7890 is not a valid phone number\
123-4456-7890 is not a valid phone number\
\
abcdef@abc.com is a valid email address\
abc!@#abc.d is not a valid email address\
#$%@abc.com is not a valid email address\
fedcba@fed.org is a valid email address\
abcdef@&*().com is not a valid email address\
abcdef@abc.123 is not a valid email address\
mail@mail.mail is a valid email address
