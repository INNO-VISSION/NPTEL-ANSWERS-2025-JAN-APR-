### Week 3 Assignment 3 - Introduction To Database

#### **Questions and Answers**

#### **1. Which of the following statements is TRUE?**
- a) A key for a relation can be figured out just by looking at the instance data.
- b) A relation has exactly one key.
- c) It is possible that a relation has no key.
- d) A key for a relation can only be determined from the meaning of its attributes.

**Answer:** d) A key for a relation can only be determined from the meaning of its attributes.

---

#### **2. State if the following statements are TRUE or FALSE:**
- In an instance of a relation, it is possible that the value of a key attribute is NULL in a certain row.
  - **Answer:** False
- It is possible for a foreign key of a relation to refer to the primary key of the relation itself.
  - **Answer:** True
- Every relation scheme can have at most one foreign key.
  - **Answer:** False
- If K is supposed to be a key for scheme R, any relation instance r on R should not have two tuples that have identical values for attributes in K.
  - **Answer:** True

---

#### **3. How many tuples exist in the query (A∪B)⟗(A.id>20∨C.id< 10)C?**
- a) 7
- b) 8
- c) 9
- d) 10

**Answer:** c) 9

---

#### **4. What is the result of the following expression: Π(X,Y)(σ(X=1)∨(X=4)(A))−Π(D,E)(σ(D≠3)(B))**
- a) {(6,8), (9,9)}
- b) Empty relation
- c) A relation with scheme (X,Y) and tuples { (6,8) }
- d) A relation with scheme (X,Y) and tuples { (9,9) }

**Answer:** c) A relation with scheme (X,Y) and tuples { (6,8) }

---

#### **5. How many tuples will there be in the result of the following relational algebra expression?**
- a) 22
- b) 23
- c) 24
- d) 25

**Answer:** c) 24

---

#### **6. What does the following relational algebra expression represent?**
- a) Courses in which all female students have enrolled.
- b) Courses in which a proper subset of female students have enrolled.
- c) Courses in which all male students have enrolled.
- d) Courses in which only female students have enrolled.

**Answer:** d) Courses in which only female students have enrolled.

---

#### **7. Choose the correct statement(s):**
- a) Two schemes are union compatible if the domain of at least one pair of corresponding attributes match.
- b) A join operation is equivalent to performing a cross product of its operands followed by a select operation using the join condition.
- c) The operators {σ,π,×,⋃,−} constitute a complete set of relational algebra operators.
- d) The difference relational algebra operator requires its operands to be union-compatible.

**Answers:**
- b) A join operation is equivalent to performing a cross product of its operands followed by a select operation using the join condition.
- c) The operators {σ,π,×,⋃,−} constitute a complete set of relational algebra operators.
- d) The difference relational algebra operator requires its operands to be union-compatible.

---

#### **8. What is the result of the relational algebra expression A ÷ B?**
- a) Empty relation
- b) A relation with scheme Z and tuple { (3) }
- c) A relation with scheme Z and tuples { (3), (5) }
- d) {3,5}

**Answer:** c) A relation with scheme Z and tuples { (3), (5) }

---

#### **9. Given two union-compatible relations X(A,B) and Y(C,D), what is the result of the operation X⋈(A=C)∧(B=D)Y?**
- a) X ∪ Y
- b) X ∩ Y
- c) X − Y
- d) X ÷ Y

**Answer:** b) X ∩ Y

---

#### **10. Which of the following statements is TRUE wrt different keys of a relational DB?**

X = set of all primary keys  
Y = set of all candidate keys  
Z = set of all super keys  

- a) X ⊆ Z ⊆ Y
- b) Z ⊆ X ⊆ Y
- c) X ⊆ Y ⊆ Z
- d) Y ⊆ X ⊆ Z

**Answer:** c) X ⊆ Y ⊆ Z
