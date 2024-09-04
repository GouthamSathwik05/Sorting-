To prove the correctness of selection sort, we'll use an inductive argument based on the properties of the algorithm:
Base Case: The sorted part of the list is initially null (or contains only the first member). The sorted requirement is trivially accomplished by this,
since a list that contains zero or one member is deemed sorted.

Inductive Step: Assume that the list's first k elements have been sorted and that the remaining k − k−1 elements have remained unsorted following k selection sort iterations. 
It is necessary to demonstrate that the top k+1 items of 𝑘 + 1 are sorted after the (𝑘 + 1) (k+1)th iteration, while the remaining 𝑛 − (𝑘 + 1) n−(k+1) elements remain unsorted.

Finding the Minimum: The algorithm locates the smallest element in the remaining unsorted segment and sets it in the (𝑘 + 1) (k+1)th position during the (𝑘 + 1) (k+1)th iteration.
The (𝑘 + 1)(k+1)th element will always be smaller than all the items in the unsorted segment thanks to this technique.

Preserving Sorted Order: According to the induction hypothesis, the first k items were previously sorted, and since the smallest unsorted element 
among the remaining k+1 elements is the (𝑘 + 1)k+1 element, the first k+1 elements are now in sorted order.

Correctness of Remaining Elements: This iteration has not affected and the remaining k+1 elements are still unsorted. 
They are 𝑛− (𝑘 + 1) n−(k+1). Nevertheless, since the procedure for determining the minimum and appropriately inserting it does not alter the sequence of already sorted elements

Termination: After n−1 iterations, the algorithm terminates and the entire list is sorted. According to the inductive hypothesis, 
the list is sorted after n−1 iterations since each member has been positioned correctly in relation to the others.
