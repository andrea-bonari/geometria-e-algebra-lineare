>[!note]
>Per essere definita base di spazio vettoriale un insieme deve essere:
>- Un insieme di vettori finitamente generato
>- Linearmente indipendente

### Teorema della base
>[!note]
> Sia $V$ uno spazio vettoriale finitamente generato, allora:
> - $V$ ha una base e tutte le basi di $V$ hanno lo stesso numero di elementi.
> - Ogni insieme linearmente indipendente in $V$ è contenuto in una base di $V$.
> - Ogni insieme di generatori di $V$ contiene una base.

>[!abstract] Conseguenze del teorema della base
>1. Sia $V$ uno spazio di dimensione finita, se $W$ è un sottospazio di $V$ allora anche $V$ è di dimensione finita e $\dim(W)\leq\dim(V)$.
>2. Sia $V$ uno spazio di dimensione finita, se $W$ è un sottospazio di $V$ e $\dim(W)=\dim(V)$ allora $W=V$.
>3. Sia $V$ uno spazio di dimensione finita, se $v_{1},v_{2},\cdots,v_{k}$ sono linearmente indipendenti in $v$ allora $k\leq\dim(V)$.
>4. Sia $V$ uno spazio di dimensione finita, se $v_{1},v_{2},\cdots,v_{k}$ generano $V$ allora $\dim(V)\leq k$.
>5. Sia $V$ uno spazio di dimensione finita, se $v_{1},v_{2},\cdots,v_{n}$ sono linearmente indipendenti e $\dim(V)=n$ allora $\{v_{1},v_{2},\cdots,v_{n}\}$ è una base di $V$.
>6. Sia $V$ uno spazio di dimensione finita, se $v_{1},v_{2},\cdots,v_{k}$ generano $V$ e $\dim(V)=k$ allora $\{v_{1},v_{2}\cdots,v_{k}\}$ è una base di $V$.

Il numero di elementi di una qualsiasi base di uno spazio $V$ è chiamato dimensione di $V$ e lo si indica con il simbolo $\dim(V)$.

### Spazio riga e spazio colonna
>[!note]
>Se $A$ è una matrice $n$x$m$ indichiamo con $A_{1},A_{2},\cdots,A_{n}$ le righe di $A$ e con $A^{1},A^{2},\cdots,A^{m}$ le colonne di $A$.
>
>Lo spazio riga di $A$ è lo spazio generato dalle righe di $A$, mentre lo spazio colonna di $A$ è lo spazio generato dalle colonne di $A$.

Se una matrice $B$ è a gradini allora le sue righe non nulle sono linearmente indipendenti e quindi sono una base del suo spazio riga.

### Operazioni tra sottospazi
- ##### Somma:
Se $U,W$ sono sottospazi di uno spazio $V$ allora lo spazio somma $U+W$ è un sottospazio.$$U+W=\{u+w\quad|\quad u\in U, w\in W\}$$
- ##### Intersezione:
Se $U,W$ sono sottospazi di uno spazio $V$ allora lo spazio intersezione $U\cap W$ è un sottospazio.$$U\cap W=\{v\quad|\quad v\in U,v\in W\}$$
>[!abstract] Formula di Grassmann
>Vale la seguente formula: $$\dim(U+W)+\dim(U\cap W)=\dim(U)+\dim(W)$$
- ##### Somma diretta
Si dice che uno spazio $V$ è somma diretta di due sottospazi $U,W$ se $$V=U+W\quad\text{e}\quad U\cap W=\{\overrightarrow{0}\}$$
La notazione della somma diretta fra $U$ e $W$ è: $V=U\oplus W$.
- ##### Complemento di un sottospazio
Se $U$ è un sottospazio di uno spazio $V$, un complemento di $U$ è un sottospazio $W$ tale che $V=U\oplus W$.
- ##### Proiezione
Sia $V=U\oplus W$, allora, dato $v\in V$ possiamo scrivere in modo unico $v=u+w$ con $u\in U$ e $v\in V$. Il vettore $u$ è detto la proiezione di $v$ su $U$ relativa alla somma diretta $V=U\oplus W$.

