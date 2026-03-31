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
