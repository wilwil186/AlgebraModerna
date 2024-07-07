### Exer. 19 

Considere el anillo de matrices $M_2(\mathbb{Z}_2)$

- Encuentre el orden del anillo, es decir, el número de elementos en él. 
- Liste todas unidades unidades en el anillo. 

*Solución:*
-
- El orden del anillo es $2^4=16$, ya que cada entrada de una matriz en  $M_2(\mathbb{Z}_2)$ puede tomar los valores 0 o 1  
- Las unidades son las matrices \(I_2\), 
$\begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix}$
, $\begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}$, $\begin{bmatrix} 1 & 1 \\ 1 & 0 \end{bmatrix}$, $\begin{bmatrix} 0 & 1 \\ 0 & 1 \end{bmatrix}$, y $\begin{bmatrix} 1 & 0 \\ 1 & 1 \end{bmatrix}$.

Diagamos que tenemos una matriz 

$\begin{bmatrix} a & b\\  c & d\end{bmatrix} \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix}  = \begin{bmatrix} a * 1 + c * 0 & b * 1  + d *0  \\ a * 0 + c *1 & b * 0 + d * 1 \end{bmatrix} = \begin{bmatrix} a & b  \\ c & d\end{bmatrix}$, lo cual verifica que en efecto se cumple con la condición de que es sea unidad. 

Pero como logramos deducir que en efecto esas son las matrices. 

sea $\begin{bmatrix} a & b\\  c & d \end{bmatrix}$ y sea $\begin{bmatrix} x & y \\  z & w \end{bmatrix}$ una matrix identidad entonces: 

$\begin{bmatrix} a & b\\  c & d\end{bmatrix} \begin{bmatrix} x & y \\ z & w \end{bmatrix}  = \begin{bmatrix} a * x + c * y & b * x  + d * y  \\ a * z + c * w & b * z + d * w \end{bmatrix} = \begin{bmatrix} a & b  \\ c & d\end{bmatrix}$

eso quiere decir que 

- $a * x + c * y = a$  
- $b * x + d * y = b$
- $a * z + c * w = c$
- $b * z + d * w = d$

Esto nos da un total de 4 ecuaciones con 4 incognitas (x,y,z, w)

Podemos despejar x de la primera ecuación y obtenemos así: 

$x = \frac{a -(c * y)}{a} $ podemos remplazar este resultado en la ecuación 2. 

y luego despejar y

$$
\begin{aligned}
b * \frac{a -(c * y)}{a} + d * y &= b \\ 
b -(\frac{(b*c)}{a} + d)*y &= b \\ 
y &= \frac{b}{b -(\frac{(b*c)}{a} + d)}
\end{aligned}
$$

recordemos que a,b,c,d solo pueden tomar valores entre 0 o 1


