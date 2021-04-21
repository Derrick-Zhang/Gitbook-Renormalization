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
\frac i A = \int_0 ^\infty ds \, e^{is A}~,\\
\left(\frac iA\right)^2 = \int_0^\infty s ds \, e^{isA}~.
$$

You can derive further identities by taking additional derivatives with respect to $$A$$. Also, we have

$$
\frac{1}{AB} = - \int_0^\infty ds \int_0^\infty dt e^{is A + i t B}
$$

when $${\rm Im}(A) > 0$$ and $${\rm Im}(B)>0$$.

Other useful related identities are

$$
\begin{align}
\frac{1}{A^n B^m} &= \frac{\Gamma(n+m)}{\Gamma(n)\Gamma(m)} \int_0^\infty ds \frac{s^{m-1}}{(A+Bs)^{n+m}}\\
\frac{1}{AB} &= \int_0^\infty ds \frac{1}{(A+Bs)^2}
\end{align}
$$



