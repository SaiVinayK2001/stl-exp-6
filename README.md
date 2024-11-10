# Ex.No: 6 To check whether the string is Palindrome and generate test cases.

### DATE:   17/09/2024                                                                         
### REGISTER NUMBER : 212222040006
### AIM: 
Write a Python program to check whether the string is Palindrome and generate test cases. 
### Algorithm:
1. Start
2. Get an input from the user by prompting 
3. Run a loop form 0 to len/2.
4. Check if the characters are the same both from the start and the end till len/2. 
5. If it is, return the result that it is a palindrome.
6. Else, return that it is not a palindrome. 
7. Stop the program.
### Program:
```

def Palindrome(string): 
    for i in range(0, int(len(string) / 2)): 
        if string[i] != string[len(string) - i - 1]:  # Corrected comparison
            return False 
    return True

s = input("Enter a string: ")
c = 1

# Check if the input contains only alphabetic characters
for i in s:
    if not i.isalpha(): 
        c = 0

if c == 0: 
    print("Enter a valid string containing only alphabetic characters.")
else:
    # Check if the string is a palindrome
    answer = Palindrome(s)
    if answer == True: 
        print("The given string is a palindrome.")
    else: 
        print("The given string is not a palindrome.")


```












### Output:

![Screenshot 2024-11-10 222319](https://github.com/user-attachments/assets/9333853c-691b-4f8b-be5d-89a762993919)




### Result:
Thus, a program to check palindrome has been written and test cases have been written and verified successfully.
