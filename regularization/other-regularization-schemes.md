# Other regularization schemes

The dimensional regularization has the disadvantage of being unphysical. Now we introduce two other regularization schemes

* The derivative method
* Pauli-Villars regularization

### Derivative method

Consider a logarithmically divergent integral, such as

$$
\mathcal I (\Delta) = \int \frac{d^4 k }{(2\pi)^4} \frac{1}{(k^2 - \Delta + i\epsilon)^2} = \infty~.
$$

If we take the derivative, the integral can be done

$$
\frac{d}{d\Delta} \mathcal I (\Delta) = \int \frac{d^4k}{(2\pi)^4} \frac{2}{(k^2 - \Delta+ i \epsilon)^3} = - \frac{i}{16 \pi^2 \Delta}~.
$$

So,

$$
\mathcal I (\Delta) = - \frac{i}{16 \pi^2} \ln \frac{\Delta}{\Lambda^2}~,
$$

where $$\Lambda$$ is an integration constant representing the UV cutoff and is formally infinite.

{% hint style="danger" %}
The derivative method is not an ideal regulator. Since the cutoff $$\Lambda$$appears as a constant of integration, there is no way to relate $$\Lambda$$from on integral to $$\Lambda$$from another.
{% endhint %}

### Pauli-Villars regularization

Pauli-Villars regularization requires that for each particle of mass $$m$$ a new unphysical **ghost** particle of mass $$\Lambda$$be added with either the wrong statistics or the wrong-sign kinetic term.

For example, at 1-loop, the Pauli-Villars Lagrangian for QED

$$
\mathcal L_{\rm PV} = - \frac{1}{4} F_{\mu \nu}^2 + \bar\psi(i \partial\!\!\!/ - eA\!\!\!/ - e\tilde A\!\!\!/-m) \psi\\
+ \frac 14 \widetilde F^2_{\mu \nu} - \frac 12 \Lambda^2 \widetilde A_\mu^2 + \bar{\widetilde \psi} (i \partial \!\!\!/ - eA\!\!\!/- e\tilde A\!\!\!/ - \Lambda)\widetilde \psi~,
$$

with $$\tilde A_\mu$$ the ghost photon and $$\widetilde \psi$$ the ghost electron. We assume that both the ghost photon and ghost electron have bosonic statistics; the ghost photon has a wrong-sign kinetic term.

In more detail, an amplitude with Pauli-Villars regularization will sum over the real particle, with mass $$m$$, and the ghost particle, with fixed large mass $$\Lambda \gg m$$,

$$
\int \frac{d^4k}{(2\pi)^4} \frac{1}{(k^2 -m^2 + i \epsilon)^2} \to \int \frac{d^4k}{(2\pi)^4} \left[\frac{1}{(k^2-m^2 + i \epsilon)^2} - \frac{1}{(k^2 - \Lambda^2 + i \epsilon)^2}\right]
$$

Evaluating this integral would give

$$
\int \frac{d^4k}{(2\pi)^4} \frac{1}{(k^2 -m^2 + i \epsilon)^2} \to - \frac{i}{16 \pi^2} \ln\frac{m^2}{\Lambda^2}
$$

