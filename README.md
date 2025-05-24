# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM
 ```
//Sudharsan S
//Reg no : 212224040334
#include <stdio.h>
int main() {
    int n = 44;
    int s = 3;
    int r = n << s;

    printf("Original number: %d\n", n);
    printf("After left shifting by %d positions: %d\n", s, r);

    return 0;
}

```
## OUTPUT
![image](https://github.com/user-attachments/assets/451eae37-cb8e-48ba-8fd2-1ebf9a46ed18)


## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.

## PROGRAM
```
//Sudharsan S
//Reg no : 212224040334
#include <stdio.h>
int main() {
   int a,b;
   printf("Enter the first number : ");
   scanf("%d",&a);
   printf("\nEnter the second number : ");
   scanf("%d",&b);
   if(a==b) printf("\nBoth are equal.");
   else printf("\nBoth not are equal.");
}

```

## OUTPUT
 ![image](https://github.com/user-attachments/assets/a6526ddc-bec0-443e-9c94-7252ae917f11)
          
## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
//Sudharsan S
//Reg no : 212224040334
#include <stdio.h>
#include <ctype.h>
int main() {
   char str[100];
   printf("Enter the string : ");
   scanf("%[^\n]",str);
   printf("\n");
   int i=0;
   for(;str[i]!='\0';i++){
       if(isupper(str[i])){
           str[i] = tolower(str[i]);
       }
   }
   printf("String after conversion to lowercase: %s",str);
}

```
## OUTPUT

![image](https://github.com/user-attachments/assets/3f20211b-470d-4669-9cc6-7131e7243ac3)



## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
//Sudharsan S
//Reg no : 212224040334
#include <stdio.h>
int main() {
   char str[100];
   printf("Enter the string : ");
   scanf("%[^\n]",str);
   int i=0,c=0;
   do{
       if(str[i]==' ') c++;
       i++;
   }while(str[i]!='\0');
   printf("\nThe total number of words in the given string is: %d",c);
}
```
## OUTPUT

![image](https://github.com/user-attachments/assets/d82b982d-3eb0-4572-b843-a0c3c8d5cd48)


## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
Step 1: Start the program.
Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable
             flag and initialize it to 0, and i for indexing.      
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered 
            (i.e., can include spaces).
Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no 
            spaces in the second string).
Step 5: Start comparing characters of both strings from index i = 0.
Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
•	If c1[i] is not equal to c2[i], set flag = 1.
•	Increment i by 1.
Step 7: After the loop, check the value of flag:
•	If flag == 0, print "strings are same".
•	Otherwise, print "strings are not same".
Step 8: End the program.

## PROGRAM
```
//Sudharsan S
//Reg no : 212224040334
#include <stdio.h>
int main() {
   char str1[100], str2[100];
   printf("Enter the string1 : ");
   scanf(" %[^\n]",str1);
   printf("\nEnter the string2 : ");
   scanf(" %[^\n]",str2);
   int s1l=0,s2l=0, f = 0;
   while(str1[s1l]!='\0')s1l++;
   while(str2[s2l]!='\0')s2l++;
   if(s1l==s2l){
      for(int i=0;i<s1l;i++){
          if(str1[i]!=str2[i]){
              f=1;
              break;
          }
      } 
   }
   else f=1;
   if(f==0) printf("\nStrings are same");
   else printf("\nStrings are not same");
  
}
```

## OUTPUT
 ![image](https://github.com/user-attachments/assets/28bf6018-0d57-4161-b4b4-9036ef0472e1)


## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

