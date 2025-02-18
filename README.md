# OPTIMIZATION-MODEL

## **Optimization Model Using Linear Programming**  

### **1. Overview**  
This project demonstrates **Linear Programming (LP)** to optimize product mix for **profit maximization**. The objective is to determine the optimal number of units for two products (**A and B**) while considering constraints such as **raw materials and labor hours**. The model is built using the **PuLP library in Python** and solved using an LP solver.

---

### **2. Problem Definition**  
A company produces **two products (A and B)**, each contributing to the total profit. However, production is limited by the availability of **raw materials and labor hours**. The goal is to **maximize total profit** while ensuring that constraints are not violated.

---

### **3. Key Components of the Model**  

#### **A. Decision Variables**  
- **Product A (A):** Number of units to produce.  
- **Product B (B):** Number of units to produce.  
- Both variables are **non-negative** (cannot be negative production).  

#### **B. Objective Function (Profit Maximization)**  
- The company earns **$3 per unit** of Product A and **$4 per unit** of Product B.  
- The total profit is calculated as:  
  \[
  \text{Total Profit} = 3A + 4B
  \]  
- The goal is to **maximize** this profit.  

#### **C. Constraints**  
1. **Raw Material Constraint:**  
   - Each unit of A requires **2 units of raw material**.  
   - Each unit of B requires **4 units of raw material**.  
   - The company has a total of **100 units of raw material** available.  
   - The constraint ensures that production does not exceed raw material availability:  
     \[
     2A + 4B \leq 100
     \]  

2. **Labor Hours Constraint:**  
   - Each unit of A requires **3 labor hours**.  
   - Each unit of B requires **2 labor hours**.  
   - The company has a total of **120 labor hours** available.  
   - The constraint ensures that labor hours are not exceeded:  
     \[
     3A + 2B \leq 120
     \]  

---

### **4. Solving the Model**  
- The **Linear Programming solver** finds the **optimal values of A and B** that maximize profit while satisfying the given constraints.  
- The solver provides an **optimal solution status**, ensuring feasibility.  

---

### **5. Interpretation of Results**  
- **Optimal production quantities** for Products A and B are determined.  
- **Maximum achievable profit** is calculated.  
- The **solution status** confirms whether the problem was solved optimally.  

---

### **6. Real-World Applications**  
This optimization model is widely used in various industries, including:  

- **Manufacturing:** Determining the best mix of products to produce given resource constraints.  
- **Retail & Inventory Management:** Deciding how much of each product to stock for maximum revenue.  
- **Supply Chain Optimization:** Allocating limited resources across multiple production lines efficiently.  
- **Project Scheduling:** Optimizing labor and material usage for maximum output.  

---

### **7. Summary**  
This Linear Programming model helps businesses **make data-driven decisions** by optimizing production for **maximum profitability** while ensuring efficient resource utilization. 
