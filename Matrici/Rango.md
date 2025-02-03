 >[!note]
>La dimensione dello spazio colonna $R(A)$ è detta rango di $A$ e la indichiamo con $\text{rk}(A)$ (numero colonne con pivot), quindi se $A$ è di dimensione $n\times m$:
>$$\text{rk}(A)=\dim R(A)=\dim(L(A^{1},A^{2},\cdots,A^{m}))$$
>Il rango è sempre minore del numero di righe e di colonne: $$\text{rk}(A)\leq n\vee\text{rk}(A)\leq m$$

### Spazio nullo
>[!note]
> Lo spazio nullo di una matrice $A$ è $\text{Sol}(A,\overrightarrow{0})$ e lo si indica con $N(A)$ (colonne senza pivot).

### Immagine
>[!note]
>L'immagine di una matrice è lo spazio colonna della matrice e lo si indica con $R(A)$ (colonne con pivot).

### Nullità
>[!note]
>La dimensione dello spazio nullo $N(A)$ è detta nullità di $A$ e si indica con $\text{null}(A)$ (numero colonne senza pivot)

### Teorema nullità più rango
>[!note]
>Considerata una matrice $A$ di dimensioni $n$x$m$ $$\text{null}(A)+\text{rk}(A)=m\quad\text{(numero di colonne)}$$Il teorema è un caso speciale di un teorema più generale detto teorema della dimensione.

### Teorema del rango
>[!note]
>Il rango di una matrice $A$ è uguale al rango della matrice trasposta, in simboli: $$\text{rk}(A)=\text{rk}(A^{T})$$

Di conseguenza:
- La dimensione dello spazio colonna è $\text{rk}(A)$
- Il numero massimo di colonne linearmente indipendenti è $\text{rk}(A)$
- La dimensione dello spazio riga è $\text{rk}(A)$
- Il numero massimo di righe linearmente indipendenti è $\text{rk}(A)$
- Il rango di $A$ di dimensioni $n$x$m$ è minore o uguale a $m$ e $n$

### Calcolo del rango
##### Matrici numeriche
>[!note]
>Siccome il rango di una matrice di $A$ è la dimensione dello spazio riga per calcolare il rango basta ridurre a gradini la matrice. Il numero di pivot rimasti dopo la riduzione è il valore del rango
##### Matrici parametriche - Metodo di Kronecker
>[!note]
>Individuando un minore $M$ con determinante diverso da zero, e calcolando i determinanti di tutti i minori orlati di $M$, se tutti i minori orlati di $M$ hanno determinante nullo allora il rango della matrice è di ordine $M$.

>[!tip] Minore Orlato
>Se $A$ è una matrice $n$x$m$ e $M$ è un minore di $A$ di ordine $r$, un minore orlato di $M$ è un minore di $A$ di ordine $r+1$ che si ottiene aggiungendo a $M$ una riga ed una colonna.