

## Konvergenz im $R^{n}$

Definition: Es sei $\left(a^{(k)}\right)$ eine Folge im $\mathbb{R}^{n}$, also $\left(a^{(k)}\right)=\left(a^{(1)}, a^{(2)}, a^{(3)}, \ldots\right)$ mit $a^{(k)}=$ $\left(a_{1}^{(k)}, \ldots, a_{n}^{(k)}\right) \in \mathbb{R}^{n}(k \in \mathbb{N})$.

a) $\left(a^{(k)}\right)$ heißt beschränkt : $\Longleftrightarrow \exists c \geq 0 \forall k \in \mathbb{N}:\left\|a^{(k)}\right\| \leq c$.

b) Der Begriff Teilfolge (TF) wird wie in HMI definiert.

c) $x_{0} \in \mathbb{R}^{n}$ heißt ein Häufungswert (HW) von $\left(a^{(k)}\right): \Longleftrightarrow$

$$
\forall \varepsilon>0: a^{(k)} \in U_{\varepsilon}\left(x_{0}\right) \text { für unendlich viele } k \in \mathbb{N} \text {. }
$$

d) $\left(a^{(k)}\right)$ heißt konvergent $: \Longleftrightarrow$

$$
\exists a \in \mathbb{R}^{n}:\left\|a^{(k)}-a\right\| \longrightarrow 0 \quad(k \rightarrow \infty) .
$$

In diesem Fall heißt a der Grenzwert ( $G W$ ) oder Limes von $\left(a^{(k)}\right)$ und man schreibt

$$
a=\lim _{k \rightarrow \infty} a^{(k)} \text { oder } a^{(k)} \longrightarrow a(k \rightarrow \infty) \text { oder } a^{(k)} \longrightarrow a .
$$

Wie in HMI zeigt man: Der Grenzwert einer konvergenten Folge ist eindeutig bestimmt.

e) Ist $\left(a^{(k)}\right)$ nicht konvergent, so heißt $\left(a^{(k)}\right)$ divergent.

Beachte:

$$
\begin{gathered}
a^{(k)} \longrightarrow a \quad(k \rightarrow \infty) \\
\Longleftrightarrow \forall \varepsilon>0 \exists k_{0} \in \mathbb{N} \forall k \geq k_{0}:\left\|a^{(k)}-a\right\|<\varepsilon \\
\Longleftrightarrow \forall \varepsilon>0: a^{(k)} \in U_{\varepsilon}(a) \text { für fast alle } k \in \mathbb{N} .
\end{gathered}
$$

Beispiel: Es sei $a^{(k)}:=\left(\frac{1}{k}, 1+\frac{1}{k}\right)(k \in \mathbb{N})$ und $a:=(0,1)$. Es gilt:

$$
\left\|a^{(k)}-a\right\|=\left\|\left(\frac{1}{k}, \frac{1}{k}\right)\right\|=\left(\frac{2}{k^{2}}\right)^{\frac{1}{2}}=\frac{\sqrt{2}}{k} \longrightarrow 0 \quad(k \rightarrow \infty)
$$

Also gilt: $a^{(k)} \longrightarrow(0,1)(k \rightarrow \infty)$

Vereinbarung: Für Elemente des $\mathbb{R}^{2}$ schreiben wir meist $(x, y)$ statt $\left(x_{1}, x_{2}\right)$ und im $\mathbb{R}^{3}$ meist $(x, y, z)$ statt $\left(x_{1}, x_{2}, x_{3}\right)$.

Satz 15.1: Es sei $\left(a^{(k)}\right)$ eine Folge im $\mathbb{R}^{n}, a^{(k)}=\left(a_{1}^{(k)}, \ldots, a_{n}^{(k)}\right)$. Dann gilt:

a) Ist $\left(a^{(k)}\right)$ konvergent, so ist $\left(a^{(k)}\right)$ beschränkt und jede Teilfolge von $\left(a^{(k)}\right)$ konvergiert gegen $\lim _{k \rightarrow \infty} a^{(k)}$.

