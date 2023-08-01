yeah so the notes start on page 224 I think of the notes below: 
A family of random variables $X_t$ for $t \in T$ is uniformly integrable if for every $\varepsilon$ there is $K > 0$ such that for all $t$, we have $\mathbb{E}|X_{t}|\mathbb{1}_{|X_{t}| > K} \leq \varepsilon$ 

I think what this means is basically that there isn't too much probability mass relegated to very large values of $X_t$, so that the random variables are close to having the same expectation, because they don't seem too funny in the tails 

There are two nice lemmas characterizing uniform integrability
![[Pasted image 20230608195816.png]]
![[Pasted image 20230608195833.png]]


and this is the definition that perhaps explains the name better (and which chatGPT gave lmfao):
![[Pasted image 20230608195858.png]]


The best part of uniform convergence is that it captures convergence in $L_p$ - it's a way to get from the weak convergence in probability (and depending on the scenario, in distribution, where you have that the sequence converges to a constant so distribution -> probability): 
![[Pasted image 20230608204759.png]]


![[prob-grad-notes.pdf]]

