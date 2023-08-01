**definition:** 
If $F$ is a proper or [[defective probability distribution]] concentrated on $[0, \infty)$ then the **Laplace transform** $\varphi$ of $F$ is the function defined for $\lambda \geq 0$ by $$\varphi(\lambda) = \int_0^\infty e^{-\lambda x} F\{dx\} = \mathbb{E}(e^{-\lambda X})$$
where we assume that $X$ is nonnegative as above so that the expected value makes sense. 

**theorem 1:** Distinct probability distributions have distinct Laplace transforms. 
Proof: Mostly by change of variables I think: ![[Pasted image 20230529130251.png]]

One consequence of the above theorem is the following theorem: 
**Theorem 2:** For $n = 1, 2, 3 \dots$ let $F_n$ be a probability distribution with Laplace transform $\varphi_n$. Furthermore, if $F_n \to F$ where $F$ is a possibly defective distribution with transform $\varphi$ then $\varphi_n(\lambda) \to \varphi(\lambda)$ for all positive $\lambda$. 
Conversely, if the sequence $\{\varphi_n(\lambda)\}_n$ converges for each $\lambda > 0$ to a limit $\varphi(\lambda)$, then $\varphi$ is the transform of a possibly defective distribution $F$ with $F_n \to F$. The limiting distribution $F$ is not defective iff $\varphi(\lambda) \to 1$ as $\lambda \to 0$. 

In other words, if we have some family of random variables $X_n$ with distributions $F_n$ that converge in distribution to $X$ with distribution $F$ then their Laplace transforms converge for all $\lambda > 0$, and if you happen to have a bunch of weird looking Laplace transforms that converge then their distributions will cough up a limiting distribution $F$. 


### properties of the Laplace transform: 
- Convolutions: Let $F$ and $G$ be probability distributions and $U$ their convolution, ie $$U(x) = \int_0^x G(x - y) F\{dy\}$$ then the corresponding Laplace transformations obey the multiplication rule, ie $\omega = \varphi \gamma$ where $\varphi$ and $\gamma$ are the Laplace transforms of $F$ and $G$, and $\omega$ is that of $U$. If $F$ and $G$ have densities $f$ and $g$ then it simplifies into the convolution you've seen before, $$u(x) = \int_0^x g(x - y) f(y) \, dy$$
- If $F$ is a probability distribution and $\varphi$ its Laplace transform then $\varphi$ possesses derivatives of all orders given by $(-1)^n \varphi^(n)(\lambda) = \int_0^\infty e^{-\lambda x} x^n F\{dx\}$. Then in particular $F$ possesses a finite $n$th moment iff a finite limit $\phi^{(n)}(0)$ exists!! This is looking suspiciously like the expressions in [[Feller 2-2 - Bernstein polynomials]]. 

