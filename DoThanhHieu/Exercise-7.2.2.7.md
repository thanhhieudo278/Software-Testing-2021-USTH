Exercise 7.2.2.7 Answer questions a–d for the graph defined by the following sets: N = {1, 2, 3} N0 = {1} Nf = {3} E = {(1, 2), (1, 3), (2, 1), (2, 3), (3, 1)} 
Also consider the following (candidate) paths: p1 = [1, 2, 3, 1] p2 = [1, 3, 1, 2, 3] p3 = [1, 2, 3, 1, 2, 1, 3] p4 = [2, 3, 1, 3] p5 = [1, 2, 3, 2, 3] 


(a) Which of the listed paths are test paths? For any path that is not a test path, explain why not.

p5 isn't a test path since there's no way to reach 2 from 3 straightforwardly

(b) List the eight test requirements for Edge-Pair Coverage (only the length two subpaths).

Test Paths		Test Requirements that are toured by test paths directly
[1,3,1,2,3]		[1,2,3], [1,3,1], [3,1,2]
[1,2,1,2,3]		[1,2,3], [1,2,1], [2,1,2]
[1,2,3,1,2,3]		[1,2,3], [2,3,1], [3,1,2]
[1,2,1,3]		[1,2,1], [2,1,3]
[1,2,3,1,3]		[1,2,3], [2,3,1], [3,1,3]


(c) Does the set of test paths from part (a) above satisfy Edge-Pair Coverage? -> Not satisfy
    If not, state what is missing. - > p1, p4 

(d) Consider the prime path [3, 1, 3] and path p2. 

Does p2 tour the prime path directly? -> No
With a sidetrip? -> With a sidetrip: [3, 1, 2, 1, 3]