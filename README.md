# Isomorphism

Prove that if two graphs $A$ and $B$ do not have the same number of nodes, they
cannot be isomorphic. I have started with the formal definition of isomorphism
below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

The part of the formal definition that we will take in interest in for the purpose of this problem is: there exists a
one-to-one and onto function (bijection)  

We can ignore edge preservation for now because if the one-to-one onto function does not exist in the first place, that becomes irrelevant. 
One-to-One means that for every node in A, which we will call nodes A<sub>1</sub> to A<sub>n</sub> with n being number of nodes, there must be a unique match in the output (B)
We will call every node in B: B<sub>1</sub> to B<sub>m</sub> with m being number of nodes  
We will then map every node A<sub>x</sub> to the corresponding B<sub>x</sub> in graph B
If n > m, or there is more nodes in graph A than in graph B, then we will have n-m leftover unpaired nodes in graph A, meaning no such one-to-one function exists if there is more nodes in graph A than in graph B
Onto means that for every node in the output of the function, in our case we are trying to make this B, there must be at least one input node, in our case a node in graph A, that maps to it.  
Using the same criteria, every node in A labled as nodes A<sub>1</sub> to A<sub>n</sub> with n being number of nodes, and every node in B labled as nodes B<sub>1</sub> to B<sub>m</sub> with m being number of nodes, if m > n, or there is more nodes in graph B than graph A, then we cannot guarantee that the Onto function pairs each node in B to a unique node in A.  
Swapping the places of A and B in this explanation shows that the same holds true for attempting the bijection the other way, and no such bijection can exist if there are mores nodes in A than B, or more nodes in B than A. Meaning the only way for the bijection to exist and satisfy the condition of the formal definition is if the number is nodes in A and B is equal
