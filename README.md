# Lab-7_202001260

# IT314 Software Engineering

## Testing

### Section A

Consider a program for determining the previous date. Its input is a triple of day, month and year with the following ranges 1 <= month <= 12, 1 <= day <= 31, 1900 <= year <= 2015. The possible output dates would be the previous date or invalid date. Design the equivalence class test cases?

> From the given constraints 1 <= month <= 12, 1 <= day <= 31, 1900 <= year <= 2015, The following are the equivalence classes obtained.
 
> There are a total of 9 equivalence classes.   
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

**P1.** The function linearSearch searches for a value v in an array of integers a. If v appears in the array a, then the function returns the first index i, such that a[i] == v; otherwise, -1 is returned.

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

**P2.** The function countItem returns the number of times a value v appears in an array of integers a.

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


**P3.** The function binarySearch searches for a value v in an ordered array of integers a. If v appears in the array a, then the function returns an index i, such that a[i] == v; otherwise, -1 is returned. Assumption: the elements in the array ‘a’ are sorted in non-decreasing order.
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


**P4.** The following problem has been adapted from The Art of Software Testing, by G. Myers (1979). The function triangle takes three integer parameters that are interpreted as the lengths of the sides of a triangle. It returns whether the triangle is equilateral (three lengths equal), isosceles (two lengths equal), scalene (no lengths equal), or invalid (impossible lengths).
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

**P5.** The function prefix(Strings1,Strings2) returns whether or not the string s1 is a prefix of string s2 (you may assume that neither s1 nor s2 is null).  
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

**P6.** Consider again the triangle classification program (P4) with a slightly different specification: The program reads floating values from the standard input. The three values A, B, and C are interpreted as representing the lengths of the sides of a triangle. The program then prints a message to the standard output that states whether the triangle, if it can be formed, is scalene, isosceles, equilateral, or right angled. Determine the following for the above program:

a) Identify the equivalence classes for the system 

> The following are the equivalence classes for different types of triangles.  
> 1. INVALID case:   
> * E1: a + b <= c   
> * E1: a + c <= b 
> * E1: b + c <= a 

> 2. EQUILATERAL case:   
> * E1: a = b, b = c, c = a 

> 3. ISOSCELES case:   
> *  E1: a = b, a != c   
> *  E1: a = c, a != b   
> *  E1: b = c, b != a   

> 4. SCALENE case:   
> *  E1: a != b, b != c, c != a   

> 5. RIGHT-ANGLED TRIANGLE case: 
> * E1: a2 + b2 = c2 
> * E1: b2 + c2 = a2 
> * E1: a2 + c2 = b2 


b) Identify test cases to cover the identified equivalence classes. Also, explicitly mention which test case would cover which equivalence class. (Hint: you must need to be ensure that the identified set of test cases cover all identified equivalence classes)
> ![image](https://user-images.githubusercontent.com/75676900/232840409-aeea885d-90b5-47be-ae2e-bc16e6a0f5ad.png)


c) For the boundary condition A + B > C case (scalene triangle), identify test cases to verify the boundary. 
> The test cases to verify boundary condition: 
> 1. a = 5, b = 4, c = 5 
> 2. a = 5, b = 5, c = 9 
> 3. a = 5, b = 6, c = 12 

d) For the boundary condition A = C case (isosceles triangle), identify test cases to verify the boundary. 
> The test cases to verify boundary condition: 
> 1. a = 5, b = 4, c = 5 
> 2. a = 5, b = 4, c = 5.1 
> 3.. a = 5, b = 4, c = 4.9 

e) For the boundary condition A = B = C case (equilateral triangle), identify test cases to verify the boundary. 
> The test cases to verify boundary condition: 
> 1. a = 5, b = 5, c = 5 (a =b=c) 
> 2. a = 10, b = 10, c = 9 (a=b but a!=c) 
> 3. a = 10, b = 11, c = 10 (a=c but a!=b) 

f) For the boundary condition A2 + B2 = C2 case (right-angle triangle), identify test cases to verify the boundary. 
> The test cases to verify boundary condition: 
> 1. a = 3, b = 4, c = 5 
> 2. a = 5, b = 12, c = 13 

g) For the non-triangle case, identify test cases to explore the boundary. 
> The test cases to verify boundary condition: 
> 1. a = 1, b = 2, c = 3 
> 2. a = 4.5, b = 5.5, c = 10 

h) For non-positive input, identify test points. 
> The test points for non-positive inputs: 
> 1. a = -4.0, b = 3.2, c = 4.5 
> 2. a = 5, b = -4.2, c = -3.2 


### Section B 


The code below is part of a method in the ConvexHull class in the VMAP system. The following is a small fragment of a method in the ConvexHull class. For the purposes of this exercise you do not need to know the intended function of the method. The parameter p is a Vector of Point objects, p.size() is the size of the vector p, (p.get(i)).x is the x component of the ith point appearing in p, similarly for (p.get(i)).y. This exercise is concerned with structural testing of code and so the focus is on creating test sets that satisfy some particular coverage criterion.

![image](https://user-images.githubusercontent.com/75676900/232841293-3b640cc9-5e63-46f5-858a-d87bd91f2925.png)

For the given code fragment you should carry out the following activities.

1. Convert the Java code comprising the beginning of the doGraham method into a control flow graph (CFG).
> ![image](https://user-images.githubusercontent.com/75676900/232841474-17fa7cde-a127-44d7-b030-fb19c0c76cae.png)


2. Construct test sets for your flow graph that are adequate for the following criteria:   
a. Statement Coverage.     
b. Branch Coverage.   
c. Basic Condition Coverage.

> The following are the test cases and their corresponding coverage of statements: 

> 1. p=[(x = 2, y = 2), (x = 2, y = 3), (x = 1, y = 3), (x = 1, y = 4)]   
> Statements covered = {1, 2, 3, 4, 5, 7, 8}   
> Branches covered = {5, 8}   
> Basic conditions covered = {5 - false, 8 - false}   

> 2. p=[(x = 2, y = 3), (x = 3, y = 4), (x = 1, y = 2), (x = 5, y = 6)]   
> Statements covered = {1, 2, 3, 4, 5, 6, 7}   
> Branches covered = {5, 8}   
> Basic conditions covered = {5 - false, true, 8 - false}  
 
> 3. p=[(x = 1, y = 5), (x = 2, y = 7), (x = 3, y = 5), (x = 4, y = 5), (x = 5, y = 6)]   
> Statements covered = {1, 2, 3, 4, 5, 6, 7, 8, 9}   
> Branches covered = {5, 8}   
> Basic conditions covered = {5 - false, true, 8 - false, true}   

> 4. p=[(x = 1, y = 2)]   
> Statements covered = {1, 2, 3, 7, 8}   
> Branches covered = {8}   
> Basic conditions covered = {}   

> 5. p=[]   
> Statements covered = {1, 2, 3}   
> Branches covered = {}   
> Basic conditions covered = {}   

> Thus, the above 5 test cases are covering all statements, branches and conditions. These 5 test cases are adequate for statement coverage, branch coverage and basic condition coverage.


























