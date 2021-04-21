# Integration parameters

To evaluate loop integrals in quantum field theory, we will use

* Feynman parameters
* Schwinger parameters

### Feynman parameters

Feynman parameters are based on a number of easily verifiable mathematical identities. The simplest is

$$
\frac{1}{AB} = \int_0^1 dx \frac{1}{[A+ (B-A)x]^2} = \int_0^1 dx dy\, \delta(x+y-1) \frac{1}{[xA + y B]^2}~.
$$

Other useful identities are

$$
\frac{1}{AB^n} = \int_0^1 dx dy \, \delta(x+ y -1) \frac{n y^{n-1}}{[xA + y B]^{n+1}}\\
\frac{1}{ABC} = \int_0^1 dx dy dz \, \delta(x+y+z-1) \frac{2}{[xA + y B + zC]^3}~.
$$

### Schwinger parameters

Schwinger parameters are based on the following mathematical identities, which hold when $${\rm Im}(A) > 0$$,

$$
\frac i A = \int_0 ^\infty ds \, e^{is A}~,
$$



