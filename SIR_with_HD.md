## SIR Models with Hamiltonian Mechanics
### A Comparison with the Lotka-Volterra Models

As stated in previous sections, there are numerous methods that can be used to describe SIR models. Further described are a combination of the ways previously used to work through the Lodka-Volterra models and the equations derived in the SIR papers. 

SIR equations: 

$$
\begin{aligned}S\left(t+\Delta t\right)=S\left(t\right)+\ \nu N(t)\Delta t\ +\beta I\left(t\right)S\left(t\right)\Delta t\ -\ \mu S(t)\Delta t &&\left(2.12\right)\end{aligned}
$$

and

$$
\begin{aligned}I\left(t+\Delta t\right)=I\left(t\right)+\beta S\left(t\right)I\left(t\right)\Delta t-\gamma I\left(t\right)\Delta t\ -\ \mu I(t)\Delta t\ \ \ \ \ \ \ \ \ \left(2.13\right)\end{aligned}
$$

are taken from the previous section to make sense of this modification. 


From here, further resources can be recalled from the Hamiltonian mechanics stated in previous sections. 

$$
\frac{\partial H}{\partial p}=Sx=Sx(x,p)=\frac{dx}{dt},
$$

and

$$
\frac{\partial H}{\partial x}=Sp=Sp(x,p)=\frac{dp}{dt} .
$$

Hence

$$
\bar S(x, p)=\left(\frac{\partial H}{\partial p}, -
\frac{\partial H}{\partial x}\right)=
\frac{d}{dt}\left[x\left(t\right),p\left(t\right)\right]
$$

Now, we can restructure this equation to tell us something different:

$$
\frac{x(t+dt)-x(t)}{dt}=S_x\left(x(t),p(t)\right),
$$

$$
\frac{p(t+dt)-p(t)}{dt}=S_p\left(x(t),p(t)\right).
$$

Here, it can be seen that if restructured, it has a very similar structure to equations 2.12 and 2.13 seen before, which were given in terms of $S(t+\Delta t)$ and $P(t+\Delta t)$, which we can alter to represent the equations how we want them.

$$
\frac{S\left(t+\Delta t\right)-S\left(t\right)}{\Delta t}= \nu N(t) +\beta I\left(t\right)S\left(t\right) - \mu S(t)
$$

$$
\frac{I\left(t+\Delta t\right) - I\left(t\right)}{\Delta t} = \beta S\left(t\right)I\left(t\right) -\gamma I\left(t\right) - \mu I(t)
$$