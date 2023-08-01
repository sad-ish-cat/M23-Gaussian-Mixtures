The proof relies on the below fact: 
![[Pasted image 20230612231250.png]]
I think, but I'm not sure, that you use that $a \prec b$ means that for a schur convex function $\phi$ we have that $tr \phi(a) \leq tr \phi(b)$. But then I'm not quite sure what to make of the expectation - does it wind up being the integral with respect to some measure? I think the thing I don't understand is that $\phi$ doesn't need to be continuous or anything, so then when you consider the expectation is it like... what. idk I am silly funny goofy at mathematics and idk what's happening. 

Anyway moving on from that you do the rest of the proof as follows: 
![[Pasted image 20230612232236.png]]
![[Pasted image 20230612232243.png]]
I think you fix $p > -1$ so that the expectations are finite, and not equal to $0$ because otherwise this particular proof doesn't quite work - but it's a similar idea, as mentioned at the end. 

If $X_i$ are iid Gaussians then you're on your way to satisfying the theorem; you apply the definition of Gaussian mixture to separate things out into their component parts $Y_i Z_i$ and for some reason you take the step in the second inequality, which I really just don't get. 

Then you pull the expectation for the standard Gaussian out and you're left with something you can apply the above result to, as noted above. 