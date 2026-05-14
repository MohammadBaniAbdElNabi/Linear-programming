# EXERCISES

4.1 A certain single-processor computer is to be used to execute five user programs. These programs may be run in any order; however, each requires a specific set of files to be resident in main memory during its execution. Furthermore, a certain amount of time is required for each file to be brought into main memory prior to use by a user program. The facts are summarized as follows:

| User Program | Files Needed for Its Execution |
| ------------ | ------------------------------ |
| 1            | B, C, E                        |
| 2            | A, B, C                        |
| 3            | A, B, D                        |
| 4            | A, D, E                        |
| 5            | B, C                           |

| File Name | Amount of Time Required to Bring It into Memory |
| --------- | ----------------------------------------------- |
| A         | 30                                              |
| B         | 20                                              |
| C         | 25                                              |
| D         | 35                                              |
| E         | 50                                              |

Initially, no files are in memory. The five user programs are to run in sequence, but any order is feasible. At most, three files will fit in memory at one time. Clearly, because some of the files are used by multiple programs, it would be wise to try to schedule the programs to take advantage of files already in memory, so as to minimize the "change-over" (setup) times between programs. Define decision variables and formulate this problem to sequence the five user programs to minimize total change-over times. Note the similarity of this problem to one of the classical integer programming models discussed in this chapter.

4.2 Suppose you have a directed acyclic graph having _n_ nodes, in which node 1 is designated as an origin and node _n_ is designated as a destination. In Chapter 3, we described the problem of finding the shortest path from the origin to the destination. Formulate this problem as a zero-one integer programing problem. (_Hint:_ Let decision variable _x<sub>ij</sub>_ = 1 if the arc from node I to node _j_ is in the shortest path.)

4.3 A small university computer laboratory has a budget of \$10,000 that can be used to purchase any or all of the four items described below. Each item's value has been assessed by the lab director, and is based on the projected utilization of the item. Use a branch-and-bound technique to determine the optimal selection of items to purchase to enhance the computing laboratory facilities. Show your branch-and-bound tree, and give the total cost and total value of the items chosen for purchase.

| Item              | Cost   | Value |
| ----------------- | ------ | ----- |
| NanoRobot         | \$4000 | 8     |
| WinDoze simulator | \$2500 | 5     |
| Network pods      | \$3000 | 12    |
| BioPrinter        | \$4500 | 9     |

4.4 Bruno the Beach Bum wishes to maximize his enjoyment of the seashore by taking along an assortment of items chosen from the list below. Help Bruno pack his beach bag with the most valuable set of items by using a branch-and-bound technique. Bruno's beach bag is rated for a 20-pound load.

| Item              | Weight | Value |
| ----------------- | ------ | ----- |
| Coconut oil       | 4      | 16    |
| Sun shades        | 2      | 10    |
| Snorkel and fins  | 8      | 16    |
| Folding chair     | 10     | 30    |
| _Bummer_ magazine | 5      | 30    |

Enumerate the number of packings (sets of items) for this problem, and draw a complete tree of possibilities. How many of these sets are feasible packings? How many subproblems are actually solved by your branch-and-bound procedure? What is the optimal feasible set of items?

4.5 If a problem formulation has _n_ variables and each variable has _m_ possible integer values, then a branch-and-bound tree could have as many as _m<sup>n</sup>_ terminal nodes. Verify this for the case _m_ = 4 and _n_ = 3.

4.6 Consider the following zero-one integer programming problem:

- maximize 5_x_1 - 7_x_2 - 10_x_3 + 3_x_4 - 4_x_5

subject to \_x_1 + 3_x_2 - 5_x_3 + \_x_4 + \_x_5 ≤ 3

- 2_x_1 - 3_x_2 + 3_x_3 - 2_x_4 - 2_x_5 ≤ -3
- 2_x_2 - 2_x_3 + 2_x_4 + \_x_5 ≤ 3
- _x<sub>i</sub>_ = 0 or 1 for all _i_

Solve this problem completely, using a branch-and-bound algorithm.

4.7 Suppose you wish to solve the following general integer programming problem using branch-and-bound techniques.

- maximize 3_x_1 + 5_x_2 + 2_x_3
- subject to \_x_1 + 5_x_2 + 3_x_3 ≤ 8
- 2_x_1 + \_x_2 + 5_x_3 ≤ 7
- 4_x_1 + 2_x_2 + 3_x_3 ≤ 8
- \_x_1 + 3_x_2 + 3_x_3 ≥ 6
- \_x_1, \_x_2, \_x_3 ≥ 0 and integer

Use up and down penalties to determine which variable would be branched on first. (_Note:_ There is no "correct" answer, but you should be able to justify your choice.)

4.8 Consider the following integer programing problem:

- maximize -4_x_1 - 5_x_2
- subject to \_x_1 + 4_x_2 ≥ 5
- 3_x_1 + 2_x_2 ≥ 7
- \_x_1, \_x_2 ≥ 0 and integer

Calculate the penalties for branching up and down on variables \_x_1 and \_x_2.

4.9 Solve the problem given in Exercise 4.8 using Gomory fractional cuts.

