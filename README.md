# Knapsack

FRACTIONAL KNAPSACK PROBLEM (Greedy Algorithm)

The basic idea of greedy approach is to calculate the ratio value/weight for each item and sort the item on basis of this ratio. Then take the item with highest ratio and add them until we can’t add the next item as whole and at the end add the next item as much as we can. Which will always be optimal solution of this problem.


0-1 KNAPSACK PROBLEM (Dynamic Programming)

There can be two cases for every item: (1) the item is included in the optimal subset, (2) not included in the optimal set.
Therefore, the maximum value that can be obtained from n items is max of following two values.
1) Maximum value obtained by n-1 items and W weight (excluding nth item).
2) Value of nth item plus maximum value obtained by n-1 items and W minus weight of the nth item (including nth item).

If weight of nth item is greater than W, then the nth item cannot be included and case 1 is the only possibility.


INTEGER KNAPSACK PROBLEM (Dynamic Programming, duplicate values permitted)

There can be three cases for every item: (1) the item is included in the optimal subset only once, (2) not included in the optimal set, (3) the item is included in optimal subset more than once.
Therefore, the maximum value that can be obtained from n items is max of following two values.
1) Maximum value obtained by n-1 items and W weight (excluding nth item).
2) Value of nth item plus maximum value obtained by n-1 items and W minus weight of the nth item (including nth item).
3) Value of nth item plus maximum value obtained by n items and W minus weight of the nth item (including nth item more than once)

If weight of nth item is greater than W, then the nth item cannot be included and case 1 is the only possibility.
