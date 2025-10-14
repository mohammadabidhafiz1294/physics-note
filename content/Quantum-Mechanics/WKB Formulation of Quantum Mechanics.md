## Derivation of WKB Connection Formulas from Asymptotic Solutions

Starting from the basic WKB asymptotic wavefunctions and following a systematic patching procedure, I'll derive the connection formulas that relate solutions across classical turning points.
#### Starting Point: WKB Asymptotic Solutions

The WKB method provides asymptotic solutions in different regions:

**Classical Region** ($E > V(x)$):
$$\psi(x) \approx \frac{1}{\sqrt{p(x)}} \left[ A e^{i\int^x p(x')\,dx'/\hbar} + B e^{-i\int^x p(x')\,dx'/\hbar} \right]$$
**Nonclassical Region** ($E < V(x)$):
$$\psi(x) \approx \frac{1}{\sqrt{|p(x)|}} \left[ C e^{\int^x |p(x')|\,dx'/\hbar} + D e^{-\int^x |p(x')|\,dx'/\hbar} \right]$$
where $$p(x) = \sqrt{2m(E - V(x))}$$ is the classical momentum.
#### Problem at Turning Points
The WKB approximation fails at classical turning points where $$E = V(x_0)$$ because $$p(x_0) = 0$$, causing the wavefunctions to diverge unphysically. The validity condition $$|\frac{d\lambda}{dx}| \ll 1$$ (where $$\lambda = \hbar/p$$ is the de Broglie wavelength) breaks down since $\lambda \to \infty$ at turning points.
#### Linear Approximation Near Turning Points
To solve this problem, we linearize the potential near the turning point $x_0$:
$$V(x) \approx E + V'(x_0)(x - x_0) = E + F_0(x - x_0)$$
where $F_0 = \left.\frac{dV}{dx}\right|_{x=x_0}$.

This transforms the Schrödinger equation to:
$$\frac{d^2\psi}{dx^2} + \frac{2mF_0}{\hbar^2}(x - x_0)\psi = 0$$
#### Airy Function Solution
By defining the scaled variable $$z = \alpha(x - x_0)$$ where $$\alpha = \left(\frac{2mF_0}{\hbar^2}\right)^{1/3}$$, the equation becomes Airy's equation:
$$\frac{d^2\psi}{dz^2} = z\psi$$

The general solution is:
$$\psi_p(z) = a\,\text{Ai}(z) + b\,\text{Bi}(z)$$

where Ai(z) and Bi(z) are Airy functions.
#### Asymptotic Forms of Airy Functions
The key to the connection formulas lies in the asymptotic behavior of Airy functions:
For $z \gg 0$:
$$\text{Ai}(z) \sim \frac{1}{2\sqrt{\pi}z^{1/4}} e^{-\frac{2}{3}z^{3/2}}$$
$$\text{Bi}(z) \sim \frac{1}{\sqrt{\pi}z^{1/4}} e^{\frac{2}{3}z^{3/2}}$$

For $z \ll 0$:
$$\text{Ai}(z) \sim \frac{1}{\sqrt{\pi}(-z)^{1/4}} \sin\left(\frac{2}{3}(-z)^{3/2} + \frac{\pi}{4}\right)$$
$$\text{Bi}(z) \sim \frac{1}{\sqrt{\pi}(-z)^{1/4}} \cos\left(\frac{2}{3}(-z)^{3/2} + \frac{\pi}{4}\right)$$
#### Patching Procedure
The patching wave function $$\psi_p(x) = a\,\text{Ai}(\alpha(x-x_0)) + b\,\text{Bi}(\alpha(x-x_0))$$ must be matched to the WKB solutions in overlap regions on either side of the turning point.
#### Classical Side ($x < x_0$)
In the classical region, we have:
$$\int^x p(x')\,dx' \approx \int^x \sqrt{-2mF_0(x'-x_0)}\,dx' = \frac{2}{3}\alpha^{-3/2}(-\alpha(x-x_0))^{3/2}$$
The WKB solution becomes:
$$\psi_{WKB}(x) = \frac{B}{\sqrt{p(x)}} e^{i\int^x p(x')\,dx'/\hbar} + \frac{C}{\sqrt{p(x)}} e^{-i\int^x p(x')\,dx'/\hbar}$$

#### Nonclassical Side ($x > x_0$)
In the nonclassical region:
$$\int^x |p(x')|\,dx' \approx \frac{2}{3}\alpha^{-3/2}(\alpha(x-x_0))^{3/2}$$
The WKB solution is:
$$\psi_{WKB}(x) = \frac{D}{\sqrt{|p(x)|}} e^{-\int^x |p(x')|\,dx'/\hbar}$$
#### Matching Asymptotic Forms
By matching the asymptotic forms of the Airy functions to the WKB solutions in the overlap regions, we obtain the connection relations:

If $b = 0$ (physically acceptable boundary condition), then:
- $$a = \frac{\sqrt{4\pi}}{\alpha^{1/2}\hbar^{1/2}} D$$- $$B = ie^{i\pi/4}D$$
- $$C = -ie^{-i\pi/4}D$$
#### Final Connection Formulas

The complete WKB connection formulas relating solutions across a turning point are:

**From nonclassical to classical region:**
$$\frac{1}{\sqrt{|p(x)|}} \exp\left(-\frac{1}{\hbar}\int_x^{x_0} |p(x')|\,dx'\right) \leftrightarrow \frac{2}{\sqrt{p(x)}} \sin\left(\frac{1}{\hbar}\int_{x_0}^x p(x')\,dx' + \frac{\pi}{4}\right)$$

**Growing exponential to oscillatory:**
$$\frac{1}{\sqrt{|p(x)|}} \exp\left(\frac{1}{\hbar}\int_x^{x_0} |p(x')|\,dx'\right) \leftrightarrow \frac{1}{\sqrt{p(x)}} \cos\left(\frac{1}{\hbar}\int_{x_0}^x p(x')\,dx' + \frac{\pi}{4}\right)$$

The characteristic $\pi/4$ phase shift arises naturally from the asymptotic behavior of the Airy functions and is crucial for proper quantization conditions in bound state problems.

These formulas allow seamless continuation of WKB solutions across turning points and form the foundation for calculating tunneling probabilities, bound state energies, and other semiclassical phenomena.
