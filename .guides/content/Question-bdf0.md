Now take a look at the following question and see how much you have learned.

Complete the following program, by selecting the correct code. 

The program is used to authenticate a user by checking that their login name exists and then matching the password they entered with one that is stored.
To make it simpler no validation is used.

The login names and passwords are stored in a 2-D array named ‘users’ as
users[[“user1], [password1], [user2], [password2], [user3], [password3] etc.]

*The program has been split into two parts as shown below and to demonstrate how indentation makes programs easier to understand, it has been removed!*

{Check It!|assessment}(fill-in-the-blanks-112428771)
|||guidance
# Solution
nameExists = False
while nameExists == **False**
inputName = input(“Please enter your login name.”)
for index = **0 to users.length – 1**
if users[index, 0] == inputName then
**nameExists = True**
endif
next index
if **nameExists == False then**
print(“That login name does not exist.”)
endif
endwhile
|||

{Check It!|assessment}(fill-in-the-blanks-849792925)
|||guidance
# Solution
passwordCorrect = False
**while passwordCorrect == False**
inputPassword = input(“Please enter your password.”)
if inputPassword == **users[index, 1] then**
passwordCorrect = True
**else**
print(“Sorry. The password is incorrect.”)
endif
endwhile
|||