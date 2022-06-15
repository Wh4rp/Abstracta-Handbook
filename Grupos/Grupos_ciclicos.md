# Grupos ciclicos
Las potencias de todo elemento $a$ de $G$ estan dentro del mismo. Esto es, $a$ multiplicado por si mismo $n$ veces, con $n$. 
Si $n$ es positvo, vamos a añadir la siguiente notacion 

$$
a^n = \underbrace{a \cdots a}_{n\text{ veces}}
$$

y analogamente

$$
a^{-n} = (a^{-1})^{n} = \underbrace{a^{-1} \cdots a^{-1}}_{n\text{ veces}}
$$

Con $n = 0$, diremos que $a^0 = e$.

Por otro lado, si $r$ y $s$ son enteros positivos entonces:

$$
a^{r} a^{s} = a^{r + s} = \underbrace{a \cdots a}_{r + s\text{ veces}}
$$

y analogamente

$$
a^{-r} a^{-s} = a^{-r - s} = \underbrace{a^{-1} \cdots a^{-1}}_{r + s\text{ veces}}
$$

Estas son las propiedades de las potencias que uno conoce de toda la vida pero definidas para _grupos_.

Pero, no necesariamente $(ab)^n = a^nb^n$. Es facil ver que sucede cuando $G$ es *abeliano*. 

:::{prf:definition} Orden de un elemento de un grupo
:label: orden-elemento-grupo

Diremos que el orden de un elemento $a$ de un grupo $G$ es el menor $n > 0$ tal que $a^n = e$. Si no existe tal $n$ entonces se dice que el orden de $a$ es _infinito_. 
:::

:::{prf:definition} Grupo ciclico
:label: grupo-ciclico

Un grupo $G$ se dice ciclico si existe un elemento $a$ tal que para todo $b$ en $G$ existe $n$ entero tal que $a^n = b$.

:::{note}
Este elemento $a$ se le llama el generador de $G$.
:::

:::
