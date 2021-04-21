# Other regulators

We can use other regulators

* Gaussian regulator

  $$
  E(r) = \frac 12 \sum_n \omega_n e^{-\left(\frac{\omega_n}{\pi \Lambda}\right)^2}
  $$

* $$\zeta$$-function regulator where we take $$s\to 0$$

  $$
  E(r) = \frac12 \sum_n \omega_n \left(\frac{\omega_n}{\mu}\right)^{-s}~
  $$

For the $$\zeta$$-function case, substituting in for $$\omega_n$$we get

$$
E(r) = \frac12 \left(\frac \pi r\right)^{1-s} \mu^s \sum_n n^{1-s}~.
$$

The sum is the definition of the [Riemann $$\zeta$$-function](https://en.wikipedia.org/wiki/Riemann_zeta_function),

$$
\sum_n n^{1-s} = \zeta(s-1) = - \frac{1}{12} - 0.165s + \cdots.
$$

So we get

$$
E(r) = \frac 1r \frac \pi 2\zeta(s-1) = \frac 1r \frac \pi 2 \left[ - \frac{1}{12} + O(s)\right]
$$

This is the same as what heat-kernel and floor-function regularization gave, although now note that the extrinsic energy term is absent.

