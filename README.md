Download Link: https://assignmentchef.com/product/solved-cpe202-lab-7-maxheap-class-to-contain-integers
<br>



<ol>

 <li><strong> Implement a class MaxHeap</strong> (a max heap) that contains integers that represent both the priority and name of the object.</li>

</ol>

(Note: Heap is like an array which start from index 1. Left child is in index i*2 and right child is in index i*2+1)




<ul>

 <li>Implement class MaxHeap of integers: o <strong>def __init__(self, capacity=50) </strong>Constructor creating an empty heap with default capacity = 50 but allows heaps of other capacities to be created.

  <ul>

   <li><strong>def insert (self, item)</strong> inserts “item” into the heap, returns true if successful, false if there is no room in the heap.</li>

   <li><strong>def find_max(self) </strong>returns max without changing the heap and return None if heap is empty. o <strong>def del_max(self)</strong>  returns max and removes it from the heap and restores the heap property and return None if heap is empty</li>

   <li><strong>def heap_contents (self) </strong>returns a list of contents of the heap in the order it is stored internal to the heap.  (This may be useful for in testing your implementation.)</li>

   <li><strong>def build_heap (self, alist) </strong>takes a single explicit argument “list of int” and builds a heap using the <strong><u>bottom up method</u></strong> discussed in class.  It should return True if the build was successful and False if the capacity of the MaxHeap object is not large enough to hold the “array of int” argument.</li>

   <li><strong>def is_empty(self) </strong>returns True if the heap is empty, false otherwise<strong>  </strong>o <strong>def is_full(self)</strong>  <strong>  </strong>returns True if the heap is full, false otherwise o <strong>def get_heap_cap(self)</strong>  returns the maximum number of a entries the heap can hold. o <strong>def get_heap_size(self)</strong>  — the actual number of elements in the heap, not the capacity</li>

  </ul></li>

</ul>

<ul>

 <li>Where possible your build, insert, and delete methods should use the following functions that work exactly as described in class.</li>

 <li><strong>def perc_down(self, i)</strong> where the parameter <strong>i</strong> is an index in the heap and perc_down moves the element stored at that location to its proper place in the heap rearranging elements as it goes.  Since this is an internal method we will assume that the element is either in the correct position or the correct position is below the current position.</li>

 <li><strong>def perc_up(self, i):</strong>. similar specification as perc_down, see class notes</li>

</ul>

Normally these would be private but make them public for testing purposes.

<ol>

 <li><strong> Add a function heap_sort_increase (self, alist) </strong>to perform heap sort to a given list of positive integers.</li>

</ol>

Add a function to the MaxHeap Class to sort a list of positive integers in increasing order.

<ul>

 <li><strong>heap_sort_increase (self, alist)</strong> takes a list of integers and returns a list containing the integers in nondecreasing order using the <u>Heap Sort algorithm as described in class</u>. Since your MaxHeap class is a max heap using the list internal to the heap to store the sorted elements will result in them being sorted in increasing order. This enables the reuse of the space but will destroy the heap order property.  However, then you can just return the appropriate part of the internal list since you will not be using the heap anymore.</li>

</ul>











