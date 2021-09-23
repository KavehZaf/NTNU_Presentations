Slide 1:
Hello everyone!
My name is Salman Zaferanlouei, an NTNU power sysems researcher.! So I work on electricity market and planning group led by associate professor, Hossein Farahmand!

I will do my best to speak slowly and clearly! but I use long sentences when I am getting excited about something. There are few places in this presenation that I swich topics, so I mention that it is a good time if you got lost in the previous section.

I would like to thank the organisers to invite me to give a talk in the yearly NTNU Battery seminar. 
My presentaion topic is actually a question!
Can we charge everyone's electric vehicles without reinforcing the electric grid?
Here electric vehicle means batteries in the grid!


Slide2:
A quick answer to this question is Yes, we can. Simulation results accuired by us (a group of reseachers in IEL NTNU, suggest that yes, it is possible!
But how?


Slide 3: 
here in this presentation I try to show how it is possible to charge electric vehciles for everyone!
In summary, this presentaiton has three phases: 
Phase I: Background and motivation
Phase II: EV Statistics
Phase III: Case Study
I would like to note that the project that I am working on is called BATTPOWER, which is an ongoing innovation project here in NTNU. If you would like to know more about us, please download our papers or contact me personally.


Slide4: 
So the first Phase of this presentation is the background and motivation of this project I have been working on. If see such a page, keep in mind that here we swich topics


Slide 5:
Here is a figure representing a TODAY prower system structure in details.
Power system includes the main Three parts:
1. power generators, or power producers, On top of this picture, 
2. power system transmission lines and substations as the heart of power systems 
3. consumers at the end point of the structure who pay for thier elecricity bill.


Slide 6:
For many reasons the TODAY power system structure is about to change substantioally. So the traditional chain between large power porducers and consumers is getting weaker and weaker!
Some of these reasons are
1. Phasing out heavy- carbon sources and nuclear power plants,
2. Increase penetration of solar and wind produtions at the end users.


Slide7:
Green shift in electicity system is needed for the reduction of co2 emissions,
Therefore integration of Distributed energy resorses is a huge challenge!
DER here means renewable generations, energy storage and Flexible demand.

Thus, Grid companies must be able to analyse the impact of DERs into the future power systems.
In this case, power flow solvers are very essentials, because in the clasification we made before, electric grid is the heart of a power systems.
Therefore integratgion of DERs calls for much more sophisticated solvers for OPF.



Slide 8:
Challenges in the power system transitions can be seperated into two parts:
1. Power systems planning, when to invest? how much to invest, and where to invest what type to invest?
2. considering that energy storage and demand flexibilities are new alternatives to grid investments!

In terms of Operational challenges!
It is challenging to operate Battery energy storages and flexible demands reliably and economically!
This means right use of demand response. value the end user flexibility for local system- and wide grid serices.
This also means simulating and operating the future electricity grid in the presence of future local energy and flexibility markets 



Slide9:
What are the limitation of today gird and operational tools?
Classical single-period OPF does not offer a possibility for optimal operation scheduling of storage and flexible demand!
We aim to develop the geneartion of Multi period ACOPF: High computational time is an issue within this approach!
Developting MPOPF is an extremely challenging task in terms of 
1. non linear and non-convexity of the ACOPF problem.
2. This is a large problem with respect ot the time and space
3. Involves stochastic generation and load

All in all, hardware is reaching to its limit wrt the cpu clock speed!



Slide 10:
What do we suggest is to develop a high performace solver specifically to solve large scale ACOPF problems efficiently. 
This means to develop algorithms and libraries for mathematical operation of large sparse matrices
The prototype models shows convincing results for real size systems, in order to see the detail of what we have done so far, please read these two paper, refered here.

W
