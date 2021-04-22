# Wick rotations

After introducing Feynman parameters and completing the square, one is often left with an integral over a loop momentum $$k^\mu$$in Minkowski space. Once the $$i\epsilon$$factors are put in for Feynman propagators, 1-loop integrals often appear as

$$
\int \frac{d^4k}{(2\pi)^4} \frac{1}{(k^2 - \Delta + i \epsilon)^n}~.
$$

Assuming $$\Delta > 0$$, the integral has poles at $$k_0 = \sqrt{\vec k^2 + \Delta} - i \epsilon$$and $$k_0 = - \sqrt{\vec k^2 + \Delta} + i \epsilon$$. Since the poles are in the top-left and bottom-right quadrants of the $$k_0$$complex plane. We can rotate the contour, $$k0 \to i k_0$$, so that $$k^2 \to -k_0^2 - \vec k^2 = - k^2_E$$, where $$k_E^2 = k_0^2 + \vec k^2$$is the Euclidean momentum. This is known as a **Wick rotation**.

{% hint style="info" %}
After the wick rotation, the $$i\epsilon$$ will no longer play a role an we can just set $$\epsilon = 0$$
{% endhint %}

Once Wick-rotated, the integrals are evaluated in a straightforward way. We will need the formula for the surface area of the Euclidean 4-sphere, $$\int d\Omega_4 = 2\pi^2$$. Using this, we find

$$
\int \frac{d^4 k_E}{(2\pi)^4} f(k_E^2) = \frac{1}{16 \pi^4} \int d \Omega_4 \int_0^\infty k_E^3 dk_E f(k_E^2) = \frac{1}{8 \pi ^2} \int_0^\infty k_E^3 dk_E f(k_E^2)~.
$$

Then, consider a simple example

$$
\begin{align}
\int \frac{d^4 k}{(2\pi)^4} \frac{1}{(k^2 - \Delta + i \epsilon)^3} &= i \int \frac{d^4 k_E}{(2\pi)^4} \frac{1}{(-k_E^2 -\Delta )^3}\\
&= (-1)^3 \frac{i}{8\pi^2} \int_0^\infty d k_E \frac{k_E^3}{(k_E^2 + \Delta)^3}\\
& = \frac{-i}{32 \pi^2 \Delta}~.
\end{align}
$$

