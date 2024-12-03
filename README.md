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
