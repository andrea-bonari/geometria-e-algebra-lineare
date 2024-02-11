### Isomorfismi
>[!note]
>Siano $V$ e $W$ spazi vettoriali. Un isomorfismo da $V$ a $W$ è una trasformazione lineare biiettiva. $$T: V\to W$$

### Vettori e coordinate
>[!note]
>Sia $V$ uno spazio vettoriale di dimensione $n$ e sia $B=\{v_{1},v_{2},\cdots,v_{n}\}$ una base di $V$.
>Se $v$ è un vettore in $V$ allora è combinazione lineare degli elementi in $B$ $$v=x_{1}v_{1}+x_{2}v_{2}+\cdots+x_{n}v_{n}$$
>Il vettore $\begin{pmatrix}x_{1}\\x_{2}\\\vdots\\x_{n}\end{pmatrix}$ è detto vettore delle coordinate di $v$ in $B$ e lo indichiamo con $C_{B}(v)$.
>
>Sia quindi $B$ una base di $V$ e sia $n$ la dimensione di $V$. Allora la funzione $C_{B}: V\to \mathbb{R}^{n}$ è un isomorfismo.


Sia $V$ uno spazio vettoriale di dimensione $n$ e $W$ uno spazio vettoriale di dimensione $m$. Siano $B$ e $B'$ basi rispettivamente di $V$ e $W$. Data $T:V\to W$ una trasformazione lineare, esiste un unica matrice $A$ di dimensione $m$x$n$ tale che $$C_{B}(T(v))=AC_{B}(v)$$
La matrice $A$ è detta matrice rappresentativa della trasformazione lineare $T$ nelle basi $B$ e $B'$ e si indica con $$M_{B'}^{B}(T)$$che è la matrice che ha per $i$-esima colonna il vettore delle coordinate in $B'$ dell'$i$-esimo elemento di $B$