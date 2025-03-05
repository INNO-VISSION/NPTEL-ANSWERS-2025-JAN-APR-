#### Week 6 : Assignment 6 - Introduction to Database Systems

##### 1. Under which of the following conditions are update operations on views NOT allowed?
(i) if the view definition has an aggregate operator  
(ii) if the view definition includes two or more tables  
(iii) if the view is defined on a single table without group by, aggregates and the SELECT clause includes the primary key of the table  
  
- A) Only (ii)  
- B) Only (iii)  
- C) Only (i) and (ii)  
- D) All (i), (ii), and (iii)  

**Answer: C) Only (i) and (ii)**  


##### 2. State whether the following statement is true or false:  
**HAVING clause can be used in a query only if GROUP BY clause is used**  

- A) True  
- B) False  

**Answer: B) False**  

---

##### 3. State whether the following statement is true or false:  
**GROUP BY clause can be used in a query only if HAVING clause is used**  
 
- A) True  
- B) False  

**Answer: B) False**  

---

##### 4. Is it mandatory to use an aggregate function in a query if GROUP BY clause is used?  

  
- A) True  
- B) False  

**Answer: B) False**  

---

##### 5. Can aggregate functions be used in GROUP BY clauses?  
 
- A) True  
- B) False  

**Answer: A) True**  

---

##### 6. In which of the following SQL clauses of a main query can a sub-query be used?  
(i) FROM (ii) WHERE (iii) HAVING  
 
- A) Only (ii)  
- B) Only (iii)  
- C) Only (ii) and (iii)  
- D) All (i), (ii), and (iii)  

**Answer: D) All (i), (ii), and (iii)**  

---

##### 7. Which query selects courses with at least 10 'W' grades in some offering of the course?
  
- A) ```sql
SELECT courseId FROM enrollment WHERE grade = 'W' 
GROUP BY courseId HAVING count(rollNo) >= 10;
```

- B) ```sql
SELECT courseId FROM enrollment WHERE grade = 'W' 
GROUP BY courseId, sem, year HAVING count(rollNo) >= 10;
```

- C) ```sql
SELECT courseId FROM enrollment WHERE grade = 'W' 
AND count(rollNo) >= 10 GROUP BY courseId;
```

- D) ```sql
SELECT courseId FROM enrollment WHERE grade = 'W' 
AND count(rollNo) >= 10 GROUP BY courseId, sem, year;
```

**Answer: B)**  

---

##### 8. Which query retrieves students whose name has 'p' as the second letter?  


- A) ```sql
SELECT rollNo FROM student WHERE name = '_p';
```

- B) ```sql
SELECT rollNo FROM student WHERE name LIKE '_p';
```

- C) ```sql
SELECT rollNo FROM student WHERE name LIKE '_p%';
```

- D) ```sql
SELECT rollNo FROM student WHERE name IN '_p%';
```

**Answer: C)**  

---

##### 9. What is the least possible number of tuples in the result of this query?

```sql
SELECT * FROM R1 FULL OUTER JOIN R2 ON R1.A = R2.C;
```

Options:  
- A) 0  
- B) 18  
- C) 8  
- D) 10  

**Answer: B) 18**  

---

##### 10. Which query is correct to find courses with no prerequisites?

- A) ```sql
SELECT courseId FROM preRequisite 
GROUP BY courseId 
HAVING count(preCourseId) = 0;
```

- B) ```sql
SELECT courseId FROM preRequisite a 
WHERE NOT EXISTS (
  SELECT preCourseId FROM preRequisite b 
  WHERE a.courseId = b.courseId);
```

- C) Both (i) and (ii)  
- D) Neither (i) nor (ii)  

**Answer: B) Only (ii)**  

---

##### 11. Which query finds the ID and name of the senior-most HOD(s)?

- A) ```sql
SELECT p1.empId, p1.name
FROM professor p1
WHERE p1.startYear IN (
  SELECT min(p.startYear)
  FROM professor p, department d
  WHERE p.empId = d.hod);
```

- B) ```sql
SELECT p1.empId, p1.name
FROM professor p1, department d1
WHERE p1.empId = d1.hod
AND p1.startYear IN (
  SELECT min(p.startYear)
  FROM professor p, department d
  WHERE p.empId = d.hod);
```

- C) None of the above  

**Answer: B)**  

---

##### 12. Which query finds the teacher(s) who taught CS1100 the highest number of times?

- A) ```sql
CREATE VIEW EmpCount AS
SELECT empId, count(*) AS cnt
FROM teaching
WHERE courseId = 'CS1100'
GROUP BY empId;

SELECT empId FROM EmpCount
WHERE cnt = (SELECT MAX(cnt) FROM EmpCount);
```

- B) ```sql
SELECT empId, max(count(*)) AS cnt
FROM teaching
WHERE courseId = 'CS1100'
GROUP BY empId;
```

- C) ```sql
SELECT empId FROM teaching
WHERE courseId = 'CS1100'
GROUP BY empId
HAVING COUNT(*) = (
  SELECT max(count(*)) 
  FROM teaching WHERE courseId = 'CS1100');
```

**Answer: A)**  

---

##### 13. Match database access approaches with their properties:

  {1: Embedded SQL; 2: API based; 3: Database language}  

  {p: Only one connection to a DB server can be active at any time;  
  q: Open Database Connectivity (ODBC);  
  r: Cursors;  
  s: Programmers need to learn a new language;  
  t: Multiple connections to DB servers can be active at any time}  

Options:  
- A) 1--p; 2--t; 3--s  
- B) 1--t; 2--q; 3--s  
- C) 1--s; 2--r; 3--p  
- D) 1--p; 2--t; 3--q  

**Answer: A) 1--p; 2--t; 3--s**  
