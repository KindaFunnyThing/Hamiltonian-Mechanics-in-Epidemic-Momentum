# Notes from the source posted by Dr. Bolker

- Humans divided into three different categories:
    * Susceptible: indictated by S
    * Infected: indicated by I
    * Removed: indicated by R
    * $S + I + R = N$, a total number of individuals

- Two main ODE's, about the rate displayed by the flow of individuals into and out of each category:
    * $\frac{dS}{dt} = -\beta SI$
    * $\frac{dI}{dt} = \beta SI - \gamma I$

    There is a third:
    * $\frac{dR}{dt} = \gamma I$

    But it is not used, because $R$ does not have an impact on the dynamics of $S$ and $I$

    $\beta$ is the transmission rate per capita, and $\gamma$ is the recovery rate, so how many people are recovering per unit time

    This means that $\frac{1}{\gamma}$ would be the mean infectious period, because it is the reciprocal of the original: $\frac{1}{time}$
$S(0) = N$, obviously, because no one knows about the disease yet so no vaccines. Of course, there would be exceptions in the real world, but this is ideal world.  

- Since the first infected person has the transmission rate and the population number, along with the infectious period's time chance to infect people around them, this means that the $basic reproduction rate$ of the disease would be $\R_0$