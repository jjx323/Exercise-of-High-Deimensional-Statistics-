```markdown
Exercise 3.10 

(a) $(\Rightarrow)$  

$$
\begin{align*} 
\left[ \text{vol}(A + B) \right]^{\frac{1}{n}}&=\left[ \text{vol}\left( \text{vol}(A)\frac{A}{\text{vol}(A)} + \text{vol}(B)\frac{B}{\text{vol}(B)} \right) \right]^{\frac{1}{n}} \\ 
&=\left[ \text{vol}\left( \frac{\text{vol}(A)}{\text{vol}(A) + \text{vol}(B)} \cdot \frac{A}{\text{vol}(A)} + \frac{\text{vol}(B)}{\text{vol}(A) + \text{vol}(B)} \cdot \frac{B}{\text{vol}(B)} \right) \right]^{\frac{1}{n}} \\ 
&\geq \left[ \frac{\text{vol}(A)}{\text{vol}(A) + \text{vol}(B)} \cdot \left( \frac{\text{vol}(A)}{\text{vol}(A)^n} \right)^{\frac{1}{n}} + \frac{\text{vol}(B)}{\text{vol}(A) + \text{vol}(B)} \cdot \left( \frac{\text{vol}(B)}{\text{vol}(B)^n} \right)^{\frac{1}{n}} \right]^{\frac{1}{n}} \\ 
&= \text{vol}(A)^{\frac{1}{n}} + \text{vol}(B)^{\frac{1}{n}} 
\end{align*}
$$  

$(\Leftarrow)$  

$$
\begin{align*} 
\text{vol}(\lambda C + (1 - \lambda)D)^{\frac{1}{n}} &\geq \left[ \text{vol}(\lambda C) \right]^{\frac{1}{n}} + \left[ \text{vol}((1 - \lambda)D) \right]^{\frac{1}{n}} \\ 
&= \lambda \left[ \text{vol}(C) \right]^{\frac{1}{n}} + (1 - \lambda) \left[ \text{vol}(D) \right]^{\frac{1}{n}} 
\end{align*}
$$  


(b) Condition:  

$$
\text{vol}(\lambda C + (1 - \lambda)D)^{\frac{1}{n}} \geq \lambda \left[ \text{vol}(C) \right]^{\frac{1}{n}} + (1 - \lambda) \left[ \text{vol}(D) \right]^{\frac{1}{n}} 
$$  

$$
\begin{align*} 
\Rightarrow \text{vol}(\lambda C + (1 - \lambda)D) &\geq \left( \lambda \left[ \text{vol}(C) \right]^{\frac{1}{n}} + (1 - \lambda) \left[ \text{vol}(D) \right]^{\frac{1}{n}} \right)^n \\ 
&\geq 2^{1 - n} \left( \lambda^n \text{vol}(C) + (1 - \lambda)^n \text{vol}(D) \right) \\ 
&= \frac{\lambda^n}{2} \text{vol}(C) + \frac{(1 - \lambda)^n}{2} \text{vol}(D) 
\end{align*}
$$  


$$
\text{vol}(C)^\lambda \text{vol}(D)^{1 - \lambda} \leq \varepsilon \cdot \text{vol}(C) + C(\varepsilon) \cdot \text{vol}(D) 
$$  

where $C(\varepsilon) = \left( \frac{\lambda}{\varepsilon} \right)^{\frac{\lambda}{1 - \lambda}} (1 - \lambda)$ （Young's inequality with $\varepsilon$） 

We need.  

$$
\frac{(2\lambda)^n}{2} \geq \varepsilon \quad \frac{(2(1 - \lambda))^n}{2} \geq (1 - \lambda) \left( \frac{\lambda}{\varepsilon} \right)^{\frac{2}{1 - \lambda}}
$$  

$$
\Downarrow 
$$  

$$
\varepsilon \geq \frac{\lambda}{(2^n)^{\frac{1 - \lambda}{\lambda}} (1 - \lambda)^{\frac{(n - 1)(1 - \lambda)}{\lambda}}}
$$  


That is to say.  

$$
\frac{(2\lambda)^n}{2} \geq \frac{\lambda}{(2^n)^{\frac{1 - \lambda}{\lambda}} (1 - \lambda)^{\frac{(n - 1)(1 - \lambda)}{\lambda}}}
$$  

needs to be true  


By simple calculation.  

$$
\log 2 \geq \lambda \log \frac{1}{\lambda} + (1 - \lambda) \log \frac{1}{1 - \lambda}
$$  

(take maximum value at $\lambda = \frac{1}{2}$)  

$$
\frac{1}{2} \log \frac{1}{\frac{1}{2}} + \frac{1}{2} \log \frac{1}{\frac{1}{2}} = \log 2
$$  


$$
\Rightarrow \text{vol}(C)^\lambda \text{vol}(D)^{1 - \lambda} \leq \text{vol}(\lambda C + (1 - \lambda)D)
$$  


(c). Condition:  

$$
\text{vol}(\lambda C + (1 - \lambda)D) \geq [\text{vol}(C)]^\lambda [\text{vol}(D)]^{1 - \lambda}
$$  

$$
\Rightarrow \text{vol}\left( \lambda \frac{C}{\text{vol}(C)^{\frac{1}{n}}} + (1 - \lambda) \frac{D}{\text{vol}(D)^{\frac{1}{n}}} \right) \geq 1
$$  
$$
\begin{align*}
&\text{vol}\left( \lambda C + (1 - \lambda) D \right)^{\frac{1}{n}} \\
&= \text{vol}\left( \frac{ \text{vol}(\lambda C)^{\frac{1}{n}} }{ \text{vol}(\lambda C)^{\frac{1}{n}} + \text{vol}\left( (1 - \lambda) D \right)^{\frac{1}{n}} } \cdot \frac{ \lambda C }{ \text{vol}(\lambda C)^{\frac{1}{n}} } + \frac{ \text{vol}\left( (1 - \lambda) D \right)^{\frac{1}{n}} }{ \text{vol}(\lambda C)^{\frac{1}{n}} + \text{vol}\left( (1 - \lambda) D \right)^{\frac{1}{n}} } \cdot \frac{ (1 - \lambda) D }{ \text{vol}\left( (1 - \lambda) D \right)^{\frac{1}{n}} } \right) \\
&\geq \frac{1}{ \left[ \text{vol}(\lambda C)^{\frac{1}{n}} + \text{vol}\left( (1 - \lambda) D \right)^{\frac{1}{n}} \right]^n } \cdot \left[ \text{vol}(\lambda C)^{\frac{1}{n}} + \text{vol}\left( (1 - \lambda) D \right)^{\frac{1}{n}} \right]^n \\
&\geq \left[ \text{vol}(\lambda C) \right]^{\frac{1}{n}} + \left[ \text{vol}\left( (1 - \lambda) D \right) \right]^{\frac{1}{n}} \\
&= \lambda \left[ \text{vol}(C) \right]^{\frac{1}{n}} + (1 - \lambda) \left[ \text{vol}(D) \right]^{\frac{1}{n}}
\end{align*}
$$
```
