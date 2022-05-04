# Ejemplos de grupos
En está sección se mostrarán ejemplos de grupos para aterrizar más la definición del mismo concepto de _grupo_. 
## Si son grupos

:::{prf:example}

$(\mathbb{Z},+)$ es un _grupo_, donde $+$ es la suma de toda la vida en los enteros. 

- Elemento neutro: $0$
- Inverso de $n \in \mathbb{Z}$: $-n$
- Asociatividad: ✔

:::

:::{prf:example}

Sea $\mathrm{m}$ un número positivo mayor que $1$, luego podemos definir la relación de equivalencia $\equiv_\mathrm{m}$ como $a \equiv_\mathrm{m} b$ si y sólo si $\mathrm{m} \mid a - b$ con $a, b \in \mathbb{Z}$. Luego podemos definir el conjunto $\mathbb{Z} / \mathrm{m}$ compuesto por las marcas de clase de $\equiv_\mathrm{m}$, es decir, $\mathbb{Z} / \mathrm{m} = \{ [0]_\mathrm{m}, [1]_\mathrm{m}, \ldots, [\mathrm{m} - 1]_\mathrm{m}\}$. 

Definimos la operación $+_\mathrm{m}$ como $[a]_\mathrm{m} +_\mathrm{m} [b]_\mathrm{m} = [c]_\mathrm{m}$ donde $\mathrm{m} \mid (a + b) - c$. 

$(\mathbb{Z} / \mathrm{m}$, $+_\mathrm{m})$ es un _grupo_.
- Elemento neutro: $[0]_\mathrm{m}$
- Inverso de $[n]_\mathrm{m} \in \mathbb{Z} / \mathrm{m}$: $[-n]_\mathrm{m}$
- Asociatividad: ✔

:::

:::{prf:example}

Definimos $\mathbb{Q}^{\times}=\mathbb{Q} \, \backslash \, \{0 \}$ y $\cdot$ la multiplicación de racionales.

$(\mathbb{Q}^{\times}, \cdot)$ es _grupo_.

- Elemento neutro: $\frac{1}{1}$
- Inverso de $\frac{a}{b} \in \mathbb{Q}^{\times}$: $\frac{b}{a}$
- Asociatividad: ✔

:::


## Son grupos (abelianos)

:::{prf:example}

Sea $V$ espacio vectorial y $+$ la suma definida dentro del espacio vectorial. $(V,+)$ es _grupo abeliano_. Esto se tiene por definición de espacio vectorial.
:::

:::{prf:example}

$(\mathbb{N},+)$ es _grupo abeliano_.
:::

## No son grupos

:::{prf:example}

$$
G=G L_{2}(\mathbb{C})=\left\{\left(\begin{array}{l}
2 b \\
c d
\end{array}\right): 2, b, c, d \in \mathbb{C}, \operatorname{det} \neq 0\right\}
$$

con $\star=$ multiplicación de matrices.
:::

## Es un grupo no abeliano
$G=\mathbb{Z} / 2 \mathbb{Z} \times \mathbb{Z} / 3 \mathbb{Z}$ con $\star$ suma coordenada a coordenada es un grupo abeliano. 

$$
D_{3}=\{I d, R, R \cdot R, S, S \cdot R, S \cdot R \cdot R\}
$$

Las simetrías del $\Delta$ con la operación "0" (composición de simetrías) es un grupo.

En un polígono regular de $n$ vértices:
$D_n$ es el prupo de las simetrías y también se obtiene con rotación $(R)$, reflexión $(S)$ y $\star$ composición de estas. 

### Grupo diedral
Dado un conjunto de $n$ elementos usualmente : $X=\{1,2, \ldots, n\}$. Tenemos las biyecciones $\varphi: X \longrightarrow X$ (o permutaciones). Luego: $G=\{$ biyecciones $X \rightarrow X\}$ es un prupo con la operación dado por la composición. Se denota $S_{n}$ (Grupo Simétrico).