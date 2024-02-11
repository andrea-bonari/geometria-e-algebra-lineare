 >[!note]
>Un insieme $\{v_{1},v_{2},\cdots,v_{r}\}$ in uno spazio euclideo $V$ si dice ortogonale se $v_{i}\neq\overrightarrow{0}$ per ogni $i$ e $v_{i}\cdot v_{j}=0$ con $i\neq j$. $$\begin{cases}v_{i}\neq 0&\forall i\\v_{i}\cdot v_{j}=0\quad (v_{i}\perp v_{2})&\forall i\neq j\end{cases}\Rightarrow\text{ ortogonali}$$Un insieme $\{v_{1},v_{2},\cdots,v_{r}\}$ in uno spazio euclideo $V$ si dice ortonormale se è ortogonale e $||v_{i}||=1$ per ogni $i$ (versore).$$\begin{cases}v_{i}\neq 0&\forall i\\v_{i}\cdot v_{j}=0\quad (v_{i}\perp v_{2})&\forall i\neq j\\||v_{i}||=1&\forall i\end{cases}\Rightarrow\text{ ortonormali}$$

>[!tip]
>Sia $\dim(V)=n$, essendo gli insiemi ortogonali/ortonormali sempre linearmente indipendenti sono basi di $v$.

### Algoritmo di Gram-Schmid
>[!note]
>Per calcolare una base ortonormale partendo da una base qualsiasi si può usare questo algoritmo ricorsivo, detto processo di ortonormalizzazione di Gram-Schmid. $$w_{i}=v_{i}-\sum\limits_{j=1}^{i-1}P_{w_{j}}(v_{i})\quad\text{ per }i=2,\cdots,n$$
>>[!example]
>>1. Scegliere una base $B=\{v_{1},\cdots,v_{n}\}$ dello spazio $v$
>>$$u_{1}=v_{1}$$
>>$$u_{2}=v_{2}-\frac{u_{1}\cdot v_{2}}{||u_{1}||^{2}}u_{1}$$
>>$$u_{n}=v_{n}-\frac{u_{1}\cdot v_{n}}{||u_{1}||^{2}}u_{1}-\cdots -\frac{u_{n-1}\cdot v_{n}}{||u_{n-1}||^{2}}u_{n-1}$$
>>2. L'insieme $\{u_{1},u_{2},\cdots,u_{n}\}$ è un insieme ortogonale.
>>3. Dividendo per il modulo si ottiene una base ortonormale $$\left\{ \frac{u_{1}}{||u_{1}||},\frac{u_{2}}{||u_{2}||},\cdots,\frac{u_{n}}{||u_{n}||} \right\}$$

### Matrici e spazio ortogonale
>[!note]
>Una matrice quadrata si dice ortogonale se $$A^{T}=A^{-1}\iff A^{T}A=I\iff AA^{T}=I$$
>Se $v$ e $w$ sono due vettori colonna allora $v\cdot w=v^{T}w$.
>Una matrice è quindi ortogonale se e solo se le sue colonne formano una base ortonormale di $\mathbb{R}^{n}$.

Si ha che $$R(A)^{\perp}=N(A^{T})$$
### B-espansione di un vettore
>[!note]
>Sia $B=\{q_{1},\cdots,q_{n}\}$ una base ortonormale di uno spazio euclideo $V$ e $v$ un vettore, allora la $B$-espansione del vettore viene definita come $$v=(v\cdot q_{1})q_{1}+\cdots+(v\cdot q_{n})q_{n}$$

### Vettore delle coordinate e matrice di trasformazione lineare ortonormale
>[!note]
>Sia $B=\{q_{1},\cdots,q_{n}\}$ una base ortonormale di uno spazio euclideo $V$, allora il vettore delle coordinate di $v$ nella base $B$ è $$C_{B}(v)=\begin{pmatrix}v\cdot q_{1}\\\vdots\\v\cdot q_{n}\end{pmatrix}$$
>Se $V$ è uno spazio euclideo e $T: V\to V$ è una trasformazione lineare, allora la matrice di $T$ in una base ortonormale $B=\{q_{1},\cdots,q_{n}\}$ è data da $$M_{B}^{B}(T)=C_{B}(T(q_{i}))=\begin{pmatrix}q_{i}\cdot T(q_{j})\\\vdots\\ q_{n}\cdot T(q_{j})\end{pmatrix}\Rightarrow a_{ij}=q_{i}\cdot T(q_{j})$$

### Decomposizione ortogonale di un vettore
>[!note]
>Se $U$ è un sottospazio di uno spazio euclideo $V$, allora $V=U\oplus U^{\perp}$ e questa viene definita decomposizione ortogonale di $V$ rispetto a $U$.

>[!abstract] Conseguenze della decomposizione ortogonale
>$$U=(U^{\perp})^{\perp}\qquad \dim(U^{\perp})=n-\dim(U)$$

### Proiezione ortogonale
>[!note]
>Se $A$ è una matrice $n$x$m$ allora $$\mathbb{R}^{n}=R(A)\oplus N(A^{T})\qquad \mathbb{R}^{m}=N(A)\oplus R(A^{T})$$Se $U$ è un sottospazio di uno spazio euclideo, allora ogni $v\in V$ si decompone in modo unico come $$v=u_{V}+w_{V}\quad u_{V}\in U, w_{V}\in U^{\perp}$$
>La trasformazione lineare $P_{U}:V \to V$ definita ponendo $P_{U}(v)=u_{v}$ è detta proiezione ortogonale su $U$.

### Matrice di proiezione
>[!note]
>La matrice $P_{U}$ di $p_{U}$ nella base canonica è detta matrice di proiezione su $U$.
>Se $B_{U}=\{q_{1},\cdots,q_{n}\}$ è una base ortonormale di $U$, sappiamo che $u_{V}=(v\cdot q_{1})q_{1}+\cdots+(v\cdot q_{r})q_{r}$. Sia $Q$ la matrice $\begin{pmatrix}q_{1}&q_{2}&\cdots&q_{r}\end{pmatrix}$, allora la matrice di proiezione su $u$ è $P_{U}=QQ^{T}$.

Per essere una matrice di proiezione ortogonale è necessario:
- Essere simmetrici: $P_{U}=QQ^{T}$
- Essere idempotenti: $P_{U}^{2}=P_{U}$
- Vale la relazione $P_{U}^{\perp}=I-P_{U}$
- $u\in U\iff P_{U}(u)=u$
- $w\in U^{\perp}\iff P_{U}(w)=\overrightarrow{0}$

### Autovettori ortogonali
>[!note]
>Se $A$ è una matrice quadrata di ordine $n$ simmetrica reale e $v,w$ sono due autovettori di $A$ relativi ad autovalori distinti allora $v$ e $w$ sono ortogonali.

Se la matrice non è simmetrica allora la base di autovalori sicuramente non è ortogonale.

### Teorema spettrale
>[!note]
>Una matrice $A$ reale quadrata di ordine $n$ è simmetrica se e solo se esiste una base ortonormale di $\mathbb{R}^{n}$ formata da autovettori di $A$. In particolare ogni matrice reale simmetrica è diagonalizzabile.
>
>Sia $A$ una matrice quadrata, allora esiste una matrice ortogonale $M$ tale che $$M^{-1}AM=M^{T}AM$$è diagonale se e solo se $A$ è simmetrica.

Quindi per il teorema spettrale $$A\text{ simmetrica}\iff\exists\text{ base ortonormale di autovettori di }A\iff M^{-1}AM=M^{T}AM$$


