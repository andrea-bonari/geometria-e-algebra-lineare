>[!note]
>Il determinante è un concetto fondamentale nell'algebra lineare, utilizzato principalmente per studiare le proprietà delle matrici quadrate.
>$$\det A\qquad\begin{vmatrix}a_{i,j}\end{vmatrix}$$

### Calcolo tramite regola di Sarrus
![[Immagine.png]]

Utilizzando lo schema di riferimento, si esegue la somma dei prodotti sulle diagonali discendenti meno la somma dei prodotti sulle diagonali ascendenti.

>[!warning]
>
Il problema di questa tecnica è la sua difficile scalabilità computazionale, dato che per le matrici di ordine $n$ la formula del determinante è la somma di $n!$ termini.

### Calcolo tramite sviluppo di Laplace

>[!note]
>Lo sviluppo di Laplace è una formula ricorsiva che riscrive il determinante di una matrice quadrata di ordine $n$ calcolando il determinante della matrice di ordine $n-1$. Utilizzare la formula generale non è conveniente perché difficile da dimostrare e si dovrebbero svolgere molti calcoli su parecchi termini. La formula dello sviluppo di Laplace è la seguente: $$\det(A)=\sum\limits_{i=1}^{m}(-1)^{i+j}\cdot a_{i,j}\cdot\det(A_{(ij}))$$

>[!tip]
>Questa formula sostanzialmente ci dice di scegliere una riga/o una colonna, sommare gli elementi di quella riga/colonna tenendo conto del segno tramite metodo della scacchiera, scegliendo $a_{ij}$ come elemento eliminato e moltiplicandolo al determinante della minore ottenuta rimuovendo la colonna e riga dell'elemento scelto.

### Proprietà

- Alternanza: Se $A_{1}$ si ottiene da $A_{0}$ scambiando 2 righe tra di loro, allora $\det(A_{1})=-\det(A_{0})$
- Multi linearità:
	- Se $A_{1}$ si ottiene da $A_{0}$ moltiplicando una riga per uno scalare $t$, allora $\det(A_{1})=t\cdot\det(A_{0})$.
	- Se la $i$-esima riga di $A$ è la somma di 2 vettori $v$ e $w$ allora $\det(A)=\det(A_{v})+\det(A_{w})$, dove $A_{v}$ e $A_{w}$ sono le matrici con $i$-esima riga i vettori termini della somma.
	- Si possono sommare e moltiplicare per un fattore le righe di una matrice e il suo determinante resterà uguale.
- Normalizzazione: $\det(I)=1$
- Simmetria: $\det(A)=\det(A^{T})$
- Formula di Bindet: $\det(A\cdot B)=\det(A)\cdot\det(B)$

