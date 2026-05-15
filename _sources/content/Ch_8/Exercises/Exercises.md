# EXERCISES


8.1 Select three appropriate applications of simulation analysis-one each from a business, engineering, or environmental setting. In each case, explain why analytical models might be inappropriate or infeasible; justify how simulation could successfully allow a useful and valid analysis of your chosen systems; and speculate on what might be learned from such a simulation study.

8.2 Consider simulating the operation of an emergency health clinic. Identify what issues should be studied, the questions to be investigated, uncontrollable characteristics and constraints within the clinic, controllable aspects of the operation of the clinic, and measures of performance of the clinic.

8.3 Suggest an appropriate method of gathering data for use in simulating the operation of the clinic described in the previous question.

8.4 Write a computer program that generates a sequence of random numbers that are Poisson distributed, with $\lambda=10$.

8.5 Select a favorite bookstore or grocery store, and observe the pattern of customer arrivals at the checkout facility. Develop a simulation of the customer arrivals by writing a computer program that starts a software clock at time zero, then prints the times at which customers arrive over a four-hour period of time. Analyze the times, and determine the longest, shortest, and average interarrival times.

8.6 Select a traffic intersection that is convenient for you to observe. Identify the physical entities that characterize this intersection (such as lanes, directions of traffic flow, stoplights, pedestrian walks, and any obstructions). Observe the operation of the intersection and notice its operating characteristics (such as number of vehicles, patterns of arrival of vehicles at the intersection, speed of traffic, pedestrian or other types of arrivals). Design a model that could be used to simulate the activities of this intersection.

8.7 Simulation can be used to study and predict weather patterns. Using the transition probabilities given in Example 6.1, simulate the most likely daily weather conditions at a ski resort during a winter holiday season beginning December 20 and continuing through January 10, assuming that it was snowy on December 19.

8.8 Develop a computer simulation of a system in which cars arrive at a toll gate on a highway according to a Poisson distribution with mean rate of 90 miles per hour. The times for passing through the gate are exponentially distributed with average 38 seconds.

a. Make a chart that displays enough information so that you can analyze the waiting times experienced by the cars going through this facility. 

b. How long must you run this simulation program to get reliable information about the queueing characteristics of your system?

c. Modify your simulation program so that it automatically gathers statistics, and reports the average number of cars waiting and the average waiting time of each car.

8.9 A computer center has one multi-user computer. The number of users in the center at any time is ten. For each user, the time for writing and entering a program is exponential with mean rate 0.5 per hour. Once a program is entered, it is sent directly to the ready queue for execution. The execution time per program is exponential with mean rate of six per hour. Assuming the mainframe computer is operational on a full-time basis, and neglecting the possibility of down-time, develop a computer simulation that allows you to find:

a. The probability that a program is not executed immediately upon arrival in the ready queue

b. The average time until a submitted program completes execution

c. The average number of programs in the ready queue

State any assumptions that you made about the computer center or the multi-user computer in the system you have analyzed.


8.10 The mean time between failures of a computer disk drive is 3,000 hours, and failures are exponentially distributed. Write a computer program that generates these failure events until 25 disk drive failures have occurred. Print out the number of hours separating successive failures that occur in your experiment.


8.11 Printer jobs are created in a computing system according to a Poisson distribution with a mean of 40 jobs per hour. Average print times are 65 seconds. Users complain of long delays in receiving their printouts, but the computing lab director will be willing to purchase a faster printer (twice as fast as the present one) only if it can be demonstrated that the current average queue length is four (or more) jobs, and only if the new printer would be idle for at most $20 \%$ of the time. Will the lab director be able to justify the acquisition of the new printer? You have already answered this question (in Exercise 7.4) using queueing formulas; now develop and run a simulation model to test your answer.

8.12 Computer programs are submitted for execution according to a Poisson distribution with mean arrival rate of 90 per hour. Execution times are exponentially distributed, with jobs requiring an average of 38 seconds. Users complain of long waiting times. Management is considering the purchase of a faster CPU that would decrease the average execution time to 30 seconds per job. This expense can be justified only if, under the current system, the average number of jobs waiting exceeds five. Also, if a new CPU is to be purchased, its percentage of idle time should not exceed $30 \%$. Can the new CPU be justified? You made the necessary calculations to make a recommendation (in Exercise 7.5). Now develop a simulation of the aforementioned scenario that might provide an even more convincing explanation to users or to management.

8.13 Develop a simulation of the vehicle refueling system described in Exercise 7.9. Determine how long you must run your simulation to obtain performance measures that are reasonably consistent with the ones you computed when you worked the problem using queueing analysis.

8.14 In Exercise 7.12, you were asked to select a system in your university, business, or community that involves queues, to develop a queueing model that describes that system, and to describe the performance characteristics of this system. Write a computer program to simulate the system you studied, and compare the statistics gathered by your simulation program to the analytical performance results that you computed with the formulas.
