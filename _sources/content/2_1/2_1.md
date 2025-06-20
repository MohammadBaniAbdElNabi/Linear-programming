# Linear Programming

## 2.1 The Linear Programming Model

Linear programming is a special class of mathematical programming models in which the objective function and the constraints can be expressed as linear functions of the decision variables. As with the more general mathematical programming models, the decision variables represent quantities that are, in some sense, controllable inputs to the system being modeled. An objective function represents some principal objective criterion or goal that measures the effectiveness of the system (such as maximizing profits or productivity, or minimizing cost or consumption). There is always some practical limitation on the availability of resources (time, materials, machines, energy, or manpower) for the system, and such constraints are expressed as linear inequalities or equations involving the decision variables. Solving a linear programming problem means determining actual values of the decision variables that optimize the objective function, subject to the limitations imposed by the constraints. <br>
The use of linear programming models for system optimization arises quite naturally in a wide variety of applications. Some models may not be strictly linear, but can be made linear by applying appropriate mathematical transformations. Still other applications are admittedly not at all linear, but can be effectively approximated by linear models. The ease with which linear programming problems can usually be solved makes this an attractive means of dealing with otherwise intractable nonlinear problems.<br>
In the following section, we will see examples of the wide variety of applications that can be modeled with linear programming. In each case, the first task will be to identify the controllable decision variables xi, where $i$ = 1, ..., $n$. Then the objective criterion will be established: to either maximize or minimize some function of the form

$$
z = c_1 x_1 + c_2 x_2 +...+ c_n x_n = \sum_{i=1}^n (c_i x_i)
$$

where $c_i$ represents problem dependent constants. Finally, resource limitations and bounds on decision variables will be written as equations or inequalities relating a linear function of the decision variables to some problem dependent constant; for example,

$$
a_1 x_1 + a_2 x_2 +...+ a_n x_n \leq b
$$

Although the primary purpose of this chapter will be to present methods of solving linear programming problems, the first critical step in successful problem-solving lies in the correct formulation of an application problem into the linear programming framework.