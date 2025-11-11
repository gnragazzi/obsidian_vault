$$g(n) = 
\begin{cases} 
1 & \text{si } n = 1 \\ 
1+g(floor(\frac{n}{2})) & \text{si } n > 1 
\end{cases}$$
Observamos que

$n>1$
$g(n)=1+g(floor(\frac{n}{2}))$
$g(n)=1+1+g(floor(\frac{floor(\frac{n}{2})}{2}))=g(n)=1+1+g(floor(\frac{n}{4}))$ por propiedad de función piso
$g(n)=1+1+1+ g(floor(\frac{n}{8}))$
(...)
$g(n)=i+ g(floor(\frac{n}{2^i}))$

$floor(x)=y⇔y≤x<y+1$

$floor(\frac{n}{2^i})=1 ⇔ 1\le \frac{n}{2^i}<1+1=2$

$1\le \frac{n}{2^i}<2$
$2^i\le n<2 . 2^i = 2^{i+1}$
$i\le lg(n)<i+1$

$floor(lg(n)) = i$ 

$g(n)=i+ g(floor(\frac{n}{2^i}))=floor(lg(n))+g(1)=floor(lg(n))+1$

$tcM(n)=\text{ [iteraciones de 1.1] } × \text{ [costo de cada iteración] }$
$tcM(n)= floor(lg(n))+1 × 2n = 2n . floor(lg(n))+ 2n$

$O(f)=\{g/g∈F∧(∃c∈ℝ⁺)(∃n_0∈ℕ_0)(∀n≥n_0):g(n)≤c.f(n)\}$

$floor(lg(n)) \le lg(n)$

$2n . floor(lg(n))+ 2n \le c . n . log(n)$
$2n . floor(lg(n))+ 2n \le 2n . lg(n)+ 2n\le c . n . log(n)$
$2 . lg(n)+ 2\le c . log(n)$
$2 . \frac{log(n)}{log(2)}+ 2\le c . log(n)$
$\frac{2}{log(2)}+ \frac{2}{log(n)}\le c$

$\frac{2}{log(2)}+ \frac{2}{log(n)}=2\frac{2}{log(2)}≈13.28\le c$

$tcM \le c . n . log(n) \Rightarrow tcM \in O(n . log(n))$








