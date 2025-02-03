>[!note]
>Dati due spazi vettoriali $V$ e $W$, una trasformazione lineare da $V$ in $W$ è una funzione $f: A\to B$ tale che dati $v_{1},v_{2}\in V$ e $t\in\mathbb{R}$: $$f(v_{1}+v_{2})=f(v_{1})+f(v_{2})\qquad f(t\cdot v_{1})=t\cdot f(v_{1})$$

Le trasformazioni lineari si indicano con la lettera maiuscola.

>[!tip]
>Ogni trasformazione lineare conserva il vettore nullo, cioè: $$T(\overrightarrow{0})=\overrightarrow{0}$$

Data una matrice $A$ di dimensioni $n\times m$ è una trasformazione lineare la funzione definita ponendo: $$T_{A}: \mathbb{R}^{m}\to \mathbb{R}^{n}\qquad T_{A}(X)=A\cdot X$$
### Tipologie particolari di funzioni
>[!note] Funzione composta
>Data una funzione $f: A\to B$ e una funzione $g: B\to C$, la funzione $h= g\circ f$ è definita come $h: A\to C$ e corrisponde a $g(f(x))$.

>[!note] Funzione invertibile
>Una funzione $f: A\to B$ viene definita invertibile se esiste una funzione $g: B\to A$ tale che $g\circ f=I_{A}$ E $f\circ g=I_{B}$. Una funzione è invertibile solo se è biiettiva.

### Nucleo e immagine
>[!note]
>In una trasformazione lineare i vettori del codominio sono i trasformati del dominio. Se $T: V\to W$ è una trasformazione lineare, allora è chiamato nucleo di $T$ l'insieme: $$\ker(T)=\{v\in V\quad |\quad T(v)=\overrightarrow{0}\}$$L'insieme immagine di una trasformazione lineare $T$ è $$\text{im}(T)=\{w\in W,\exists v\in V\quad | w=T(v)\}$$

Il nucleo e l'immagine di una trasformazione lineare $T: V\to W$ sono sottospazi vettoriali rispettivamente di $V$ e di $W$.

- Il nucleo di $T_{A}$ è lo spazio colonna nullo di $A$: $\ker(T_{A})=N(A)\Rightarrow \dim(\ker(T_{A}))=\text{null}(A)$
- L'immagine di $T_{A}$ è lo spazio colonna di $A$: $\text{im}(T_{A})=R(A)\Rightarrow \dim(\text{im}(T_{A}))=\text{rk}(A)$

### Teorema della dimensione
>[!note]
>Come conseguenza del teorema di nullità più rango, se $T: V\to W$ è una trasformazione lineare tra due spazi vettoriali e $V$ è di dimensione finita, allora:
>- $\text{im}(T)$ è di dimensione finita.
>- $\dim(V)=\dim(\ker((T)))+\dim(\text{im}(T))$

>[!abstract] Conseguenze del teorema della dimensione
>Siano $V$ e $W$ spazi vettoriali di dimensione finita e $T: V\to W$ una trasformazione lineare, allora:
>1. Se $T$ è iniettiva allora $\dim(V)\leq\dim(W)$.
>2. Se $T$ è suriettiva allora $\dim(V)\geq\dim(W)$.
>3. Se $\dim(V)=\dim(W)$ allora $T$ è iniettiva se e solo se è biiettiva.
>4. Se $\dim(V)=\dim(W)$ allora $T$ è suriettiva se e solo se è biiettiva.

### Composta di trasformazioni lineari
>[!note]
>Se $T: V\to W$ e $S:W\to U$ sono trasformazioni lineari, allora $(S\circ T): V\to U$ è una trasformazione lineare. $$(S\circ T)(v)=S(T(v))$$

### Inversa di trasformazione lineare
>[!note]
>Se $T: V\to W$ è una trasformazione lineare biiettiva (quindi invertibile) allora $T^{-1}: W\to V$ è lineare.

Per essere invertibile una matrice $A$ deve essere quadrata e con $\det(A)\neq0$.
Inoltre vale anche $T^{-1}_{A}=T_{A^{-1}}$
