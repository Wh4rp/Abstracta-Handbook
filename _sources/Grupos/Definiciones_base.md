# Definiciones base
Bajo nuestra noción de grupo vamos a primero presentar lo que es una operacion binaria.
## Prueba
```{prf:definition} Operación binaria
:label: operacion-binaria

Una operación binaría $\star$ en un conjunto, es una regla que asigna a cada par ordenado de elementos de un conjunto, algún elemento del conjunto.
```


Sea $G$ un conjunto no vacío y $\star : G \times G \to G$ una operación binaria se dice que $(G, \star)$ es _grupo_ si cumple con:
1. (**Asociatividad**) 
$\forall f,  g$, $h \in G$; $$f \star (g \star h) = (f \star g) \star h$$ 

2. (**Elemento neutro**) 
Existe un elemento $e \in G$ tal que 
$$
e \star g = g = g \star e, \forall g \in G$$

3. (**Elemento inverso**) 
$\forall g \in G$; $\exists h \in G$ tal que  
$$g \star h = e = h \star g$$ 

```{note}
Si la operación $\star$ conmuta se dice que el grupo $(G, \star)$ es abeliano. 
```


## Propiedades
1. El elemento neutro es único
2. Dado $g \in G$ su inverso ($g^{-1}$) es único. 
3. $(a \star b)^{-1}=b^{-1} \star a^{-1}$

```{prf:axiom} Completeness of $\mathbb{R}$
:label: my-axiom

Every Cauchy sequence on the real line is convergent.
```

````{prf:criterion} Weyl's criterion
:label: weyls-criterion

Weyl's criterion states that the sequence $a_n$ is equidistributed modulo $1$ if
and only if for all non-zero integers $m$,

```{math}
\lim_{n \rightarrow \infty} \frac{1}{n} \sum_{j=1}^{n} \exp^{2 \pi i m a_j} = 0
```
````

```{prf:conjecture} Fake $\gamma$ conjecture
:label: my-conjecture

This is a dummy conjecture to illustrate that one can use math in titles.
```