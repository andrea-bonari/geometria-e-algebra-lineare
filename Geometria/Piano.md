>[!note]
>Fissiamo un punto $P_{0}$ sul piano $\alpha$ e due vettori $v$ e $w$ non paralleli pere cui le rette passanti per $P_{0}$ aventi direzione $v$ e $w$ giacciono sul piano. $$P\in\alpha\iff P=P_{0}+t_{1}\cdot v+t_{2}\cdot w$$Questa è detta forma vettoriale del piano e i vettori $v$ e $w$ sono detti direzioni del piano. Di fatto abbiamo definito il piano come la combinazione lineare di due vettori applicati su un punto:$$\alpha=P_{0}+L(v,w)$$

### Equazione parametrica del piano nello spazio
>[!note]
>Esplicitando $$P_{0}=(x_{0},y_{0},z_{0})\quad P=(x,y,z)\quad v=l_{1}\overrightarrow{i}+m_{1}\overrightarrow{j}+n_{1}\overrightarrow{k}\quad w=l_{2}\overrightarrow{i}+m_{2}\overrightarrow{j}+n_{2}\overrightarrow{k}$$Sostituiamo nella forma vettoriale del piano e si ottiene$$\begin{cases}x=x_{0}+t_{1}l_{1}+t_{2}l_{2}\\y=y_{0}+t_{1}m_{1}+t_{2}m_{2}\\z=z_{0}+t_{1}n_{1}+t_{2}n_{2}\end{cases}$$
>
>Per verificare che sia un piano basta calcolare $$\text{rk}\begin{pmatrix}l_{1}&m_{1}&n_{1}\\l_{2}&m_{2}&n_{2}\end{pmatrix}=2$$

### Forma normale di un piano nello spazio
>[!note]
>Fissiamo un punto $P_{0}$ appartenente al piano $\alpha$ e sia $\overrightarrow{n}$ un vettore normale al piano. Un punto $P$ sta sul piano $\alpha$ se e solo se: $$\overrightarrow{P_{0}P}\cdot \overrightarrow{n}=0$$
>![[Pasted image 20240109131459.png]]

### Equazione cartesiana di un piano nello spazio
>[!note]
>Se esplicitiamo $$P=(x,y,z)\qquad P_{0}=(x_{0},y_{0},z_{0})\qquad \overrightarrow{n}=a\overrightarrow{i}+b\overrightarrow{j}+c\overrightarrow{k}$$allora la forma normale diventa $$a(x-x_{0})+b(y-y_{0})+c(z-z_{0})=0$$
>Se poniamo $d=ax_{0}+by_{0}+cz_{0}$ troviamo l'equazione cartesiana del piano nello spazio.$$ax+by+cz=d$$
>$a,b,c$ sono detti parametri direttori.

### Piano passante per tre punti non allineati
>[!note]
>Dati tre punti non allineati (vettori associati linearmente indipendenti)
>$$P_{0}=(x_{0},y_{0},z_{0})\qquad P_{1}=(x_{1},y_{1},z_{1})\qquad P_{2}=(x_{2},y_{2},z_{2})$$
>- Equazione parametrica
>$$\begin{cases}x=x_{0}+t_{1}(x_{1}-x_{0})+t_{2}(x_{2}-x_{0})\\y=y_{0}+t_{1}(y_{1}-y_{0})+t_{2}(y_{2}-y_{0})\\z=z_{0}+t_{1}(z_{1}-z_{0})+t_{2}(z_{2}-z_{0})\end{cases}$$
>- Equazione cartesiana
>Valori per cui $$\det\begin{pmatrix}x-x_{0}&y-y_{0}&z-z_{0}\\x_{1}-x_{0}&y_{1}-y_{0}&z_{1}-z_{0}\\x_{2}-x_{0}&y_{2}-y_{0}&z_{2}-z_{0}\end{pmatrix}=0$$
>Se il determinante è nullo i tre punti sono allineati.

### Fascio di piani
>[!note]
>L'insieme dei piani passanti per una retta $r$ è detto fascio di piani di centro $r$
>Se la retta ha equazione $$\begin{cases}a_{1}x+b_{1}y+c_{1}z=d_{1}\\a_{2}x+b_{2}y+c_{2}z=d_{2}\end{cases}$$
>Allora un piano di equazione $ax+by+cz=d$ appartiene al fascio di piani di centro $r$ se e solo se $$\text{rk}\begin{pmatrix}a_{1}&b_{1}&c_{1}&d_{1}\\a_{2}&b_{2}&c_{2}&d_{2}\\a&b&c&d\end{pmatrix}=2$$
>Da cui otteniamo $$ax+by+cz-d=\lambda(a_{1},b_{1},c_{1},d_{1})+\mu(a_{2},b_{2},c_{2},d_{2})$$
>Questa equazione è detta equazione del fascio di piani in quanto al variare di $(\lambda,\mu)\neq\overrightarrow{0}$ descrive tutti i piani appartenenti al fascio.

>[!example]
>Considero il punto $P=(1,1,1)$ e la retta $$\begin{cases}2x+y-z=1\\x+y+2z=0\end{cases}$$
>Il piano cercato appartiene al fascio di piani con centro $r$ e quindi la sua equazione ha forma $$\lambda(2x+y-z-1)+\mu(x+y+2z)=0$$
>Imponiamo il passaggio per $P=(1,1,1)$ e troviamo $\lambda+4\mu=0$
>Ponendo $\mu=1$ (deve essere diverso da 0) si trova $\lambda=-4$, quindi l'equazione del piano è $$-7x-3y+6z=-4$$
