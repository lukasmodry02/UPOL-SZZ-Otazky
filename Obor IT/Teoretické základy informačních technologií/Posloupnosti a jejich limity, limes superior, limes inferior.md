## Posloupnost
- Každé zobrazení $f: \mathbb{N} \to A$ nazýváme **číselná posloupnost**
	- kde $A$ je libovolná množina libovolných objektů
	- pokud je obor hodnot číselný, pak mluvíme o **číselné posloupnosti**
- Posloupnost je **konečná**, jestliže je definičním oborem množina $\{1, 2, ..., k\}$, kde $k \in \mathbb{N}$
	- takové posloupnosti označujeme jako *uspořádáné $n$-tice*
- **Funkční hodnotu** funkce $f$ v bodě $n$ nazýváme $n$**-tý člen** posloupnosti a značíme $a_{n},\   b_{n}$ apod.
- **Posloupnost s $n$-tým členem** pak zapisujeme $(a_{n})^{\infty}_{n=1}$ nebo jen $(a_{n})$
- Neformálně lze chápat jako kolekci hodnot, ve které jsou prvky dány svým pořadím (sekvence)

### Způsoby zadání posloupnosti
- Číselná posloupnost bývá zadána:
	1. **Několika prvními členy** 
		- z kterých jsou zřejmé následující členy $$\frac{1}{1 \cdot 4}, \frac{3}{4 \cdot 7}, \frac{5}{7 \cdot 10}, \frac{7}{10 \cdot 13}, ...$$
	1. **Předpisem vyjadřující n-tý člen** $$a_n = \left(\frac{n}{n+1}\right)^\infty,a_n=  \left( (-1)^{n}n \right)^\infty,\ a_n = \left( \left(1 + \frac{1}{n}\right)^{n} \right)^\infty$$
	2. **Rekurentně**
		- Členy posloupnosti jsou určeny pomocí jednoho nebo více předcházejících členů
		- Typickým příkladem je Fibonacciho posloupnost: $$a_1=0, a_2=1, a_{n+2}=a_{n+1}+a_n$$
### Podposloupnost
- Posloupnost $(b_{n})$ se nazývá **podposloupnost** $(a_{n})$, právě když existuje posloupnost přirozených čísel $k_{1} < k_{2} < k_{3} < ...$ tak, že $\forall{n \in \mathbb{N}}$ je $b_{n} = a_{kn}$.

## Speciální posloupnosti
### Aritmetická posloupnost
- Posloupnost $(a_n)_{n=1}^{\infty}$ se nazývá **aritmetická**, právě když existuje číslo $d \in \mathbb{R}$ takové, že pro každé $n \in \mathbb{N}$ platí
$$
a_{n+1} = a_n + d. \tag{6.1}
$$

- Číslo $d$ nazýváme *diference* aritmetické posloupnosti.

### Geometrická posloupnost
- Posloupnost $(a_n)_{n=1}^{\infty}$ se nazývá **geometrická**, právě když existuje takové $q \in \mathbb{R}$, že pro libovolné $n \in \mathbb{N}$ platí
$$
a_{n+1} = a_n \cdot q. \tag{6.3}
$$

- Číslo $q$ nazýváme *kvocientem* geometrické posloupnosti.


