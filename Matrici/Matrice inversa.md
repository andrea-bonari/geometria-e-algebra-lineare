### Matrice invertibile
>[!note]
>Una matrice viene definita invertibile se esiste una matrice quadrata $B$ tale che $A\cdot B=B\cdot A=1$. $$\exists B_{n,n}\quad|\quad A\cdot B=B\cdot A=1$$
>Se $A$ è invertibile allora $B$ è unica e si indica con $A^{-1}$

Per calcolare la matrice inversa è necessario che $\det(A)\neq0$

### Calcolo matrice inversa (metodo dei determinanti)

$$A^{-1}= \frac{1}{\det(A)}\cdot\text{agg}(A)$$
Per calcolare $\text{agg}(A)$:

- Calcoliamo la matrice dei cofattori, cioè una matrice dove i valori di ogni elemento sono il determinante della minore complementare.
- $\text{agg}(A)$ sarà la trasposta della matrice dei cofattori.

### Calcolo matrice inversa (algoritmo di Gauss-Jordan)

1. Consideriamo una matrice $A_{n\times n}$ e scriviamo una matrice composta da $(A | I_{n})$
2. Svogliamo operazioni lineari di riga per arrivare alla forma $(I_{n}|A)$
3. In caso la matrice non fosse invertibile non riusciremo a scrivere la matrice in tale forma poiché $\det(A)=0$

### Matrici particolari

- Matrice a blocchi:
>[!note]
>Una matrice $A$ viene definita a blocchi quando si presenta nella forma $$A=\begin{pmatrix}A_{1}&0\\0&A_{2}\end{pmatrix}$$dove $A,A_{1},A_{2}$ sono matrici quadrate.

L'inversa di una matrice a blocchi si ottiene invertendo le singole matrici interne:

$$A^{-1}=\begin{pmatrix}(A_{1})^{-1}&0\\0&(A_{2})^{-1}\end{pmatrix}$$
- Matrici diagonale: $$A=\begin{pmatrix}a&0&0\\0&b&0\\0&0&c\end{pmatrix}\quad A=\begin{pmatrix}0&0&a\\0&b&0\\c&0&0\end{pmatrix}$$
- Matrici triangolari: $$\begin{pmatrix}a&b&c\\0&d&e\\0&0&f\end{pmatrix}\quad\begin{pmatrix}a&b&c\\d&e&0\\f&0&0\end{pmatrix}\quad\begin{pmatrix}0&0&a\\0&b&c\\d&e&f\end{pmatrix}\quad\begin{pmatrix}a&0&0\\b&c&0\\d&e&f\end{pmatrix}$$
