# Lesson 2. Variables 

## What you will Learn 
- What variables are 
- How to store information 
- Different types of data 
- How to name things 

## What is a variable 
a variable is basically a labeled box in which you put different types of data in it 
in crystal each box can only contain or store a single type of data i.e you can't put a string in a box of Int
```crystal
x = 64 
```
The above code is a variable x holding 64( an  Integer )
a box labeled x in the box there is 64 in it 

crystal is smart enough to determine your data type 
you can also explicitly tell crystal e.g 
```crystal 
x : Int32 = 64 
```
This way you are telling crystal that variable x is an integer attempting to add a string will result in error 

## Creating variables 
```crystal
name = "syscr"
age = 17
country = "Nigeria"
is_male = true
```
The above crystal code contains different data types 
String 
Int 
String
Bool
it can also be written as 
```crystal
name : String = "name"
age : Int32 = 17
country : String = "Nigeria"
is_male : Bool = true 
```
as programmers, we are lazy you will agree with me the first version is better just focus on writing and let the compiler figure it out 

## Why Types (data types) matters 
Try this 
```crystal
age = 17
puts age + 10 
# this will work age is int and 10 is int 
```
```crystal
age = 17 
puts age + "10" # Error can't add number to text 
# This isnt the actual error response but just know you can't and shouldn't mix up types 
```
## Naming your variables 
as a quote i saw from the Odin project which says "write codes as if the future maintainer is the most laziest person on earth"
i doubt if this is the exact text but what am just trying to say is you should try make you codes readable 
```text 
crystal allows you to name variables 
but it shouldn't begin with a number 
and capital letter should be reserved for Constants 
and shouldn't be a keyword reserved for the compiler use  
shouldnt contain special characters like @ % ... 
```
```crystal
first_name = "John"
# clean readable
user_age = 23
```
## Changing a variable 
you can assign a new value to an already initialized variable crystal uses the new one 
> you still can't  change the data type 
```crystal
age = 17
puts age # 17 
age = 19 
puts age # age is now changed to 19 
age = 24
puts age # is now 24 
age = "13"
puts age # Error different data types 
```crystal

## Constants: Variables That Never Change

Sometimes you have values that should stay the same throughout your program. Crystal lets you create constants for this.

```crystal
Age = 17  # Notice the capital A
puts Age  #17
```
```crystal
Age = 17 
puts Age # 17 
Age = 19 
puts Age # Error Age is a const
``` 
## Common Mistake 
```crystal 
name = John 
# the compiler will think John here is a variable 
name = "John" 
# correct way with double quotes 
name = 'John' 
# still correct with single quotes 
```
```crystal
# using wrong names 
my-name = "John"
# wrong no hypen 
my_name = "John"
# correct way
```
## Summary 
- variables store information 
- Different types: Int, String, Bool...
- Types can't change once sets 
- Constant

## Additional Resources 
- [Assignments](https://crystal-lang.org/reference/1.19/syntax_and_semantics/assignment.html)
- [local](https://crystal-lang.org/reference/1.19/syntax_and_semantics/local_variables.html)

