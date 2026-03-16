## Writing Draft in Docs

Intro to Lotka-Volterra models

In order to better understand the growth and decay rates of animal populations mathematical models were created to more analytically analyze the patterns present in these rates. One of these models is the Lotka-Volterra model which, in their most simple, single species form, are modelled using the density of the species(⍴), the amount of the species present (N) and the carrying capacity of the environment for the species(K).

(Write it [Eq.1.2, Pg. 4])


In a Lotka-Volterra model that is modelling the presence of more than one species there are more complex equations and considerations. In a two species system with a predator and prey, the change in either population is dependant on the population of the other and can be modelled by

(simple Lotka-Volterra models)
(simple Lotka Volterra models)

Where a,b,c,d are constants, N is the prey population and P is the predator population.

As seen in these equations and figure 1, when these are plotted, they show periodic orbits. That is to say that the populations of the prey and predator continuously fluctuate but always return to the same places. Intuitively, this means that once an initial set of conditions has been set,assuming a≠bP, d≠cN, and all variables are positive, the populations as time progresses are able to be predicted. Due to the nature of each population relying on the population of the other, the fluctuations repeat themselves with the initial state being returned to repeatedly as the populations move through time.

(figure 1.1)

These equations are in fact Hamiltonian in nature. When rearranging the equations 1.1 and 1.2, a new equation (the Hamiltonian function) can be obtained that can be directly substituted with canonical Hamiltonian coordinates. This results in a perfect overlap of Hamiltonian mechanics onto the Lotka-Volterra models.

(Write it [Eq.1, Pg.2])
(Write it [Eq.3, Pg.2])
(Write it [p=logN])
(Write it [q=logP)
(Write it [Eq. 1 and 2, Pg.3])

These equations are not wholly realistic however as they ignore fundamental parts of species interacting with one another, namely competition and mutualism. These factors affect the rates of change of a species population greatly and are necessary inclusions in mathematical models that attempt to present the fluctuations of populations. The models can be modified to incorporate competition and mutualism. In the case of competition it involves adding an additional parameter to the single species equation (equation 1.0) which represents the negative effect of the other species presence on the species.

(Write it [Eq. 1.3, Pg. 5])

