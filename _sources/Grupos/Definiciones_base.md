# Conceptos base
Bajo la noción de grupo que se va a presentar en este libro se va a definir la operación binaria.
## Operaciones
:::{prf:definition} Operación binaria
:label: operacion-binaria

Una operación binaría $\star$ en un conjunto, es una regla que asigna a cada par ordenado de elementos de un conjunto, algún elemento del conjunto.
:::

Luego ya estamos listos para definir un _grupo_ como tal.

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
 se dice que el grupo $(G, \star)$ es **abeliano**. 
```


## Propiedades

:::{prf:property}
El elemento neutro es único
:::

:::{prf:property}
Dado $g \in G$ su inverso ($g^{-1}$) es único. 
:::

:::{prf:property}
$(a \star b)^{-1}=b^{-1} \star a^{-1}$
:::