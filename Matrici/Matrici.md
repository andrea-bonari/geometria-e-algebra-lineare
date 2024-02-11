>[!note]
>Una matrice $n$x$m$ può essere vista come una tabella di numeri reali composta da $n$ righe e $m$ colonne. Una matrice è un vettore i cui elementi sono anch'essi vettori, quindi un vettore di vettori. $$\begin{pmatrix}
a_1 & a_2 & a_3 \\
b_1 & b_2 & b_3 \\
c_1 & c_2 & c_3
\end{pmatrix}$$

### Matrici degeneri

- Vuota: $0$x$0$
- Quadrata: $n$x$n$
- $n$-vettore: $1$x$n$
- $n$-vettore colonna: $n$x$1$
- Nulla: $a_{i,j}\quad|\quad a_{i,j}=0\quad\forall i,j: 1<i\leq n\vee 1<j\leq m$ (ogni elemento della matrice è 0)
- Identità: viene definita per matrici quadrate, ha tutti gli $1$ sulla diagonale principale ed il resto tutti $0$, si indica con $I_{n}=\begin{pmatrix}1&0\\0&1\end{pmatrix}$

### Operazioni con le matrici

- Somma: è importante che le matrici abbiano le stesse dimensioni $n$x$m$$$(a_{i,j})+(b_{i,j})=(a_{i,j}+b_{i,j})$$
- Prodotto per scalare:$$t\cdot(a_{i,j})=(t\cdot a_{i,j})$$
>[!info]
>Valgono le stesse proprietà degli $n$-vettori per le operazioni somma e prodotto per scalare.

- ###### Prodotto riga per colonna

>[!abstract] Matrici conformabili
>Una matrice $A$ $n$x$m$ è conformabile ad una matrice $B$ $r$x$s$ se il numero di colonne di $A$ è uguale al numero di righe di $B$.$$(m\times n)\cdot(r\times s)=(c_{s,m})\iff n=r$$

Una volta stabilito che le matrici $A$ e $B$ sono conformabili:
$$A\cdot B=C$$
$$C=\sum\limits_{k=1}^{m}(a_{i,k})\cdot(b_{k,j})$$
>[!info]
>Le dimensioni della matrice prodotto saranno il numero di colonne di $A$ e il numero di righe di $B$.

![[Pasted image 20240104153943.png]]

>[!warning]
>Valgono le proprietà associative e distributive, ma non vale quella commutativa $$A\cdot B\neq B\cdot A$$

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