4.10 Consider the following integer programming problem:

- maximize -3_x_1 - 4_x_2
- subject to 2_x_1 + \_x_2 ≥ 1
- \_x_1 + 3_x_2 ≥ 4
- \_x_1, \_x_2 ≥ 0 and integer

(a) Compute the up and down penalties for branching on variable \_x_2\. Which way would you branch first? Explain why.

(b) What can you say about variable \_x_3, the surplus variable on constraint 1, with respect to up and down penalties? Explain.

4.11 Suppose that you are solving a large zero-one linear programming problem, and the LP solution has

- _x_\* = (0.3, 0.9, 0.1, 0.9, 0.9, 0.8, 0.9, 0.9, 0.7, 0)

One of the constraints in the problem is

- 10_x_1 - 2_x_2 - 4_x_3 + 7_x_4 + -6_x_5 - 11_x_6 + 9_x_7 - 3_x_8 + \_x_9 + 12_x_10 ≤ -1

In Section 4.6, we used a knapsack model to find a cover inequality that cuts off the current LP solution. Describe the knapsack for this particular problem.

4.12 Suppose we are given a zero-one linear programming problem in which one of the constraints is

- 3_x_1 + 4_x_2 - 7_x_3 -3_x_4 + 5_x_5 -6_x_6 + 3_x_7 ≥ 0

Find a cover inequality that cuts off the current LP solution _x_\* = (0, , 0, 1, 1, , 0)

4.13 A certain zero-one linear programming problem involves the constraint

- \_x_1 + 3_x_2 + 4_x_3 + 5_x_4 ≤ 6

and the current LP optimum occurs at _x_\*= (0.3, 0.3, 0.2, 0.8).

Find a minimal cover inequality that cuts off the point _x\*_.

4.14 Solve the problem in Exercise 4.6 again by first constructing cover inequalities, and then using branch-and-bound if necessary.

4.15 We wish to assign three customers to two warehouses having limited capacity. Each customer must be assigned to precisely one warehouse. The assignment costs and the capacities are given in the following table. Solve this problem using Lagrangian relaxation.

|            | Warehouse 1 | Warehouse 2 | Demand |
| ---------- | ----------- | ----------- | ------ |
| Customer 1 | 2           | 8           | 18     |
| 2          | 5           | 3           | 15     |
| 3          | 7           | 3           | 14     |
| Capacity   | 30          | 18          |        |

4.16 Suppose that you are the manager of a small store that is open 7 days per week. You require the following minimum number of staff to work each day:

Sunday 5

Monday 3

Tuesday 4

Wednesday 4

Thursday 5

Friday 7

Saturday 7

Each employee can work only 5 days per week, and must have the weekend off (Saturday and Sunday) once every 2 weeks. The objective is to meet the demand using the minimum number of employees. Describe a formulation of this problem using column-generation. (_Hint:_ Try to construct a work pattern for a 2-week period.) Describe the meaning of the rows and columns in the master problem. Provide an initial formulation of the LP; that is, pick a starting set of columns, and write out the LP. Perform a few iterations of column generation. Describe how you would formulate the subproblem.

4.17 In Section 4.8, it was suggested that column-generation can be used to solve the cutting stock problem. The simplest (one-dimensional) cutting stock problem can be illustrated by the following example. Suppose we have a large supply of steel reinforcing bars to be used in the construction of concrete pillars. The bars are all 50 feet long. We have a set of orders for re-bars of the following lengths:

| Length  | Quantity |
| ------- | -------- |
| 15 feet | 3        |
| 10 feet | 2        |
| 13 feet | 5        |
| 18 feet | 4        |
| 19 feet | 5        |
| 23 feet | 1        |

These orders are to be cut from some of the 50-foot-long pieces. It is not economical to keep an inventory of the leftover pieces, so we sell them as scrap. We want to minimize the total cost of scrap for cutting this set of orders. Suppose that it costs (net) 0.50 per inch to throw away a scrap piece of re-bar. Formulate this as a column-generation problem. Generate the initial solution, and perform one iteration of column generation. Explain your algorithm for solving the subproblem.

4.18 Big City Wheel Trans (for disabled public transit users) has a large list of clients who must be picked up and delivered to locations around the city. Each client has a specific required pick-up time, and we assume that each customer travels alone. Describe how to formulate this problem using column-generation. Suppose that the primary objective is to minimize the number of vehicles required to satisfy all demand. Describe what the subproblem would look like and what algorithm you could use to solve it. Recall that the subproblem we solved in Section 4.8 was solved "by inspection," but in this exercise, you should define an algorithm to solve the subproblem.

4.19 Formulate the examination timetabling problem as a zero-one programming problem. Let _c<sub>ik</sub>_ be the number of students who must take both exams _i_ and _k_. Define a penalty of (100 × _c<sub>ik</sub>_) for having examinations _i_ and _k_ in the same time period, and a penalty of (5 × _c<sub>ik</sub>_) for having examinations _i_ and _k_ in adjacent time periods. The objective is to minimize the total penalty costs. Let _n_ denote the number of examinations to be scheduled, and _m_ denote the number of time periods available for exams.
