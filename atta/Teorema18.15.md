El **Teorema 18.15** establece que **todo dominio de ideales principales (DIP) es un dominio de factorización única (DFU)**. Vamos a demostrarlo paso a paso y de manera detallada.

---

## **Demostración del Teorema 18.15**: Todo DIP es un DFU

La demostración se divide en dos partes:
1. **Existencia de la factorización**: Todo elemento distinto de cero y que no sea una unidad puede escribirse como un producto de elementos irreducibles.
2. **Unicidad de la factorización**: Si un elemento tiene dos factorizaciones en irreducibles, estas son esencialmente la misma salvo el orden y la multiplicación por unidades.

---

### **Paso 1: Existencia de la factoración**
#### **1.1 Caso base: irreducibles**
Sea \( D \) un dominio de ideales principales (DIP) y sea \( a \) un elemento distinto de cero que no sea una unidad. Si \( a \) es irreducible, entonces ya hemos terminado, pues no necesita más factorización.

#### **1.2 Caso general: no irreducible**
Si \( a \) no es irreducible, significa que puede factorizarse como:
\[
a = a_1 b_1
\]
donde \( a_1 \) y \( b_1 \) no son unidades.

Como \( D \) es un **dominio de ideales principales**, los ideales generados por estos elementos cumplen la propiedad de contenerse unos dentro de otros:

\[
\langle a \rangle \subset \langle a_1 \rangle
\]

> "Esto implica que \( \langle a \rangle \neq \langle a_1 \rangle \), pues si fueran iguales, existiría una unidad \( u \) tal que \( a = u a_1 \), lo que significaría que \( b_1 \) es una unidad, contradiciendo la suposición de que \( b_1 \) no es una unidad."

#### **1.3 Continuación del proceso**
Aplicamos el mismo argumento a \( a_1 \) y \( b_1 \) si no son irreducibles:

\[
a_1 = a_2 b_2
\]

\[
\langle a_1 \rangle \subset \langle a_2 \rangle
\]

Podemos continuar este proceso, generando una **cadena ascendente de ideales**:

\[
\langle a \rangle \subset \langle a_1 \rangle \subset \langle a_2 \rangle \subset \dots
\]

#### **1.4 Aplicación de la condición de cadenas ascendentes (CCA)**
En un DIP, la condición de cadenas ascendentes (CCA) se cumple (esto es una propiedad de los anillos de ideales principales), lo que significa que existe un entero \( N \) tal que:

\[
\langle a_N \rangle = \langle a_{N+1} \rangle = \dots
\]

En otras palabras, el proceso de factorización debe detenerse en un número finito de pasos, lo que implica que en algún punto obtenemos una factorización en elementos irreducibles:

\[
a = p_1 p_2 \dots p_r
\]

con cada \( p_i \) irreducible. **Esto prueba la existencia de la factorización.**

---

### **Paso 2: Unicidad de la factoración**
Supongamos que \( a \) tiene dos factorizaciones en irreducibles:

\[
a = p_1 p_2 \dots p_r = q_1 q_2 \dots q_s
\]

donde todos los \( p_i \) y \( q_j \) son irreducibles.

#### **2.1 Aplicación del Corolario 18.13**
Por el **Corolario 18.13**, en un DIP, **todo irreducible es primo**. Esto implica que cada \( p_i \) debe dividir a uno de los \( q_j \). Como \( p_1 \) divide al producto \( q_1 q_2 \dots q_s \), por la definición de número primo, debe dividir a algún \( q_j \), digamos \( q_1 \). En consecuencia, existe una unidad \( u_1 \) tal que:
\[
q_1 = u_1 p_1
\]

Reordenando, tenemos:

\[
a = p_1 p_2 \dots p_r = u_1 p_1 q_2 \dots q_s
\]

Cancelamos \( p_1 \) de ambos lados:

\[
p_2 \dots p_r = u_1 q_2 \dots q_s
\]

#### **2.2 Continuación del argumento**
Repetimos este argumento con \( p_2 \), luego con \( p_3 \), y así sucesivamente, hasta que obtenemos:

\[
p_1 p_2 \dots p_r = u_1 u_2 \dots u_r q_1 q_2 \dots q_s
\]

Dado que los \( p_i \) y \( q_j \) son irreducibles, la única posibilidad es que \( r = s \) y que los factores sean los mismos salvo por una reordenación y multiplicación por unidades.

Esto demuestra la **unicidad de la factorización**.

---

### **Conclusión**
Dado que hemos demostrado que **cada elemento puede factorizarse en irreducibles y que esta factorización es única**, concluimos que **todo dominio de ideales principales (DIP) es un dominio de factorización única (DFU)**.

✦ **Q.E.D.** ✦

---


