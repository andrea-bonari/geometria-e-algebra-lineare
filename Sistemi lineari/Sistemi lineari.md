>[!note]
>Considero un sistema di $m$ equazioni in $n$ incognite: $$\begin{cases}a_{11}\cdot x_{1}&+&a_{12}\cdot x_{2}&+&\cdots&+&a_{1n}\cdot x_{n}&=&b_{1}\\
>a_{21}\cdot x_{1}&+&a_{22}\cdot x_{2}&+&\cdots&+&a_{2n}\cdot x_{n}&=&b_{2}\\
>\vdots&+&\vdots&+&\vdots&+&\vdots&=&\vdots\\a_{m1}\cdot x_{1}&+&a_{m2}\cdot x_{2}&+&\cdots&+&a_{mn}\cdot x_{n}&=&b_{m}
>\end{cases}$$
>- La matrice $a_{ij}$ prende il nome di matrice dei coefficienti $$\begin{pmatrix}a_{11}&a_{12}&\cdots&a_{1n}\\a_{21}&a_{22}&\cdots&a_{2n}\\\vdots&\vdots&\ddots&\vdots\\a_{m1}&a_{m2}&\cdots&a_{mn}\end{pmatrix}$$
>- Il vettore colonna $b=\begin{pmatrix}b_{1}\\b_{2}\\\vdots\\b_{m}\end{pmatrix}$ prende il nome di vettore di termini noti.
>- Il vettore colonna $X=\begin{pmatrix}x_{1}\\x_{2}\\\vdots\\x_{m}\end{pmatrix}$ prende il nome di vettore delle incognite.

La matrice completa di un sistema è $(A\space|\space b)$.

I sistemi possono essere:
- omogenei ($b=\overrightarrow{0}$):
	- Se $x_{1},x_{2}$ sono soluzioni del sistema anche $x_{1}+x_{2}$ è soluzione.
	- Se $x_{0}$ è soluzione del sistema, allora anche $t\cdot x_{0}$ è soluzione.
- non omogenei.
	- La soluzione sarà in formato: $\text{sol}(A,b)=x_{\text{part}}+\text{sol}(A,\overrightarrow{0})$

>[!tip] Matrice a gradini
>Una matrice si dice a gradini se il pivot di ogni riga è in una colonna successiva a quella del pivot della riga precedente, con pivot si intende il primo elemento non nullo di una riga della matrice. Allo stesso modo un sistema è definito a gradini se la sua matrice completa è a gradini.

### Numero di soluzioni di un sistema
>[!note]
>Diremo che una matrice ha $\infty^{k}$ soluzioni se ha almeno una soluzione e $\dim(\text{sol}(A,\overrightarrow{0}))=k$. Se un sistema $AX=b$ ha soluzioni all'ora l'espressione $$X=X_\text{part} + t_{1}X_{1}+t_{2}X_{2}+\cdots+t_{k}X_{k}$$descrive tutte le soluzioni in k parametri, ed è detta soluzione generale del sistema.

##### Teorema di Rouchè-Capelli
>[!note]
>Sia $A$ una matrice $n\times m$ e si consideri il sistema lineare di $n$ equazioni e $m$ incognite $AX=b$. Il sistema ha soluzione se e solo se $$\text{rk}(A)=\text{rk}(A\space |\space b)$$

##### Metodo di Cramer
>[!note]
>Sia $A$ una matrice quadrata di ordine $n$, allora il sistema crameriano $AX=b$ ha un'unica soluzione se e solo se $\det(A)\neq0$.

>[!abstract] Sistema crameriano
>Un sistema di $n$ equazioni e $n$ incognite è detto crameriano. Se un sistema crameriano $AX=b$ è tale che $\det(A)\neq0$ allora ha un unica soluzione.

Procedimento del metodo di Cramer:

1. Consideriamo il sistema crameriano $AX=b$ tale che $\det(A)\neq0$
2. Considero il vettore colonna $S=\begin{pmatrix}s_{1}\\s_{2}\\\vdots\\s_{n}\end{pmatrix}$
3. Allora l'unica soluzione si calcola con $$s_{i}=\frac{\det(A(i,b))}{\det(A)}$$dove $A(i,b)$ è la matrice che si ottiene sostituendo alla $i$-esima colonna di $A$ il vettore $b$.

