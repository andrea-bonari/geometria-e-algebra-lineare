>[!note]
>Una matrice viene definita invertibile se:$$\exists B\quad|\quad A\cdot B=B\cdot A=1$$
>Se $A$ è invertibile allora $B$ è unica e si indica con $A^{-1}$

Per calcolare la matrice inversa è necessario che $\det(A)\neq0$

##### Calcolo matrice inversa (metodo dei determinanti)
>[!note]
$$A^{-1}= \frac{1}{\det(A)}\cdot\text{agg}(A)$$

>[!tip] Matrice dei cofattori
>La matrice dei cofattori $(\text{agg}(A))^{T}$ di $A$ è una matrice dove i valori di ogni elemento sono il determinante della minore complementare.
##### Calcolo matrice inversa (algoritmo di Gauss-Jordan)
>[!note]
>Consideriamo una matrice $A_{n\times n}$ e scriviamo una matrice $(A\space |\space I_{n})$. Svolgendo le operazioni lineari di riga tentiamo di arrivare alla forma $(I_{n}\space |\space B)$, dove $B$ sarà la nostra matrice inversa $A^{-1}$.

##### Calcolo di matrice inversa a blocchi
>[!note]
>L'inversa di una matrice a blocchi si ottiene invertendo le singole matrici interne: $$A^{-1}=\begin{pmatrix}(A_{1})^{-1}&0\\0&(A_{2})^{-1}\end{pmatrix}$$
