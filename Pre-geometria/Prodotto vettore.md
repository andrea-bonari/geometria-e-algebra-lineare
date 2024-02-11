>[!note]
>Il prodotto vettore di due vettori $v$ e $w$ nello spazio è il vettore $v\wedge w$
>- La norma è $||v||||w||\sin(\theta)$ dove $\theta$ è l'angolo minimo tra i due vettori.
>- La direzione è quella ortogonale sia a $v$ che a $w$
>- Il verso è determinato dalla regola della mano destra
>![[Pasted image 20240109105247.png]]

Proprietà:
- Antisimmetrica: $v\wedge w=-w\wedge v$
- Omogeneità: $kv\wedge w=k(v\wedge w)\quad,\quad v\wedge kw=k(v\wedge w)$ 
- Distributività: $(v+w)\wedge u=v\wedge u+w\wedge u\quad,\quad v\wedge(w+u)=v\wedge w+v\wedge u$

### Basi orientate sinistrorse e destrorse
La $n$-upla $\{\overrightarrow{i},\overrightarrow{j},\cdots\}$ di $n$ vettori nel piano/spazio è detta base orientata.

Una base orientata $\{\overrightarrow{i},\overrightarrow{j}\}$ viene detta:
- Destrorsa se l'angolo minimo viene percorso in senso antiorario da $\overrightarrow{i}$ a $\overrightarrow{j}$
- Sinistrorse se l'angolo minimo viene percorso in senso antiorario da $\overrightarrow{j}$ a $\overrightarrow{i}$

Una base orientata $\{\overrightarrow{i},\overrightarrow{j},\overrightarrow{k}\}$ è detta:
- Destrorsa se $\overrightarrow{k}=\overrightarrow{i}\wedge\overrightarrow{j}$
- Sinistrorsa se $\overrightarrow{k}=\overrightarrow{j}\wedge\overrightarrow{i}$

### Espressione analitica del prodotto vettore

L'espressione analitica del prodotto vettore tra $$v=x\overrightarrow{i}+y\overrightarrow{j}+z\overrightarrow{k}\qquad w=x'\overrightarrow{i}+y'\overrightarrow{j}+z'\overrightarrow{k}$$
- ##### Destrorsa
$$v\wedge w=(yz'-y'z)\overrightarrow{i}-(xz'-x'z)\overrightarrow{j}+(xy'-x'y)\overrightarrow{k}$$

- ##### Sinistrorsa
$$v\wedge w=(yz'-y'z)\overrightarrow{i}+(xz'-x'z)\overrightarrow{j}-(xy'-x'y)\overrightarrow{k}$$

>[!tip]
>Siccome la formula non è comoda da ricordare si può imparare, usando un abuso di notazione, come determinante della matrice $3$x$3$
>- Destrorsa: $$v\wedge w=\det\begin{pmatrix}\overrightarrow{i}&\overrightarrow{j}&\overrightarrow{k}\\x&y&z\\x'&y'&z'\end{pmatrix}$$
>- Sinistrorsa: $$v\wedge w=-\det\begin{pmatrix}\overrightarrow{i}&\overrightarrow{j}&\overrightarrow{k}\\x&y&z\\x'&y'&z'\end{pmatrix}$$