b) Ist $a=\left(a_{1}, \ldots, a_{n}\right) \in \mathbb{R}^{n}$, so gilt:

$$
a^{(k)} \longrightarrow a(k \rightarrow \infty) \Longleftrightarrow \forall j \in\{1, \ldots, n\}: a_{j}^{(k)} \longrightarrow a_{j}(k \rightarrow \infty)
$$

D.h.: Konvergenz $i m \mathbb{R}^{n}$ ist gleichbedeutend mit koordinatenweiser Konvergenz.

c) Ist $\left(b^{(k)}\right)$ eine weitere Folge im $\mathbb{R}^{n}, a, b \in \mathbb{R}^{n},\left(\beta_{k}\right)$ eine Folge in $\mathbb{R}, \beta \in \mathbb{R}$ und gilt $a^{(k)} \longrightarrow a, b^{(k)} \longrightarrow b$ und $\beta_{k} \longrightarrow \beta$, so gilt:

(i) $a^{(k)}+b^{(k)} \longrightarrow a+b$

(ii) $\beta_{k} a^{(k)} \longrightarrow \beta a$,

(iii) $a^{(k)} \cdot b^{(k)} \longrightarrow a \cdot b$

(iv) $\left\|a^{(k)}\right\| \longrightarrow\|a\|$.

d) Cauchykriterium:

$$
\left(a^{(k)}\right) \text { ist konvergent } \Longleftrightarrow \forall \varepsilon>0 \exists k_{0} \in \mathbb{N} \forall k, l \geq k_{0}:\left\|a^{(k)}-a^{(l)}\right\|<\varepsilon
$$

e) Bolzano-Weierstraß: Ist $\left(a^{(k)}\right)$ beschränkt, so enthält $\left(a^{(k)}\right)$ eine konvergente Teilfolge.

Beweis: a) Wie in HMI.

b) Es sei $j \in\{1, \ldots, n\}$. Nach 14.1 h) gilt:

$$
\forall k \in \mathbb{N}:\left|a_{j}^{(k)}-a_{j}\right| \leq\left\|a^{(k)}-a\right\| \leq \sum_{i=1}^{n}\left|a_{i}^{(k)}-a_{i}\right|
$$

Damit folgt die Behauptung.

c) Folgt aus b)

d),$\Rightarrow$ "Wie in HMI. , $\Leftarrow "$ Übung $($ mit b) und $14.1 \mathrm{~h}))$.

e) Der Übersicht wegen sei $n=2$, also $a^{(k)}=\left(x_{k}, y_{k}\right)(k \in \mathbb{N})$. Es gilt

$$
\left|x_{k}\right| \leq\left\|a^{(k)}\right\|,\left|y_{k}\right| \leq\left\|a^{(k)}\right\| \quad(k \in \mathbb{N})
$$

Also sind $\left(x_{k}\right)$ und $\left(y_{k}\right)$ beschränkte Folgen in $\mathbb{R}$. Nach 2.12 enthält $\left(x_{k}\right)$ eine konvergente Teilfolge $\left(x_{k_{j}}\right)$. Die Folge $\left(y_{k_{j}}\right)$ ist beschränkt. Nach 2.12 enthält $\left(y_{k_{j}}\right)$ eine konvergente Teilfolge $\left(y_{k_{j_{l}}}\right)$. Dann ist auch $\left(x_{k_{j_{l}}}\right)$ konvergent.

Mit b) folgt: $\left(a^{\left(k_{j_{l}}\right)}\right)=\left(\left(x_{k_{j_{l}}}, y_{k_{j_{l}}}\right)\right)$ ist konvergent.

![](https://cdn.mathpix.com/cropped/2023_04_17_432e7474c7eddb656036g-005.jpg?height=51&width=1572&top_left_y=1601&top_left_x=274)
$: \Longleftrightarrow$ Es existiert eine Folge $\left(a^{(k)}\right)$ in $A \backslash\left\{x_{0}\right\}$ mit $a^{(k)} \rightarrow x_{0}(k \rightarrow \infty)$.

\section{Beispiele:}

a) $x_{0}$ ist Häufungspunkt von $U_{1}(0) \Longleftrightarrow x_{0} \in \overline{U_{1}(0)}$.

