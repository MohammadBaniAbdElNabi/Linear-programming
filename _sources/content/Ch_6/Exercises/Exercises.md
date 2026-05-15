# EXERCISES


6.1 Suppose

$$
\mathrm{P}=\left[\begin{array}{cccc}
0.080 & 0.184 & 0.368 & 0.368 \\
0.632 & 0.368 & 0 & 0 \\
0.264 & 0.368 & 0.368 & 0 \\
0.080 & 0.184 & 0.368 & 0.368
\end{array}\right]
$$

Obtain the steady state probabilities for the Markov chain whose one-step probabilities are given by P .

6.2 Write a computer program to compute the state probabilities $\mathrm{p}(50)$ for a five state system whose initial probabilities are (lllll $0.2 \quad 0.2 \quad 0.2 \quad 0.2 \quad 0.2)$ and whose one step transition probabilities are:

$$
\mathrm{P}=\left[\begin{array}{lllll}
0.1 & 0.1 & 0.1 & 0.1 & 0.6 \\
0.2 & 0.2 & 0.3 & 0.1 & 0.2 \\
0.2 & 0.2 & 0.2 & 0.2 & 0.2 \\
0.5 & 0.1 & 0.1 & 0.1 & 0.2 \\
0.3 & 0.3 & 0.1 & 0.2 & 0.1
\end{array}\right]
$$

by raising P to the 50 -th power.

a. Do the elements in your result vector $\Pi$ sum to 1 ? <br>

b. After how many steps do the state probabilities cease to change observably? <br>

c. If your state probabilities stabilize, but then exhibit small changes as you continue to compute higher powers of P , how would you explain this? <br>

d. Compare your result with the steady state probabilities you obtain by solving the system $\Pi \mathrm{P}=\Pi$ and $\sum \Pi=1$. Do these steady state probabilities sum to 1 ? <br>

e. Which method of establishing state probabilities takes greater computation time? (Use a timing function on your computer to determine this.) <br>

f. Which method appears to yield more accurate results? (How can you make this determination?) <br>

6.3 Why is the Markov process described by the following transition probability matrix not an ergodic process?

$$
\mathrm{P}=\left[\begin{array}{llll}
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 \\
1 & 0 & 0 & 0
\end{array}\right]
$$

What do you discover if you try to establish steady state probabilities by solving the steady-state equations for this process?

6.4 Raise the following transition probability matrices to successively higher powers, and note the difference in the number of steps required to reach steady state in each case:

$$
\mathrm{P}_{\mathrm{A}}=\left[\begin{array}{ccc}
0.3 & 0.3 & 0.4 \\
0.4 & 0.3 & 0.3 \\
0.5 & 0.2 & 0.3
\end{array}\right] \quad \mathrm{P}_{\mathrm{B}}=\left[\begin{array}{ccc}
0.90 & 0.05 & 0.05 \\
0.05 & 0.95 & 0 \\
0 & 0.10 & 0.90
\end{array}\right]
$$

6.5 Try to establish steady state probabilities by solving the steady-state equations corresponding to the Markov system shown in Figure 6.3. Is there any computational difficulty caused by the transient and recurrent states?

6.6 A doubly stochastic matrix is one whose row elements sum to 1 and whose column elements also sum to 1 . Find the steady-state probabilities for the chain whose one-step transition probabilities are given by the doubly stochastic matrix

$$
\mathrm{P}=\left[\begin{array}{ccc}
1 / 3 & 2 / 3 & 0 \\
1 / 6 & 1 / 3 & 1 / 2 \\
1 / 2 & 0 & 1 / 2
\end{array}\right]
$$

In general, for any doubly stochastic matrix, it is true that:

$$
\Pi_{\mathrm{j}}=1 / \mathrm{n} \text { for } \mathrm{j}=1, \ldots, \mathrm{n}
$$

where n is the number of states.

6.7 In a hospital for seriously ill patients, each patient is classified as being either in critical, serious, or stable condition. These classifications are updated each morning as a physician makes rounds and assesses the patients' current conditions. The probabilities with which patients have been observed to move from one classification to another are shown in the following table, where the $(\mathrm{i}, \mathrm{j})$-th entry represents the probability of a transition from condition i to condition j .

|  | Critical | Serious | Stable |
| :--- | :---: | :---: | :---: |
| Critical | 0.6 | 0.3 | 0.1 |
| Serious | 0.4 | 0.4 | 0.2 |
| Stable | 0.1 | 0.4 | 0.5 |

a. What is the probability that a patient who is in critical condition on Tuesday will be in stable condition on the following Friday? <br>

b. How many days on average will pass before a patient in serious condition will be classified as being in stable condition? <br>

c. What is the probability that a patient in stable condition on Monday will experience some sort of reversal and will not become stable again for three days? <br>

d. What proportion of the patient rooms should be designed and equipped for patients in critical condition? In serious condition? In stable condition? <br>

Discuss the validity of the Markov assumption and the stationarity assumption, in the context of this problem.

6.8 Construct a transition probability matrix to model the promotion of high school students through grades 10-12. Ninety-two percent of tenth graders are passed on to the next grade, $4 \%$ fail and repeat the tenth grade, and $4 \%$ fail and drop out of school. At the end of the eleventh grade, $88 \%$ pass to the next grade, $7 \%$ fail and repeat, and 5\% fail and drop out. Of the twelfth graders, 96\% graduate from high school successfully, $3 \%$ fail and repeat the twelfth grade, and $1 \%$ fail and do not ever complete high school. Students may repeat a grade any number of times, but no student ever returns to a lower grade. Comment on the structure of the transition probability matrix. Of 1,000 students entering the tenth grade, how many are expected to graduate after three years in high school? What other information about the high school students can be obtained from the data given earlier?

