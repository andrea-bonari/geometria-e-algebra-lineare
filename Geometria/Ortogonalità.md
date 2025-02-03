>[!note] Ortogonalità rette nel piano
>Considero due rette in equazione cartesiana con vettori normali $\overrightarrow{n},\overrightarrow{n'}$ $$r: ax+by+c=0\qquad \overrightarrow{n}=a\overrightarrow{i}+b\overrightarrow{j}\qquad s: a'x+b'y+c'=0\qquad \overrightarrow{n'}=a'\overrightarrow{i}+b'\overrightarrow{j}$$
>$$r:\begin{cases}x=x_{0}+lt\\y=y_{0}+mt\end{cases}\qquad s:\begin{cases}x=x_{0}'+l't\\y=y_{0}'+m't\end{cases}$$
>- Rette in equazione cartesiana
>$$r\perp s\iff \overrightarrow{n}\cdot\overrightarrow{n'}=0\Rightarrow aa'+bb'=0$$
>- Rette in equazione parametrica
>$$v_{r}=\begin{pmatrix}l\\m\end{pmatrix}\quad v_{s}=\begin{pmatrix}l'\\m'\end{pmatrix}$$
>$$r\perp s\iff v_{r}\cdot v_{s}=0\iff ll'+mm'=0$$
>- Parametrica e l'altra in cartesiana
>$$r\perp s\iff \det\begin{pmatrix}a&b\\l&m\end{pmatrix}=0$$

>[!note] Ortogonalità piano-piano
>Due piani sono ortogonali se e solo se i vettori normali sono ortogonali e quindi se i due piani hanno equazione cartesiana $$\alpha: a_{1}x+b_{1}y+c_{1}z=d_{1}\quad \overrightarrow{n_{\alpha}}=a_{1}\overrightarrow{i}+b_{1}\overrightarrow{j}+c_{1}\overrightarrow{k}$$$$\beta: a_{2}x+b_{2}y+c_{2}z=d_{2}\quad \overrightarrow{n_{\beta}}=a_{2}\overrightarrow{i}+b_{2}\overrightarrow{j}+c_{2}\overrightarrow{k}$$
>Allora sono ortogonali se e solo se $$\overrightarrow{n_{\alpha}}\cdot\overrightarrow{n_{\beta}}=a_{1}a_{2}+b_{1}b_{2}+c_{1}c_{2}=0$$

>[!note] Ortogonalità piano-retta
>Un piano e una retta sono ortogonali se il vettore normale al piano è parallelo al vettore direzione della retta. Se sia la retta che il piano sono dati mediante la loro equazione cartesiana.
>$$\alpha: ax+by+cz=d\quad r:\begin{cases}a_{1}x+b_{1}y+c_{1}z=d_{1}\\a_{2}x+b_{2}y+c_{2}z=d_{2}\end{cases}$$
>Allora la condizione di ortogonalità si ricava dal fatto che $\overrightarrow{n_{\alpha}}$ deve essere su una giacitura della retta $r$, quindi $\overrightarrow{n}$ deve essere soluzione del sistema: $$\begin{cases}a_{1}a+b_{1}b+c_{1}c=0\\a_{2}a+b_{2}b+c_{2}c=0\end{cases}$$

>[!note] Ortogonalità retta-retta nello spazio
>Due rette si dicono ortogonali se sono incidenti e i rispettivi vettori direzione sono ortogonali. Se le rette sono date in forma vettoriale $$r=P+tv\quad s=Q+tw$$ allora sono ortogonali se e solo se $$\text{rk}(A,b)<4\qquad v\cdot w=0$$

### Intersezione tra due piani
>[!note]
>Considero la retta descritta dall'intersezione di due piani $$r:\begin{cases}a_{1}x+b_{1}y+c_{1}z=d_{1}\\a_{2}x+b_{2}y+c_{2}z=d_{2}\end{cases}$$Il vettore direzione della retta $r$ è $$\overrightarrow{v}=(a_{1}\overrightarrow{i}+b_{1}\overrightarrow{j}+c_{1}\overrightarrow{z})\wedge(a_{2}\overrightarrow{i}+b_{2}\overrightarrow{j}+c_{2}\overrightarrow{k})$$
