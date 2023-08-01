So the way I think it might work is this: 

We're trying to prove the following theorem, but for [[gaussian mixture definition#multivariate case|multivariate]] GMs: 
![[Pasted image 20230621100201.png]]
we should modify the RHS of the implication to simply be the $p$th power and in the definition of $L_p$ change from the absolute value in the univariate case to being the Euclidean norm in $\mathbb{R}^n$ 

The proof in 1d we've seen already I think in [[rough tkocz paper notes]] but it bears repeating: 
We have the following result for Schur convex functions from $\mathbb{R}^n \to \mathbb{R}$: 
![[Pasted image 20230621100401.png]]

and the actual proof is given by: 
![[Pasted image 20230621100425.png]]
![[Pasted image 20230621100432.png]]


I think the first part of the the proof works approximately the same for the multivariate case, but now instead you can reason as follows: 
For each $X_i$, replace with the corresponding $A_i Z_i$, where $A_i$ is some matrix. 
We know that linear transformations of Gaussians stay Gaussian, and I think sums of multivariate gaussians also stay gaussian (a linear transformation or characteristic functions or something idk) $A_i Z_i + A_j Z_j$ is also gaussian; see: 
![[Pasted image 20230621101350.png]]
in [this post](https://stats.stackexchange.com/questions/9879/addition-of-multivariate-gaussians)

In any case, it has mean 0 again and variance matrix (of dimension $d \times d$ I think) $A_i^T A_i + A_j^T A_j$. I think you need that all the $A_i$ are invertible (?) for them to be positive definite, but if you just want positive semidefinite I don't think you care what they look like, and the sum of two psd matrices is also psd (consider the definition where $u^TAu \geq 0$ and likewise for pd) so this sum winds up being some $C^TC$ (where depending on psd/pd you get that $C$ is invertible as well) and you can find the specific form of $C$ with something something mumble mumble jordan normal form mumble mumble idk I'll figure it out later. 

Anyway now I'm stuck in multiple directions because the tricks that worked for the final equality in the proof break down a little bit here - like, you still can't use the thing where you take $p/2$ as the power, idk. 