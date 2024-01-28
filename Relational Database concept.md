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
Roll-----------Name---------Subject   
------------------------------------   
101------------ABC-----------C, C++   
102------------DEF -----------JAVE   

this example is wrong because subject Contains multiple values
Which Violate rulo no-2

Correct Solution:   

Roll-----------Name---------Subject   
------------------------------------   
101-------------ABC------------C   
101-------------ABC---------- C++   
102-------------DEF---------- JAVA   



