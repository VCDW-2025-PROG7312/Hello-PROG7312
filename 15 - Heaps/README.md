## Heaps – Managing Gadget Deliveries

### Activity 1 – Build a Generic Heap
Build an app that manages gadget deliveries in a warehouse using a generic heap data structure. Each gadget has a Name and a Weight (in kilograms). The goal is to ensure that lighter gadgets are always given priority — meaning they should appear closer to the top of the heap.

Implement a generic Heap<T> class that supports insertion, extraction, and peeking operations. Your heap should use a Min-Heap ordering by default (lighter = higher priority), but the implementation should be flexible enough to work as a Max-Heap if required.

You can consult the PROG7312 bot or any resource of your choice for guidance on generic types, comparison interfaces, and heap algorithms.

An interesting read:
* https://www.geeksforgeeks.org/dsa/applications-of-heap-data-structure/

### Activity 2 – Explore Heap Variants and Use Cases
As a follow-up to the above activity, explore variations and real-world applications of heaps in scheduling, gaming, and system optimization.

Questions to explore:
* How does a Min-Heap differ from a Max-Heap in terms of use cases and data ordering?
* How can heaps be used to implement a Priority Queue?
* What are the time complexities of insertion, extraction, and search operations in a heap compared to other data structures such as arrays or binary search trees?
* How does Heap Sort leverage the heap structure to achieve efficient sorting?
* In what scenarios would you prefer using a heap instead of a binary search tree?

Extension:
Redo your Heap<T> implementation to sort gadgets using Heap Sort, displaying them from lightest to heaviest.