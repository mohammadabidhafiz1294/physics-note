<img src="https://r2cdn.perplexity.ai/pplx-full-logo-primary-dark%402x.png" style="height:64px;margin-right:32px"/>

# Derivation of WKB Connection Formulas from Asymptotic Solutions

Starting from the basic WKB asymptotic wavefunctions and following a systematic patching procedure, I'll derive the connection formulas that relate solutions across classical turning points.

## Starting Point: WKB Asymptotic Solutions

The WKB method provides asymptotic solutions in different regions:

**Classical Region** ($E > V(x)$):
$\psi(x) \approx \frac{1}{\sqrt{p(x)}} \left[ A e^{i\int^x p(x')\,dx'/\hbar} + B e^{-i\int^x p(x')\,dx'/\hbar} \right]$

**Nonclassical Region** ($E < V(x)$):
$\psi(x) \approx \frac{1}{\sqrt{|p(x)|}} \left[ C e^{\int^x |p(x')|\,dx'/\hbar} + D e^{-\int^x |p(x')|\,dx'/\hbar} \right]$

where $p(x) = \sqrt{2m(E - V(x))}$ is the classical momentum.[^1][^2][^3]

## Problem at Turning Points

The WKB approximation fails at classical turning points where $E = V(x_0)$ because $p(x_0) = 0$, causing the wavefunctions to diverge unphysically. The validity condition $|\frac{d\lambda}{dx}| \ll 1$ (where $\lambda = \hbar/p$ is the de Broglie wavelength) breaks down since $\lambda \to \infty$ at turning points[^4][^5][^6].

## Linear Approximation Near Turning Points

To solve this problem, we linearize the potential near the turning point $x_0$:
$V(x) \approx E + V'(x_0)(x - x_0) = E + F_0(x - x_0)$

where $F_0 = \left.\frac{dV}{dx}\right|_{x=x_0}$[^1][^3][^7].

This transforms the Schrödinger equation to:
$\frac{d^2\psi}{dx^2} + \frac{2mF_0}{\hbar^2}(x - x_0)\psi = 0$

## Airy Function Solution

By defining the scaled variable $z = \alpha(x - x_0)$ where $\alpha = \left(\frac{2mF_0}{\hbar^2}\right)^{1/3}$, the equation becomes Airy's equation:
$\frac{d^2\psi}{dz^2} = z\psi$

The general solution is:
$\psi_p(z) = a\,\text{Ai}(z) + b\,\text{Bi}(z)$

where Ai(z) and Bi(z) are Airy functions.[^5][^6][^1]

## Asymptotic Forms of Airy Functions

The key to the connection formulas lies in the asymptotic behavior of Airy functions:[^4][^6]

For $z \gg 0$:
$\text{Ai}(z) \sim \frac{1}{2\sqrt{\pi}z^{1/4}} e^{-\frac{2}{3}z^{3/2}}$
$\text{Bi}(z) \sim \frac{1}{\sqrt{\pi}z^{1/4}} e^{\frac{2}{3}z^{3/2}}$

For $z \ll 0$:
$\text{Ai}(z) \sim \frac{1}{\sqrt{\pi}(-z)^{1/4}} \sin\left(\frac{2}{3}(-z)^{3/2} + \frac{\pi}{4}\right)$
$\text{Bi}(z) \sim \frac{1}{\sqrt{\pi}(-z)^{1/4}} \cos\left(\frac{2}{3}(-z)^{3/2} + \frac{\pi}{4}\right)$

## Patching Procedure

The patching wave function $\psi_p(x) = a\,\text{Ai}(\alpha(x-x_0)) + b\,\text{Bi}(\alpha(x-x_0))$ must be matched to the WKB solutions in overlap regions on either side of the turning point.[^6][^4][^5]

### Classical Side ($x < x_0$)

In the classical region, we have:
$\int^x p(x')\,dx' \approx \int^x \sqrt{-2mF_0(x'-x_0)}\,dx' = \frac{2}{3}\alpha^{-3/2}(-\alpha(x-x_0))^{3/2}$

The WKB solution becomes:
$\psi_{WKB}(x) = \frac{B}{\sqrt{p(x)}} e^{i\int^x p(x')\,dx'/\hbar} + \frac{C}{\sqrt{p(x)}} e^{-i\int^x p(x')\,dx'/\hbar}$

### Nonclassical Side ($x > x_0$)

In the nonclassical region:
$\int^x |p(x')|\,dx' \approx \frac{2}{3}\alpha^{-3/2}(\alpha(x-x_0))^{3/2}$

The WKB solution is:
$\psi_{WKB}(x) = \frac{D}{\sqrt{|p(x)|}} e^{-\int^x |p(x')|\,dx'/\hbar}$

## Matching Asymptotic Forms

By matching the asymptotic forms of the Airy functions to the WKB solutions in the overlap regions, we obtain the connection relations:[^4][^5][^6]

If $b = 0$ (physically acceptable boundary condition), then:

- $a = \frac{\sqrt{4\pi}}{\alpha^{1/2}\hbar^{1/2}} D$
- $B = ie^{i\pi/4}D$
- $C = -ie^{-i\pi/4}D$


## Final Connection Formulas

The complete WKB connection formulas relating solutions across a turning point are:[^2][^3][^1]

**From nonclassical to classical region:**
$\frac{1}{\sqrt{|p(x)|}} \exp\left(-\frac{1}{\hbar}\int_x^{x_0} |p(x')|\,dx'\right) \leftrightarrow \frac{2}{\sqrt{p(x)}} \sin\left(\frac{1}{\hbar}\int_{x_0}^x p(x')\,dx' + \frac{\pi}{4}\right)$

**Growing exponential to oscillatory:**
$\frac{1}{\sqrt{|p(x)|}} \exp\left(\frac{1}{\hbar}\int_x^{x_0} |p(x')|\,dx'\right) \leftrightarrow \frac{1}{\sqrt{p(x)}} \cos\left(\frac{1}{\hbar}\int_{x_0}^x p(x')\,dx' + \frac{\pi}{4}\right)$

The characteristic $\pi/4$ phase shift arises naturally from the asymptotic behavior of the Airy functions and is crucial for proper quantization conditions in bound state problems.

These formulas allow seamless continuation of WKB solutions across turning points and form the foundation for calculating tunneling probabilities, bound state energies, and other semiclassical phenomena.
<span style="display:none">[^10][^11][^12][^13][^14][^15][^16][^17][^18][^19][^20][^21][^22][^23][^24][^25][^8][^9]</span>

<div align="center">⁂</div>

[^1]: Quantum-Mechanics-Thankappan.pdf

[^2]: David-J.-Griffiths-Darrell-F.-Schroeter-Introduction-to-Quantum-Mechanics-Cambridge-University-P.pdf

[^3]: David-J.-Griffiths-Darrell-F.-Schroeter-Introduction-to-Quantum-Mechanics-Cambridge-University-P.pdf

[^4]: http://web.mit.edu/8.322/Spring 2007/notes/connection030507.pdf

[^5]: http://www.phys.ufl.edu/~kevin/teaching/6646/04spring/connection.pdf

[^6]: http://phys.iit.edu/~segre/phys406/21S/modules_09.pdf

[^7]: https://math.mit.edu/classes/18.305/WWW_2004_HungCheng/eleven.pdf

[^8]: A-Students-Guide-to-the-Schrodinger-Equation-Daniel-A.-Fleisch-Z-Library.pdf

[^9]: Quantum-Mechanics-Zettili.-pdf.pdf

[^10]: https://physicspages.com/pdf/Quantum mechanics/WKB approximation - turning points.pdf

[^11]: https://en.wikipedia.org/wiki/WKB_approximation

[^12]: https://www.reddit.com/r/AskPhysics/comments/jbt0wm/can_anyone_explain_the_wkb_method_patching_like/

[^13]: https://webhome.phy.duke.edu/~mehen/465/WKB_Connection.pdf

[^14]: https://www.youtube.com/watch?v=Lkugsh6bQWI

[^15]: https://www.classe.cornell.edu/~dlr/teaching/p443/wkb.pdf

[^16]: https://appquantmech.quantumtinkerer.tudelft.nl/wkb_connection/

[^17]: https://www.sciencedirect.com/science/article/abs/pii/S0022039624003711

[^18]: https://www.youtube.com/watch?v=xAVcVi6VWn0

[^19]: https://www.youtube.com/watch?v=57FzqyY-ZjU

[^20]: https://www.scribd.com/document/564306344/wkb

[^21]: https://phys.libretexts.org/Bookshelves/Quantum_Mechanics/Quantum_Mechanics_(Fowler)/08:_Approximate_Methods/8.03:_Note_on_the_WKB_Connection_Formula

[^22]: https://www.govinfo.gov/content/pkg/GOVPUB-C13-2735f63e0bbd35896a3f06459d624c02/pdf/GOVPUB-C13-2735f63e0bbd35896a3f06459d624c02.pdf

[^23]: https://userswww.pd.infn.it/~zwirner/WKB-3.pdf

[^24]: https://webusers.imj-prg.fr/~frederic.klopp/papiers/Airy-difference-eq.pdf

[^25]: https://faculty.washington.edu/seattle/physics541/14text.pdf

