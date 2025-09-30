# EXP-18-Queue-in-C-

# Aim :
Constructing Queue  using Array .

# Theory :
A queue in C++ is a type of container adapter that operates on the First-In, First-Out (FIFO) principle. This means the element that was added to the queue first will be the first one to be removed.

# Key Characteristics:
FIFO Principle: The fundamental rule is that elements are inserted at the back (or "tail") and removed from the front (or "head").

Restricted Access: Elements can only be inserted at one end (back) and removed from the other end (front). You cannot access or modify elements in the middle of the queue.

Underlying Container: The C++ Standard Template Library (STL) std::queue is not a standalone container; it's a container adapter that uses other STL containers (like std::deque by default, or optionally std::list) to perform its operations.


# Algorithm :
Start the program.
Define a Queue class with:
An array arr[SIZE].
Two integers front and back.
Initialize front = -1, back = -1 in the constructor.
For Enqueue operation:
If back == SIZE-1, print Queue Overflow.
If front == -1, set front = 0.
Increment back and insert value into arr[back].
For Dequeue operation:
If front == -1 or front > back, print Queue Underflow/Empty Queue.
Otherwise, print and remove arr[front], then increment front.
For Display operation:
If front == -1 or front > back, print Queue is empty.
Otherwise, traverse from front to back and print all elements.
In main(), demonstrate enqueue, dequeue, and display operations.
End the program.

# Conclusion :

A queue in C++ (std::queue) is a container adapter that enforces a First-In, First-Out (FIFO) ordering.

It is used for scenarios that require elements to be processed in the exact order they were received.

Operation	Description	Time Complexity
push()	Adds an element to the back (tail).	O(1)
pop()	Removes the element from the front (head).	O(1)
front()	Accesses the element at the front (next to be removed).	O(1)

Export to Sheets
Conclusion: Queues are an efficient (O(1)) and restricted data structure ideal for managing sequential tasks, such as in operating system scheduling or network packet handling.














