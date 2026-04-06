## Writing Draft in Docs

Introduction to Lotka-Volterra models in conjunction with Hamiltonian Mechanics

In order to better understand the growth and decay rates of animal populations mathematical models were created to more analytically analyze the patterns present in these rates. One of these models is the Lotka-Volterra model which, in their most simple, single species form, are modelled using the density of the species(⍴), the amount of the species present (N) and the carrying capacity of the environment for the species(K),

$$
\frac{dN}{dt} = \rho N(1 − \frac{N}{K})
$$

In a Lotka-Volterra model that is modelling the presence of more than one species there are more complex equations and considerations. In a two species system with a predator and prey, the change in either population is dependant on the population of the other and can be modelled by
$$
\frac{1}{N}dNdt=a − bP
$$
$$
1PdPdt=cN − d
$$
Where a,b,c,d are constants, N is the prey population and P is the predator population. As seen in these equations and figure 1, when these are plotted, they show periodic orbits. That is to say that the populations of the prey and predator continuously fluctuate but always return to the same places. Intuitively, this means that once an initial set of conditions has been set,assuming a≠bP, d≠cN, and all variables are positive, the populations as time progresses are able to be predicted. Due to the nature of each population relying on the population of the other, the fluctuations repeat themselves with the initial state being returned to repeatedly as the populations move through time.

(insert Figure 1.1)
Figure 1: The periodic orbits of the solutions to the two-species Lotka-Volterra model

These equations are in fact Hamiltonian in nature. When rearranging the equations 1.1 and 1.2, a new equation (the Hamiltonian function) can be obtained that can be directly substituted with canonical Hamiltonian coordinates. This results in a perfect overlap of Hamiltonian mechanics onto the Lotka-Volterra models.

−(cN − d)NdNdt +(a − bP)PdPdt = 0

H(N, P) = d log N − cN + a log P − bP

This is changed to canonical Hamiltonian coordinates using 

p = log N, q = log P

dpdt=1NdNdt= a − bP = a − beq = ∂h∂q
dqdt=1PdPdt= cN − d = cep − d = -∂h∂p

These equations are not wholly realistic however as they ignore fundamental parts of species interacting with one another, namely competition and mutualism. These factors affect the rates of change of a species population greatly and are necessary inclusions in mathematical models that attempt to present the fluctuations of populations. The models can be modified to incorporate competition and mutualism. In the case of competition it involves adding an additional parameter to the single species equation (equation 1.0) which represents the negative effect of the other species presence on the species.

dN1dt=ρ1N1(1 − N1K1− c1N2)
dN2dt=ρ2N2(1 − N2K2− c2N1)

With c > 0 representing the competitiveness of the species. However, in order to fully understand the impact of the two species on one another the nullclines of the equation can be calculated which will allow us to discover which steady states are feasible and stable. The first step that needs to be taken is the simplification of the equation allowing us to more easily see the interaction occurring. To reduce the number of variables, ui = Ni/Ki and a12 = c1K2 while a21 = c2K1. In addition, time will be altered to become dimensionless to remove additional parameters from the equation with τ = ⍴1t as well as ⍴ = ⍴2/⍴1. This leads to simpler equations that retain the same properties of the originals.

du1dτ=u1 (1 − u1 − a12u2)
du2dτ=ρu2 (1 − u2 − a21u1)

The nullclines of these equations are fairly easy to see with whether setting the first or second term to equal 0 and solving for either the term outside the bracket or within the bracket. This leads to 4 possible steady states

(u∗1, u∗2) = (0, 0), (1, 0), (0, 1), P =(1 − a121 − a12a21,1 − a211 − a12a21)

Which of these steady states is obtained depends entirely on the competitiveness of the species. If a12 < 1 and a21 < 1, then the species exist in coexistence and P becomes stable and each of the others become unstable leading to populations of both species coexisting. In the case that a12 > 1 and a21 > 1, (1,0) and (0,1) become the only stable points, representing competitive dominance of one species and the extinction of the other. The species that dominates is determined by the initial conditions or whichever one&#39;s competitive coefficient was higher. If a12 < 1 and a21 > 1, then there exists only one steady state that the population falls to, (1,0), with complete dominance of the first species. The same but opposite can be said if the situations are reversed with a12 > 1 and a21 < 1, this situation leads to complete dominance of species 2 with a steady state at (0,1). P, the interior steady state, can only exist within the first two cases due to the constraints of reality. P must have two positive values which is only possible if a12 and a21 are both either greater than or smaller than 1. If one of the competitive coefficients is greater than 1 while the other is smaller it leads to a negative population of animals which is not possible. These results indicate that there are no periodic orbits within this competitive model nor are there any total extinctions. A steady state must always be reached meaning that at least one species must survive within the ecosystem.

