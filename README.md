Deque (Double Ended Queue) Implementation Using Linked List in C

This project demonstrates how to implement a Deque (Double Ended Queue) using a Doubly Linked List in C programming language.

A Deque allows insertion and deletion from both ends (front and rear).

📌 Description

In this program:

A Doubly Linked List is used to implement a Deque.

Two pointers are maintained:

front → Points to first node

rear → Points to last node

The following operations are implemented:

Insert at Front

Insert at Rear

Delete from Front

Delete from Rear

Display Deque

🧠 What is a Deque?

A Deque (Double Ended Queue) is a linear data structure in which elements can be inserted and removed from both ends.

It combines features of:

Stack (LIFO)

Queue (FIFO)

📂 Data Structure Used
struct Node {
    int data;
    struct Node *prev;
    struct Node *next;
};

Each node contains:

data → Value of node

prev → Pointer to previous node

next → Pointer to next node

🔹 Operations Implemented
1️⃣ insertFront(int value)

Inserts element at the beginning.

Updates front pointer.

2️⃣ insertRear(int value)

Inserts element at the end.

Updates rear pointer.

3️⃣ deleteFront()

Removes element from front.

Adjusts pointers accordingly.

4️⃣ deleteRear()

Removes element from rear.

Adjusts pointers accordingly.

5️⃣ display()

Displays all elements from front to rear.

▶️ Example Execution (main function)
insertRear(10);
insertRear(20);
insertFront(5);
display();

deleteFront();
deleteRear();
display();
▶️ Sample Output
Inserted at rear: 10
Inserted at rear: 20
Inserted at front: 5
Deque elements: 5 10 20
Deleted from front: 5
Deleted from rear: 20
Deque elements: 10
⚙️ How to Compile and Run
1️⃣ Compile
gcc deque_linkedlist.c -o deque_linkedlist
2️⃣ Run
./deque_linkedlist
⏱️ Time & Space Complexity

Insertion (Front/Rear): O(1)

Deletion (Front/Rear): O(1)

Display: O(n)

Space Complexity: O(n)

Where:

n = Number of elements in Deque

📚 Concepts Covered

Deque Data Structure

Doubly Linked List

Dynamic Memory Allocation

Pointer Manipulation

Front and Rear Handling

⚠️ Limitations

No menu-driven interface.

Memory is freed only during deletion.

No error handling for malloc() failure.

👨‍💻 Author

Ritik Chauhan

If you want, I can also provide:

Menu-driven Deque program

Deque using array

Comparison README (Queue vs Deque)

Short exam-ready version
