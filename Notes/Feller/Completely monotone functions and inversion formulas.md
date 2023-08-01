Recall from [[moment problems and completely monotone functions]] that a function is completely monotone if it possesses derivatives of all orders and they alternate sign, ie $(-1)^n \varphi^{(n)}(\lambda) \geq 0$ for any $\lambda > 0$. As $\lambda \to 0$ the values of the derivatives typically approach limits denoted by $\varphi^{(n)}(0)$ 

### the most important theorem in the world (in these notes) 
**Theorem:** A function $\varphi : (0, \infty)$  is the [[Laplace transforms|Laplace transform]] of a probability distribution function $F$ iff it is completely monotone and $\varphi(0) = 1$. Wow!!!!!!!!! 

A more restricted version of the theorem states the following: 
$\varphi$ is completely monotone on $(0, \infty)$ iff it is of the form $$\varphi(\lambda) = \int_0^\infty e^{-\lambda x} F\{dx\}$$ where $F$ is a measure on $(0, \infty)$ 

I'll start by just copy-pasting the theorem and it's proof, and inside the proof the related theorems they call upon, and then try and figure out what in the sweet and holy fuck is happening myself 
![[Pasted image 20230529155454.png]]
as stated above. 
![[Pasted image 20230529155508.png]]

(2.4) from above was from  ![[Pasted image 20230529155539.png]]

from section 2.2 - properties - see [[Laplace transforms#properties of the Laplace transform]]. 

That is, the first part says that by (2.4), if you have the above form of this funny looking integral for your $\varphi$ then you get complete monotonicity for free by 2.4, just because you know what all the derivatives look like and they happen to alternate signs all nice like

The theorem from the previous section was the one that you read; namely, 
![[Pasted image 20230529162357.png]]

idk man lmao I'm not gonna lie I think the theorems are the more important parts to remember 