b) 0 ist Häufungspunkt von $U_{1}(0) \backslash\{0\}$.

c) Endliche Mengen haben keine Häufungspunkte.

Satz 15.2: Es sei $A \subseteq \mathbb{R}^{n}$.

a) Die folgenden Aussagen sind äquivalent:

(i) A ist abgeschlossen. (ii) Für jede konvergente Folge $\left(a^{(k)}\right)$ in $A$ gilt: $\lim _{k \rightarrow \infty} a^{(k)} \in A$.

(iii) Jeder Häufungspunkt von A gehört zu A.

b) $A$ ist kompakt $\Longleftrightarrow$ Jede Folge in A enthält eine konvergente Teilfolge deren Grenzwert zu A gehört.

Ohne Beweis. 

\section{Kapitel 16}

\section{Grenzwerte bei Funktionen, Stetigkeit}

In diesem Kapitel seien stets $n, m \in \mathbb{N}, \emptyset \neq D \subseteq \mathbb{R}^{n}$ und $f: D \rightarrow \mathbb{R}^{m}$ eine (vektorwertige) Funktion. Mit $x=\left(x_{1}, \ldots, x_{n}\right) \in D$ hat $f$ die Darstellung:

$$
f(x)=f\left(x_{1}, \ldots, x_{n}\right)=\left(f_{1}\left(x_{1}, \ldots, x_{n}\right), f_{2}\left(x_{1}, \ldots, x_{n}\right), \ldots, f_{m}\left(x_{1}, \ldots, x_{n}\right)\right)
$$

$\operatorname{mit} f_{j}: D \rightarrow \mathbb{R}(j=1, \ldots, m)$ Kurz: $f=\left(f_{1}, \ldots, f_{m}\right)$

Beispiel: $n=2, m=3, D=\mathbb{R}^{2}, f(x, y)=\left(x y, x+y, x e^{y}\right)$. Also $f=\left(f_{1}, f_{2}, f_{3}\right)$ mit

$$
f_{1}(x, y)=x y, \quad f_{2}(x, y)=x+y, \quad f_{3}(x, y)=x e^{y}
$$

Veranschaulichung möglich im Fall $m=1$ (reellwertige Funktionen), und
a) $n=1$ (bekannt)
b) $n=2$

Definition: Es sei $x_{0} \in \mathbb{R}^{n}$ ein Häufungspunkt von $D$ und $y_{0} \in \mathbb{R}^{m}$.

$\lim _{x \rightarrow x_{0}} f(x)=y_{0}: \Longleftrightarrow$ Für jede Folge $\left(x^{(k)}\right)$ in $D \backslash\left\{x_{0}\right\}$ mit $x^{(k)} \rightarrow x_{0}(k \rightarrow \infty)$ gilt:

$f\left(x^{(k)}\right) \rightarrow y_{0}(k \rightarrow \infty)$

In diesem Fall schreiben wir auch: $f(x) \rightarrow y_{0}\left(x \rightarrow x_{0}\right)$.

Beispiel: Es sei $f=\left(f_{1}, f_{2}, f_{3}\right)$ wie in obigem Beispiel. Es sei $\left(\left(x_{k}, y_{k}\right)\right)$ eine Folge in $\mathbb{R}^{2}$ $\operatorname{mit}\left(x_{k}, y_{k}\right) \rightarrow(1,1)$. Nach 15.1 gilt dann $x_{k} \rightarrow 1, y_{k} \rightarrow 1$, also

$$
f_{1}\left(x_{k}, y_{k}\right)=x_{k} y_{k} \rightarrow 1, f_{2}\left(x_{k}, y_{k}\right)=x_{k}+y_{k} \rightarrow 2, f_{3}\left(x_{k}, y_{k}\right)=x_{k} e^{y_{k}} \rightarrow e
$$

