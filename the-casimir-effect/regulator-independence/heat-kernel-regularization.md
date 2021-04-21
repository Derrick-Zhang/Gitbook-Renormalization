# Heat-kernel regularization

Another reasonable physical assumption besides a hard cutoff would be that there is some penetration depth of the modes into the walls, with high-frequency modes getting further. This means the contribution of high-frequency modes to the relevant energy sum is exponentially suppressed,

$$
E(r) = \frac12 \sum_n \omega_n e^{-\omega_n / (\pi \Lambda)}~.
$$

This is called the heat-kernel regularization.

Expanding with $$\omega_n = \frac \pi r n$$,

$$
E(r) = \frac{1}{r}\frac\pi 2 \sum_{n = 1}^\infty n e^{-n/(\Lambda r)} = \frac 1r \frac \pi 2 \sum_{n = 1}^{\infty}n e^{-\epsilon n}~, \quad \epsilon = \frac{1}{\Lambda r} \ll 1~.
$$

Now we can calculate

$$
\sum_{n=1}^\infty n e^{-\epsilon n} = - \partial_\epsilon \sum_{n=1}^\infty e^{-\epsilon n} = - \partial_\epsilon\frac{1}{1-e^{-\epsilon}} = \frac{e^{-\epsilon}}{(1-e^{-\epsilon})^2} = \frac{1}{\epsilon^2} - \frac{1}{12} + \frac{\epsilon^2}{240} + \cdots
$$

Therefore

$$
E(r) = \frac 1r \frac \pi 2 \left[\Lambda^2 r^2 - \frac{1}{12} + \frac{1}{240 r^2 \Lambda^2} + \cdots\right] = \frac\pi 2 r \Lambda^2 - \frac{\pi}{24r}+ \cdots
$$

Then

$$
F(a) = - \frac{d}{da} [E(L-a)+ E(a)] = \frac{\pi}{24} \left(\frac{1}{(L-a)^2} - \frac{1}{a^2}\right)
$$

Now take $$L \to \infty$$ and we get

$$
F(a) = -\frac{\pi}{24 a^2} \hbar c~.
$$



