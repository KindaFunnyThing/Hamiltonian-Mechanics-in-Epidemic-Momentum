## SIR Models with Hamiltonian Mechanics
### A Comparison with the Lotka-Volterra Models

As stated in previous sections, there are numerous methods that can be used to describe SIR models. Further described are a combination of the ways previously used to work through the Lodka-Volterra models and the equations derived in the SIR papers. 

SIR equations: 

$$
\begin{aligned}S\left(t+\Delta t\right)=S\left(t\right)+\ \mu N(t)\Delta t\ +\beta I\left(t\right)S\left(t\right)\Delta t\ -\ \mu S(t)\Delta t &&\left(2.12\right)\end{aligned}
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
\frac{S\left(t+\Delta t\right)-S\left(t\right)}{\Delta t}= \mu N(t) +\beta I\left(t\right)S\left(t\right) - \mu S(t)=\frac{\partial S}{\partial t}
$$

$$
\frac{I\left(t+\Delta t\right) - I\left(t\right)}{\Delta t} = \beta S\left(t\right)I\left(t\right) -\gamma I\left(t\right) - \mu I(t)=\frac{\partial I}{\partial t}
$$

For $\Delta t$ small enough, we can refer to is as $dt$, which ends up being the perfect set of equations we require in order to set up a Hamiltonian:

$$
\frac{dx}{dt}=\frac{\partial H}{\partial p}\Longleftrightarrow \frac{\partial H}{\partial I}=\frac{\partial S}{\partial t},
$$

$$
\frac{dp}{dt}=-\frac{\partial H}{\partial x}\Longleftrightarrow -\frac{\partial H}{\partial S}=\frac{\partial I}{\partial t}.
$$

This conversion to Hamiltonian dynamics is the same that was done to the Lodka-Volterra system. Indeed, we can set up the SIR equations to resemble the equation:

$$
H(N, P) = d \log{N} − cN + a \log{P} − bP.
$$

A more inferring version of the eqaution can be looked at in order to convert the SIR equations into the necessary format. We are going to look at the SIR models through the lens of a $Lyapunov \ function$, where: 

<div align="right">

$$\begin{aligned}V(S,I)=S- \hat S \log{S} + I - \hat I \log{I}\end{aligned}$$

</div>

This is done to prove the asymptotic nature of the equation, and proclaims that V approaches 0. Such an alteration means that it resembles the equations of SIR itself, since it is a modified version that is derived from those equations. These models work only in an extremely specific circumstance: to prove that the equations approach a certain value, which in this case would be 0. Although, since it is derived from the root equations of the SIR models, it is practical to use it in comparison to the Lodka-Volterra system. This also lets us see the equation in a format that resembles the Lodka-Volterra Hamiltonian Dynamics equation: 

$$
H(N, P) = − cN + d \log{N} − bP + a \log{P} \Longleftrightarrow V(S,I)=S- \hat S \log{S} + I - \hat I \log{I}
$$

Here, one can clearly see that the equations have similarities within them, and the only thing needed in order for both to have the same properties is for the signs to be flipped. This bridges the gap in between Hamiltonian Dynamics, Lodka-Volterra systems, and SIR models, all in simplistic circumstances. 

#### Inference and Discussion of this Section

It is important to note that the ability to convert the SIR model to a Hamiltonian Dynamics model proves nothing except for the chance of solving very simple, specific situations in this type of setup. The ability to do this only exists if there are a lot of real world factors not taken into account, such as the loss of information, and the inability for this system to be closed. Miniscule steps are required to not blow up the model, and steps either in the future or the past are rarely acquirable in accuracy. The loss of information in a conserved model is what throws off the Hamiltonian the most, and there are very strict values and conserved species that truly allow the Hamiltonian to be followed within SIR models. 