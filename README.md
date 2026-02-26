# 🏭 Food Processing Plant Simulation  
## Operating Systems – Reader–Writer Problem

This project demonstrates the **Reader–Writer synchronization problem** using a real-world analogy of a food processing plant.

The system models different stages of vegetable processing such as washing, peeling, chopping, and packaging, where multiple processes access shared resources like conveyor belts and storage bins.


---

## 📌 Problem Statement

In a food processing plant:

- Some stages **read** shared resources (e.g., monitoring vegetables on conveyor belts).
- Some stages **write/modify** shared resources (e.g., adding or removing items).

The challenge is to:

- Allow multiple readers simultaneously.
- Allow only one writer at a time.
- Prevent deadlock.
- Prevent starvation.

This directly represents the classical **Reader–Writer Problem** in Operating Systems.

---

## 🧠 Core OS Concepts Implemented

### 1️⃣ Mutual Exclusion

Ensures that:

- Only one writer modifies a shared resource at a time.
- Prevents conflicts or data corruption.

**Example:**  
If the chopping stage is using the conveyor belt, the peeling stage must wait before modifying it.

---

### 2️⃣ Progress

Guarantees that:

- The system does not enter deadlock.
- Processes do not wait indefinitely.

**Solution Approach:**

- Fixed order of acquiring resources.
- Controlled access sequence.

This prevents circular dependency between stages.

---

### 3️⃣ Bounded Waiting

Ensures:

- No process waits forever (no starvation).
- Every stage eventually gets access.

**Solution Used:**

- Assign time slots or controlled scheduling.
- Limit how long one stage can hold a resource.

---

## 🏗 System Model

### Stages Modeled as Processes:

- Washing
- Peeling
- Chopping
- Packaging

### Shared Resources:

- Conveyor belts
- Storage bins
- Processing machines

Each resource is protected using synchronization techniques.

---

## ⚙ How the Simulation Works

1. Processes request access to shared resources.
2. Reader processes can access simultaneously.
3. Writer processes must acquire exclusive access.
4. Locks ensure mutual exclusion.
5. Scheduling prevents deadlock and starvation.

---

## 🛠 Technologies Used

- Operating Systems Concepts
- Synchronization Mechanisms
- Concurrency Modeling
- Web-based visualization (Live Demo)

---

## 🌐 Live Project Demo

👉 https://sujankarthikm.github.io/dragonfly1/

---

## 🎯 Learning Outcomes

- Understanding of Reader–Writer problem
- Application of Mutual Exclusion
- Deadlock prevention strategies
- Starvation prevention
- Real-world analogy of OS synchronization
- Modeling concurrent systems

---

## 👥 Team Members

- Bharath Kumar – CB.EN.U4CSE22507  
- Sujan Karthik – CB.EN.U4CSE22547  
- N Siddharth – CB.EN.U4CSE22529  
- Nandhakumar – CB.EN.U4CSE22530  
- Kamalakrishnan – CB.EN.U4CSE22519  

---

## 📌 Conclusion

This project successfully demonstrates how synchronization concepts in Operating Systems can be modeled using real-world scenarios.  

The Food Processing Plant analogy provides a clear and intuitive understanding of:

- Mutual Exclusion  
- Progress  
- Bounded Waiting  

It highlights how proper resource management ensures system stability and efficiency.

---
