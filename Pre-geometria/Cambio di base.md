- ##### Matrice della composizione di due trasformazioni lineari
Siano $T:V\to W$ e $S:W\to U$ due trasformazioni lineari. Fissiamo una base $B$ di $V$ una base $B'$ di $W$ e una base $B''$ di $U$, allora: $$M_{B''}^{B}(S\circ T)=M_{B''}^{B'}(S)\cdot M_{B'}^{B}(T)$$
- ##### Matrice dell'identità
Consideriamo l'identità $I:V\to V$, cioè $I(v)=v$. Se $B$ è una base di $V$ allora $M_{B'}^{B}(I)=I$. Se $B$ e $B'$ sono basi di $V$ allora $M_{B'}^{B}(I)$ è invertibile e $$M_{B'}^{B}(I)^{-1}=M^{B'}_{B}(I )$$
- ##### Matrice del cambiamento di base
Sia $V$ uno spazio vettoriale di dimensione finita e siano $B$ e $B'$ basi di $V$. Sia $v$ un vettore in $V$ e siano $X$ e $X'$ i vettori delle coordinate di $v$ nelle basi $B$ e $B'$ rispettivamente, allora $$X' =M_{B'}^{B}(I)X$$
Per questo motivo la matrice $M_{B'}^{B}(I)$ è detta matrice del cambiamento di base.

### Matrice rappresentativa
>[!note]
>Sia $T: V\to W$ una trasformazione lineare. Siano $B$,$B_{1}$ basi di $V$ e $B'$,$B_{1}'$ basi di $W$, allora $$M_{B_{1}'}^{B_{1}}=M_{B_{1}'}^{B'}(I)\cdot M^{B}_{B'}(T)\cdot M^{B_{1}}_{B}(I)$$

### Trasformazioni lineari diagonalizzabili
>[!note]
>Una trasformazione lineare $T:V\to V$ si dice diagonalizzabile se esiste una base $B$ di $V$ in cui la matrice $M_{B}^{B}(T)$ è diagonale. Inoltre è diagonalizzabile se e solo se in una qualsiasi base $B'$ di $V$ $M_{B'}^{B'}(T)$ è diagonalizzabile.

