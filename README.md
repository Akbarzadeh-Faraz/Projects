simple database management system for a cruise company. The system maintains records for its passengers for a trip. 
Each record contains name, age, embark port, and the fare paid, and the cabin class (e.g., Economic, Middle, UpperMiddle), which
is based on the embark port and fare. If a passenger’s fare info has been updated, then a history of classes is maintained.
The database maintains a collection of member records.
The program will provide several basic functionalities:
• Accepting entry of a new passenger record into the current database, and generating the cabin
class for the passenger.
• Displaying all records in the current database
• Removing an existing passenger’s record in the current database
• Updating fare info of an existing passenger, and generating new cabin calss for the
member
• Sorting the records in the current database
• Clearing the current database
Specifically, the program keeps on prompting the user with a menu, until q or Q is chosen, which terminates the program.
The program should fulfill the following functionalities:
• Keeps on prompting and responding to user inputs. Valid input includes N/n, D/d, U/u,
C/c, R/r, S/s and Q/q. 
When the users enter n or N, which represents New record, the program further prompts the
user to enter a new passenger record into the database. The function reads in the passenger’s
name, age, embark port and fare paid (in $). It then calculates the cabin class for the new
passenger. The function then creates a new passenger record and inserts the new record into
the database (i.e., the pointer array).
The company operates three embark ports: Cherbourg, Queenstown, Southampton
Cabin classification is calculated based on embark port and the fare paid, as show in the table:

Cherbourg            Queenstown         Southampton          Cabin classes
fare < 9             fare < 7           fare < 8             Economic
9 ≤ fare <30         7 ≤ fare <18       8 ≤ fare <24         LowerMiddle
30 ≤ fare <100       18 ≤ fare <76      24 ≤ fare < 80       Middle
100 ≤ fare <200      76 ≤ fare < 150    80 ≤ fare < 180      UpperMiddle
fare ≥ 200           fare ≥ 150         fare ≥ 180           Wealthy

Assume the user enters the correct port name, i.e., one of Cherbourg, or Queenstown or
Southampton.
• When the user enters d or D, displays the current database of (all) patient records.
• When the user enters c or C, clear the current database. 
When user chooses R or r, which represents Remove record, the system should
further prompt the user for the name of the member whose record is to be removed
(case sensitive). If no record by that name is found in the current database, then the
error message “record not found!” should be printed out. If the record is found, the
record is removed from the database, with message “record [xx] removed successfully”. 
When the user chooses u or U, which represents Update record, the system allows a
user to update fare info of existing passengers. The system prompts the user for the name
of the passenger whose record is to be update (case sensitive). If no record by that name is
found in the current database, then the error message “record not found!” should be
displayed. If the record is found, the system further prompts the user for a new fare. It
then displays message “record [xx] updated successfully”. Internally, the system replaces
the existing fare of the passenger. Also, calculate the new cabin class using the new fare,
and append the new class to the existing class(es). (Assume a passenger’s embark port
never changes). This way, the system keeps track of the class changes of the passenger.
When the user chooses S or s, which represents Sort database, the program further
prompts the user with an option to sort records based on name (in alphabetic order) or based
on the current fare (in ascending order). The function then sorts the database accordingly.
Assume the user entered either n or f,




