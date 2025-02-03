>[!note]
>Una matrice $A$ si dice diagonalizzabile se è simile a una matrice diagonale. Ciò significa che deve esistere una matrice $M$ invertibile, detta modale, tale che:
>$$M^{-1}AM=\begin{pmatrix}a_{1}&\cdots&0\\\vdots&\ddots&0\\0&0&a_{n}\end{pmatrix}$$

>[!abstract] Matrici simili
>Due matrici quadrate $A$ e $B$ si dicono simili se esiste una matrice invertibile $M$ tale che: $$M^{-1}AM=B$$

>[!abstract] Matrice diagonale
>Una matrice $A$ si dice diagonale se è quadrata e si presenta nella forma: $$\begin{pmatrix}a_{1}&\cdots&0\\\vdots&\ddots&0\\0&0&a_{n}\end{pmatrix}\qquad\forall a\in\mathbb{R}$$
### Autovalori e autovettori
>[!note]
>Sia $A$ una matrice quadrata di ordine $n$, si dice che un numero $\lambda\in\mathbb{R}$ è un autovalore per $A$ se esiste un vettore $v\in\mathbb{R}^{n}$ non nullo tale che $A\cdot v=\lambda\cdot v$.
>
>Se $\lambda$ è un autovalore di una matrice $A$ allora il vettore $v$ viene chiamato autovettore di $A$ relativo all'autovalore $\lambda$, viceversa se $v$ è un autovettore di $A$ allora $a$ viene chiamato autovalore relativo all'autovettore $v$.

>[!abstract] Polinomio caratteristico
>Sia $A$ una matrice quadrata di ordine $n$. La funzione di una variabile reale $p(t)=\det(A-tI)$ è un polinomio di grado $n$ che è chiamato polinomio caratteristico di $A$. Lo si indica con $p_{a}(t)$.
>
>Gli autovalori di $A$ sono le radici del polinomio caratteristico di $A$. $\lambda$ è autovalore di $A$ se e solo se: $$p_{a}(\lambda)=\det(A-\lambda I)=0$$

L'insieme delle soluzioni del sistema lineare $(A-\lambda I)X=\overrightarrow{0}$ è detta autospazio relativo all'autovalore $\lambda$. L'autospazio è l'insieme di tutti gli autovettori $v$ relativi a $\lambda$ unito con $\{\overrightarrow{0}\}$.

>[!abstract] Molteplicità geometrica
>La dimensione dell'autospazio viene chiamata la molteplicità geometrica dell'autovalore $\lambda$ e si indica con $m_{g}(\lambda)$
>$$m_{g}(\lambda)=\dim(\text{sol}(A-\lambda I,\overrightarrow{0}))=\dim(N(A-\lambda I))=\text{null}(A-\lambda I)=n-\text{rk}(A-\lambda I)$$

>[!abstract] Molteplicità algebrica
>Se $p(t)$ è un polinomio e $\lambda_{1},\lambda_{2},\cdots,\lambda_{r}$ sono tutte le sue radici distinte $$p(t)=(t-\lambda_{1})^{m_{1}}(t-\lambda_{2})^{m_{2}}(\cdots)(t-\lambda_{r})^{m_{r}}q(t)$$con $m_{i}\geq 1$ e $q(t)$ un polinomio senza radici allora l'esponente $m_{i}$ è detto la molteplicità algebrica della radice $\lambda_{1}$. Lo si indica con $m_{a}(\lambda)$.

Il rapporto fra la molteplicità algebrica e geometrica è $$m_{g}(\lambda)\leq m_{a}(\lambda)$$
Un autovalore si dice semplice se $m_{a}(\lambda)=1$ e si dice regolare se $m_{g}(\lambda)=m_{a}(\lambda)$.

### Criteri di diagonalizzazione
1. Se una matrice $A$ quadrata di ordine $n$ ha $n$ autovalori distinti allora la matrice è diagonalizzabile.
2. Una matrice quadrata $A$ di ordine $n$ è diagonalizzabile se e solo se la somma delle molteplicità algebriche è $n$ e ogni autovalore è regolare.

Per diagonalizzare verifico i criteri, poi costruisco la matrice modale inserendo gli autovettori nelle colonne. Moltiplico poi questa matrice per una matrice la cui diagonale ha gli autovettori relativi alla stessa colonna della matrice modale. Infine moltiplico per l'inversa della matrice modale.