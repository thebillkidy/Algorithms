# Heap

* A heap is a binary tree where every element satisfies the heap property
* It is created to efficiently support basic priority queue operations
* In a **binary heap** the keys are stored in an array
* This heap property depends on the sort heap:

  * **Max-Heap:** parent &gt; children \(root is the biggest element\)
  * **Min-Heap:** parent &lt; children \(root is the smallest element\)

  ![](../../.gitbook/assets/heap.png)

## Reheapify - Restore Heap Order

### Bottom-Up \(Swim\)

* For every element in array from 0 to floor\(N/2\)
  * Check heap condition, swap if needed
  * If swapped, repeat swap check on the child
* Performance is O\(n\)

### Top-Down \(Sink\)

* Start from root and check children
* Swap if needed depending on the heap
* Repeat for the subheap

[https://www.cs.princeton.edu/~wayne/kleinberg-tardos/pdf/DemoHeapify-2x2.pdf](https://www.cs.princeton.edu/~wayne/kleinberg-tardos/pdf/DemoHeapify-2x2.pdf)

