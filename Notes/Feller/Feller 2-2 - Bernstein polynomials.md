The left side of the equation in [[Feller 2-1 use of law of large numbers with binomial distribution]] is called the Bernstein polynomial of degree $n$ and we can write 
![[Pasted image 20230525111633.png]]
and as before $1/n - h$. However, invoking the second example in [[difference notation]] we can see that it can be written as ![[Pasted image 20230525111710.png]]
Recall that the stone weierstrass approximation theorem states that every continuous function on a closed interval has associated polynomials that approximate it - in particular, for every $\varepsilon > 0$ there's a polynomial $p$ st for all $x \in [a, b]$ we have $|f(x) - p(x)| < \varepsilon$, or indeed $||f - p|| < \varepsilon$. The nice thing about the above expression for the Bernstein polynomial is that we now have the specific coefficients for the polynomials in question - the nth polynomial is given by $B_{n, \theta}$  and indeed it pops up in the wikipedia page lol 

### characterization of functions representable by power series
If we have $u(x) = p_0 + p_1 x + \dots$ where $p_j \geq 0$ and $0 \leq x < 1$ then evidently $u^{(n)}(x) \geq 0$ for all $n$ and evidently the derivatives all exist. 

The surprising fact is that the converse is also true; that is, any function where $u^{(n)}(x) \geq 0$ (known as an absolutely monotone function) admits a power series representation. These equivalent facts are also equivalent to a third, that $\Delta_h^k u_c(0) \geq 0$ (what is u_c? who knows)

%%%%At this point I have to ask the question: numerous sources state that completely/totally/absolutely monotone functions actually have $(-1)^n u^{(n)}(x) \geq 0$ instead, so now I'm very confused. 

oh haha jussssst kidding in literally the next section they define completely monotone functions %%%%

Anyway the book goes on to state that the important result is that all three are equivalent. 
![[Pasted image 20230525114510.png]]
![[Pasted image 20230525114522.png]]



