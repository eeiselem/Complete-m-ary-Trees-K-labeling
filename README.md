# Complete-m-ary-Trees-K-labeling
Goal: Implement B Tree to store at least 1000, most used English words.

The best data-structure to store this tree in memory is as a number of nodes connected by edges, in other
words, a tree data structure. The connected, hierarchical properties of this data structure make it ideal for the
m-ary tree. They are also particularly useful for recursive algorithms, such as the one used in the code
included later in this document

The general algorithm used was algorithm 4 from the paper ‘Computing edge irregularity strength of complete
m-ary trees using algorithmic approach’ [1]

When assigning labels and edges in this tree structure there are two types of traversals. For each subtree coming from
the first set of children from 1 to m-1 (children of the main node) a level order traversal is performed. For the subtree
coming from the m-th child a reverse level order traversal is performed, where the lowest values come on the bottom level
and the highest value is from the topmost node of that subtree. The topmost layer, consisting of the main root and it’s
children, are assigned labels and edges in a level order or preorder traversal if taken/assigned independently of the rest of
the tree. It is not clear if it is preorder or level order traversal as it only concerns one layer it could be either.

1. Asim, Muhammad & Hasni, Roslan & Ahmad, Ali. (2019). Edge irregular k-labeling for several classes of trees.
Utilitas Mathematica. 111. 75-83.
