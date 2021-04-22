# Dimensional regularization

### Scalar integrals

Instead of considering integrals in 4 dimensional spacetime, we will consider in general $$d$$-dimensional spacetime. The angular volume is given by

$$
\Omega_d = \int d \Omega_d = \frac{2\pi ^{d/2}}{\Gamma(d/2)}
$$

{% hint style="success" %}
This is derived from

$$
(\sqrt{\pi})^d = \left(\int_{-\infty}^\infty e^{-x^2}\right)^d = \int d\Omega_d \int_0^\infty dr r^{d-1} e^{-r^2}
$$

and

$$
\Gamma(z) = \int_0^\infty x^{z-1} e^{-x}dx~.
$$
{% endhint %}

$$\Gamma(z)$$has simple poles at 0 and all the negative integers. We will often need to expand $$\Gamma(z)$$around the pole at $$x = 0$$,

$$
\Gamma(\epsilon) = \frac{1}{\epsilon} - \gamma_E + \mathcal O(\epsilon)+\cdots~,
$$

where $$\gamma_E$$ is the Euler-Mascheroni constant, $$\gamma_E \approx 0.577$$. We may also define the Euler $$\beta$$-function as

$$
\beta(a,b) = \frac{\Gamma(a) \Gamma(b)}{\Gamma(a+b)} = \int_0^1 dx (1-x)^{a-1} x^{b-1}~.
$$

This final equality can be seen by calculating

$$
\Gamma(a) \Gamma(b) = \int_0^\infty u^{a-1} e^{-u} du \int _0^\infty v^{b-1} e^{-v} dv \\
= \int e^{-u-v} u^{a-1} v^{b-1} du dv~.
$$

Now make change of variables, $$u = z t $$and $$v = z(1-t)$$,

$$
\Gamma(a)\Gamma(b) = \int_0^\infty dz \, e^{-z} z^{a + b -1} \int_0^1 dt \, t^{a-1} (1-t)^{b-1}\\
= \Gamma(a+b) \beta(a,b)~.
$$

The integrals over Euclidean $$k_E$$are straightforward. Let $$x = \Delta/(k_E^2 + \Delta)$$

$$
\int dk_E \frac{k_E^a}{(k_E^2 + \Delta)^b} = \Delta^{\frac{a+1}{2} -b} \frac{\Gamma(\frac{a+1}{2}) \Gamma(b- \frac{a+1}{2})}{2 \Gamma(b)}~.
$$

Therefore, in general

$$
\int \frac{d^d k}{(2\pi)^d} \frac{k^{2a}}{(k^2 - \Delta)^b} = i (-1)^{a-b} \frac{1}{(4\pi)^{d/2}} \frac{1}{\Delta^{b-a - \frac d2}} \frac{\Gamma(a + \frac d2)\Gamma(b - a - \frac d2)}{\Gamma(b)\Gamma(\frac d2)}~.
$$

Dimensionally regulated versions of divergent integrals will have poles at $$d = 4$$. Therefore, we often expand $$d = 4 - \epsilon$$ and drop terms of order $$\epsilon$$.

### Field dimensions

For the action to be dimensionless, the Lagrangian density should have mass dimension $$d$$. For example, in QED, the Lagrangian is

$$
\mathcal L = - \frac 14 (\partial_\mu A_\nu - \partial_\nu A_\mu)^2 + \bar \psi (i \gamma^\mu \partial_\mu - m) \psi - e\bar \psi \gamma^\mu \psi A_\mu~,
$$

which implies the mass dimensions

$$
[A_\nu] = \frac{d-2}{2}, \quad [\psi] = \frac{d-1}{2}, \quad [m] = 1, \quad [e] = \frac{4-d}{2}~.
$$

However, rather than have a non-integer dimensional coupling, it is conventional to take

$$
e \to \mu^{\frac{4-d}{2}} e~,
$$

where $$\mu$$ is an arbitrary parameter of mass dimension 1. Then $$e$$ remains dimensionless. Then the loop integral will change as

$$
\int \frac{d^4k}{(2\pi)^4} \frac{e^2}{(k^2 - \Delta + i\epsilon)^2} \to \mu^{4-d} \int \frac{d^d k}{(2\pi)^d} \frac{e^2}{(k^2 - \Delta + i\epsilon)}~.
$$

{% hint style="warning" %}
Keep in mind that $$\mu$$ is not a large scale. It is not a UV cutoff. The dimensional regularization is removed when $$d \to 4$$, not when $$\mu \to \infty$$. In fact, we will often use $$\mu$$ as a proxy for a physical infrared scale associated with a renormalization group point.
{% endhint %}

The logarithmically divergent integral becomes

$$
\int \frac{d^4 k}{(2\pi)^4} \frac{e^2}{(k^2 - \Delta + i\epsilon)^2} \to \mu^{4-d} \frac{i e^2}{(4\pi)^{d/2}} \Gamma\left(2- \frac{d}{2}\right) \left(\frac{1}{\Delta}\right)^{2 - \frac{d}{2}}~.
$$

Now letting $$ d= 4- \epsilon$$ we expand this around $$\epsilon = 0$$and get

$$
\frac{ie^2}{16 \pi^2} \left(\frac2 \epsilon - \gamma_E + \ln \frac{4\pi \mu^2}{\Delta}\right) = \frac{ie^2}{16 \pi^2} \left(\frac2 \epsilon + \ln \frac{4\pi \mu^2 e^{-\gamma_E}}{\Delta}\right)
$$

We define

$$
\tilde \mu^2 \equiv 4\pi e^{-\gamma_E} \mu^2
$$

leading to

$$
\int \frac{d^4k}{ (2\pi)^4 } \frac{e^2}{(k^2 - \Delta+ i \epsilon)^2} \to \frac{i e^2}{16 \pi^2} \left(\frac{2}{\epsilon} + \ln\frac{\tilde \mu^2}{\Delta} + \cdots\right)
$$

### $$k^\mu$$ integrals

We will often have integrals with factors of momenta, such as $$k^\mu k^\nu$$, in the numerator,

$$
F^{\mu \nu} (\Delta) = \int \frac{d^4k}{(2\pi)^4} \frac{k^\mu k^\nu}{(k^2 - \Delta)^n} = \frac{1}{d} g^{\mu \nu} \int \frac{d^d k}{(2\pi)^d} \frac{k^2}{(k^2 -\Delta)^n}~.
$$

If there is just one factor of $$k^\mu$$in the numerator, for example in

$$
F(p^2) = \int \frac{d^4k}{(2\pi)^4} \frac{k \cdot p}{(k^2 - p^2)^4}~,
$$

then the integrand is antisymmetric under $$k \to -k$$. Since we are integrating over all $$k$$, the integral must vanish. So we will only need to keep terms with even powers of $$k$$ in the numerator.

