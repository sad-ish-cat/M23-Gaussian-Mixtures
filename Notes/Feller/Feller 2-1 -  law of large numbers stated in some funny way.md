We consider a family of distributions $F_{n, \theta}$ with expectation $\theta$ (so they're all the same) and variance $\sigma_n^2 (\theta)$ where $\theta$ varies in some interval. For expectation we define 
$$\mathbb{E}_{n, \theta} (u) = \int_{-\infty}^\infty u(x) F_{n, \theta}(x) \, dx$$ where I'm pretty sure $F$ is the PDF? idk lmao it's not like they're continuous but if it's a CDF then for large $x$ $F_{n, \theta} \approx 1$ but anyway. Oh man I should go back and read the chapter where they define how distributions work in this book lol

Lemma: 
If $u$ is bounded and continuous and $\sigma^2_n(\theta) \to 0$ for every $\theta$ then $E_{n, \theta}(u) \to u(\theta)$, and the convergence is uniform in every closed interval where $\sigma^2_n(\theta) \to 0$ uniformly, since on a closed interval since $u$ is continuous and bounded it's uniformly continuous and you can see in the proof that $u$ being UC implies the convergence is uniform.  

Proof: 
![[Pasted image 20230525102957.png]]

cf: [[Feller 2-1 use of law of large numbers with binomial distribution]] and afterwards [[difference notation]]