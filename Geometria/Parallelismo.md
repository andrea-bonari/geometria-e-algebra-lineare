>[!note]
>Due spazi affini in $\mathbb{R}^{n}$ si dicono paralleli se la giacitura di uno è contenuta nella giacitura dell'altro.
>
>Ad esempio la retta $r=P+L(v)$ è parallela al piano $\alpha=Q+L(v_{1},v_{2})$ se e solo se $$r||\alpha\iff L(v)\subset L(v_{1},v_{2})$$

>[!abstract] Spazi affini
>Le rette e i piani vengono anche chiamati spazi affini. Se $S=P_{0}+V$ è uno spazio affine allora lo spazio $V$ è chiamato giacitura di $S$.
>
>La dimensione di uno spazio affine è la dimensione della sua giacitura
>- Le rette sono spazi affini di dimensione uno
>- I piani sono spazi affini di dimensione due
>- La massima dimensione in $\mathbb{R}^{n}$ è $(n-1)$

### Due rette in due dimensioni
>[!note]
>Considero due rette $r,s$ nel piano in forma vettoriale:
>$$r=P+tv\quad s=Q+tu\quad v=l\overrightarrow{i}+m\overrightarrow{j}\quad u=l'\overrightarrow{i}+m'\overrightarrow{j}$$
>Che hanno equazione cartesiana$$r: ax+by=c\quad s:a'x+b'y=c'$$
>$$r||s\iff\det\begin{pmatrix}l&m\\l'&m'\end{pmatrix}=0\iff\det\begin{pmatrix}a&b\\a'&b'\end{pmatrix}=0$$

### Due piani in tre dimensioni
>[!note]
>I piani di equazione $\alpha:ax+by+cz=d$ e $\beta: a_{1}x+b_{1}y+c_{1}z=d_{1}$ sono paralleli se hanno la stessa giacitura, quindi se e solo se $$\alpha||\beta\iff\text{rk}\begin{pmatrix}a&b&c\\a_{1}&b_{1}&c_{1}\end{pmatrix}=1$$

### Due rette in tre dimensioni
>[!note]
>Date le rette $r,s$ nello spazio di equazione cartesiana $$r:\begin{cases}a_{1}x+b_{1}y+c_{1}z=d_{1}\\a_{2}x+b_{2}y+c_{2}z=d_{2}\end{cases}\qquad s:\begin{cases}a_{1}'x+b_{1}'y+c_{1}'z=d_{1}'\\a_{2}'x+b_{2}'y+c_{2}'z+d_{2}'\end{cases}$$
>Le rette sono parallele se e solo se: $$r||s\iff \text{rk}\begin{pmatrix}a_{1}&b_{1}&c_{1}\\a_{2}&b_{2}&c_{2}\\a_{1}'&b_{1}'&c_{1}'\\a_{2}'&b_{2}'&c_{2}'\end{pmatrix}=2$$

### Retta e piano in tre dimensioni
>[!note]
>Dato il piano $\alpha$ e la retta $r$ di equazione: $$r: ax+by+cz=d\quad \alpha=\begin{cases}a_{1}x+b_{1}y+c_{1}z=d_{1}\\a_{2}x+b_{2}y+c_{2}z=d_{2}\end{cases}$$
>Il piano e la retta sono paralleli se e solo se $$r||\alpha\iff\det\begin{pmatrix}a&b&c\\a_{1}&b_{1}&c_{1}\\a_{2}&b_{2}&c_{2}\end{pmatrix}=0$$

### Piano con fascio di piani
>[!example]
>Calcolare l'equazione di un piano passante per la retta $r$ e parallelo alla retta $s$
>$$r:\begin{cases}2x+y-z=1\\x+y+2z=0\end{cases}\quad s:\begin{cases}-x+2y+z=1\\x+y+z=-1\end{cases}$$
>L'equazione del fascio di piani è $$\lambda(2x+y-z-1)+\mu(x+y+2z)=0$$
>Imponiamo la condizione del parallelismo con $s$:
>$$\det\begin{pmatrix}2\lambda+\mu&\lambda+\mu&-\lambda+2\mu\\-1&2&1\\1&1&1\end{pmatrix}=0\Rightarrow 7\lambda-3\mu=0$$
>Scegliendo dei valori arbitrari troviamo l'equazione del piano cercato.

