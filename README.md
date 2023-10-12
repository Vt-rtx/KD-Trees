# KD-Trees
A K-d-tree is a binary tree where the
underlying space is partitioned on the basis of the value of just one attribute (dimension) at each
level of the tree, thereby making d tests at each level. For instance, we pick a dimension i < d and also
a value p, such that all the points whose i-th coordinate value is less than p is assigned to the left
subtree at this level and other points are assigned to the right subtree.
This data structure is very useful while searching range queries, i.e., all those points that are
within a certain distance of a given query point q.
Let us for the moment assume that d = 3 and q = (a,b,c). If we want to find all the data points
that are less than distance ‘r’, it is sufficient to search the subtrees that have values in the range (r-a,
r+a) for a particular dimension i, and similarly for the other a

ributes/ dimensions. Thus searching

for neighbours within a range amounts to traversing through this data structure wisely.
To Implement:
● Created 200 points from [-10, 10]5
, i.e., the points come from a 5-dimensional space with the

max values along any dimension lying between -10 and 10.
● Constructed a K-d-tree and given an arbitrary query point q and distance r, find the nearest
neighbours of q that lie within this radius r, where the distance is the usual Euclidean
distance.
●Changed the Euclidean distance to,Manhattan or Max norm distance,Verified with the brute force method.
