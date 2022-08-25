There are 4 .ipynb files which includes BB, BC, CP and TSP (Branch and Bound, Branch and Cut, Cutting Plane and Travelling Salesman 
respectively.)

You can model any linear integer programming problem with maximizing or minimizing objective, where objective is linear (c^T.x),
default is minimizing, suppose you want to minimize 5 y_1 + 10 y_2 , then c= [5,10] but if you want to maximize 5 y_1 + 10 y_2, it is equal to 
minimizing -5 y_1 - 10 y_2 , so c= [-5,-10] . Greater than constratint AX>=B can be written as -AX<=-B,
Equality constraints AX=B can be put as two unequality constraints AX<=B and AX>=B (-AX<=-B)

The files BB, BC, CP includes the code for 3 algorithms (Branch and Bound, Branch and Cut, and Cutting Planes)
where you can modify values of A, B and C modify values such that solution is feasible, if infeasible, it will tell solution is infeasible,
Branch and Bound and Branch and Cut are accurate and will converge always to an algorithm unless memory is exhausted while cutting
plane in some rare cases, will show exception that constraint can't be found or fraction 0/0 error. We have given a special case of 
production planning example.

The file TSP is specifically for travelling salesman, and here there are two inputs given, one is "n" , which is no. of cities or countries 
or nodes, while second is "use" which is 0 by default, and use Branch and Bound, if you will make it equal to 1, then
 it will use Branch and Cut, ensure that n=3 to 8, for n>8 , the program may crash.

You can model any linear integer programming problem with maximizing or minimizing objective, where objective is linear (c^T.x),
default is minimizing, suppose you want to minimize 5 y_1 + 10 y_2 , then c= [5,10] but if you want to maximize 5 y_1 + 10 y_2, it is equal to 
minimizing -5 y_1 - 10 y_2 , so c= [-5,-10] . Greater than constratint AX>=B can be written as -AX<=-B,
Equality constraints AX=B can be put as two unequality constraints AX<=B and AX>=B (-AX<=-B)