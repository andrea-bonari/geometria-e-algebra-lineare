 >[!note]
>Una quadrica è il luogo di punti definito nel piano o nello spazio definito da un'equazione di secondo grado: $$p(x_{1},\cdots,x_{n})=0\text{ con }p(x_{1},\cdots,x_{n})=\sum\limits_{i\leq j}a_{ij}x_{i}x_{j}+\sum\limits b_{i}x_{i}+f$$
>
>In base al valore di $n$ le quadriche assumono diversi nomi:
>- Coniche: $n=2$
>- Cubiche: $n=3$
>- Quadratiche: $n=4$

### Sfere
>[!note]
>La sfera di centro $(x_{0},y_{0},z_{0})$ e di raggio $R$ è il luogo di punti di equazione: $$(x-x_{0})^{2}+(y-y_{0})^{2}+(z-z_{0})^{2}=R^{2}$$

### Cono
>[!note]
>Un cono è una superficie per ogni punto della quale passa una retta $g$ tutta contenuta nella superficie e passante per un punto fisso $V$, detto vertice del cono. Le rette $g$ si dicono generatrici del cono, mentre una curva che interseca tutte le generatrici in un punto è detta direttrice del cono.
>
>Un cono quadrico è un cono che è anche una superficie quadrica.
>

>[!example]
>$$x^{2}+y^{2}-z^{2}=0$$
>È il cono quadrico con vertice l'origine e come direttrice la circonferenza di raggio $1$ centro $(0,0,1)$ giacente nel piano $z=1$

### Cilindro
>[!note]
>Chiamiamo cilindro una superficie per ogni punto della quale passa una retta $g$ di direzione assegnata tutta contenuta nella superficie. Le rette $g$ si dicono generatrici del cilindro, mentre una curva che interseca tutte le generatrici in un punto è detta direttrice del cilindro.
>
>Un cilindro quadrico è un cilindro che è anche una superficie quadrica.

>[!example]
>$$x^{2}+y^{2}-1=0$$
>È un cilindro quadrico con generatrici parallele all'asse $z$ e direttrice la circonferenza di raggio $1$ centro $(0,0,0)$ giacente nel piano $z=0$

### Superfici di rotazione
>[!note]
>Data una curva $\gamma$ e una retta $r$ la superficie descritta da i punti di $\gamma$ durante una rotazione di $2\pi$ attorno alla retta $r$ si dice superficie di rotazione generata da $\gamma$ e $r$ si dice asse di rotazione.
>
>Le quadriche di rotazione sono le superfici quadriche che sono anche superfici di rotazione.

### Isometrie
>[!note]
>Un isometria su $\mathbb{R}^{n}$ è una funzione $F:\mathbb{R}^{n}\to\mathbb{R}^{n}$ che rispetta la distanza tra i punti $$d(F(P),F(Q))=d(F,Q)$$

### Isometrie lineari
>[!note]
>Un isometria lineare di $\mathbb{R}^{n}$ è una trasformazione lineare $T$ tale che: $$T(x)\cdot T(y)=x\cdot y$$
>
>Le proprietà delle isometrie lineari sono:
>- Preserva la norma $$||T(x)||=||x||$$
>- Preserva gli angoli $$\widehat{T(x)T(y)}=\widehat{xy}$$
>- Preserva la distanza tra i punti $$d(T(P),T(Q))=d(P,Q)$$

La trasformazione lineare $T$ è un'isometria lineare se e solo se la sua matrice $A$ è una matrice ortogonale.

Le isometrie lineari nel piano ($\mathbb{R}^{2}$) sono: $$A=\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix}\qquad A=\begin{pmatrix}\cos\theta&\sin\theta\\\sin\theta&-\cos\theta\end{pmatrix}$$
### Traslazione
>[!note]
>Dato un vettore $v$, la traslazione $T_{v}$ è una funzione definita ponendo: $$T_{v}(P)=P+v$$
>Se il vettore $v\neq \overrightarrow{0}$ allora la traslazione $T_{v}$ non è lineare poiché $T(\overrightarrow{0})=v\neq\overrightarrow{0}$, tuttavia le traslazioni sono comunque isometrie

### Rototraslazione
>[!note]
>Una rototraslazione è un'isometria lineare seguita da una traslazione. Sia $R=T_{v}\circ T$ una rototraslazione con $T$ isometria lineare (rotazione) e $T_{v}$ l'isometria non lineare (traslazione). Sia $A$ la matrice di $T$ (rotazione) nella base canonica. Allora $$R(X)=T_{v}(AX)=AX+v$$
>
>Proprietà:
>- siccome $T$ è un isometria lineare, $A$ è ortogonale.
>- L'isometria lineare $T$ è anche detta parte lineare di $R$.
>- Si può dimostrare che tutte le isometrie del piano o dello spazio sono rototraslazioni.

>[!abstract] Composta di isometrie
>La composta di due isometrie $F$ e $G$ è ancora un isometria $$d(F\circ G(P), F\circ G(Q))=d(P,Q)$$

Se $R=T_{v}\circ T$ è una rototraslazione con parte lineare $T$ e $M_{0}$ è la matrice di $T$ allora la matrice associata alla rototraslazione $R$ è: $$M=\begin{pmatrix}M_{0}&v\\\overrightarrow{0}&1\end{pmatrix}$$

L'inversa $R^{-1}$ di una rototraslazione $R$ è anch'essa una rototraslazione. Se $R(X)=T_{v}(AX)=AX+v$ è una rototraslazione all'ora l'inversa è: $$R^{-1}=A^{-1}(X-1)=T_{-A^{-1v}}A^{-1}X$$
Se $R$ ha matrice $\begin{pmatrix}M_{0}&v\\\overrightarrow{0}&1\end{pmatrix}$ allora $R^{-1}$ ha matrice: $$\begin{pmatrix}M_{0}^{-1}&-M_{0}^{-1}v\\\overrightarrow{0}&1\end{pmatrix}=\begin{pmatrix}M_{0}^{T}&-M_{0}^{T}v\\\overrightarrow{0}&1\end{pmatrix}$$

