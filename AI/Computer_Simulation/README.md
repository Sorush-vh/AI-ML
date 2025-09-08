This simulation project is based on a simplification from the paper "Queuing-Based Energy Consumption Management for Heterogeneous Residential Demands in Smart Grid", Yi Liu, Chau Yuen, Yan Zhang, June 2015.
The Original Paper Proposes a method in which the electricity demand of households is classified into 3 groups of: essesntial, flexible-delay-sensitive and flexible-delay-tolerant.
The paper Proposes a method to minimize the cost function (consisting of system's workload and waiting time for flexible demands), while assuring the fairness of the queue system.
In my simplified simulation, we choose 3 scenarios to test different policies for queue management: 1) Barely Managable Workload, 2)Infeasible 3) 1st scenario but with hourly power outages.
The policies have been tested under our scenarios, and the results have been appended. I have also mixed policies together to see their effect.
along the policies under test, a simplified model related to the reference paper is implemented, which yielded to similiar results with FIFO policy.
later on, it is attempted to empower the model with suggested Qlearning methods in the paper, which sadly resulted into overfitness.
A Documentation of the Project is also attached (in persian)
Hopefully, This Project will one day be thoroughly fulfilled! (doubted tho, since i have passed the related course)