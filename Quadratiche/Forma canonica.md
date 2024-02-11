Ogni quadrica può essere spostata con una rototraslazione in una particolare forma detta forma canonica della quadrica.

### Matrice di una quadrica
>[!note]
>All'equazione di una quadrica $$p(x_{1},\cdots,x_{n})=0\text{ con }p(x_{1},\cdots,x_{n})=\sum\limits_{i\leq j}a_{ij}x_{i}x_{j}+\sum\limits b_{i}x_{i}+f$$si associa la matrice: $$A=\begin{pmatrix}A_{0}&q\\q^{T}&f\end{pmatrix}$$dove $A_{0}$ è la matrice di Gram di $\sum\limits a_{ij}x_{i}x_{j}$ e quindi $$(A_{0})_{ii}=a_{ii}\quad (A_{0})_{ij}= \frac{a_{ij}}{2}\quad q_{i}=\frac{b_{i}}{2}$$
>L'equazione si può scrivere come $$\begin{pmatrix}X^{T}&1\end{pmatrix}A\begin{pmatrix}X\\1\end{pmatrix}\qquad X=\begin{pmatrix}x_{1}\\\vdots\\x_{n}\end{pmatrix}$$
>Si omogeneizza il polinomio: $$Q(x_{1},x_{2},\cdots,x_{n},x_{n+1})=\sum\limits_{i\leq j}a_{ij}x_{i}x_{j}+\sum\limits b_{i}x_{i}x_{n+1}+fx^{2}_{n+1}$$
>$Q$ è quindi una forma quadratica in $\mathbb{R}^{n+1}$

### Equazione della rototraslazione di una quadrica
>[!note]
>Se $Q$ è una quadrica di equazione $p(X)=0$ e $R$ è una rototraslazione, allora la quadrica $R(Q)$ ha equazione: $$p(R^{-1}(X))=0$$
>
>Sia $Q$ una quadrica, $R$ una rototraslazione e $A$ la matrice di $Q$. $$Q=\begin{pmatrix}A_{0}&q\\q^{T}&f\end{pmatrix}\qquad M=\begin{pmatrix}M_{0}&v\\\overrightarrow{0}&1\end{pmatrix}$$
>Allora la matrice di $R(Q)$ è $$(M^{-1})^{T}AM^{-1}$$

### Calcolo della forma canonica
Il metodo consiste nel modificare l'equazione della quadrica in due passaggi moltiplicandola per un fattore $k$ non nullo oppure effettuando una rototraslazione. In genere si applicano due procedimenti:
- Diagonalizzazione
- Eliminazione dei termini lineari

Data l'equazione della quadrica
$$p(x_{1},\cdots,x_{n})=0\text{ con }p(x_{1},\cdots,x_{n})=\sum\limits_{i\leq j}a_{ij}x_{i}x_{j}+\sum\limits b_{i}x_{i}+f$$
Allora
- La diagonalizzazione consiste nella diagonalizzazione della matrice $A_{0}$ e l'effetto è quello di eliminare i termini $a_{ij}x_{i}x_{j}$ con $i\neq j$ dall'equazione.
- L'eliminazione dei termini lineari consiste in una traslazione e l'effetto è quello di eliminare dall'equazione termini del tipo $b_{i}x_{i}$.
- La forma canonica è quella che si ottiene eliminando tutti i termini $a_{ij}x_{i}x_{j}$ con $i\neq j$ e il maggior numero possibile di termini lineari.

##### Eliminazione dei termini lineari
Effettuiamo la traslazione che manda il centro $c_{0}$ nell'origine degli assi
$$\begin{pmatrix}T_{-c_{0}}(X)\\1\end{pmatrix}$$
La matrice dell'equazione diventa$$A'=\begin{pmatrix}A_{0}&0\\0&f'\end{pmatrix}$$
L'equazione della quadrica traslata è $$p'(X)=X^{T}A_{0}X+f'=0
$$
Se vogliamo calcolare solo $f'$:
- Se $\det(A_{0})\neq0$
$$f'=\frac{\det(A')}{\det(A_{0})}$$
- Se $\det(A_{0})=0$
$$f'=p'(0)=p(T_{c_{0}}(0))=p(c_{0})$$

##### Diagonalizzazione
Siccome $A_{0}$ è una matrice simmetrica sappiamo che $A_{0}$ ammette una matrice modale $M_{0}$ ortogonale, abbiamo dunque che $$M_{0}^{T}A_{0}M_{0}=M_{0}^{-1}A_{0}M_{0}=\begin{pmatrix}\lambda_{1}&0&\cdots&0\\0&\lambda_{2}&\cdots&0\\\vdots&\vdots&\ddots&\vdots\\0&0&\cdots&\lambda_{n}\end{pmatrix}$$
Si effettua l'isometria lineare $$\begin{pmatrix}R(X)\\1\end{pmatrix}=\begin{pmatrix}M_{0}^{-1}&0\\0&1\end{pmatrix}\begin{pmatrix}X\\1\end{pmatrix}$$
$$A''=\begin{pmatrix}X^{T}&1\end{pmatrix}\begin{pmatrix}\lambda_{1}&0&\cdots&0\\0&\lambda_{2}&\cdots&0\\\vdots&\vdots&\ddots&\vdots\\0&0&\cdots&\lambda_{n}\end{pmatrix}\begin{pmatrix}X\\1\end{pmatrix}$$
che corrisponde all'equazione $$\sum\limits\lambda_{i}X_{i}^{2}+f'=0$$
### Quadriche con centro di simmetria
>[!note]
>Sia $A=\begin{pmatrix}A_{0}&q\\q^{T}&f\end{pmatrix}$ la matrice di una quadrica $Q$. Una quadrica con centro di simmetria è una quadrica tale che esiste una soluzione $c_{0}$ di $$A_{0}X+q=\overrightarrow{0}$$
>E il punto $c_{0}$ è un centro di simmetria della quadrica.
>
>Siano quindi $\lambda_{1},\cdots,\lambda_{r}$ gli autovalori positivi, e $\mu_{1},\cdots,\mu_{s}$ gli autovalori negativi. Negando gli autovalori negativi l'equazione diventa $$\sum\limits_{i=1}^{r}\lambda_{i}x^{2}_{i}-\sum\limits_{i=1}^{s}-\mu_{i}x_{i}^{2}=-f'\qquad \lambda_{i}>0,-\mu_{i}>0$$
>
>Questa equazione è detta forma canonica della quadrica con centro di simmetria

