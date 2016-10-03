Validation is the process of checking that all input is sensible, reasonable and appropriate to be processed by the program.

Sanitisation is the process of checking the input to ensure it is safe and is not intended as a security threat to the system e.g. SQL injection. In this case the input must be modified.

The programmer should incorporate validation routines for all of the possible types of input they can predict users will make and the ways in which users may try to misuse the system.
By doing this they are planning for contingences and anticipating misuse.

For example validation routines could: 

**Check that data has in fact been entered**
Often users may press the Enter key without actually making any input. A validation routine should check for this and one is shown below.
```
entered = “”
while entered == “”
	entry = input(“Please enter your choice.”)
	if entry == “” then
		print(“No entry has been made.”)
	end if
endwhile
```
A condition controlled loop has been used to check that an entry has been made. The loop will repeat if none is made and print an error message.

**Check that the entry is within a certain range**
Often a user may enter a number, either deliberately or by mistake, which is obviously incorrect and a range check should be used to check for this. 
For example they may have to enter the month of their birth as a number which should obviously be between 1 and 12. A way to do this is shown below.
```
correctMonth = False
while correctMonth == false
	month = input(“Please enter the month of your birth as a number.”
	if month >= 1 AND month <=12 then
			correctMonth = True
	else
		print(“Sorry but your entry is not between 1 and 12.”)
	endif
endwhile
```

**Check that the entry is of a required length**
This can be used to check that a fixed length password has been entered correctly.
For example if the required number of characters is 8 then the following routine could be used.
```
password = input(“Please enter the password.”)
if password.length != 8 then
	print(“Sorry. You have not entered the correct number of characters.”)
endif
```
Obviously other checks will also need to be made i.e. whether the correct characters have been entered.
