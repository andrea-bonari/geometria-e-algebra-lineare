>[!note]
>Un sottospazio di uno spazio vettoriale $V$ è un sottoinsieme non vuoto $W$ di $V$ tale che:
>- Se $v,w$ sono in $W$ allora anche $v+w$ è in $W$ (chiuso alla somma)
>- Se $v$ è in $W$ e $t$ è un numero allora $tv$ è in $W$ (chiuso rispetto al prodotto per scalare)

>[!tip]
>- Se $V$ è uno spazio vettoriale allora $V$ è sottospazio di se stesso e $\{\overrightarrow{0}\}$ è un sottospazio di $V$.
>- Il vettore $\overrightarrow{0}$ appartiene ad ogni sottospazio.
>- Ogni proprietà che vale per gli spazi vettoriali vale anche per tutti i sottospazi.

### Combinazioni e dipendenza lineare
>[!note]
>In uno spazio vettoriale si dice che il vettore $v$ è combinazione lineare dei vettori $v_{1},v_{2},\cdots,v_{k}$ se $$v=a_{1}\cdot v_{1}+a_{2}\cdot v_{2}+\cdots+a_{k}\cdot v_{k}$$con $a_{1},a_{2},\cdots,a_{k}$ numeri reali.

I vettori $v_{1},v_{2},\cdots,v_{k}$ si dicono linearmente dipendenti se esiste una combinazione lineare di $v_{1},v_{2},\cdots,v_{k}$ con coefficienti non tutti nulli.

### Spazi e insiemi generati
>[!note]
>L'insieme di tutte le combinazioni lineari dei vettori $v_{1},v_{2},\cdots,v_{k}$ viene chiamato lo spazio generato da $v_{1},v_{2},\cdots,v_{k}$ e lo si indica con $$L(v_{1},v_{2},\cdots,v_{k})\qquad<v_{1},v_{2},\cdots,v_{k}>\qquad\text{span}(v_{1},v_{2},\cdots,v_{k})$$

Diremo che $\{v_{1},v_{2},\cdots,v_{k}\}$ è un insieme di generatori per lo spazio $V$ se $L(v_{1},v_{2},\cdots,v_{k})=V$.