### Quadriche senza centro di simmetria
>[!note]
>Se $A_0X+q$ non ha soluzione, si decompone $q$ rispetto a $R(A)$ (decomposizione ortogonale) $$\mathbb{R}^{n}=R(A_{0})\oplus R(A_{0})^{\perp}=R(A_{0})\oplus N(A_{0}^{T})=R(A_{0})\oplus N(A_{0})$$
>Siccome la matrice è simmetrica, allora $A^{T}=A$ e quindi $N(A_0)=N(A_0^T)$. La decomposizione ortogonale del vettore $q$ è $$q=q_{0}+q_{1}\text{ con }q_{0}\in N(A_{0}),q_{1}\in R(A_{0})$$
>
>Se $c_{0}$ è una soluzione di $A_{0}X+q_{1}=\overrightarrow{0}$, allora si trasla $c_{0}$ nell'origine e la matrice traslata diventa: $$\begin{pmatrix}A_{0}&q_{0}\\q_{0}^{T}&f'\end{pmatrix}$$
>Si calcola una matrice modale ortogonale $M_{0}$ di $A_{0}$ e si trasforma la quadrica con l'isometria lineare $R(X)=M_{0}^{T}$. La matrice si trasforma in $$\begin{pmatrix}\lambda_{1}&0&\cdots&0&b'_{1}\\0&\lambda_{2}&\cdots&0&b'_{2}\\\vdots&\vdots&\ddots&\vdots&\vdots\\0&0&\cdots&\lambda_{n}&b'_{n}\\b'_{1}&b'_{2}&\cdots&b'_{n}&f'\end{pmatrix}$$
###  Teorema della rototraslazione delle quadriche
>[!note]
>Ogni quadrica può essere portata con una rototraslazione in una quadrica con equazione in una delle tre seguenti forme:
>- Se $\text{rk}(A)=\text{rk}(A_{0})$: $$\sum\limits_{i=1}^{r}\lambda_{i}x_{i}^{2}-\sum\limits_{i=1}^{s}\mu_{i}x_{i+r}^{2}=0\qquad \lambda_{i}>0,\mu_{i}>0$$
>- Se $\text{rk}(A)=\text{rk}(A_{0})+1$: $$\sum\limits_{i=1}^{r}\lambda_{i}x_{i}^{2}-\sum\limits_{i=1}^{s}\mu_{i}x_{i+r}^{2}=c\qquad c\neq0,\lambda_{i}>0,\mu_{i}>0$$
>- Se $\text{rk}(A)=\text{rk}(A_{0})+2$:
>$$\sum\limits_{i=1}^{r}\lambda_{i}x_{i}^{2}-\sum\limits_{i=1}^{s}\mu_{i}x_{i+r}^{2}-cx_{r+s+1}=0\qquad c>0,\lambda_{i}>0,\mu_{i}>0$$

>[!tip] Conseguenze del teorema
>- Se $M$ è invertibile allora $\text{rk}(AM)=\text{rk}(A)=\text{rk}(MA)$
>- Se si rototrasla una quadrica con la rototraslazione $R(X)=M_{0}X+v$ allora la sua matrice $A$ si trasforma in $A'=(M^{-1})^{T}AM^{-1}$ dove $M$ è la matrice di $R$. Inoltre $A_{0}'=M_{0}A_{0}M_{0}^{T}$, ne segue che il rango di $A$ e $A_{0}$ non cambiano.
>- Per calcolare esattamente la forma in cui corrisponde una quadrica non è necessario calcolare gli autovettori ma solo gli autovalori:
>	1. Se $\text{rk}(A)=\text{rk}(A_{0})$ si è nel primo caso e bastano gli autovalori.
>	2. Se $\text{rk}(A)=\text{rk}(A_{0})+2$ si è nel terzo tipo e bastano gli autovalori poiché $c=2||q_{0}||$
>	3. Se $\text{rk}(A)=\text{rk}(A_{0})+1$ e
>		- $\det(A_{0})\neq0$ bastano gli autovalori poiché $c=-\frac{\det(A)}{\det(A_{0})}$
>		- $\det(A_{0})=0$ allora oltre agli autovalori si calcola un centro $c_{0}$ e $c=-p(c_{0})$


