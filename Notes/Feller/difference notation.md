useful for [[Feller 2-1 use of law of large numbers with binomial distribution]] and [[Bernstein polynomials]]
for a sequence $\{a_i\}_i \in \mathbb{N}$, $\Delta$ is defined to be the differencing operator, so that $\Delta a_i = a_{i +1} - a_i$ and then 
![[Pasted image 20230525104832.png]]

#### reciprocity relation
for two arbitrary sequences $a_i$ and $c_i$ we can express the differences $\Delta^r a_i$ in terms of $\Delta^r c_i$ if we want; you can take the above formula and do.... shenanigans... on it to discover that ![[Pasted image 20230525105015.png]]

It seems as though you'd probably have to do a good bit of work or pick smart sequences for one or the other if you want to use this to resolve questions about what the $\Delta^r$ differences actually are, as exemplified in the inversion formula: 

Examples:
If we pick $a_i = 1$ for all $i$, then $\Delta^0 a_i$ is the only nonzero sequence and the above reduces to 
![[Pasted image 20230525105152.png]]

Another example: 
If $0 < \theta < 1$ and $c_r = \theta^r$ then using the above formula we find that the differences are ![[Pasted image 20230525105245.png]]

and the reciprocity formula takes the form ![[Pasted image 20230525105308.png]]

One more important definition before we begin to discuss bernstein polynomials and completely monotone functions: 

We can define the difference *ratios* $\Delta_{h} = \Delta/h$  when working with sequences that look like $a_k = u(x + kh)$ so that ![[Pasted image 20230525110221.png]]


