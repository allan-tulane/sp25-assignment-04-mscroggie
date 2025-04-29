# CMPS 2200 Assignment 5
## Answers

**Name:** Mary Ella Scroggie






- **1a.**
$log<sub>d</sub>(n(d-1))$


- **1b.**
work for delete root: log<sub>d</sub>(d * log(d))
work for insert: log<sub>d</sub>(log(d))
- **1c.**
O((|V| + |E|)*log_d(|V|))
- **1d.**
d = |E| gives the best result

- **2a.**
- APSP(0,1,0) = -2
- APSP(0,1,1)= -2
- APSP(0,1,2) = -2
- APSP(1,2,0)= 0
- APSP(1,2,1)= 1
- APSP(1,2,2) = 0
- APSP(0,2,0) = -1
- APSP(0,2,1) = 2
- APSP(0,2,2) = -1

- **2b.**
ASPS(i,j,2) = min(ASPS(i,j,0), ASPS(i,j,1))

- **2c.**
ASPS(i,j,k) = min(ASPS(i,j,k-1),ASPS(i,k,k-1)+ASPS(k,j,k-1))
- **2d.**
- there are n^3 sub problems each calculated once, meaning the work is 0(n^3)
- **2e.**
this works best when the graph is small but dense, but johnsons works better overall 


- **3a.**
No, because it is a greedy algorithm that might choose two short paths over a long one, even if the sum of the two is greater

- **3b.**
Find the MST, then add an edge not in it and remove one that is. Keep going until you find the next shortest path

- **3c.**
 - The work is mlog(n) to find the initial MST, and the swapping steps take log(n)