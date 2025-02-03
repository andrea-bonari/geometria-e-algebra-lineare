>[!note]
>Una matrice $n\times m$ può essere vista come una tabella di numeri reali composta da $n$ righe e $m$ colonne. Una matrice è un vettore i cui elementi sono anch'essi vettori, quindi un vettore di vettori. $$\begin{pmatrix}
a_1 & a_2 & a_3 \\
b_1 & b_2 & b_3 \\
c_1 & c_2 & c_3
\end{pmatrix}$$
>Si definiscono le operazioni di somma e prodotto per uno scalare: $$\begin{align*}
&(a_{i,j})+(b_{i,j})=(a_{i,j}+b_{i,j})\text{ con }A,B\text{ matrici di stessa dimensione}\\
&t\cdot(a_{i,j})=(t\cdot a_{i,j})\quad t\in\mathbb{R}
\end{align*}$$

Le matrici più importanti sono
- Vuota: $0\times 0$
- Quadrata: $n\times n$
- $n$-vettore: $1\times n$
- $n$-vettore colonna: $n\times 1$
- Nulla: $a_{i,j}\quad|\quad a_{i,j}=0\quad\forall i,j: 1<i\leq n\vee 1<j\leq m$ (ogni elemento della matrice è 0)
- Identità: viene definita per matrici quadrate, ha tutti gli $1$ sulla diagonale principale ed il resto tutti $0$, si indica con $I_{n}=\begin{pmatrix}1&0\\0&1\end{pmatrix}$
- Matrice a blocchi: una matrice è detta a blocchi quando si presenta nella forma $A=\begin{pmatrix}A_{1}&0\\0&A_{2}\end{pmatrix}$ dove $A_{1},A_{2}$ e $A$ sono matrici quadrate
### Prodotto riga per colonna
>[!note]
>Siano $A$ e $B$ matrici conformabili, si definisce il prodotto riga per colonna come: $$A\cdot B=\sum\limits_{k=1}^{m}(a_{i,k})\cdot(b_{k,j})$$
![[Pasted image 20240104153943.png]]
>

>[!abstract] Matrici conformabili
>Una matrice $A$ $n$x$m$ è conformabile ad una matrice $B$ $r$x$s$ se il numero di colonne di $A$ è uguale al numero di righe di $B$.$$(m\times n)\cdot(r\times s)=(c_{s,m})\iff n=r$$

Le dimensioni della matrice prodotto saranno il numero di colonne di $A$ e il numero di righe di $B$.

In questa operazione valgono le proprietà associative e distributive, ma non vale quella commutativa: $$A\cdot B\neq B\cdot A$$
>[!tip] Potenze di matrici quadrate
>Consideriamo una matrice quadrata di ordine $n$, grazie alla proprietà associativa la potenza ennesima è definita come: $$A^{n}=\prod\limits^{n}A$$
>
>Valgono le proprietà classiche delle potenze:
>- $A^{0}=1$
>- $A^{n}+A^{m}=a^{n+m}$
>- $(A^{n})^{m}=A^{n\cdot m}$
>

### Sottomatrici e minori
>[!note]
>Viene definita sottomatrice di $A$ una matrice ottenuta togliendo alcune righe e colonne dalla matrice $A$.

Se la sottomatrice è quadrata di ordine $m$ allora si chiama minore di ordine $m$.

Il minore complementare $M_{1}$ dell'elemento $a_{i,j}$ è il minore che si ottiene togliendo ad $M$ la $i$-esima riga e la $j$-esima colonna.

### Trasposta di una matrice
>[!note]
>La trasposta della matrice $A$ è la matrice che si ottiene scambiando righe e colonne, e si indica con $A^{T}$
> - La matrice si dice simmetrica quando $A=A^{T}$
> - La matrice si dice antisimmetrica quando $A=-A^{T}$

Si ha che
- $(A+B)^{T}=A^{T}+B^{T}$
- $(s\cdot A)^{T}=s\cdot A^{T}$
- $(A^{T})^{T}=A$
- $(A\cdot B)^{T}=A^{T}\cdot B^{T}$

### Determinante
>[!note]
>Il determinante di una matrice è un numero associato a ciascuna matrice quadrata $n\times n$, e ne esprime alcune proprietà algebriche e geometriche: $$\det(A)\qquad |A|$$

Il determinante ha le seguenti proprietà:
- Alternanza: Se $A_{1}$ si ottiene da $A_{0}$ scambiando 2 righe tra di loro, allora $\det(A_{1})=-\det(A_{0})$
- Multi linearità:
	- Se $A_{1}$ si ottiene da $A_{0}$ moltiplicando una riga per uno scalare $t$, allora $\det(A_{1})=t\cdot\det(A_{0})$.
	- Se la $i$-esima riga di $A$ è la somma di 2 vettori $v$ e $w$ allora $\det(A)=\det(A_{v})+\det(A_{w})$, dove $A_{v}$ e $A_{w}$ sono le matrici con $i$-esima riga i vettori termini della somma.
	- Si possono sommare e moltiplicare per un fattore le righe di una matrice e il suo determinante resterà uguale.
- Normalizzazione: $\det(I)=1$
- Simmetria: $\det(A)=\det(A^{T})$
- Formula di Bindet: $\det(A\cdot B)=\det(A)\cdot\det(B)$

##### Determinante tramite regola di Sarrus
>[!note]
>Per calcolare il determinante di una radice quadrata $n\times n$ è possibile applicare la regola di Sarrus:
>1. Sommare i prodotti lungo le prime $n$ diagonali complete da sinistra verso destra
>2. Sommare i prodotti lungo le ultime $n$ antidiagonali complete da destra verso sinistra
>3. Calcolare la differenza tra i risultati ottenuti al punto 1 e 2
>
>![[Immagine.png]]

>[!warning]
Il problema di questa tecnica è la sua difficile scalabilità computazionale, dato che per le matrici di ordine $n$ la formula del determinante è la somma di $n!$ termini.

##### Determinante tramite sviluppo di Laplace
>[!note]
>Lo sviluppo di Laplace è una formula ricorsiva che riscrive il determinante di una matrice quadrata di ordine $n$ calcolando il determinante della matrice di ordine $n-1$: $$\det(A)=\sum\limits_{i=1}^{m}(-1)^{i+j}\cdot a_{i,j}\cdot\det(A_{(ij}))$$
>
>Questa formula ci dice di scegliere una riga/o una colonna, sommare gli elementi di quella riga/colonna tenendo conto del segno tramite metodo della scacchiera, scegliendo $a_{i,j}$ come elemento eliminato e moltiplicandolo al determinante della minore ottenuta rimuovendo la colonna e riga dell'elemento scelto.