6.9 What is the name given to a Markov state that is reachable from the initial state and whose steady-state probability is zero? What is the name given to a Markov state whose steady-state probability is 1 ? <br>

6.10 What is the interpretation of the element $\mathrm{a}_{\mathrm{ij}}$ in the matrix A , where A is the product of the matrices F and R ? What is the interpretation of the element $\mathrm{f}_{\mathrm{ij}}$ in the fundamental matrix F of a Markov process? <br>

6.11 Suppose the following one-step transition probability matrix describes a Markov process:

| States | $\mathbf{1}$ | $\mathbf{2}$ | $\mathbf{3}$ |
| :--- | ---: | :---: | :---: |
| 1 | 0.2 | 0.7 | 0.1 |
| 2 | 0 | 0.3 | 0.7 |
| 3 | 0 | 0.1 | 0.9 |

a. Determine the steady-state probabilities for this process. <br>

b. What is the probability that a first passage from state 2 to state 3 will occur after exactly two transition steps? <br>

c. What is the expected number of transitions that will occur for the system in state 2 to return again to state 2? <br>

6.12 A machine maintenance problem can be modeled as a Markov process. Each day, the machine can be described as either excellent, satisfactory, marginal, or inoperative. For each day the machine is in excellent condition, a net gain of $\$ 18,000$ can be expected. A machine in satisfactory condition yields an expected $\$ 12,000$ per day. A marginal machine can be expected to bring a daily net gain of $\$ 4,000$, and an inoperative machine causes a net loss of $\$ 16,000$ a day. An excellent machine will be excellent the next day with probability $90 \%$, satisfactory the next day with probability $4 \%$, and marginal with probability $2 \%$, and inoperative with probability $4 \%$. A satisfactory machine will the next day be satisfactory with probability $80 \%$, marginal with probability $12 \%$, and inoperative with probability $8 \%$. A marginal machine will be marginal again the next day with probability $70 \%$, and inoperative with probability $30 \%$. Repairs are made without delay, but only on inoperative machines, and the repairs take exactly one day. (The day long repair process costs $\$ 16,000$, which accounts for the daily net loss stated earlier.) A machine having undergone repair is $90 \%$ likely to be in excellent condition the next day, but in $10 \%$ of cases the repairs are ineffective and the inoperative machine will remain out of commission, necessitating a repeat of the repair process on the following day (at an additional cost of $\$ 16,000$ ). Find the steady state probabilities for the four states of this machine. Then, assuming that this machine is active (in one of its four states) 365 days per year, find the long-term annual profitability of this machine?

6.13 Given the one step transition probability matrix in the following, compute the expected first passage times from state i to state j , for all i and j .

$$
\left[\begin{array}{cccc}
0 & 0 & 0.5 & 0.5 \\
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0.5 & 0.5 & 0
\end{array}\right]
$$

6.14 A computer network is observed hourly to determine whether the network is operational (up) or not (down). If the network is up, there is a $98 \%$ probability that it will be up at the next observation. If it is down, there is a $30 \%$ probability that effective repairs will have been completed by the next hourly observation, but a $70 \%$ chance that repairs are still in progress and the network is still down the next hour. Analyze the expected first passage times for this computer network. Comment on the performance of the network in general, and in particular interpret and comment on the first passage probabilities. In what type of network environment would the performance of this network be acceptable?

6.15 Customers are often faced with the option of purchasing an extended warranty for a new appliance. Suppose that GalleyKleen dishwashers offer a warranty plan that covers the first three years of ownership of a dishwasher. During the first year of operation, $5 \%$ of dishwashers fail. During the second year of operation, $8 \%$ fail. And 11\% of dishwashers in their third year of service fail. The basic warranty from GalleyKleen covers replacement only when failures occur during the first year. If a failure occurs, a repair during the second year is expected to cost the owner (customer) $\$ 150$, and during the third year is expected to cost $\$ 200$. For $\$ 80$, the customer can purchase an extended warranty that provides free repairs or replacement in case of failures any time within the first three years. Use a Markov model to track the progression of dishwashers through their first three years of service.

a. Is the extended warranty a good buy for the customer? <br>

b. By what amount should GalleyKleen increase the sales price of the dishwasher so that the basic (no charge) warranty could be extended to cover three years? <br>

c. If the basic warranty did cover two years, what is a fair price for the customer to purchase a one-year extension, providing a total of three years of warranty coverage? <br>

6.16 Two companies, one selling Ol' Boy Biscuits and the other selling Yuppy Puppy Pleasers, have cornered the market for dog treats. Each product is packaged to contain a four-week supply of treats, and customers always purchase treats as soon as necessary so as never to run out. For a customer whose last purchase was $\mathrm{Ol}^{\prime}$ Boy, there is a 75\% chance of a brand change on the next purchase; and for a customer who most recently bought Yuppy Puppy, there is an $85 \%$ chance of a brand change on the next purchase. Ol' Boys are sold at a per unit profit of $60 ¢$, and Yuppy Puppys yield a per unit profit of $70 ¢$.

a. What proportion of the market is held by each of these two products? <br>

b. If 30 million customers regularly purchase these products, what are the annual expected profits for each company? <br>

6.17 Consider the assumptions that were made in analyzing the memory allocation processes described in Section 6.9.2. Can you provide arguments that these assumptions are justified in practice? <br>
