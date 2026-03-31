# Notes from the source posted by Dr. Bolker

- Humans divided into three different categories:
    * Susceptible: indictated by S
    * Infected: indicated by I
    * Removed: indicated by R
    * $S + I + R = N$, a total number of individuals

Two main ODE's, about the rate displayed by the flow of individuals into and out of each category:
* $\fracdS dt = -\beta SI$
* $\fracdI dt = \beta SI - \gamma I$