# Regulator-independent derivation

Casimir showed in his [original paper ](https://www.dwc.knaw.nl/DL/publications/PU00018547.pdf)a way to calculate the force in a regulator-independent way. Define the energy as

$$
E(a) = \frac \pi 2 \sum_n \frac n a f\left(\frac{n}{a\Lambda}\right)~,
$$

where $$f(x)$$ is some function whose properties we will determine shortly.

With this definition, the energy of the $$L-a$$side of the box is

$$
E(L-a) = \frac \pi 2 (L-a) \Lambda^2 \sum_n \frac{n}{(L-a)^2 \Lambda^2} f\left(\frac{n}{(L-a)\Lambda}\right)~.
$$

Now take $$L \to \infty$$and $$x = \frac{n}{(L-a)\Lambda}$$, we have

$$
E(L-a) = \frac \pi 2 L \Lambda^2 \int x dx f(x) - \frac \pi 2a \Lambda^2 \int x dx f(x)
$$

The first integral is just the extrinsic vacuum energy, with energy density

$$
\rho = \frac \pi 2 \Lambda^2 \int x dx f(x)~.
$$

The total energy is

$$
E_{\rm tot} = E(a) + E(L-a) = \rho L + \frac{\pi}{2a}\left[\sum_n n f\left(\frac{n}{a \Lambda}\right) - \int n dn f\left(\frac{n}{a \Lambda}\right)\right]~.
$$

This contains the difference between an infinite sum and an infinite integral. Such a difference is given by the [Euler-Maclaurin series](https://en.wikipedia.org/wiki/Euler–Maclaurin_formula),

$$
\begin{align}
\sum_{n=1}^N&F(n) - \int_0^N F(n)dn \\
&= \frac{F(0)+ F(N)}{2} + \frac{F'(N)-F'(0)}{12} + \cdots + B_j \frac{F^{(j-1)}(N) - F{(j-1)}(0)}{j!} + \cdots~,
\end{align}
$$

where $$B_j$$ are Bernoulli numbers. In particular, $$B_2 = \frac 16$$ and $$B_j$$ for odd $$j > 1$$ happen to vanish.

In our case $$F(n) = n f\left(\frac{n}{a \Lambda}\right)$$. So, assuming that $$f(x)$$ dies sufficiently fast,

$$
\lim_{x\to \infty} x f^{(j)} (x) = 0
$$

then

$$
E_{\rm tot} = \rho L - \frac{\pi f(0)}{24 a} - \frac{B_4}{4!} \frac{3\pi}{2a^3 \Lambda^2} f''(0) + \cdots~.
$$

Now it is clear that the regulator will give this force as long as

$$
\lim_{x \to \infty} x f^{(j)}(x) = 0 \quad {\rm and } \quad f(0) = 1~.
$$

{% hint style="success" %}
The first requirement, that $$f(x)$$die fast enough at high energy, means that UV modes go right through the box. It is this requirement that makes the force finite.

The second requirement, that $$f(0) = 1$$, means that the regulator does not affect the spectrum in the IR. On physical grounds, only modes of size $$\frac1a$$can reach both walls of the box to transmit the force, thus our deformation should not affect those modes.
{% endhint %}

We have two conclusions from this analysis

* The Casimir force is independent of any regulator
* The Casimir force is an infrared effect

