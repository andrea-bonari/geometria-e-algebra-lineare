>[!note]
>Le forme quadratiche su $\mathbb{R}^{n}$ sono i polinomi di grado due omogenei in $n$ variabili, se $$X=\begin{pmatrix}x_{1}\\\vdots\\x_{n}\end{pmatrix}\qquad q(x)=\sum\limits_{i,j}a_{ij}x_{i}x_{j}$$

>[!example]
>In $\mathbb{R}^{2}$
>$$q\left(\begin{pmatrix}x\\y\end{pmatrix}\right)=ax^{2}+bxy+cy^{2}$$
>In $\mathbb{R}^{3}$
>$$q\left(\begin{pmatrix}x\\y\\z\end{pmatrix}\right)=ax^{2}+bxy+cy^{2}+dxz+ez^{2}+fyz$$

### Forme quadratiche e matrici
>[!note]
>Sia $q(x)=\sum\limits_{i,j}a_{ij}x_{i}x_{j}$ una forma quadratica e $A$ la matrice dei coefficienti $(a_{ij})$. Ponendo $X=\begin{pmatrix}x_{1}\\\vdots\\x_{n}\end{pmatrix}$ possiamo riscrivere la forma quadratica come $$q(X)=X^{T}AX$$

### Matrice di Gram di una forma quadratica
>[!note]
>Se $q(X)$ è una forma quadratica allora possiamo sempre scrivere la forma quadratica nella seguente forma, dove $S$ è una matrice simmetrica unica $$q(X)=X^{T}SX$$
>La matrice $S$ è unica ed è detta matrice di Gram di una forma quadratica.

>[!example]
>Considero la quadrica $$q(x,y,z)=axy+bxz+cyz+dx^{2}+ey^{2}+fz^{2}$$
>Si scrive la matrice formata dai coefficienti $$\begin{pmatrix}d& \frac{a}{2}& \frac{b}{2}\\ \frac{a}{2}&e& \frac{c}{2}\\ \frac{b}{2}& \frac{c}{2}&f\end{pmatrix}$$ 

### Segnatura di una forma quadratica
>[!note]
>Sia $A$ una matrice simmetrica reale. Sia $r$ il numero di autovalori positivi di $A$ contati con la loro molteplicità geometrica e sia $s$ il numero di autovalori negativi contati con la loro molteplicità geometrica.
>La coppia $(r,s)$ è detta segnatura della matrice $A$.

>[!tip]
>La segnatura di una forma quadratica è riferita alla matrice di Gram, quindi molteplicità geometrica e algebrica sono equivalenti.

### Criterio di Cartesio
>[!note]
>Dato il polinomio $$p(t)=\sum\limits_{j=0}^{r}a_{j}t_{j}^{i}\quad a_{j}\neq 0\quad 0\leq i_{0}< i_{1}<\cdots< i_{r}$$
>Il numero di variazioni di segno è il numero di $j$ tali che $$\text{sgn}(a_{j})\neq\text{sqn}(a_{j-1})$$
>
>Il numero di variazioni di un polinomio è il massimo numero di radici positive del polinomio. Se il polinomio ha solo radici reali allora il numero di variazioni è il numero di radici positive contato con la loro molteplicità.

Applicazione del criterio al calcolo della segnatura di una matrice simmetrica. Se $A$ è simmetrica allora il polinomio caratteristico ha solo radici reali, quindi: $$\#\text{ autovalori positivi}=\#\text{ n. variazioni}$$$$\#\text{ autovalori nulli}=\text{null}(A)$$$$\#\text{ autovalori negativi}=n-\text{null}(A)-\#\text{ autovalori positivi}=\text{rk}(A)-\#\text{ n. variazioni}$$
Sapendo questo possiamo riscrivere la segnatura $(r,s)$ di $q(x)$ come:
- $r$: numero di variazioni del polinomio caratteristico della matrice di Gram di $q(x)$
- $s$: $\text{rk}(S)-r$

### Forme quadratiche particolari e segnatura
>[!note]
>Sia $q(X)$ una forma quadratica su $\mathbb{R}^{n}$
>1. Si dice che $q$ è nondegenere se il rango della sua matrice di Gram è $n$.
>2. Si dice che $q$ è semidefinita positiva se: $$q(X)\geq0\quad\forall X\in\mathbb{R}^{n}$$
>3. Si dice che $q$ è semidefinita negativa se $$q(X)\leq0\quad\forall X\in\mathbb{R}^{n}$$
>4. Si dice che $q$ è definita positiva se $$\begin{cases}q(X)\geq0\quad\forall X\in\mathbb{R}^{n}\\q(X)=0\iff X=0\end{cases}$$
>4. Si dice che $q$ è definita negativa se $$\begin{cases}q(X)\leq0\quad\forall X\in\mathbb{R}^{n}\\q(X)=0\iff X=0\end{cases}$$
>5. Si dice che $q$ è indefinita se esiste un vettore $v$ per cui $$\begin{cases}\exists v|q(v)>0\\\exists w|q(w)<0\end{cases}$$

1. La forma $q$ su $\mathbb{R}^{n}$ è semidefinita positiva se e solo se ha segnatura $(r,0)$
2. La forma $q$ su $\mathbb{R}^{n}$ è definita positiva se e solo se ha segnatura $(n,0)$
3. La forma $q$ su $\mathbb{R}^{n}$ è semidefinita negativa se e solo se ha segnatura $(0,s)$
4. La forma $q$ su $\mathbb{R}^{n}$ è definita negativa se e solo se ha segnatura $(0,n)$
5. La forma $q$ su $\mathbb{R}^{n}$ è indefinita se e solo se la segnatura è $(r,s)$ con $r\neq 0$, $s\neq 0$
6. La forma $q$ su $\mathbb{R}^{n}$ è non degenere se e solo se $r+s=n$

### Traccia di una matrice
>[!note]
>La traccia di una matrice $A$ quadrata di ordine $n$ è la somma degli elementi sulla diagonale principale della matrice: $$\text{tr}(A)=\sum\limits_{i=1}^{n}a_{ii}$$

La traccia di $AB$ è pari alla traccia di $BA$ $$\text{tr}(AB)=\text{tr}(BA)$$
Se $A$ e $B$ sono matrici simili, allora hanno la stessa traccia e lo stesso determinante $$\text{tr}(A)=\text{tr}(B)\qquad\det(A)=\det(B)$$
### Traccia-determinante-autovalori
>[!note]
>Se $A$ è una matrice diagonalizzabile e $\lambda_{1},\lambda_{2},\cdots,\lambda_{n}$ sono i suoi autovalori allora $$\det(A)=\lambda_{1}\cdot\lambda_{2}\cdot\cdots\cdot\lambda_{n}\qquad \text{tr}(A)=\lambda_{1}+\lambda_{2}+\cdots+\lambda_{n}$$

### Segnatura di una quadratica nel piano
Data la forma quadratica $q(x)$ con matrice di Gram $S$ $$q(x)=ax^{2}+bxy+cy^{2}\qquad S=\begin{pmatrix}a& \frac{b}{2}\\ \frac{b}{2}&c\end{pmatrix}$$
- $\det(S)>0$ e $a>0\quad\Rightarrow\quad (2,0)$
- $\det(S)>0$ e $a<0\quad\Rightarrow\quad (0,2)$
- $\det(S)<0\quad\Rightarrow\quad (1,1)$
- $\det(S)=0$ e $a+c>0\quad\Rightarrow\quad (1,0)$
- $\det(S)=0$ e $a+c<0\quad\Rightarrow\quad (0,1)$