(Insert figure 1.3)
Figure 2: These show the nullcline of the two-species Lotka-Volterra model with a competition term. In the top left, a12 = 0.75 and a21 = 0.75. In the top right, a12 = 1.25 and a21 = 1.25. In the bottom left, a12 = 0.75 and a21 = 1.25. In the bottom right, a12 = 1.25 and a21 = 0.75. The ⍴ is held constant at 2.0. 

In the case of mutualism, the equation of competition is utilized with the negative effect of the ciKj term changed to a positive effect

dN1dt=ρ1N1(1 − N1K1+ c1N2)
dN2dt=ρ2N2(1 − N2K2+ c2N1)

Using the same changes to the parameters that were used for competition, these equations and be changed to be easier to interpret

du1dτ=u1 (1 − u1 − a12u2)
du2dτ=ρu2 (1 − u2 − a21u1)

Due to the now positive slant of the nullclines, which cross either once at a steady state or not at all, there always exists three steady states, (0,0), (1,0), (0,1). In addition, when a12a21 < 1, then there exists a fourth steady state

ū=(1 + a211 − a12a21,1 + a121 − a12a21)

When this fourth steady state exists all orbits converge on it and each of the species, through mutual benefit, either meet or exceed their carrying capacity so long as a12 and a21 ≥ 0. If a12a21 > 1 then the fourth steady state does not exist, the nullclines do not meet each other at any point in the positive quadrant and each species population approaches infinity as their beneficial qualities on one another are solely dependent on the mutualistic coefficient and their populations.

(insert Figure 1.4)
Figure 2: These are nullclines for the two-species Lotka-Volterra Model with a mutualistic  term added. The graph on the left shows a12 = 0.4 and a21=0.3. The graph of the right shows a12 = 2.0 and a21 = 1.0.



SIR models: Understanding Epidemics (Working heading) (All the equations were done in word bc we are working on like 3 different platforms and will be much cleaner when finalized)

Epidemics have a long and storied history concerning and relating to human beings. Many have had enormous death tolls both to do with infection from the pathogen and the social havoc it has the potential to wreak. So, in order to combat these events, models have been created in order to further understand and dissect the spread of infectious agents. One model that is useful for doing this is the SIR, or Susceptible-Infected-Recovered model (also known as Susceptible-Infected-Removed), model. This model splits the population into;

	Susceptible (S): the individuals in the population that are able to be infected by the pathogen
	Infected (I): the individuals who have already been infected with the pathogen and have not yet recovered from the infection
	Recovered (R): the individuals who have been infected and then have recovered from the infection and cannot be reinfected

These categories by themselves are useful for looking at a population in a specific point in time but when looking at the changes in them as the epidemic progresses, insight as to how long epidemics can last and how they will resolve themselves can be gleaned. In order to do this an ordinary differential equation (ODE), equations 2.1, 2.5 and 2.3, can be assigned to each category,
\begin{align}\frac{dS}{dt}=\sigma N\ -\ \mu S-\beta I\frac{S}{N}#\left(2.1\right)\end{align}
In this equation, N is the total population that is being affected by the epidemic where   N = S + I + R. σ is the birth rate of the population and µ is the death rate. In equation 2.2, these two are equal to each other creating a population whose change in population is zero (dN/dt = 0). 
\begin{align}\frac{dS}{dt}=\mu\left(N-S\right)-\beta I\frac{S}{N}#\left(2.2\right)\end{align}
This creates a constant population and eliminates one factor when examining infectious diseases, creating a limitation on the kind of scenario and pathogen that can be examined but simplifying the analysis. This equation can be further refined by a closed epidemic where in there are no births or deaths making the first term in equation 2.2 equal to 0,
\frac{dS}{dt}=-\beta I\frac{S}{N}

Here, ß represents the transmission rate per capita of the pathogen, showing how many people the infection will spread to from one individual. Additionally, the terms S, I and R are all integers in these equation. This equation is also sometimes presented as shown in equation 2.4, where these terms are represented in percentages of the population, eliminating the factor N and instead incorporating it into the S term,
\begin{align}\frac{dS}{dt}=-\beta IS#\left(2.4\right)\end{align}
This paper will be utilizing the form of these equations wherein the S,I, and R terms are integers. 

