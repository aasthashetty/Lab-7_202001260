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
> 1.	v = 2, a = {4,2,3,2,1}, expected output: 2   
> 2.	v = 3, a = {4,2,3}, expected output: 1 
> 3.	v = 20, a = {1,2,3}, expected output: 0   
> 4.	v = 1, a = {}, expected output: 0  

> JUnit Testing:
> ![image](https://user-images.githubusercontent.com/75676900/232836686-02564939-a1e4-4e8e-9f9a-06fdfc45863e.png)
> ![image](https://user-images.githubusercontent.com/75676900/232836727-61768125-94e1-4f08-a678-88cb0081855a.png)


P3. The function binarySearch searches for a value v in an ordered array of integers a. If v appears in the array a, then the function returns an index i, such that a[i] == v; otherwise, -1 is returned. Assumption: the elements in the array ‘a’ are sorted in non-decreasing order.
![image](https://user-images.githubusercontent.com/75676900/232836562-7fc3c081-1a4c-45b2-9e71-dc1ed7f63fce.png)

> Equivalence Partitioning: 
![image](https://user-images.githubusercontent.com/75676900/232836874-296b0155-7c68-46a5-9129-efc951a9e5a2.png)

> Boundary Value Analysis:
![image](https://user-images.githubusercontent.com/75676900/232836977-34e9859f-e21c-485b-95a7-79966205eec7.png)

> Test Cases:   
> 1.	v = 2, a = {0,1,2,3,4}, expected output: 2   
> 2.	v = -4, a = {1,2,3,4,5}, expected output: -1   
> 3.	v = 5, a = {2,3,4,5,5,6}, expected output: 3 or 4   

> JUnit Testing:
![image](https://user-images.githubusercontent.com/75676900/232837131-2f0182e6-6d0f-4fd1-86af-29bd20d2de2f.png)
![image](https://user-images.githubusercontent.com/75676900/232837174-fb0d455b-6bab-449d-8f68-a507cc9e503f.png)


P4. The following problem has been adapted from The Art of Software Testing, by G. Myers (1979). The function triangle takes three integer parameters that are interpreted as the lengths of the sides of a triangle. It returns whether the triangle is equilateral (three lengths equal), isosceles (two lengths equal), scalene (no lengths equal), or invalid (impossible lengths).
![image](https://user-images.githubusercontent.com/75676900/232837334-186cda53-8433-4d05-b23e-e2303a678b82.png)

> Equivalence Partitioning:
> ![image](https://user-images.githubusercontent.com/75676900/232837729-bab64a6b-89e1-4e20-9a27-a7da9616fa53.png)

> Boundary Value Analysis:
> ![image](https://user-images.githubusercontent.com/75676900/232837795-0fbab50a-3799-45f7-905d-6fb5e3676a83.png)

> Test Cases: 
> 1.	a = 4, b = 4, c = 4, expected output: EQUILATERAL 
> 2.	a = 1, b = 2, c = 3, expected output: INVALID 
> 3.	a = -1, b = 2, c = 3, expected output: INVALID 
> 4.	a = 3, b = 4, c = 5, expected output: SCALENE 
> 5.	a = 5, b = 5, c = 9, expected output: ISOSCELES 
> 6.	a = 5, b = 5, c = 10, expected output: INVALID

> JUnit Testing:
![image](https://user-images.githubusercontent.com/75676900/232837962-8e34d26e-73e5-4d8d-9389-4ff5ca2250d7.png)
![image](https://user-images.githubusercontent.com/75676900/232837984-018e3cca-7a59-4d53-bed4-b536948fec98.png)

P5. The function prefix(Strings1,Strings2) returns whether or not the string s1 is a prefix of string s2 (you may assume that neither s1 nor s2 is null).
![image](https://user-images.githubusercontent.com/75676900/232838121-c900f9d8-11f7-4aa3-92dc-36189d1be0e5.png)

> Equivalence Partitioning:
> ![image](https://user-images.githubusercontent.com/75676900/232838241-4495c7f0-ea14-4b31-8029-4d1128025468.png)

> Boundary Value Analysis:
> ![image](https://user-images.githubusercontent.com/75676900/232838360-f0f08128-1bc8-4861-996e-fab569acc5a2.png)

> Test Cases: 
> 1.	s1 = “soft”, s2 = “software”, expected output: true 
> 2.	s1 = “abd”, s2 = “abc”, expected output: False 
> 3.	s1 = “health”, s2 = “health”, expected output: True 
> 4.	s1 = “one”, s2 = “two”, expected output: False 
> 5.	s1 = “”, s2 = “pdf”, expected output: True 

> JUnit Testing:
> ![image](https://user-images.githubusercontent.com/75676900/232838921-85888dde-3511-438b-b885-b58d8cd7dfbc.png)
![image](https://user-images.githubusercontent.com/75676900/232838951-552ba586-af9d-4447-bd8e-bd502c7ee36d.png)

















