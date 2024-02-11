 ### Vettore differenza
>[!note]
>Sia $\overrightarrow{P_{1}P_{2}}$ il vettore libero rappresentato dal segmento $P_{1}P_{2}$. Il vettore differenza è $$\overrightarrow{P_{1}P_{2}}=(x_{2}-x_{1})\overrightarrow{i}+(y_{2}-y_{1})\overrightarrow{j}+(z_{2}-z_{1})\overrightarrow{k}$$
>Che ha norma $||\overrightarrow{P_{1}P_{2}}||$ .
>![[Pasted image 20240109111848.png]]

### Forma vettoriale della retta
>[!note]
>Dato un punto $P$ e un vettore libero $v$ si indica con $P+v$ il punto $Q$ tale che: $$\overrightarrow{PQ}=\overrightarrow{v}$$Se $P$ ha coordinate $(x_{0},y_{0},z_{0})$ e $v=x\overrightarrow{i}+y\overrightarrow{j}+z\overrightarrow{k}$ allora $$P+\overrightarrow{v}=(x_{0}+x,y_{0}+y,z_{0}+z)$$
>
>Sia $P_{0}$ un punto nel piano o nello spazio e fissiamo un vettore libero $v$. La retta $r$ che passa per $P_{0}$ la cui direzione è determinata da $v$ può essere descritta come l'insieme di punti: $$P=P_{0}+tv$$Questa equazione è detta forma vettoriale della retta $r$. Si noti che $r=P_{0}+L(v)$
>![[Pasted image 20240109112438.png]]

### Equazione parametrica della retta
>[!note]
>Esplicitando $$P_{0}=(x_{0},y_{0},z_{0})\qquad P=(x,y,z)\qquad v=l\overrightarrow{i}+m\overrightarrow{j}+n\overrightarrow{k}$$ Sostituiamo nella forma vettoriale della retta e si ottiene $$\begin{cases}x=x_{0}+tl\\y=y_{0}+tm\\z=z_{0}+tn\end{cases}$$

### Retta passante per due/tre punti
>[!note]
>Nel piano la retta passante per due punti è una sola:
>Dati due punti $P_{0}=(x_{0},y_{0})$ e $P_{1}=(x_{1},y_{1})$ possiamo esprimere la retta come un vettore direzione che congiunge i due punti e un punto stesso $$\begin{cases}x=x_{0}+t(x_{1}-x_{0})\\y=y_{0}+t(y_{1}-y_{0})\end{cases}$$Nello spazio devo considerare tre vettori e un punto per descrivere la retta$$\begin{cases}x=x_{0}+t(x_{1}-x_{0})\\y=y_{0}+t(y_{1}-y_{0})\\z=z_{0}+t(z_{1}-z_{0})\end{cases}$$

### Forma normale della retta
>[!note]
>Data una retta $r$ sia $n$ un vettore normale alla retta.
>Fissato un punto di passaggio $P_{0}=(x_{0},y_{0})$ abbiamo che un punto $P$ sta sulla retta se e solo se $\overrightarrow{P_{0}P}$ è ortogonale a $\overrightarrow{n}$. Otteniamo quindi l'equazione $\overrightarrow{n}\cdot\overrightarrow{P_{0}P}$ che è detta forma normale della retta.
>In simboli $$\overrightarrow{n}=a\overrightarrow{i}+b\overrightarrow{j}$$
>L'equazione cartesiana quindi è $$a(x-x_{0})+b(y-y_{0})=0\Rightarrow ax+bx=c$$

### Equazione cartesiana di una retta nello spazio
>[!note]
>Una retta può anche essere espressa come intersezione di due piani, quindi come insieme delle soluzioni del sistema: $$\begin{cases}a_{1}x+b_{1}y+c_{1}z=d_{1}\\a_{2}x+b_{2}y+c_{2}=d_{2}\end{cases}$$Con la condizione che il sistema abbia $\infty^{1}$ soluzione, quindi $$\text{rk}\begin{pmatrix}a_{1}&b_{1}&c_{1}\\a_{2}&b_{2}&c_{2}\end{pmatrix}=2$$

