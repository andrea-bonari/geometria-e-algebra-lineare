### Invarianti metrici
>[!note]
>Data l'equazione di una conica, sia $A$ la sua matrice: $$A=\begin{pmatrix}A_{0}&q\\q^{T}&f\end{pmatrix}\qquad A_{0}=A_{0}^{T}\in\mathbb{R}^{2\times2}$$
>Gli invarianti metrici della conica sono:
>- Invariante cubico $I_{3}=\det(A)$
>- Invariante quadratico $I_{2}=\det(A_{0})=\lambda_{1}\cdot\lambda_{2}$
>- Invariante lineare $I_{1}=\text{tr}(A_{0})=\lambda_{1}+\lambda_{2}$
>
>Gli invarianti metrici rimangono invariati se si applica una rototraslazione alla conica.

### Coniche

- Coniche non degeneri $I_{3}\neq0$

| Condizione | Nome |
| ---- | ---- |
| $I_2>0\vee I_1I_3>0$ | Ellisse immaginaria |
| $I_2>0\vee I_1I_3<0$ | Ellisse |
| $I_2<0$ | Iperbole |
| $I_2=0$ | Parabola |

- Coniche degeneri $I_{3}=0$
 
| Condizione | Nome |
| ---- | ---- |
| $I_2>0$ | Ellisse degenere (un punto) |
| $I_2<0$ | Iperbole degenere (due rette incidenti) |
| $I_2=0\vee\text{rk}(A)=1$ | Retta doppia |
| $I_2=0\vee I_1f'<0$ | Rette parallele |
| $I_2=0\vee I_1f'>0$ | Rette immaginarie |
Nei casi degeneri con $I_{2}=0$ gli invarianti metrici non bastano: bisogna calcolare $f'$
$$f'=P(c_{0})\quad c_{0}=\text{centro}$$

### Quadriche

La classificazione dipende dalla segnatura della forma quadratica che ha la matrice $A_{0}$ come matrice di Gram:
$$q_{0}(X)=X^{T}A_{0}X$$
- Quadriche non degeneri $\det(A)\neq0$

| Nome | Segnatura $q_{0}$ | Condizione |
| ---- | ---- | ---- |
| Ellissoide immaginario | $(3,0)$ o $(0,3)$ | $\det(A)>0$ |
| Ellissoide | $(3,0)$ o $(0,3)$ | $\det(A)<0$ |
| Iperboloide iperbolico | $(2,1)$ o $(1,2)$ | $\det(A)>0$ |
| Iperboloide ellittico | $(2,1)$ o $(1,2)$ | $\det(A)<0$ |
| Paraboloide iperbolico |  | $\det(A)>0\vee \text{rk}(A_0)=2$ |
| Paraboloide ellittico |  | $\det(A)<0\vee \text{rk}(A_0)=2$ |

- Quadriche con $\text{rk}(A)=3$

| Nome | Segnatura $q_{0}$ | Condizione |
| ---- | ---- | ---- |
| Un punto (cono immaginario) | $(3,0)$ o $(0,3)$ |  |
| Cono | $(2,1)$ o $(1,2)$ |  |
| Cilindro immaginario | $(2,0)$ o $(0,2)$ | $\text{tr}(A_0)f'>0$ |
| Cilindro ellittico | $(2,0)$ o $(0,2)$ | $\text{tr}(A_0)f'<0$ |
| Cilindro iperbolico | $(1,1)$ |  |
| Cilindro parabolico | $(1,0)$ o $(0,1)$ |  |

- Quadriche con $\text{rk}(A)\leq 2$

| Nome | Segnatura $q_{0}$ | Condizione |
| ---- | ---- | ---- |
| Una retta (due piani immaginari incidenti) | $(2,0)$ o $(0,2)$ |  |
| Due piani incidenti | $(1,1)$ |  |
| Vuoto (due piani paralleli immaginari) | $(1,0)$ o $(0,1)$ | $\text{rk}(A)=2\vee \text{tr}(A_0)f'>0$ |
| Due piani paralleli | $(1,0)$ o $(0,1)$ | $\text{rk}(A)=2\vee \text{tr}(A_0)f'<0$ |
| Piano doppio | $(1,0)$ o $(0,1)$ | $\text{rk}(A)=1$ |

### Coniche nello spazio

Una conica nello spazio viene descritta come l'intersezione di una quadrica con un piano non contenuto nella quadrica. Per riconoscere affinemente la conica è sufficiente eliminare un parametro dall'equazione della quadrica usando l'equazione del piano e classificare affinemente l'equazione che si ottiene.