## Monotónnost posloupnosti
- Posloupnost $(a_n)_{n=1}^{\infty}$ se nazývá
$$
\left\{
\begin{array}{l}
\text{rostoucí} \\
\text{klesající} \\
\text{nerostoucí} \\
\text{neklesající} \\
\text{konstantní}
\end{array}
\right.
\text{ je-li pro všechna } n \in \mathbb{N}
\left\{
\begin{array}{l}
a_{n+1} > a_n \\
a_{n+1} < a_n \\
a_{n+1} \le a_n \\
a_{n+1} \ge a_n \\
a_{n+1} = a_n
\end{array}
\right.
$$
- Má-li posloupnost některou z prvních 4 vlastností, nazýváme ji **monotónní**.
- Je-li posloupnost rostoucí nebo klesající, nazýváme ji **ryze monotónní**

## Omezenost posloupnosti
- Posloupnost $(a_n)_{n=1}^{\infty}$ se nazývá
$$
\left\{
\begin{array}{l}
\text{shora omezená} \\
\text{zdola omezená}
\end{array}
\right.
\text{, existuje-li takové číslo}
\left\{
\begin{array}{l}
H \in \mathbb{R} \\
D \in \mathbb{R}
\end{array}
\right.
\text{, že pro každé } n \in \mathbb{N} \text{ je}
\left\{
\begin{array}{l}
a_n \leq H \\
a_n \geq D
\end{array}
\right.
$$

## Limity posloupnosti
- Zkoumáme chování posloupnosti pro velká přirozená čísla
- Jedná se o hodnotu, ke které se posloupnost přibližuje, postupuje-li do nekonečna

### Konečné limity posloupnosti
>[!text] Definice
>Číslo $a \in \mathbb{R}$ se nazývá **limita posloupnosti** $(a_n)_{n=1}^{\infty}$ právě když $$\forall \epsilon > 0 \ \exists n_{0}; \forall n > n_{0}: |a_{n}-A|< \epsilon$$
>![[MacBook-2024-08-18-001933.png]]
- Píšeme $\lim_{{n \to \infty}} a_n = a$
- Takovou posloupnosti $(a_n)_{n=1}^{\infty}$ pak nazýváme **konvergentní**
	- říkáme že posloupnost $(a_n)_{n=1}^{\infty}$ konverguje k $a$
	- např. geometrická posloupnost $(a_n)_{n=1}^\infty$, pro jejíž kvocient $q$ platí $|q| < 1$ , je konvergentní a  $\lim_{{n \to \infty}} a_n = 0$, konverguje tedy k $0$
- Místo $\lim_{{n \to \infty}} = a$ píšeme také $a_{n} \to a$, čteme posloupnost $a_n$ **konverguje** ke své limitě $a$ 

### Nekonečné limity posloupnosti
- Posloupnost $a_n$, která nemá konečnou limitu, nazýváme **divergentní**

>[!def] Definice
>Říkáme, že posloupnost $(a_n)_{n=1}^{\infty}$ má limitu $+\infty$, právě když $$\forall K \ \exists n_{0} \in \mathbb{N}; \forall n \geq n_{0}: a_{n} > K$$
>Píšeme $\lim_{{n \to \infty}} a_n = +\infty$.
>Analogicky definiujeme $-\infty$.

### Vlastnosti limit 

>[!info] Vlastnosti limit
>1. Každá posloupnost má nejvýše jednu limitu.
>	- posloupnost **buď limitu nemá** (je **divergentní**) nebo **má právě jednu**
>2. Každá konvergentní posloupnost **je omezená**
>3. Nechť $(a_{n})_{n=1}^{\infty}$ a $(b_{n})_{n=1}^{\infty}$ **jsou konvergentní posloupnosti** a nechť $\lim_{x \rightarrow \infty}(a_{n})=a$ a $\lim_{n \rightarrow \infty} (b_{n}) = b$.
>	i) $\lim_{x \rightarrow \infty}(a_{n} \pm b_{n}) = \lim_{n \rightarrow \infty}(a_{n}) \pm \lim_{n \rightarrow \infty} (b_{n}) = a \pm b$
>	ii) $\lim_{x \rightarrow \infty} (a_{n} \cdot b_{n}) = \lim_{n \rightarrow \infty}(a_{n}) \cdot \lim_{n \rightarrow \infty}(b_{n}) = a \cdot b$
>	iii) $\lim_{x \rightarrow \infty} (\frac{a_{n}}{b_{n}}) = \frac{\lim_{x \rightarrow \infty}(a_{n})}{\lim_{x \rightarrow \infty}(b_{n})} = \frac{a}{b}$ (pro $b \neq 0$; $\forall n \in \mathbb{N}: b_{n} \neq 0$)
>	iv) $\lim_{x \rightarrow \infty}(c \cdot a_{n}) = c \cdot \lim_{x \rightarrow \infty}(a_{n}) = c \cdot a ($pro $c \in \mathbb{R}, c \neq 0)$

>[!Example]- Isibalo - Věty o limitách posloupností
><iframe width="660" height="385" src="https://www.youtube.com/embed/VvBPNeOYQdI?si=KeYNvbsj0alltZ8g" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
## Limes inferior a Limes superior
- Tyto pojmy můžeme chápat jako omezení zespoda a seshora pro hodně velké $n$ (v nekonečnu)
- Posloupnost těchto mezí buďto nabývá nebo se nekonečně blíží v konečném počtu případů
- Na rozdíl od limity, limes inferior i limes superior vždy existují
	- Limita posloupnost existuje, jestliže $\limsup a_n = \liminf a_n$
- $\liminf_{n \to \infty} a_n \leq \limsup_{n \to \infty} a_n$
- $\liminf_{n \to \infty} a_n = \limsup_{n \to \infty} (-a_n)$

![[limes-inf-sup.png | 400]]
### Limes superior
- Nechť $(a_n)_{n \in \mathbb{N}}$ je posloupnost reálných čísel. Pak definujeme
$$
\limsup a_n := 
\begin{cases} 
\lim_{n \to \infty} \sup \{a_k; k \geq n\}, & \text{jestliže je } a_n \text{ shora omezená} \\
\infty, & \text{jestliže je } a_n \text{ shora neomezená}.
\end{cases}
$$

- Tuto hodnotu nazýváme **limes superior** posloupnosti $\{a_n\}_{n \in \mathbb{N}}$. 
- Alternativní zápis: $$\limsup a_n := \lim_{n \to \infty} (\sup_{k \geq n} a_k)$$
### Limes inferior
- Nechť $(a_n)_{n \in \mathbb{N}}$ je posloupnost reálných čísel. Pak definujeme$$
\liminf a_n := 
\begin{cases} 
\lim_{n \to \infty} \inf \{a_k; k \geq n\}, & \text{jestliže je } a_n \text{ zdola omezená} \\
-\infty, & \text{jestliže je } a_n \text{ zdola neomezená}.
\end{cases}$$
- Tuto hodnotu nazýváme **limes inferior** posloupnosti $\{a_n\}_{n \in \mathbb{N}}$. 
- Alternativní zápis: $$\liminf a_n := \lim_{n \to \infty} (\inf_{k \geq n} a_k)$$

##### Navigace

Předchozí: [[Funkce jedné reálné proměnné, základní vlastnosti]]
Následující: [[Limita funkce včetně nevlastních, jednostranné limity]]
Celý okruh: [[1. Teoretické základy informačních technologií]]
