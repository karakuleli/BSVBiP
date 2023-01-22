# Selection/ Insertion Sort project


## Question 1: 

[22,27,16,2,18,6] -> Insertion Sort

Write the steps of the above sequence according to the sort type.

Please, provide the Big-O 

Time Complexity: After the sequence is sorted, which of the following cases does the number 18 fall into?



1. Average case: The number we are looking for is in the middle
2. Worst case: The number we are looking for is at the end
3. Best case: The number we are looking for is at the beginning of the array.


## Question 2: 

Write the first 4 steps of [7,3,5,8,2,9,4,15,6] according to the Selection Sort.


## Solution:

**Step 1: **[22,27,16,2,18,6] - No change, as the first element is already in its correct position.

**Step 2:** [22,27,16,2,18,6] - No change, as the second element is already in its correct position.

**Step 3: **[16,22,27,2,18,6] - The third element (16) is compared to the second element (22) and since 16 is smaller, it is swapped with the second element. The list now looks like [16,22,27,2,18,6].

**Step 4:** [2,16,22,27,18,6] - The fourth element (2) is compared to the third element (16) and since 2 is smaller, it is swapped with the third element. The list now looks like [2,16,22,27,18,6].

**Step 5:** [2,16,18,22,27,6] - The fifth element (18) is compared to the fourth element (22) and since 18 is smaller, it is swapped with the fourth element. The list now looks like [2,16,18,22,27,6].

**Step 6: **[2,6,16,18,22,27] - The sixth element (6) is compared to the fifth element (22) and since 6 is smaller, it is swapped with the fifth element. The list now looks like [2,6,16,18,22,27].

At this point, the list is fully sorted and no more swaps are needed. The final list is [2,6,16,18,22,27].


### Big O Notation:

Insertion sort is a comparison-based sorting algorithm. The best case scenario for insertion sort is when the input list is already sorted, in which case the algorithm will simply iterate through the list, comparing each element to the one before it and making no swaps. In this case, the time complexity is O(n) where n is the number of elements in the input list.

The average case scenario for insertion sort is when the input list is not already sorted, but is not in reverse order either. In this case, the algorithm will have to make some swaps as it iterates through the list, but the number of swaps will not be as high as in the worst case scenario. The time complexity in this case is O(n^2) where n is the number of elements in the input list.

The worst case scenario for insertion sort is when the input list is in reverse order. In this case, the algorithm will have to make the maximum number of swaps as it iterates through the list. As a result, the time complexity in this case is also O(n^2) where n is the number of elements in the input list.


### Time Complexity: After the sequence is sorted, which of the following cases does the number 18 fall into?

**Average Case:**  After sorting the list, searching for the number 18 would fall under the average case scenario if it is located in the middle of the list, under the worst case scenario if it is located at the end of the list, and under the best case scenario if it is located at the beginning of the list. The time complexity for searching in a sorted list using insertion sort is O(n) in the average and worst case scenarios, and O(1) in the best case scenario.


## The first 4 steps of [7,3,5,8,2,9,4,15,6] according to the Selection Sort.

Step 1: [7,3,5,8,2,9,4,15,6] - The algorithm starts by finding the smallest element in the list, which is 2. 2 is swapped with the first element, 7. The list now looks like [2,3,5,8,7,9,4,15,6].

Step 2: [2,3,5,8,7,9,4,15,6] - The algorithm then moves on to the second element in the list, and finds the smallest element in the remaining sublist (3,5,8,7,9,4,15,6), No -swab required.. The list now looks like [2,3,5,8,7,9,4,15,6].

Step 3: [2,3,4,8,7,9,5,15,6] - The algorithm then moves on to the third element in the list, and finds the smallest element in the remaining sublist (4,8,7,9,5,15,6), which is 4. 4 is swapped with the third element, 5. The list now looks like [2,3,4,8,7,9,5,15,6].

Step 4: [2,3,4,5,7,9,8,15,6] - The algorithm then moves on to the fourth element in the list, and finds the smallest element in the remaining sublist (5,7,9,8,15,6), which is 5. 5 is swapped with the fourth element, 8. The list now looks like [2,3,4,5,7,9,8,15,6].

And the process continues until all the elements are sorted.