Mit 15.1 folgt: $f\left(x_{k}, y_{k}\right) \rightarrow(1,2, e)$. Also: $\lim _{(x, y) \rightarrow(1,1)} f(x, y)=(1,2, e)$. Beispiel 16.1: $m=1, D=\mathbb{R}^{2}$

$$
f(x, y):= \begin{cases}\frac{x y}{x^{2}+y^{2}}, & (x, y) \neq(0,0) \\ 0, & (x, y)=(0,0)\end{cases}
$$

Es gilt

$$
\begin{aligned}
\left(\frac{1}{k}, 0\right) \rightarrow(0,0), f\left(\frac{1}{k}, 0\right) & =0 \rightarrow 0 \\
\left(\frac{1}{k}, \frac{1}{k}\right) \rightarrow(0,0), f\left(\frac{1}{k}, \frac{1}{k}\right) & =\frac{1}{2} \rightarrow \frac{1}{2} .
\end{aligned}
$$

Damit folgt: $\lim _{(x, y) \rightarrow(0,0)} f(x, y)$ existiert nicht.

Satz 16.2: Es sei $x_{0}$ ein Häufungspunkt von $D \subseteq \mathbb{R}^{n}, f, g: D \rightarrow \mathbb{R}^{m}$ und $h: D \rightarrow \mathbb{R}$ seien Funktionen. Es seien $y_{0}, z_{0} \in \mathbb{R}^{m}$ und $\alpha \in \mathbb{R}$.

a) Ist $f=\left(f_{1}, \ldots, f_{m}\right)$ und $y_{0}=\left(y_{1}, \ldots, y_{m}\right)$, so gilt:

$$
f(x) \rightarrow y_{0}\left(x \rightarrow x_{0}\right) \Longleftrightarrow \forall j \in\{1, \ldots, m\}: f_{j}(x) \rightarrow y_{j}\left(x \rightarrow x_{0}\right)
$$

b) Es gilt:

$\lim _{x \rightarrow x_{0}} f(x)=y_{0} \Longleftrightarrow \forall \varepsilon>0 \exists \delta>0 \forall x \in D \backslash\left\{x_{0}\right\}:\left\|x-x_{0}\right\|<\delta \Rightarrow\left\|f(x)-y_{0}\right\|<\varepsilon$.

c) Es gelte $f(x) \rightarrow y_{0}, g(x) \rightarrow z_{0}$ und $h(x) \rightarrow \alpha\left(x \rightarrow x_{0}\right)$. Dann gilt:

(i) $f(x) \otimes g(x) \rightarrow y_{0} \otimes z_{0}\left(x \rightarrow x_{0}\right)$, wobei $\otimes \in\{+,-, \cdot\}$ („." Skalarprodukt);

(ii) $h(x) f(x) \rightarrow \alpha y_{0}\left(x \rightarrow x_{0}\right)$;

(iii) $\|f(x)\| \rightarrow\left\|y_{0}\right\|\left(x \rightarrow x_{0}\right)$;

(iv) Ist $\alpha \neq 0$ und $h(x) \neq 0(x \in D)$, so gilt:

$$
\frac{1}{h(x)} \rightarrow \frac{1}{\alpha} \quad\left(x \rightarrow x_{0}\right)
$$

Beweis: a) folgt aus 15.1. Den Rest beweist man wie in HMI mit $\|\cdot\|$ statt $|\cdot|$.

\section{Definition:}

a) $f$ heißt in $x_{0} \in D$ stetig : $\Longleftrightarrow$ Für jede Folge $\left(x^{(k)}\right)$ in $D$ mit $x^{(k)} \rightarrow x_{0}$ gilt:

$$
f\left(x^{(k)}\right) \rightarrow f\left(x_{0}\right)
$$

b) $f$ heißt auf $D$ stetig : $\Longleftrightarrow f$ ist in jedem $x \in D$ stetig. In diesem Fall schreiben wir: $f \in C\left(D, \mathbb{R}^{m}\right)$.

Beispiel 16.3: $f$ sei wie in 16.1. Es gilt:

