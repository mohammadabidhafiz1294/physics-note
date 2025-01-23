***Q:*** Find the secret string s if 

    f(00)=0  
    f(01)=1  
    f(10)=1  
    f(11)=0.

Write your answer directly without any quotation mark etc. Ex: 00

*Solutions*:
	To find the secret string \( s \) in the context of the Bernstein-Vazirani algorithm, we need to understand that \( f(x) \) is given by:

$f(x) = s \cdot x \mod 2$

where \( s \) is the secret \( n \)-bit string, and $\cdot$ denotes the bitwise dot product.

Given the function values:

- \( f(00) = 0 \)
- \( f(01) = 1 \)
- \( f(10) = 1 \)
- \( f(11) = 0 \)

We can set up equations to determine \( s \). Let's denote the bits of \( s \) as \( s = $s_1s_0$ \).

1. For \( x = 00 \):
   $$f(00) = s_1 \cdot 0 + s_0 \cdot 0 = 0$$ 
   This equation doesn't give any information about \( $s_1$ \) and \( $s_0$ \).

2. For \( x = 01 \):
    $$f(01) = s_1 \cdot 0 + s_0 \cdot 1 = s_0 \equiv 1 \mod 2$$
   Thus, \( $s_0$ = 1 \).

3. For \( x = 10 \):
   $$f(10) = s_1 \cdot 1 + s_0 \cdot 0 = s_1 \equiv 1 \mod 2$$
   Thus, \( $s_1$ = 1 \).

4. For \( x = 11 \):
	$$f(11) = s_1 \cdot 1 + s_0 \cdot 1 = s_1 + s_0 \equiv 0 \mod 2$$ 
   Given that \( $s_0$ = 1 \) and \( $s_1$ = 1 \), we have:
   \[ 1 + 1 \equiv 0 \mod 2 \]
   This equation is satisfied and consistent with \( $s_0$ = 1 \) and \( $s_1$ = 1 \).

Hence, the secret string \( s \) is \( $11$ \).

The secret string \( s \) is:

\[ $s = 11$ \]

This matches the given function values for ( $f(x)$).

***Q*** : 
Let $n$,. Suppose that the quantum state
$$\frac{1}{2^n} \sum_{x \in \{0, 1\}^n} \sum_{z \in \{0, 1\}^n} (-1)^{x \cdot z + f(x)} |z\rangle$$
is measured, where $\ket{z}$ is a two-qubit state. Which state is observed if $f(x) = 0$ for all $X$ ?

**Solutions**: 
The given quantum state can be interpreted and simplified step by step. Let's denote \( n \) as the number of qubits, and let's analyze the state and the conditions provided.

The state is given by:

$$\frac{1}{2^n} \sum_{x \in \{0, 1\}^n} \sum_{z \in \{0, 1\}^n} (-1)^{x \cdot z + f(x)} |z\rangle$$

Where \( f(x) = 0 \) for all \( x \). Thus, the expression simplifies to:

$$\frac{1}{2^n} \sum_{x \in \{0, 1\}^n} \sum_{z \in \{0, 1\}^n} (-1)^{x \cdot z} |z\rangle$$

Here, \($x \cdot z$ \) denotes the bitwise dot product (also known as the inner product) of the binary vectors \( x \) and \( z \).

### Simplifying the Sum

To understand which state is observed upon measurement, let's look at the coefficients of \( $|z\rangle$\) in the superposition. The key term is (-$1)^{x \cdot z}$, which determines the phase.

#### Orthogonality Consideration

To compute the sum $\sum_{x \in \{0, 1\}^n} (-1)^{x \cdot z}$, we use the fact that this sum is zero unless \( z = 0 \):

- When \( z = 0 \), \( $x \cdot z = 0$ \) for all \( x \), so the sum over all \( x \) is simply \( 2^n \).
- When \($z \neq 0$ \), the sum $$\sum_{x \in \{0, 1\}^n} (-1)^{x \cdot z} = 0$$ due to the orthogonality of the basis states in the Hadamard transform.

Thus, the sum simplifies to:

$$\frac{1}{2^n} \sum_{z \in \{0, 1\}^n} \left( \sum_{x \in \{0, 1\}^n} (-1)^{x \cdot z} \right) |z\rangle$$

Since $$\sum_{x \in \{0, 1\}^n} (-1)^{x \cdot z}$$  is zero for any \( $z \neq 0$ \), only \( z = 0 \) contributes to the sum:

$$\frac{1}{2^n} \cdot 2^n |0\rangle = |0\rangle$$
When the given quantum state is measured, and given \( $f(x) = 0$ \) for all \( x \), the observed state will be \( $|0\rangle$ \), which in a two-qubit system (where \( n = 2 \)), corresponds to the state \( $|00\rangle$ \).

Thus, the state observed upon measurement is ( $|00\rangle$).