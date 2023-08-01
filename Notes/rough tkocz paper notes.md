Result: In the Khinchine inequality (7) at the start of the paper, for $p \geq 2$ and $a \leq b$ (idk how to do the majorize latex) then the result in (6) follows. Now once you have it you can do two things: 

You can see that $\mathbb{E}|\sum a_j U_j |^2 = (\sum a_j^2) Var(U_i)$ and furthermore we know by assumption that $\sum a_j^2 = 1$ so the trick is incorporating that fact into $6$ we get that the lower inequality is equivalent to showing that for all vectors $a$, $\mathbb{E}|U_1|^p (3 \mathbb{E}|\sum a_j U_j|^2)^{p/2} \leq \mathbb{E}|\sum a_j U_j|^p$, because once we splice the $a_j$ into the expression on the left, which was originally just $\mathbb{E}|U_1|^p$, we're ok. 

Alternatively you can consider $A_p = \inf_n \inf_a \frac{||\sum a_j U_j ||_p}{||\sum a_j U_j||_2}$ and simplifying with the above and the original inequality you can cough the result back up 



For $B_p$ you take it to be $\sqrt{3} \sup_{n \geq 1} \sup_{a \in S^{n - 1}} ||\sum a_j U_j||_p$. For a fixed $n$ we know that the inner supremum becomes $\sqrt{3} \sup_{n \geq 1} ||\sum \frac{U_j}{\sqrt{n}}||_p$ and now we apply CLT, where vanilla CLT gives us that $\sum \frac{U_j}{\sqrt{n}}$ tends in distribution to 




**you can get from convergence in distribution to convergence of the pth moments** by using [[uniform integrability]]

anyway at some point you need to work it out on paper 


things to ask: 
just to confirm, uniform integrability is a way of making sure that your random variables all have the same-ish mean?? idk 

