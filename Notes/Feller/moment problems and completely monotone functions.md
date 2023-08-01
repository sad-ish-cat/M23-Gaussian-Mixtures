We now consider functions whose derivatives do alternate in sign, or **competely monotone functions**. 

If we let $F$ be a probability distribution on $[0, 1]$ and denote by $\mathbb{E}(u)$ the integral of $u$ with respect to $F$; then the $k$th moment of $F$ is defined as $$c_k = \mathbb{E}(X^k) = \int_0^1 x^k F \, dx$$
where it's understood that the interval of integration is on the closed interval (although I don't know why that would matter....)

As it turns out we know that $(-1)^r \Delta^r c_k = \mathbb{E} (X^k (1 - X)^{r - k})$ and so the moment sequence $\{c_k\}$ is completely monotone. If $u$ is a continuous function on the closed interval $[0, 1]$ we can integrate the expression 2.1 from [[Feller 2-2 - Bernstein polynomials]] for the bernstein polynomial $B_{n, u}$ with respect to $F$ to get that $$\mathbb{E} (B_{n, u}) = \sum_{j = 0}^n u(jh) {n \choose j} (-1)^{n - j} \Delta^{n - j}c_j = \sum_{j = 0}^n u(jh) p_j^{(n)}$$ where we write $p_j^{(n)} = {n \choose j} (-1)^{n - j} \Delta^{n - j}c_j$. 

If we pick $u(x) = 1$ then the $p_j^{(n)}$ adds to unity, so that for each $n$ they define a probability distribution (!!) with weight $p_j^{(n)}$ at point $jh = j/n$.  

Since by [[Feller 2-1 use of law of large numbers with binomial distribution]] the Bernstein polynomial tends to $u$ we have that $\mathbb{E}_n(u) \to \mathbb{E}(u)$. But actually it turns out that it doesn't matter that we picked $\{c_k\}$ to be the moment sequence of a given distribution $F$; it can actually be an arbitrary completely monotone sequence and define the same $p_j^{(n)}$. By the reciprocity formula from [[difference notation]] we see that 
![[Pasted image 20230525121624.png]]
and taking $u = 1$ the right side becomes $c_0$ and the identity works out fine. 

Then any completely monotone sequence $c_k$ where $c_0 = 1$ defines a probability distribution and the expectation is given by the above equation. When $n \to \infty$, and $u$ a polynomial of degree $N$, we see that $$\mathbb{E}_n(u) \to \sum_{r = 0}^N \frac{c_r}{r!}u^{(r)}(0)$$ and in particular when $u(x) = x^r$ we get that $$\mathbb{E}_n(X^r) \to c_r$$

Weird! The rth moment of the probability distribution $F_n$ tends to $c_r$, and in the funny spot in the limit there is the following theorem: 

**theorem:** 
The moments $c_r$ of a probability distribution function $F$ form a completely monotone sequence with $c_0 = 1$, and conversely an arbitrary completely monotone sequence $c_r$ subject to the norming $c_0 = 1$  coincides with the moment sequence of a unique probability distribution. 

one direction is easy by 3.8 and the "uniform approximation theorem" from [[Feller 2-2 - Bernstein polynomials]] and specifically the approximating polynomials given (I think). 

The other direction is long but if we start from an arbitrary completely monotone sequence $c_k$ we'll have to find the $F$ such that the limit $\mathbb{E}(u)$ coincides with the expectation of $u$ wrt $F$. Here's the proof: 
![[Pasted image 20230525132710.png]]
![[Pasted image 20230525133421.png]]

Fun fact actually: 
If F is an arbitrary probability distribution function on $[0, 1]$ then 3.11 above represents an inversion formula expressing $F$ in terms of its moments; in fact, 
![[Pasted image 20230525134931.png]]

this is so cool!!!! that a distribution with support on $[0, 1]$ can be represented by its moments


