# Notes on Hamiltonian Mechanics
## This is a documentation of the playlist and brief notes
### Pertaining to Math
* The math for hamiltonian mechanics is essentially displaying the position and momentum in a different way
* Position on the x axis and momentum (p) on the y
* Would be able to figure out the path taken as either position or time changes, stated as a function. Call the function *H(x,p)*
* Drawing contours from this, we are able to determine that the gradient of H can't provide much information, but if the variables are altered and made orthogonal, we are able to figure out the tangent of the function of *(x(t),p(t))*
* This also means that we are able to find out that the tangent of this function, let's call it S<sub>x</sub> and S<sub>p</sub>, would be equivalent to the 90$\degree$ grad of the H function
* Ultimately, through algebra, it is found that the derivative of *(x(t),p(t))* over *dt* is just $\bar{S}$*(x(t),p(t))* 
* Extracted from this, we can derive that $div(\bar{S})$ is 0

### Pertaining to Measurements
* Hamiltonian mechanics can be used for measurements' uncertainty the same way, mapping the variance of a measurement into another measurement that is an alteration of infinitesimal point from the original measurement
    * This is to say, *x(t<sub>f</sub>) = x(t<sub>i</sub> + dt)*
* The calculation for this reveals that Hamiltonian mechanics makes it so the jacobian's value is 1, which means that no matter what the change of space is, the uncertainty carries over, which represents that Hamiltonian mechanics make the measurement deterministic and reversible

### Pertaining to Thermodynamics
* Flux of an area can be determined mathematically through a surface integral of energy of a system
* This flux can be algebraically altered in order to find the integral of the divergence of $\bar{S}$, which is supposed to be 0
* This means that the energy would be preserved no matter what path you take to get to the second point, or switch from the second to the first

### Pertaining to Information Theory
* 