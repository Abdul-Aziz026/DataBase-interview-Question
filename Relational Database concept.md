## Why Normalization Need see below 2 picture and guess Why it's needed :)
![image](https://github.com/Abdul-Aziz026/DataBase-interview-Question/assets/57495952/ed487e7d-075f-4062-842f-a156c5983975)

![image](https://github.com/Abdul-Aziz026/DataBase-interview-Question/assets/57495952/ad8cb8fa-b12c-4a17-9bce-9c36bf89f41b)


Normalization Types:
1. First Normal Form (1NF).
2. Second Normal Form (2NF).
3. Third Normal Form (3NF).
4. Boyce-Codd Normal Form (BCNF).
5. Fourth Normal Form (4NF).
6. Fifth Normal Form (5NF).

### First Normal Form (1NF).
**Rules:**
1. Each Colum Must have Unique Names.
2. Each Column must have atomic(single) values.
3. A colum should contain value must be in same type.(Name colum contains only name, Dob contain only DOB)
4. order of save data doesn't matter.

Example:   
```cpp
Roll-----------Name---------Subject   
------------------------------------   
101      -      ABC   -      C, C++   
102      -      DEF   -      JAVA
```

this example is wrong because subject Contains multiple values
Which Violate rulo no-2

Correct Solution:   
```cpp
Roll-----------Name---------Subject   
------------------------------------   
101      -      ABC   -      C   
101      -      ABC   -      C++   
102      -      DEF   -      JAVA
```


### Second Normal Form (2NF).
**Rules:**
1. It should be in 1st Normal Form.
2. It should not have any partial dependencies.all its non-prime attributes are fully functionally dependent on the primary key.

**To achieve 2NF, you need to do the following:**

- Identify the primary key of the table.
- Identify any attributes that are functionally dependent on only part of the primary key.
- Separate these attributes into their own tables, along with the part of the primary key they are dependent on.
**Example: **
```cpp
Employee_ID  -  Employee_Name  -  Project_ID  -  Project_Name  -   Department
--------------------------------------------------------------------------------
1      -        John	    -       101	    -      Project_A    -   	HR
2      -        Alice	    -       102	    -      Project_B    -   	IT
3      -        Bob	    -       101     -      Project_A    -     	HR
4      -        Mary	    -       103	    -      Project_C    -   	Finance

have partial dependencies issues.

#SOLUTION---------->>>>
Employee Table:                                                  |                      Project Table:
Employee_ID  -  Employee_Name  -   Department                    |                      Project_ID  -  Project_Name
------------------------------------------------                 |                      -------------------------------
1      -        John	    -       HR                           |                       101    -       Project_A
2      -        Alice	    -       IT                           |                       102     -      Project_B
3      -        Bob	    -       HR                           |                       103     -      Project_C
4      -        Mary	    -       Finance                      |                      
```
### 
### Third Normal Form (2NF).
**Rules:**
1. It should be in 2nd Normal Form.
2. It should not have any transitive dependencies.
