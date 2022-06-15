# Conceptos base

El concepto de ___grupo___ deviene de observar que hay propieades no triviales que son invariantes entre diversos conjuntos que poseen una operación asociada, por ejemplo los tanto en conjunto de las funciones biyectivas y el de las matrices se tiene que el inverso de $AB$ o $f \circ g$ es de la forma $B^{-1}A^{-1}$ o $g^{-1} \circ f^{-1}$ respectivamente. 

Lo interesante de esto es que dichos resultados no estan presenten por simple coincidencia sino que debido a que sus operaciones asociadas cumple con ciertos tres (o cuatro) axiomas principales. Y debido a esta _abstracción_ se derivan las demás propieades no triviales. 

## Operación binaria

Bajo la noción de grupo que se va a presentar en este libro primero se definirá la operación binaria. 

:::{prf:definition} Operación binaria
:label: operacion-binaria

Una operación binaria $\star$ bajo un conjunto no vacio $A$, es una función $\star : (A \times A) \to A$. Es decir, asigna a cada par ordenado de elementos de $A$, algún elemento de $A$.
:::

:::{note}
Se dice que $a \star b = c$ si y sólo si $\star(a, b) = c$ para $a, b, c \in A$. 
:::

De la forma en que está definido la operación binaria se pide que sea *cerrado*. Es decir, para cualquiera que sean los dos operandos, digamos $a$ y $b$ en $A$, el resultado de $a \star b$ siempre está dentro de $A$. 

Al decir "par ordenado" se infiere que $a \star b$ puede llegar a ser distinto que $b \star a$, es decir, el orden importa al momento de operar.


:::{prf:example}
Tomemos $\mathbb{Z}^+$ y la operación binaria $\star$ como $a \star b$ que es igual al mínimo entre $a$ y $b$ o el valor común si $a = b$. 

Así, $2 \star 11 = 2$; $15 \star 10 = 10$ y $3 \star 3 = 3$.
:::

## Grupo

Con la noción de operación binaria en mente, para definir un _grupo_ vamos a solicitar más condiciones para trabajar bajo una estructura que "se comporte de buena manera". Informalmente se dice que un grupo es un conjunto con operación que funciona _bien_. De tal manera que se comporta como uno está habituado a que funcionen conjuntos como los que elementalmente ve en el colegio; los enteros con la suma o reales con la multiplicación. 

::::{prf:definition} Grupo
:label: grupo

Sea $G$ un conjunto no vacío y $\star : G \times G \to G$ una operación binaria se dice que $(G, \star)$ es _grupo_ si satisface las siguientes tres propieades:
1. (**Asociatividad**) 
Para todo $f, g, h \in G$ se cumple que

$$
f \star (g \star h) = (f \star g) \star h
$$

2. (**Elemento neutro**) 
Existe un elemento $e \in G$ tal que

$$
e \star g = g = g \star e, \forall g \in G
$$

3. (**Elemento inverso**) 
Para todo $g \in G$, existe $h \in G$ tal que

$$
g \star h = e = h \star g
$$
::::

```{note}
Si la operación $\star$ conmuta, 
i.e. para todo $f, g \in G$ se tiene que $f \star g = g \star f$,
 se dice que $(G, \star)$ es **grupo abeliano**. 
```

Es común que muchas veces se obvie el operador en la notación $(G, \star)$ y tan sólo se escriba:

> Sea $G$ grupo $\ldots$

## Propiedades
A continuación se muestran algunas propiedades básicas que se desprenden de la definición de grupo $(G, \star)$, es recomendable para *soltar el lapiz* intentar demostrarlas antes de leer inmediatamente la demostración.

::::{prf:property}
El elemento neutro es único

:::{admonition} Demostración
:class: dropdown

Procedamos por contradicción y supongamos que existen dos $e_1$ y $e_2$ elementos neutros distintos. Pero podemos operar entos dos entre si de tal forma que 

$$
e_1 = e_1 \star e_2 = e_2
$$

llegamos a que $e_1 = e_2$ contradicción.

Por ende el elemento neutro es único.
:::

::::

::::{prf:property}
Dado $g \in G$ su inverso ($g^{-1}$) es único. 

:::{admonition} Demostración
:class: dropdown

Procedamos por contradicción. Sea $g \in G$ cualquiera, luego supongamos que existen dos $h_1, h_2 \in G$ tales que

$$
\begin{align*}
g \star h_1 = e = h_1 \star g \\
g \star h_2 = e = h_2 \star g \\
\end{align*}
$$

Luego notemos que

$$
h_1 \star g \star h_2 = (h_1 \star g) \star h_2 = e \star h_2 = h_2
$$

y por otro lado, dado que $\star$ es asociativo

$$
h_1 \star g \star h_2 = h_1 \star (g \star h_2) = h_1 \star e = h_1
$$

Entonces llegamos a que $h_1 = h_2$, contradicción. 

Por lo tanto dado $g \in G$ su inverso es único. 
:::

::::

::::{prf:property}
$(a \star b)^{-1}=b^{-1} \star a^{-1}$

:::{admonition} Demostración
:class: dropdown

Por definición basta probar que 

$$
(a \star b) \star (b^{-1} \star a^{-1}) = e = (b^{-1} \star a^{-1}) \star (a \star b)
$$

En efecto, utilizando la propiedad asociativa desallorramos como sigue

$$
\begin{align*}
(a \star b) \star (b^{-1} \star a^{-1}) & = a \star (b \star (b^{-1} \star a^{-1})) \\
& = a \star ((b \star b^{-1}) \star a^{-1}) \\
& = a \star (e \star a^{-1}) \\
& = a \star a^{-1} \\
& = e
\end{align*}
$$

Y análogamente para el otro lado

$$
\begin{align*}
(b^{-1} \star a^{-1}) \star (a \star b) & = b^{-1} \star (a^{-1} \star (a \star b)) \\
& = b^{-1} \star ((a^{-1} \star a) \star b) \\
& = b^{-1} \star (e \star b) \\
& = b^{-1} \star b \\
& = e
\end{align*}
$$

Que era lo que queríamos demostrar.
:::

::::