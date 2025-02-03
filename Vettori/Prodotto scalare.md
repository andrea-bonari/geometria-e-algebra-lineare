>[!note]
>Dati due vettori $v$ e $w$ nel piano o nello spazio il loro prodotto scalare è $$v\cdot w=||v||\cdot||w||\cdot\cos(\theta)$$dove $\theta$ è l'angolo tra i due vettori.

>[!abstract] Norma di un vettore
>La norma di un vettore è la lunghezza e si indica con $||v||$. Si trova grazie al teorema di Pitagora, ad esempio la norma del vettore $$||v||=||x\overrightarrow{i}+y\overrightarrow{j}||=\sqrt{x^{2}+y^{2}}$$

>[!tip]
>- Due vettori $v$ e $w$ sono ortogonali se e solo se il loro prodotto scalare è nullo: $v\perp w\iff v\cdot w=0$
>- Norma del prodotto scalare: $||v||=\sqrt{v\cdot v}$
>- Distanza e prodotto scalare: $d(P,Q)=||\overrightarrow{PQ}||=\sqrt{\overrightarrow{PQ}\cdot\overrightarrow{PQ}}$

Possiamo ricavare $\theta$ (angolo minimo tra i vettori $v$ e $w$) usando $$\theta=\arccos\left(\frac{v\cdot w}{||v||\cdot||w||}\right)=\arccos\left(\frac{x_{1}x_{2}+y_{1}y_{2}}{\sqrt{x_{1}^{2}+y_{1}^{2}}\cdot\sqrt{x_{2}^{2}+y_{2}^{2}}}\right)$$
Consideriamo i due vettori $v=x_{1}\overrightarrow{i}+y_{1}\overrightarrow{j}+z_{1}\overrightarrow{k}$ e $w=x_{2}\overrightarrow{i}+y_{2}\overrightarrow{j}+z_{2}\overrightarrow{k}$, il prodotto scalare sarà $$v\cdot w=x_{1}x_{2}+y_{1}y_{2}+z_{1}z_{2}$$
Sia $V$ uno spazio vettoriale. Un prodotto scalare su $V$ è una funzione che associa a ogni coppia di vettori $v$ e $w$ in $V$ un numero reale $v\cdot w$ e tale che valgono le proprietà di simmetria, bilinearità e positività.

>[!abstract] Spazi euclidei
>Uno spazio vettoriale su cui è stato definito un prodotto scalare viene detto spazio euclideo.

### Disuguaglianza di Schwarz
>[!note]
>Se $v$ e $w$ sono vettori in $V$ allora vale la seguente disuguaglianza: $$|v\cdot w|\leq||v||\cdot||w||$$

### Disuguaglianza triangolare
>[!note]
>Se $v$ e $w$ sono $n$-vettori allora vale la seguente disuguaglianza: $$||v+w||\leq||v||+||w||$$
>![[Pasted image 20240106180613.png]]




