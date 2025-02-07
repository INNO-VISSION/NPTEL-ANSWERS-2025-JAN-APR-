#### Week 4 : Assignment 4 - Introduction to Database Systems

##### *1. Which of the following relational query languages have the same expressive power?*  
I) Relational Algebra  
II) Tuple relational calculus restricted to safe expressions  
III) Relational Algebra with Select, Project, Cross-Product, Union, and Difference operators only  

*a)* II and III only  
*b)* I and II only  
*c)* I and III only  
*d)* I, II, and III  

*Answer:* d) I, II, and III  

---
##### *2. What is the relational algebra expression equivalent to the following tuple relational calculus expression, where r is a relation name?*  
   { t | r(t) ⋀ ( t.A = 10 ⋀ t.B = 20) }  

*a)* σ(A=10⋁B=20)(r)  
*b)* σ(A=10)(r)∪σ(B=20)(r)  
*c)* σ(A=10)(r)∩σ(B=20)(r)  
*d)* σ(A=10)(r)ーσ(B=20)(r)  

*Answer:* c) σ(A=10)(r)∩σ(B=20)(r)  

---

##### *3. Consider the following two statements and choose the correct option:*  
S1: Each record of the referencing relation can relate to at most one record of the referenced relation.  
S2: Each record of the referenced relation can relate to at most one record of the referencing relation.  

*a)* S1 is true, S2 is true  
*b)* S1 is false, S2 is true  
*c)* S1 is false, S2 is false  
*d)* S1 is true, S2 is false  

*Answer:* d) S1 is true, S2 is false  

---

##### *4. Given the following relational schema:*  
*Employee( EmpID, EmpName, Salary, Age, Address, Department, HireDate )*  

Which of the following TRC query retrieves employee IDs where the employee's salary is greater than ₹ 60,000, the employee's age is less than 40, the employee's department is either "IT" or "Marketing", and the employee's hire date is after January 1st, 2020?  

*a)* { t.EmpID | Employee(t) ∧ t.Salary > 60000 ∧ t.Age < 40 ∧ (t.Department = "IT" ⋁ t.Department = "Marketing") ∧ t.HireDate > '01/01/2020'}  
*b)* { t.EmpID | Employee(t) ∧ t.Salary > 60000 ⋁ t.Age < 40 ⋁ (t.Department = "IT" ∧ t.Department = "Marketing") ⋁ t.HireDate > '01/01/2020'}  
*c)* { t.EmpID | Employee(t) ∧ (t.Salary > 60000 ∧ t.Age < 40) ⋁ (t.Department = "IT" ∧ t.Department = "Marketing") ∧ t.HireDate > '01/01/2020'}  
*d)* { t.EmpID | Employee(t) ∧ (t.Salary > 60000 ⋁ t.Age < 40) ∧ (t.Department = "IT" ⋁ t.Department = "Marketing") ∧ t.HireDate > '01/01/2020'}  

*Answer:* a) { t.EmpID | Employee(t) ∧ t.Salary > 60000 ∧ t.Age < 40 ∧ (t.Department = "IT" ⋁ t.Department = "Marketing") ∧ t.HireDate > '01/01/2020'}  

---

##### *5. There are two weak entities E1 and E2, where E1 is the owner entity for E2.*  
Consider relational representation of E1 and E2 and choose the correct option:  

*a)* Mapping of E1 should be done before E2  
*b)* Mapping of E2 should be done before E1  
*c)* E1 and E2 can be mapped in any order  
*d)* Partial key of E1 includes the partial key of E2  

*Answer:* a) Mapping of E1 should be done before E2  

---

##### *6. Consider the relation:*  
*employee( name, sex, supervisorName )*  

What does the following Tuple Relational Calculus query produce?  

{ e.name | employee(e) ⋀ (∀x) [ ¬employee(x) ⋁ x.supervisorName ≠ e.name ⋁ x.sex = “male” ]}  

*a)* Names of employees with a male supervisor  
*b)* Names of employees with no immediate male supervisees  
*c)* Names of employees with no immediate female supervisees  
*d)* Names of employees with a female supervisor  

*Answer:* b) Names of employees with no immediate male supervisees  

---

##### *7. Given the following relational schemas:*  
*Student (rollNo, name, age, sex, deptNo, advisor)*  
*Department (deptId, dName, hod, phoneNo)*  

Which of the following will be the TRC query to obtain the department names that do not have any girl students?  

*a)* {d.dname | department(d) ∧ ¬((∃(s)) student(s) ∧ s.sex ≠ ‘F’ ∧ s.deptNo = d.deptId)}  
*b)* {d.dname | department(d) ∧ ((∀(s)) student(s) ∧ s.sex ≠ ‘F’ ∧ s.deptNo = d.deptId)}  
*c)* {d.dname | department(d) ∧ ¬((∃(s)) student(s) ∧ s.sex = ‘F’ ∧ s.deptNo = d.deptId)}  
*d)* None of these.  

 *Answer:* c) {d.dname | department(d) ∧ ¬((∃(s)) student(s) ∧ s.sex = ‘F’ ∧ s.deptNo = d.deptId)}  

---

##### *8. Consider the relations S1( A, B, C ) and S2( C, D, E )*  
The relation S1 contains 2000 tuples and S2 contains 2500 tuples. The maximum size of the join *S1 ⋈ S1.C = S2.C S2* is  

*a)* 2000  
*b)* 2500  
*c)* 4500  
*d)* 5000  

 *Answer:* d) 5000  

---

##### *9. Consider the following relational schema where rollNo and courseId are foreign keys in Enrollment referring to rollNo in Student and courseId in Courses, respectively:*  
Which one of the following is the correct interpretation of the TRC query?  

*a)* Retrieve rollNo and name of students who have enrolled for exactly one course  
*b)* Retrieve rollNo and name of students who have enrolled for more than one course  
*c)* Retrieve rollNo and name of students who have enrolled for at least one course  
*d)* Retrieve rollNo and name of students who have all enrolled for the same course  

*Answer:* c) Retrieve rollNo and name of students who have enrolled for at least one course  

---

##### *10. Consider the statements given below:*  
*P:* Tuple Relational Calculus (TRC) is a non-procedural query language  
*Q:* TRC expression specifies what is to be retrieved rather than how to retrieve it  

*a)* P is true and Q is false  
*b)* Both P and Q are true and Q is the correct reason for P  
*c)* Both P and Q are true and Q is not the correct reason for P  
*d)* Both P and Q are false  

*Answer:* b) Both P and Q are true and Q is the correct reason for P
