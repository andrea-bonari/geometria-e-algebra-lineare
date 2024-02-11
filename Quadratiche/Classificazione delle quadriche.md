### Forma canonica delle coniche
Applichiamo la classificazione delle quadriche al caso delle coniche.

1.  Caso $\text{rk}(A)=\text{rk}(A_{0})$
	- $\text{rk}(A_{0})=2$ -> l'equazione è del tipo $\lambda_{1}x^{2}+\lambda_{2}y^{2}=0$
		- Autovalori tutti dello stesso segno (ellisse degenere): $$\frac{x^{2}}{a^{2}}+\frac{y^{2}}{b^{2}}=0$$
		- Autovalori con segno discorde (iperbole degenere): $$\frac{x^{2}}{a^{2}}-\frac{y^{2}}{b^{2}}=0$$
	- $\text{rk}(A_{0})=1$ -> l'equazione si riduce a $y^{2}=0$ che è una retta (retta doppia)
2. Caso $\text{rk}(A)=\text{rk}(A_{0})+1$
	- $\text{rk}(A_{0})=2$ -> l'equazione è del tipo $\lambda_{1}x^{2}+\lambda_{2}y^{2}=c$ con $c\neq0$. dividendo per $c$ si ottiene $$rx^{2}+sy^{2}=1$$
		- se $r>0\vee s>0$ ellisse: $$\frac{x^{2}}{a^{2}}+\frac{y^{2}}{b^{2}}=1$$
		- Se $r>0\vee s<0$ iperbole: $$\frac{x^{2}}{a^{2}}- \frac{y^{2}}{b^{2}}=1$$
		- Se $r<0\vee s<0$ insieme vuoto (ellisse immaginaria) $$\frac{x^{2}}{a^{2}}+ \frac{y^{2}}{b^{2}}=-1$$
	- $\text{rk}(A_{0})=1$ -> l'equazione è del tipo $\lambda X^{2}=c$ con $c\neq 0$. Dividendo per $\lambda$ si ottiene $$y^{2}=a$$
		- Se $a<0$ si ha l'insieme vuoto (rette immaginarie)
		- Se $a>0$ si ha una coppia di rette parallele
3. Caso $\text{rk}(A)=\text{rk}(A_{0})+2$
	- $\text{rk}(A_{0})=2$ -> l'equazione è del tipo $\lambda y^{2}=cx$ con $c\neq 0$. Dividendo per $\lambda$ si ottiene una parabola non degenere: $$y^{2}=ax\qquad a>0$$

| Nome | Forma canonica |
| ---- | ---- |
| Ellisse reale | $\frac{x^2}{a^2}+\frac{y^2}{b^2}=1$ |
| Ellisse immaginaria | $\frac{x^2}{a^2}+\frac{y^2}{b^2}=-1$ |
| Iperbole | $\frac{x^2}{a^2}-\frac{y^2}{b^2}=1$ |
| Ellisse degenere (un punto) | $\frac{x^2}{a^2}+\frac{y^2}{b^2}=0$ |
| Iperbole degenere (due rette incidenti) | $\frac{x^2}{a^2}-\frac{y^2}{b^2}=0$ |
| Parabola | $y^2=ax$ |
| Rette parallele  | $y^2=a\qquad a>0$ |
| Rette immaginarie | $y^2=a\qquad a<0$ |
| Retta doppia | $y^2=0$ |

### Forma canonica delle quadriche

| Nome | Forma canonica |
| ---- | ---- |
| Autovalori tutti dello stesso segno: un punto (cono immaginario) | $\lambda_1x^2+\lambda_2y^2+\lambda_3z^2=0$ |
| Cono | $z^2=\frac{x^2}{a^2}+\frac{y^2}{b^2}$ |
| Autovalori con lo stesso segno: una retta | $\lambda_1x^2+\lambda_2y^2=0$ |
| Autovalori con segno discorde: una coppia di piani incidenti | $\lambda_1x^2+\lambda_2y^2=0$ |
| Un piano | $x^2=0$ |
| $a>0\vee b>0\vee c>0$ ellissoide | $ax^2+by^2+cz^2=1$ |
| $a>0\vee b>0\vee c<0$ iperboloide iperbolico | $ax^2+by^2+cz^2=1$ |
| $a>0\vee b<0\vee c<0$ iperboloide ellittico | $ax^2+by^2+cz^2=1$ |
| $a<0\vee b<0\vee c<0$ insieme vuoto (ellissoide immaginario) | $ax^2+by^2+cz^2=1$ |
| $a<0\vee b<0$ insieme vuoto | $ax^2+by^2=1$ |
| $a>0\vee b>0$ cilindro ellittico | $ax^2+by^2=1$ |
| $ab<0$ cilindro iperbolico | $ax^2+by^2=1$ |
| $u>0$ due piani paralleli | $x^2=u$ |
| $u<0$ insieme vuoto (piani immaginari) | $x^2=u$ |
| $a>0\vee b>0$ paraboloide ellittico | $ax^2+by^2=z$ |
| $a>0\vee b<0$ paraboloide iperbolico | $ax^2+by^2=z$ |
| Cilindro parabolico | $x^2=az$ |
