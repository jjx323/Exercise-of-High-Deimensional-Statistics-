## Exercise 3.10.

**(a)** $(\Rightarrow)$

$$
\begin{align*}
\left\[ \text{vol}(A+B) \right\]^{1/n} & = \left\[ \text{vol}\left( \text{vol}(A)\frac{A}{\text{vol}(A)} + \text{vol}(B)\frac{B}{\text{vol}(B)} \right) \right\]^{1/n} \\
& = (\text{vol}(A) + \text{vol}(B))\left\[ \text{vol}\left( \frac{\text{vol}(A)}{\text{vol}(A) + \text{vol}(B)}\frac{A}{\text{vol}(A)} + \frac{\text{vol}(B)}{\text{vol}(A) + \text{vol}(B)}\frac{B}{\text{vol}(B)} \right) \right\]^{1/n} \\
& \geq (\text{vol}(A) + \text{vol}(B)) \left( \frac{\text{vol}(A)}{\text{vol}(A) + \text{vol}(B)} \left( \frac{A}{\text{vol}(A)^n} \right)^{1/n}  + \frac{\text{vol}(B)}{\text{vol}(A) + \text{vol}(B)} \left( \frac{B}{\text{vol}(B)^n} \right)^{1/n}  \right) \\
& = \text{vol}(A)^{1/n} + \text{vol}(B)^{1/n}. 
\end{align*}
$$

$(\Leftarrow)$

$$
\begin{align*}
\text(vol)(\lambda C + (1-\lambda)D)^{1/n} & \geq \text{vol}(\lambda C)^{1/n} + \text{vol}((1-\lambda)D)^{1/n} \\ 
& = \lambda \text(vol)(C)^{1/n} + (1-\lambda) \text{vol}(D)^{1/n} 
\end{align*}
$$

**(b)**. 
