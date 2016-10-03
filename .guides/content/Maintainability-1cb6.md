Once a program has been coded it may have to be changed, updated or errors may have to be corrected. This may be some time after it has been created and the programmer may have forgotten exactly how it works or the maintenance may be done by a different programmer.
To make this task easier the logic behind code should be as easy to follow as possible and two ways of accomplishing this are to use:

- **indentation**
  - All code that depends on previous statement should be indented as in the examples above where statements contained within the ‘while’ and ‘if’ constructs are indented. Some programming languages demand indentation.

- **comments**
  - Explanations should be added to show the logic behind the code. Symbols are used to indicate that they are comments and should not be compiled or interpreted. In OCR pseudocode two forward slashes (//) are used. Comments could be added to the code above to check that an input has been made.
```
entered = “”
//The variable ‘entered’ is set to an empty string as the loop will run while it is empty.
while entered == “”
//A ‘while’ loop is started. It will run until an entry is made.
entry = input(“Please enter your choice.”)	
if entry == “” then			
  print(“No entry has been made.”)
    //If no entry is made the user is informed.
  end if
endwhile
//This closes the ‘while’ loop.
```
