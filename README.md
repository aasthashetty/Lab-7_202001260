# Lab-7_202001260

# IT314 Software Engineering

## Testing

### Section A

Consider a program for determining the previous date. Its input is a triple of day, month and year with the following ranges 1 <= month <= 12, 1 <= day <= 31, 1900 <= year <= 2015. The possible output dates would be the previous date or invalid date. Design the equivalence class test cases?

> From the given constraints 1 <= month <= 12, 1 <= day <= 31, 1900 <= year <= 2015, The following are the equivalence classes obtained.
 
>There are a total of 9 equivalence classes.   
  E1 = {1 <= date <= 31}    
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

![image](https://user-images.githubusercontent.com/75676900/232834883-18308785-2b43-47a9-ba0f-b6764bdeb8be.png)

> Equivalence Partitioning:  
![image](https://user-images.githubusercontent.com/75676900/232835016-158eba57-a54b-461a-a719-fd327c004da9.png)

> Boundary Value Analysis:
![image](https://user-images.githubusercontent.com/75676900/232835132-b8a9e150-b0ca-4096-aadb-54ab5638297f.png)

> Test Cases: 
> 1.	v = 2, a = {4,3,2}, expected output: 2  
> 2.	v = 3, a = {4,2,1}, expected output: -1   
> 3.	v = 4, a = {}, expected output: -1   
> 4.	v = 2, a = {1,2,3,2,4}, expected output: 1  

> JUnit Testing:
![image](https://user-images.githubusercontent.com/75676900/232835425-089e302a-264b-48fd-af22-2c964ae285b9.png)
![image](https://user-images.githubusercontent.com/75676900/232835472-efc81c0d-9e06-40ee-bf71-8424a3914f48.png)

P2. The function countItem returns the number of times a value v appears in an array of integers a.

![image](https://user-images.githubusercontent.com/75676900/232836026-9174b54e-ad9e-4d4f-b302-52098377db2e.png)

> Equivalence Partitioning: 
![image](https://user-images.githubusercontent.com/75676900/232836111-2a27742b-19fc-45ad-a33e-ee23ec4fb86d.png)

> Boundary Value Analysis:
![image](https://user-images.githubusercontent.com/75676900/232836182-0f942785-6f9a-44fd-aeef-e0a8a38d23d4.png)

> Test Cases:   
1.	v = 2, a = {4,2,3,2,1}, expected output: 2   
2.	v = 3, a = {4,2,3}, expected output: 1 
3.	v = 20, a = {1,2,3}, expected output: 0   
4.	v = 1, a = {}, expected output: 0  