$$
\left(\frac{1}{k}, \frac{1}{k}\right) \rightarrow(0,0), \quad f\left(\frac{1}{k}, \frac{1}{k}\right) \longrightarrow \frac{1}{2} \neq 0=f(0,0)
$$

Also ist $f$ in $(0,0)$ nicht stetig. Aber: Ist $\left(x_{0}, y_{0}\right) \in \mathbb{R}^{2} \backslash\{(0,0)\}$, so ist $f$ in $\left(x_{0}, y_{0}\right)$ stetig.

Satz 16.4: Es sei $x_{0} \in D$ und $f, g: D \rightarrow \mathbb{R}^{m}$ und $h: D \rightarrow \mathbb{R}$ seien Funktionen.

a) $f=\left(f_{1}, \ldots, f_{m}\right)$ ist in $x_{0}$ stetig $\Longleftrightarrow \forall j \in\{1, \ldots, m\}: f_{j}$ ist in $x_{0}$ stetig $\Longleftrightarrow$

$$
\forall \varepsilon>0 \exists \delta>0 \forall x \in D:\left\|x-x_{0}\right\|<\delta \Rightarrow\left\|f(x)-f\left(x_{0}\right)\right\|<\varepsilon
$$

b) Ist $x_{0}$ Häufungspunkt von $D$, so gilt:

$$
f \text { ist stetig in } x_{0} \Longleftrightarrow \lim _{x \rightarrow x_{0}} f(x)=f\left(x_{0}\right)
$$

c) $f, g$ und $h$ seien stetig in $x_{0}$. Dann sind stetig in $x_{0}$ :

(i) $f \otimes g$, wobe $\otimes \in\{+,-, \cdot\}$

(ii) $h f, x \mapsto\|f(x)\|$;

(iii) $\frac{1}{h}($ falls $h(x) \neq 0(x \in D))$.

d) $C\left(D, \mathbb{R}^{m}\right)$ ist ein reeller Vektorraum.

Beweis: 15.1 bzw. wie in HMI.

Definition: $f$ heißt auf $D$ beschränkt $\Longleftrightarrow \exists \exists M 0 \forall x \in D:\|f(x)\| \leq M$.

Wie in HMI zeigt man:

Satz 16.5: a) Es sei $f: D \rightarrow \mathbb{R}^{m}$ in $x_{0} \in D$ stetig, $E \subseteq \mathbb{R}^{m}, f(D) \subseteq E$ und es sei $g: E \rightarrow \mathbb{R}^{p}$ stetig in $f\left(x_{0}\right)$. Dann ist

$$
g \circ f: D \longrightarrow \mathbb{R}^{p}
$$

stetig in $x_{0}$.

b) Es sei $D$ kompakt und $f \in C\left(D, \mathbb{R}^{m}\right)$. Dann gilt:

(i) $f(D)$ ist kompakt, insbesondere ist $f$ beschränkt.

(ii) Ist $m=1$, so existieren $x_{1}, x_{2} \in D$ mit

$$
f\left(x_{1}\right) \leq f(x) \leq f\left(x_{2}\right) \quad(x \in D)
$$

Satz 16.6: Es sei $f: \mathbb{R}^{n} \rightarrow \mathbb{R}^{m}$ linear. Dann gilt:

$$
f \in C\left(\mathbb{R}^{n}, \mathbb{R}^{m}\right)
$$

Beweis: Es existiert eine reelle $m \times n$-Matrix $A$ mit $f(x)=A x\left(x \in \mathbb{R}^{n}\right)$. Es sei $x_{0} \in \mathbb{R}^{n}$. Dann gilt:

$$
\left\|f(x)-f\left(x_{0}\right)\right\|=\left\|A x-A x_{0}\right\|=\left\|A\left(x-x_{0}\right)\right\| \stackrel{\S 14}{\leq}\|A\|\left\|x-x_{0}\right\|
$$

Also: $f(x) \rightarrow f\left(x_{0}\right)\left(x \rightarrow x_{0}\right)$.

Beispiel: $f: \mathbb{R}^{2} \rightarrow \mathbb{R}, f(x, y)=x+y$ ist stetig auf $\mathbb{R}^{2}$. 