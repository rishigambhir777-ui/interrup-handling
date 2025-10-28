# ⚙️ Interrupt-Driven System Simulation (Java)

## 📘 Overview
This project simulates an **interrupt-driven system** using **Java multithreading**.  
It models how a CPU handles interrupts from multiple devices — **Keyboard**, **Mouse**, and **Printer** — in real-time.  
Each device generates interrupts asynchronously, and the controller manages them based on predefined priorities, demonstrating core **Operating System concepts** like interrupt handling, masking, and synchronization.

---

## 🎯 Objectives
- To emulate interrupt-driven I/O handling using software threads.  
- To demonstrate priority-based interrupt processing.  
- To implement masking and real-time event logging.  
- To gain hands-on experience with **Java concurrency** and **thread synchronization**.

---

## 🧩 Features
- Three independent device threads (Keyboard, Mouse, Printer).  
- Priority-based interrupt handling (`Keyboard > Mouse > Printer`).  
- Dynamic **masking/unmasking** of devices during runtime.  
- Real-time **logging** of handled interrupts in `interrupt_log.txt`.  
- **Menu-driven console interface** for user interaction.  
- Prevents race conditions through synchronized blocks.

---

## 🧠 Working Principle
Each device runs in its own thread and randomly triggers interrupts.  
The main controller continuously polls for these signals, checks priorities, and executes the corresponding **Interrupt Service Routine (ISR)**.  
Every event handled is recorded in the log file with a timestamp for verification.

---

## 🚀 How to Run
1. Clone or download the repository.  
2. Open the folder in your terminal or IDE.  
3. Compile and run the program:
   ```bash
   javac InterruptController.java
   java InterruptController# interrup-handling
