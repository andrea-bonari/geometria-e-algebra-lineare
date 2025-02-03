### Isomorfismi
>[!note]
>Siano $V$ e $W$ spazi vettoriali. Un isomorfismo da $V$ a $W$ è una trasformazione lineare biiettiva. $$T: V\to W$$

### Vettori e coordinate
>[!note]
>Sia $V$ uno spazio vettoriale di dimensione $n$ e sia $B=\{v_{1},v_{2},\cdots,v_{n}\}$ una base di $V$. Se $v$ è un vettore in $V$ allora è combinazione lineare degli elementi in $B$: $$v=x_{1}v_{1}+x_{2}v_{2}+\cdots+x_{n}v_{n}$$
>Il vettore $\begin{pmatrix}x_{1}\\x_{2}\\\vdots\\x_{n}\end{pmatrix}$ è detto vettore delle coordinate di $v$ in $B$ e lo indichiamo con $C_{B}(v)$.
>
>Sia quindi $B$ una base di $V$ e sia $n$ la dimensione di $V$. Allora la funzione $C_{B}: V\to \mathbb{R}^{n}$ è un isomorfismo.

Sia $V$ uno spazio vettoriale di dimensione $n$ e $W$ uno spazio vettoriale di dimensione $m$. Siano $B$ e $B'$ basi rispettivamente di $V$ e $W$. Data $T:V\to W$ una trasformazione lineare, esiste un unica matrice $A$ di dimensione $m$x$n$ tale che $$C_{B}(T(v))=AC_{B}(v)$$
La matrice $A$ è detta matrice rappresentativa della trasformazione lineare $T$ nelle basi $B$ e $B'$ e si indica con $$M_{B'}^{B}(T)$$che è la matrice che ha per $i$-esima colonna il vettore delle coordinate in $B'$ dell'$i$-esimo elemento di $B$.

### Matrici del cambiamento di base
>[!note] Matrice del cambiamento di base
Sia $V$ uno spazio vettoriale di dimensione finita e siano $B$ e $B'$ basi di $V$. Sia $v$ un vettore in $V$ e siano $X$ e $X'$ i vettori delle coordinate di $v$ nelle basi $B$ e $B'$ rispettivamente, allora $$X' =M_{B'}^{B}(I)X$$
Per questo motivo la matrice $M_{B'}^{B}(I)$ è detta matrice del cambiamento di base.

>[!note] Matrice della composizione di due trasformazioni lineari
>Siano $T:V\to W$ e $S:W\to U$ due trasformazioni lineari. Fissiamo una base $B$ di $V$ una base $B'$ di $W$ e una base $B''$ di $U$, allora: $$M_{B''}^{B}(S\circ T)=M_{B''}^{B'}(S)\cdot M_{B'}^{B}(T)$$

>[!note] Matrice dell'identità
Consideriamo l'identità $I:V\to V$, cioè $I(v)=v$. Se $B$ è una base di $V$ allora $M_{B'}^{B}(I)=I$. Se $B$ e $B'$ sono basi di $V$ allora $M_{B'}^{B}(I)$ è invertibile e $$M_{B'}^{B}(I)^{-1}=M^{B'}_{B}(I )$$

### Matrice rappresentativa
>[!note]
>Sia $T: V\to W$ una trasformazione lineare. Siano $B$,$B_{1}$ basi di $V$ e $B'$,$B_{1}'$ basi di $W$, allora $$M_{B_{1}'}^{B_{1}}=M_{B_{1}'}^{B'}(I)\cdot M^{B}_{B'}(T)\cdot M^{B_{1}}_{B}(I)$$

### Trasformazioni lineari diagonalizzabili
>[!note]
>Una trasformazione lineare $T:V\to V$ si dice diagonalizzabile se esiste una base $B$ di $V$ in cui la matrice $M_{B}^{B}(T)$ è diagonale. Inoltre è diagonalizzabile se e solo se in una qualsiasi base $B'$ di $V$ $M_{B'}^{B'}(T)$ è diagonalizzabile.

