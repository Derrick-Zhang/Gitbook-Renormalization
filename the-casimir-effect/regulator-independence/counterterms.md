# Counterterms

In the above analysis, we not only took $$\omega_{\rm max} \to \infty$$but also $$ L \to \infty$$. Why did we need this third boundary at $$r = L$$at all? Let us suppose we did not have it, and just calculated the energy inside the box of size $$r$$. Then we would get

$$
E(r) = \frac \pi 2 r \Lambda^2 - \frac{\pi}{24 r}+ \cdots.
$$

The first term is the extrinsic energy, which is

* linear in the volume
* regulator dependent

It can be interpreted as saying there is some finite energy density $$\rho = E_0/r = \frac \pi 2 \Lambda^2$$. Now suppose that instead of just the free-field Lagrangian $$\mathcal L$$ we used to calculate the ground-state energy, we took

$$
\mathcal L = \mathcal L' + \rho_c~,
$$

where $$\rho_c$$is constant. This new term gives an infinite contribution in the action. Now if we choose $$\rho_c = - \frac \pi 2 \Lambda^2$$, the new term exactly cancels the $$\frac \pi 2 r \Lambda^2 $$term we found using the heat-kernel regulator.

{% hint style="info" %}
In the $$\zeta$$-function regulator, where no divergent terms come out of the calculation, we could take $$\rho_c = 0$$.
{% endhint %}

The point is that since $$\rho_c$$ is unmeasurable we can choose it to be whatever is convenient. $$\rho_c$$ is called a **counterterm**. Counterterms give purely infinite contributions to _intermediate steps_ in calculations, but when we compute _physical quantities_ they drop out.

