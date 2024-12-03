# **Artificial Intelligence Lab Manual**

### **Department of Computer Science**

---

## **PART 1: Implementation of Blind Search Algorithm**

### **Problem Statement**
You need to implement a **cube solver** using blind search algorithms:  
- **Depth-First Search (DFS)**  
- **Breadth-First Search (BFS)**  

### **Cube Representation**
The cube is represented as a 2D array where:  
- `0`: Open spaces  
- `1`: Walls  
- **Start (S)**: Located at `(0, 0)` (top-left corner)  
- **Goal (G)**: Located at `(n-1, m-1)` (bottom-right corner)  

**Example Cube:**


---

### **Tasks**

#### **1. Reading the Cube**
- **Objective**: Write a function to read the cube from a text file and return a 2D array.  
- **Input**: Filename (string)  
- **Output**: 2D array representing the cube.  

#### **2. Implementing DFS and BFS**
- **Objective**: Write two separate functions for DFS and BFS.  
- **Input**: Cube (2D array)  
- **Output**: Path from the start to the goal as a list of coordinates, or `-1` if no path exists.  

#### **3. Returning the Path**
- Both DFS and BFS should return the shortest path from the start to the goal state.  
- If the path doesn't exist, return `-1`.  
- Ensure your implementation accounts for **multiple goal states**, which may result in different paths.

---

### **Output Requirements**
- **DFS** and **BFS** should return:  
  - A **list of coordinates** for the path to the goal.  
  - `-1` if no path exists.

---

## **PART 2: Implementation of A* Search Algorithm**

### **Problem Statement**
You need to implement a **cube solver** using the **A\*** algorithm. This version of the problem includes two types of walls:  
- **Short walls (2)**: Can be jumped over.  
- **High walls (1)**: Cannot be crossed.  

The goal is to find the path to the goal state with the **minimum number of short walls** crossed.

---

### **Cube Representation**
The cube uses three values:  
- `0`: Open spaces  
- `1`: High walls  
- `2`: Short walls  

**Example Cube:**


---

### **Tasks**

#### **1. Reading the Cube**
- **Objective**: Write a function to read the cube from a text file and return a 2D array.  
- **Input**: Filename (string)  
- **Output**: 2D array representing the cube.  

#### **2. Implementing A\***
- **Objective**: Write a function to implement the A\* search algorithm.  
- **Input**: Cube (2D array)  
- **Output**: Path from the start to the goal state with the **least number of short walls crossed**, or `-1` if no path exists.  

---

### **Output Requirements**
- **A\*** should prioritize paths with the fewest short walls.  
- **Example**: In the sample cube, the **yellow path** is optimal with **2 short walls** compared to other paths with **3 short walls**.

---

## **General Requirements**
1. Use appropriate **data structures** to represent the cube, store paths, and manage search queues.
2. Implement efficient algorithms to handle large cube dimensions.
3. Test your algorithms on multiple input files with varying cube configurations.

---

## **Output Format**
- For all tasks, the output should be:  
  - A **list of coordinates** representing the path, or  
  - `-1` if no path exists.

---

## **Files to Submit**
1. **Python File**: `YourRollNo.py`  
2. **Jupyter Notebook**: `YourRollNo.ipynb`

---

## **Evaluation Criteria**
1. Correctness of the implemented algorithms (DFS, BFS, A\*).  
2. Code structure, readability, and comments.  
3. Handling of edge cases and multiple goal states.  

--- 

