# 💻 Data Structures & Algorithms in C

## 📘 AIM
To implement basic data structure operations in C language such as **Searching**, **Sorting**, **Stack**, **Queue**, and **Linked List** using functions and dynamic memory allocation.

---

## 🧩 LIST OF PROGRAMS AND ALGORITHMS

---

### 🔹 **1. Linear Search**

**Algorithm:**
1. Start the program.  
2. Read the number of elements `n` and store them in an array.  
3. Read the element to be searched (`target`).  
4. Traverse the array from index `0` to `n-1`.  
5. If `arr[i] == target`, print that the element is found and stop.  
6. If not found, print that the element does not exist in the list.  
7. Stop the program.  

---

### 🔹 **2. Binary Search**

**Algorithm:**
1. Start the program.  
2. Read a sorted array of `n` elements.  
3. Initialize `left = 0` and `right = n - 1`.  
4. Repeat while `left <= right`:  
   - Find `mid = (left + right) / 2`.  
   - If `arr[mid] == target`, return mid (element found).  
   - If `arr[mid] < target`, search in the right half (`left = mid + 1`).  
   - Else, search in the left half (`right = mid - 1`).  
5. If not found, print that the element does not exist.  
6. Stop the program.  

---

### 🔹 **3. Stack Implementation using Array**

**Algorithm:**
1. Start the program.  
2. Initialize an empty array `stack[MAX]` and variable `top = -1`.  
3. **Push:**  
   - If `top == MAX-1`, display "Stack Overflow".  
   - Else, increment `top` and insert the element.  
4. **Pop:**  
   - If `top == -1`, display "Stack Underflow".  
   - Else, delete the top element and decrement `top`.  
5. **Peek:** Display the element at `stack[top]`.  
6. **Display:** Print all elements from `top` to `0`.  
7. Stop the program.  

---

### 🔹 **4. Queue Implementation using Array**

**Algorithm:**
1. Start the program.  
2. Initialize `front = -1` and `rear = -1`.  
3. **Enqueue:**  
   - If `(rear + 1) % MAX == front`, Queue is full.  
   - Else, insert the element and update `rear`.  
4. **Dequeue:**  
   - If `front == -1`, Queue is empty.  
   - Else, remove the element at `front` and update pointers.  
5. **Display:** Print all elements from `front` to `rear`.  
6. Stop the program.  

---

### 🔹 **5. Circular Queue using Array**

**Algorithm:**
1. Initialize an array `queue[MAX]` with `front = -1`, `rear = -1`.  
2. **Enqueue:**  
   - If `(rear + 1) % MAX == front`, display "Queue is Full".  
   - If empty, set `front = rear = 0`.  
   - Else, `rear = (rear + 1) % MAX` and insert element.  
3. **Dequeue:**  
   - If empty, print "Queue is Empty".  
   - If one element left, reset `front = rear = -1`.  
   - Else, `front = (front + 1) % MAX`.  
4. **Display:** Traverse circularly from `front` to `rear`.  
5. Stop the program.  

---

### 🔹 **6. Stack using Linked List**

**Algorithm:**
1. Create a structure `Node` with `data` and `next`.  
2. Maintain a pointer `top` initialized to NULL.  
3. **Push:**  
   - Create a new node.  
   - Set `newNode->next = top` and update `top = newNode`.  
4. **Pop:**  
   - If `top == NULL`, print "Stack Underflow".  
   - Else, delete the top node and update `top`.  
5. **Display:** Print all nodes from `top` to `NULL`.  
6. Stop the program.  

---

### 🔹 **7. Queue using Linked List**

**Algorithm:**
1. Create a structure `Node` with `data` and `next`.  
2. Maintain two pointers — `front` and `rear` initialized to NULL.  
3. **Enqueue:**  
   - Create a new node.  
   - If queue is empty, set both `front` and `rear` to new node.  
   - Else, `rear->next = newNode` and update `rear`.  
4. **Dequeue:**  
   - If queue is empty, display "Queue is Empty".  
   - Else, delete the node pointed by `front` and move `front` forward.  
   - If `front == NULL`, set `rear = NULL`.  
5. **Display:** Print all nodes with their addresses, data, and next pointers.  
6. Stop the program.  

---

### 🔹 **8. Singly Linked List**

**Algorithm:**
1. Define a structure `Node` with `data` and `next`.  
2. **Insert at Beginning:** Create new node → point its `next` to head → update head.  
3. **Insert at End:** Traverse to last node → attach new node.  
4. **Insert at Position:** Traverse to (pos - 1) → link new node.  
5. **Delete by Value:** Locate node with value → adjust pointers → free node.  
6. **Display:** Print all nodes (addresses, data, next pointer).  
7. Stop the program.  

---

### 🔹 **9. Infix to Postfix Conversion and Evaluation**

**Algorithm:**
1. Read infix expression.  
2. Scan each character:  
   - If operand → add to postfix.  
   - If '(' → push to stack.  
   - If ')' → pop until '(' is found.  
   - If operator → pop operators with higher or equal precedence.  
3. After scanning, pop remaining operators to postfix.  
4. **Evaluation:**  
   - Scan postfix expression.  
   - If operand → push to stack.  
   - If operator → pop two operands, perform operation, push result.  
   - Final result at top of stack.  

---

### 🔹 **10. String Reversal**

**Algorithm:**
1. Read a string from the user.  
2. Initialize `start = 0` and `end = strlen(string) - 1`.  
3. Swap characters at `start` and `end`.  
4. Increment `start` and decrement `end`.  
5. Repeat until `start >= end`.  
6. Display the reversed string.  

---

## 🧠 CONCLUSION
All the above programs demonstrate the implementation of **basic data structures** and **algorithmic logic** using C language, covering both **array-based** and **linked list-based** operations.

---

## 👨‍💻 AUTHOR
**Name:** Sandeep Kumar Bollavaram  
**Register Number:** 11249A040  
**Course:** B.Tech – Computer Science & Engineering  
**Project Name:** Data Structure Lab Programs  
**Faculty In-Charge:** Suresh Bhadram
