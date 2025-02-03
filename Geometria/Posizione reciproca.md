>[!note] Posizione piano-retta
>Sia il piano $\alpha$ e la retta $r$ definiti come: $$\alpha: ax+by+cz=d\qquad r:\begin{cases}a_{1}x+b_{1}y+c_{1}z=d_{1}\\a_{2}x+b_{2}y+c_{2}z=d_{2}\end{cases}$$
>L'intersezione del piano con la retta è data dalle soluzioni del sistema $$\begin{cases}ax+by+cz=d\\a_{1}x+b_{1}y+c_{1}z=d_{1}\\a_{2}x+b_{2}y+c_{2}z=d_{2}\end{cases}$$
>Allora la posizione reciproca del piano e della retta sarà:
>
>| $\text{rk}(A)$ | $\text{rk}(A,\overrightarrow{b})$ | Numero di soluzioni | risultato |
>| - | -| - | - |
>| 2 | 2 | $\infty^{1}$ | La retta sta sul piano |
>| 2 | 3 | nessuna | Piano e retta paralleli e distinti |
>| 3 | 3 | 1 | Piano e retta incidenti |

>[!note] Posizione retta-retta
>Date le rette $r,s$ nello spazio di equazione cartesiana $$r:\begin{cases}a_{1}x+b_{1}y+c_{1}z=d_{1}\\a_{2}x+b_{2}y+c_{2}z=d_{2}\end{cases}\qquad s:\begin{cases}a_{1}'x+b_{1}'y+c_{1}'z=d_{1}'\\a_{2}'x+b_{2}'y+c_{2}'z+d_{2}'\end{cases}$$
>Studiamo la loro intersezione: $$\begin{cases}a_{1}x+b_{1}y+c_{1}z=d_{1}\\a_{2}x+b_{2}y+c_{2}z=d_{2}\\a_{1}'x+b_{1}'y+c_{1}'z=d_{1}'\\a_{2}'x+b_{2}'y+c_{2}'z+d_{2}'\end{cases}$$
>Allora la posizione reciproca del piano e della retta sarà:
>
>| $\text{rk}(A)$ | $\text{rk}(A,\overrightarrow{b})$ | Numero di soluzioni | risultato |
>| - | -| - | - |
>| 2 | 2 | $\infty^{1}$ | Rette coincidenti |
>| 2 | 3 | nessuna | Rette parallele e distinte |
>| 3 | 3 | 1 | Rette incidenti |
>| 3 | 4 | nessuna | rette sghembe |

### Rette complanari e sghembe
>[!note]
>Due rette si dicono complanari se appartengono allo stesso piano (parallele o incidenti). Se due rette non sono complanari allora sono sghembe. Due rette sono complanari se e solo se $\text{rk}(A,\overrightarrow{b})<4$ quindi se e solo se $\det(A,b)=0$
>
>Se due rette $r,s$ in equazione parametrica: $$r:\begin{cases}x=x_{0}+tl\\y=y_{0}+tm\\z=z_{0}+tn\end{cases}\quad s:\begin{cases}x=x_{0}'+tl'\\y=y_{0}'+tm'\\z=z_{0}'+tn'\end{cases}$$
>Allora la condizione di complanarità è: $$\det\begin{pmatrix}x_{0}'-x_{0}&y_{0}'-y_{0}&z_{0}'-z_{0}\\l&m&n\\l'&m'&n'\end{pmatrix}=0$$

