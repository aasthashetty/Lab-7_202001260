# Lab-7_202001260

# IT314 Software Engineering

## Testing

### Section A

Consider a program for determining the previous date. Its input is a triple of day, month and year with the following ranges 1 <= month <= 12, 1 <= day <= 31, 1900 <= year <= 2015. The possible output dates would be the previous date or invalid date. Design the equivalence class test cases?

> From the given constraints 1 <= month <= 12, 1 <= day <= 31, 1900 <= year <= 2015, The following are the equivalence classes obtained.
 

>There are a total of 9 equivalence classes. 

>E1 = {1 <= date <= 31}    
  E2 = {date < 1} 
  E3 = {date > 31} 
  E4 = {1 <= month <= 12} 
  E5 = {month < 1} 
  E6 = {month > 12}
  E7 = {1900 <= year <= 2015} 
  E8 = {year < 1900} 
  E9 = {year > 2015} 

> The following are the weak normal equivalence class test cases: 
 ![image](https://user-images.githubusercontent.com/75676900/232832048-c51b0d8f-85fa-41ae-8668-3a191551c326.png)

Write a set of test cases (i.e., test suite) – specific set of data – to properly test the programs. Your test suite should include both correct and incorrect inputs. 
1.	Enlist which set of test cases have been identified using Equivalence Partitioning and Boundary Value Analysis separately.
2.	Modify your programs such that it runs on eclipse IDE, and then execute your test suites on the program. While executing your input data in a program, check whether the identified expected outcome (mentioned by you) is correct or not.
Programs:

P1. The function linearSearch searches for a value v in an array of integers a. If v appears in the array a, then the function returns the first index i, such that a[i] == v; otherwise, -1 is returned.





