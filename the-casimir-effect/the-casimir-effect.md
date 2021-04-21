# The Casimir effect

The Hamiltonian for a free scalar field is

$$
H = \int \frac{d^3k}{(2\pi)^3} \omega_k \left(a_k^\dagger a_k + \frac12\right)~,
$$

So the contribution to the vacuum energy of the zero modes is

$$
E = \langle 0 | H | 0 \rangle = \int \frac{d^3 k }{(2\pi)^3 } \frac{\omega_k}{2} = \frac{1}{4 \pi^2} \int k^3 dk = \infty~,
$$

known as the **zero-point energy**.

{% hint style="info" %}
While the zero-point energy is infinite, it is also not observable. Only energy differences matter and the absolute energy is unphysical.
{% endhint %}

Consider the zero-point energy in a box of size $$a$$. If the energy changes with $$a$$, then we can calculate the force

$$
F = - \frac{dE}{da}~.
$$

We have a natural low-energy cutoff $$|\vec k| > \frac1a$$. This does not cut off the high-energy divergence at large $$k$$; we will show that there will be a finite residual dependence on $$a$$that will give an observable force, called the **Casimir force**.

{% hint style="info" %}
If we change $$a$$, then the energy inside and outside the box will change. We can put in a third wall on our box far away, at$$L \gg a$$. Then the zero-point energy outside the box is independent of $$a$$, so we can drop it.
{% endhint %}

We will work with a one-dimensional box. In a one-dimensional box of size $$r$$ the classically quantized frequencies are

$$
\omega_n = \frac{\pi}{r}n~.
$$

Then the zero-point energy is

$$
E(r) = \sum_n \frac{\omega_n}{2} = \frac{1}{r}\frac{\pi}{2}\sum_n n~.
$$

The total energy is the sum of the energy on the right side, $$r = L - a$$, plus the energy on the left side, $$r = a$$,

$$
E_{\rm tot} = E(a) + E(L-a) = \left(\frac1a + \frac{1}{L-a}\right) \frac{\pi}{2} \sum_{n = 1}^\infty n~.
$$

We hope the force is finite

$$
F(a) = - \frac{dE_{\rm tot}}{da} = \left(\frac{1}{a^2}- \frac{1}{(L-a)^2}\right) \frac{\pi}{2} \sum_{n=1}^\infty n~.
$$

{% hint style="warning" %}
What are we missing? At boundaries, there are walls made of atoms. Consider super-high-energy radiation modes, with super-small wavelengths. They are going to just plow through the walls, these ultra-high-frequency modes should be irrelevant.
{% endhint %}

