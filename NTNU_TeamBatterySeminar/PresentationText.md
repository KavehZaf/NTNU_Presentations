Slide 1:
Hello everyone!
My name is Salman Zaferanlouei, an NTNU power sysems researcher.! 



I would like to thank the organisers to invite me to give a talk. 
My presentaion topic is:
Can we charge everyone's electric vehicles without reinforcing the electric grid?
Here electric vehicle means: mobile batteries.


Slide2:
A quick answer to this question is Yes, we can. But how?
Without doing anything, the present network can host only 20% ev penetration.
With price based charge control, network can host 36%
with our porposal method, the electric grid can host 100% and even more!


Slide 3: 
In summary, this presentaiton has three phases: 
Phase I: Background and motivation
Phase II: EV Statistics
Phase III: Case Study


Slide4: 
Now the background and motivation,

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
2. Increase penetration of solar and wind produtions at tail of the network.


Slide7:
Green shift in electicity system is needed for the reduction of co2 emissions,
(click)
Therefore integration of Distributed energy resourses is a huge challenge!
DER here means renewable generations, energy storage and Flexible demand.
(click)
Thus, Grid companies must be able to analyse the impact of DERs into the future power systems.
(click)
In this case, power flow solvers are very essentials, which means the detailed analysis of electricity flow in the network has to be done. which means how the the power flow affects the voltage, congestion, energy loss, and life time of componenets
because electric grid is the heart of a power systems. 
Optimal power flow solvers does this analysis.
(click)
Therefore integratgion of DERs calls for much more sophisticated solvers for OPF.



Slide 8:
Challenges in the power system transitions can be seperated into two parts:
1. Power systems planning, when to invest? how much to invest? where to invest?, and  what type to invest?
2. considering that energy storage and demand flexibilities are new alternatives to grid investments!
(click)
In terms of Operational challenges!
It is challenging to operate Battery energy storages and flexible demands reliably and economically!
This means right use of demand response and the end user flexibility for local system- and wide grid serices.
This also means simulating and operating the future electricity grid senarios


Slide9:
What are the limitation of today gird and operational tools?
Classical single-period OPF does not offer a possibility for optimal operation scheduling of storage and flexible demand!
(click)

We aim to develop a new geneartion of Multi period ACOPF: but high computational time is the main challenge.
(click)
Developting MPOPF is an extremely challenging task in terms of 
1. Mathematical compexity: non linear and non-convexity of the ACOPF problem
2. This is a problem  with respect ot the time and space when you simulate a large system with a  long  horizon.
3. This also Involves stochastic senarios for generation and load during the future horizon.
(click)
All in all, hardware is reaching to its limit wrt the cpu clock speed!



Slide 10:
What do we suggest is to develop a high performace solver specifically to solve large scale ACOPF problems efficiently. 
This means to develop algorithms and libraries for mathematical operations of large sparse matrices
The prototype models we developed shows convincing results for real size systems which you can see in our case study, in the Third phase of this presentaiton,
(click)
The benefits are optiaml utilisation of stored energy and flexibilty
(click)
It also can be used for the grid planning and opration of local market

 in order to see the detail of what we have done so far, please read these two paper, refered here.



Slide 11
This slide shows the today power systems, I made it a animation to highlight the imporance of time in this slide.
There are few PV generations in the residential area, there are few PV and wind farms, but the main producers are conventional power plants

The power flow is still single directional from large producesrs to end users.

Slide 12:
This slide shows the future of power systme. The main take away from this slide is that You need to have a large computational power to operate such asystem efficiently.



Slie 14
now few statistical data
(click)

you can see EV sale precenage is increasing year by year.


Sile 15:

At the moment we have 10% EV penetration, Keep in mind that norwegian parlement has decided on a national goal to sell 100 % xero emission cars by 2025

Slide 16:
Case study is a real distribution nework which has 856 consumers, 32 medum volaatge transformer and 2 feeders.
The different color in this figure show different voltage level in the network and how thy are distributed.

Simulations are conducted by having access to one year of consumer's base load, the year of 2012 which there is almost zero EV in the network.


Slide 17:
Simulations for this network is conducted through time with the proposed BATTPOWER solver.

Through time things changes, not everybody arrives and connects his ev at the same time, so The number of charging EVs, varies in different time.



Slide 18
Now we are back to the simulation results shown in the second slide.

Dumb charging mode means: EV charges when it arrives
20% here means that the network can only host 20 cars to be EV, if more it will break. Arrival and departure times are considered based on norwegian driving stndards and are taken from published reports.

(click)
Market price base means we charge the EVs when it is the minmum market price:
In this example minimum maket price is between 4:00 to 5:00 AM.
So the simulation reults suggest that 36% of cars can be EV, if more it will break

Our proposed charging method is based on considering both market price and grid operational limits, which are voltage and flow limits.
With this method, it is possible to host 100% EV in this network.
