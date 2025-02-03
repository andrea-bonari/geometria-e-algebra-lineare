>[!note]
>Indichiamo con $d(P,Q)$ la distanza tra due punti, quindi: $$d(P,Q)=||\overrightarrow{PQ}||$$
>Dati due spazi affini $A,B$ nel piano o nello spazio si definisce la distanza $d(A,B)$ come la minima distanza tra i punti di $A$ e quelli di $B$. In simboli $$d(A,B)=\min_{P\in A, Q\in B}(d(P,Q))$$
>Se $A=P+U$ e $B=Q+W$ sono spazi affini con giaciture $U,W$ rispettivamente allora: $$d(A,B)=||p_{(U+W)^{\perp}}(\overrightarrow{PQ})||$$
 
### Distanza punto-retta nel piano
>[!note]
>Sia $r$ la retta di equazione $ax+by+c=0$. Siccome $\overrightarrow{n}=a\overrightarrow{i}+b\overrightarrow{j}$ è un vettore normale alla retta allora la distanza da $P_{0}$ a $r$ è: $$d(P_{0},r)=||p_{\overrightarrow{n}}(\overrightarrow{PP_{0}})=\frac{|\overrightarrow{PP_{0}}\cdot \overrightarrow{n}|}{||\overrightarrow{n}||}$$
>Esplicitando $P=(x,y)$, $P_{0}=(x_{0},y_{0})$, $\overrightarrow{n}=a\overrightarrow{i}+b\overrightarrow{j}$: $$d(P_{0},r)=\frac{|ax_{0}+by_{0}+c|}{\sqrt{a^{2}+b^{2}}}$$

### Distanza punto-piano
>[!note]
>Consideriamo un punto $P_{0}=(x_{0},y_{0},z_{0})$ e un piano $\alpha: ax+by+cz=d$ in $\mathbb{R}^{3}$, la formula della distanza diventa $$d(P_{0},\alpha)=\frac{|ax_{0}+by_{0}+cz_{0}+d|}{\sqrt{a^{2}+b^{2}+c^{2}}}$$

### Distanza piano-piano paralleli
>[!note]
>Considero due piano paralleli $\alpha_{1},\alpha_{2}$:
>$$\alpha_{1}: a_{1}x+b_{1}y+c_{1}z=d_{1}\quad \alpha_{2}: a_{2}x+b_{2}y+c_{2}z=d_{2}$$
>La formula della distanza tra i due piani paralleli è$$d(\alpha_{1},\alpha_{2})=\frac{|d_{1}-d_{2}|}{\sqrt{a^{2}+b^{2}+c^{2}}}$$

### Distanza retta-retta sghembe
>[!note]
>Date due rette sghembe in forma vettoriale: $$r: P=P_{0}+tv\quad s: P=Q_{0}+tv$$
>Si ha che la minima distanza tra le due rette è la proiezione $\overrightarrow{P_{0}Q_{0}}$ di lungo un vettore ortogonale sia a $v$ che a $w$
>Da questa osservazione si ricava la formula generale $$d(r,s)=\frac{|\overrightarrow{P_{0}Q_{0}}\cdot (v\wedge w)|}{||v\wedge w||}$$
>
>Se consideriamo le rette in forma parametrica: $$r:\begin{cases}x=x_{0}+tl\\y=y_{0}+tm\\z=z_{0}+tn\end{cases}\qquad s:\begin{cases}x=x_{0}'+tl'\\y=y_{0}'+tm'\\z=z_{0}'+tn'\end{cases}$$
>Allora la formula diventa $$d(r,s)=\frac{|\det\begin{pmatrix}x_{0}'-x_{0}&y_{0}'-y_{0}&z_{0}'-z_{0}\\l&m&n\\l'&m'&n'\end{pmatrix}|}{\sqrt{(mn'-m'n)^{2}+(ln'-l'n)^{2}-(lm'-l'm)^{2}}}$$

### Distanza punto-retta nello spazio
>[!note]
>Dato un punto $P$ e una retta in forma vettoriale $r=P_{0}+tv$, allora la distanza del punto dalla retta è data da: $$||\overrightarrow{P_{0}P}||\sin\theta$$
>Dove $\theta$ è l'angolo minimo tra i vettori $\overrightarrow{P_{0}P}$ e $\overrightarrow{v}$.
>La formula per trovare la distanza punto retta in $\mathbb{R}^{3}$ è $$d(P,r)=\frac{||\overrightarrow{P_{0}P}\wedge v||}{||v||}$$ 

### Principio di ortogonalità
>[!note]
>Sia $V$ uno spazio vettoriale e sia $(v\cdot w)$ un prodotto scalare su $V$.
>Sia $U$ un sottospazio di $V$. Allora, dato $v\in V$, il vettore $U$ che minimizza la distanza da $v$ è la proiezione ortogonale di $v$ su $U$. Questo vettore è unico ed è definito come $$\min_{u\in U}||v-u||=||v-p_{U}(v)||=||p_{U^{\perp}}(v)$$