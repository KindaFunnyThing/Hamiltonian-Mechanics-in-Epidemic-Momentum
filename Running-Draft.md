## Writing Draft in Docs

Introduction to Lotka-Volterra models in conjunction with Hamiltonian Mechanics

In order to better understand the growth and decay rates of animal populations mathematical models were created to more analytically analyze the patterns present in these rates. One of these models is the Lotka-Volterra model which, in their most simple, single species form, are modelled using the density of the species(⍴), the amount of the species present (N) and the carrying capacity of the environment for the species(K),

dNdt = ρN(1 − NK)

In a Lotka-Volterra model that is modelling the presence of more than one species there are more complex equations and considerations. In a two species system with a predator and prey, the change in either population is dependant on the population of the other and can be modelled by

1NdNdt=a − bP
1PdPdt=cN − d

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

Which of these steady states is obtained depends entirely on the competitiveness of the species. If a12 < 1 and a21 < 1, then the species exist in coexistence and P becomes stable and each of the others become unstable leading to populations of both species coexisting. In the case that a12 > 1 and a21 > 1, (1,0) and (0,1) become the only stable points, representing competitive dominance of one species and the extinction of the other. The species that dominates is determined by the initial conditions or whichever one's competitive coefficient was higher. If a12 < 1 and a21 > 1, then there exists only one steady state that the population falls to, (1,0), with complete dominance of the first species. The same but opposite can be said if the situations are reversed with a12 > 1 and a21 < 1, this situation leads to complete dominance of species 2 with a steady state at (0,1). P, the interior steady state, can only exist within the first two cases due to the constraints of reality. P must have two positive values which is only possible if a12 and a21 are both either greater than or smaller than 1. If one of the competitive coefficients is greater than 1 while the other is smaller it leads to a negative population of animals which is not possible. These results indicate that there are no periodic orbits within this competitive model nor are there any total extinctions. A steady state must always be reached meaning that at least one species must survive within the ecosystem.

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
