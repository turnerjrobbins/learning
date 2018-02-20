# Linear Algebra
I will be trying to teach myself Linear Algebra using "Linear Algebra Done Wrong" by Sergei Treil from Brown.
Linear algebra is fundamentally important for doing complex mathematics, and will provide a foundation for my future studies in data science and machine learning. Unsure of how this document will be organized at the moment, but I am just going to allow some sort of organization to naturally grow. I am planning on using this repository for notes, homeworks, projects, etc... basically for storing any sort of document related to my studies in this course.

## Chapter 1 - Basic Notions

Vector Space V: collection of objects v called vectors along with 2 operations s.t. 8 properities (axioms of a vector space) hold:
Addition:
1. Commutativity: **v** + **w** = **w** + **v** for all v, w that are elements of V
2. Associativity: (**u** + **v**) + **w** = **u** + (**v** + **w**) for all u,v,w elements of V
3. Zero vector: there exists a special vector **0** such that **v** + **0** = **v** for all **v** element of V
4. Additive inverse: for every vector **v** element of V there exists a vector **w** element of V such that **v** + **w** = **0**. This additive inverse is usually denoted as **-v**
Multiplication
5. Multiplicative identity: 1**v** = **v** for all **v** element of V
6. Multiplicative associativity: (alpha*beta)**v** = alpha*(beta**v**) for all **v** element V and all scalars alpha, beta
Distributive Properties
7. alpha*(**u** + **v**) = alpha***u** + alpha**v** for all **u**, **v** elements V and scalars alpha
8. (alpha + beta)**v** = alpha**v** + beta**v** for all **v** elements of V and scalars alpha, beta

wow, got all of those typed out. 
YOU CANNOT MULTIPLY TWO VECTORS OR ADD A NUMBER TO A VECTOR

Vector Space can be real or complex.

It is possible to consider vector space over rationals, but not over the integers.

The space R^n is all columns of size n
The space C^n is all columns of size n of complex numbers

### Matrix Notation
An m x n matrix has m rows and n columns. We call each element an **entry**.
entry in row j and column k can be denoted by A<sub>j,k</sub>.
Given matrix *A* its **transpose** AT, is defined by making the rows columns.
|1, 2, 3|
|4, 5, 6|
becomes
|1, 4|
|2, 5|
|3, 6|
Formally A<sup>T</sup><sub>j,k</sub> = A<sub>k,j</sub>

Exercises
1.1 **x** = (1,2,3)T, **y** = (y1,y2,y3)T, **z** = (4,2,1)T. 
Compute 2**x**, 3**y**, **x** + 2**y** - 3**z**
2**x** is (2, 4, 6)T
3**y** is (3*y1, 3*y2, 3*y3)T
**x** + 2**y** - 3**z** is (-11+2y1,-4+2y2, y3)T
1.2 Which of the following sets are vector spaces? Justify
+ a) the set of all continuous functions on the interval [0,1];
consider f and g as continuous functions on the interval. 
f+g = g+f is true
for all alpha, beta in Real numbers and all f alpha(beta*f) = (alpha*beta)*f
for all f 1f = f
Basically, just show that continuous functions preserve the properties of vectors
+ b) the set of all non-negative functions on the interval [0,1]
Not a vector space because it violates property 4
+ c) the set of all polynomials of degree exactly n
Is a vector space. I don't think it violates any vector space properties
+ d) the set of all symmetric n x n matrices (matrices such that AT = A)
sure why not
