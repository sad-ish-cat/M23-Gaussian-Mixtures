From ![[(Graduate Texts in Mathematics 169) Rajendra Bhatia (auth.) - Matrix Analysis-Springer-Verlag New York (1997).pdf]]

Anyway my summary of the notes is as follows: 
- ![[Pasted image 20230602100500.png]]
- An equivalent condition is ![[Pasted image 20230602100521.png]]
- ![[Pasted image 20230602100530.png]]

### relationship between doubly stochastic matrices and majorization 
![[Pasted image 20230602100554.png]]
definition: ![[Pasted image 20230602101016.png]]
Theorem: 
![[Pasted image 20230602101028.png]]
The proof is by induction on $n$, where you fiddle around with the coordinates and T-transform until you can apply the IH 

![[Pasted image 20230602101143.png]]

### cool stuff is happening and/or matching problems and Birkhoff's thm
![[Pasted image 20230602101451.png]]

Note: weirdly enough to express any doubly stochastic matrix you need only at most $n^2 - 2n + 2$ permutation matrices to combine to get it. 

Definition: 
![[Pasted image 20230602101831.png]]
![[Pasted image 20230602101842.png]]

![[Pasted image 20230602101929.png]]
And as you may have expected, here's the analogous theorem for doubly substochastic matrices: 
![[Pasted image 20230602102015.png]]


## the connection to completely monotone functions
![[Pasted image 20230602102129.png]]
weird!!!!!!! they even use the same greek letter as Feller, conveniently

luckily if you only have weak submajorization you can do 
![[Pasted image 20230602102309.png]]

definition: 
![[Pasted image 20230602102320.png]]

new definitions!!!!!!! they also define convex and stuff: For $\Phi : \mathbb{R}^n \to \mathbb{R}^m$ 
![[Pasted image 20230602102356.png]]

theorem!!
![[Pasted image 20230602102441.png]]

![[Pasted image 20230602102549.png]]


COOL THEOREM!!!!!
![[Pasted image 20230602102617.png]]



and now a characterization of Schur convexity: 
![[Pasted image 20230602102909.png]]