The change in the infected portion of the population is given by equation 2.5 containing a term to do with the infection of the susceptible portion of the population, the recovery from the existing infected pool, and the death rate associated with the infected population. For simplicity the infection will be non-lethal causing the death rate of the population to be equal to the death rate in each category of the population,
\begin{align}\frac{dI}{dt}=\beta I\frac{S}{N}-\gamma I-\mu I#\left(2.5\right)\end{align}
The γ term represents the recovery rate of infected individuals transferring them to the recovered pool with equation 2.6,
\begin{align}\frac{dR}{dt}=\gamma I-\mu R#\left(2.6\right)\end{align}

With these three equations we assume that the infection rate of the pathogen does not change throughout the period of infection, that once they have been exposed to the pathogen that a susceptible individual is immediately infectious, that people in the recovered category are now immune to reinfection and that there are no changing social factors (which may be included in the ß term). These assumptions, like the death and birth rate assumptions, limit the application of these equations but also simplify the analysis of the situation. For this SIR model, the basic reproductive ratio is shown in equation 2.7. 
$$
\begin{align}R_0=\frac{\beta}{\gamma+\mu}\left(2.7\right)\end{align}
$$
This ratio is defined as the number of cases that are expected to appear in a completely susceptible population when a single infected individual is present. This ratio can then be modified using the fraction of the population that is susceptible to the pathogen (s) in order to create the running ratio (RE), or the estimated number of people that will be infected from a single individual in a population that is not fully susceptible, shown in equation 2.8,
$$
\begin{align}R_E=sR_0\left(2.8\right)\end{align}
$$

R0 and RE are extremely important values as they represent whether a pathogen can establish itself within a community and whether it will be able sustain itself within a community. If R0 or RE are below 1, the pathogen will not be able to get a foothold in the community or, if already present, sustain itself as the infection rate is simply not large enough to outpace the recovery rate (γ), the death rate (µ) or some combination of the two. In other words, if each infected individual passes the pathogen to less than one other individual the number of infected individuals will eventually fall to zero.

The SIR models described in the equations above can be taken in the form of an open or a closed epidemic. One where the susceptible category is not finite and new individuals are added to it either through birth, immigration or losing immunity to the pathogen, and the other where the susceptible category is finite. These two situations have different final sates of the epidemic. A closed epidemic results in the pathogen burning through everyone in the susceptible category reaching a state where S is equal to some portion of the population that escaped infection, an I equal to zero as everyone who was infected recovered or died, and an R equal to the portion of the population that recovered. This is different in an open epidemic with a pathogen whose recovery rate is not too fast and who is not highly deadly. This allows for the pool of susceptible individuals to refill and for a new epidemic to start once the last one has ended and the pathogen burned through the majority of the susceptible population. Eventually, as the population is re-exposed to this pathogen a steady state is achieved defined as (S*, I*, R*). These are defined by equations 2.9, 2.10, and 2.11, wherein the changes in these populations are set to zero and then rearranged;

$$
S^\ast=\frac{\left(\gamma+\mu\right)}{\beta}=\frac{1}{ℝ_0} \qquad (2.9)
$$
$$
I^\ast=\frac{\mu\left(R_0-1\right)}{\beta} \qquad \left(2.10\right)
$$
$$
R^\ast=N-S^\ast-I^\ast \qquad \left(2.11\right)
$$

These models can be solved in various ways, including using the Eulers approximation wherein the ODE’s are solved and incrementally calculated by a computer using the equations described in equations 2.12 and 2.13;

$$
\begin{aligned}S\left(t+\Delta t\right)=S\left(t\right)+\ \nu N(t)\Delta t\ +\beta I\left(t\right)S\left(t\right)\Delta t\ -\ \mu S(t)\Delta t &&\left(2.12\right)\end{aligned}
$$

and

$$
\begin{aligned}I\left(t+\Delta t\right)=I\left(t\right)+\beta S\left(t\right)I\left(t\right)\Delta t-\gamma I\left(t\right)\Delta t\ -\ \mu I(t)\Delta t\ \ \ \ \ \ \ \ \ \left(2.13\right)\end{aligned}
$$

Both of these methods provide a reoccurring epidemic that eventually levels off into a steady state as described above. These equations when plotted as the population of the infected category against time will show a dampening effect on the number of infected individuals ever new epidemic that occurs until it reaches the steady state defined by the pathogen and populations parameters, seen in figure ?a. However, when transferring this to phase space as is done in figure ?b, which plots the infected population against the susceptible population it forms a two-dimensional oblong spiral, which still exhibits the dampening effect, whose center is the steady state of the epidemic. In figure (?+1), the nullclines of the system are shown intersecting the center of the spiral. Similarly to the Lotka-Volterra predator-prey models whose competitive factors a12 and a21 are below 1, the nullclines intersect one another and push the two components to a steady state.

