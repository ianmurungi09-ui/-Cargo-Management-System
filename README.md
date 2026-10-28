# 📦 Cargo Management System: OS Core Simulation

The **Cargo Management System** is a modular operating system simulation project that models core OS principles—including **CPU Scheduling (Round Robin & SRTF)**, **Virtual Memory Management (FIFO Page Replacement)**, **Process Control Blocks (PCBs)**, and **Resource Synchronization**—applied directly to a logistics and cargo tracking environment.

🛡️ **Project Overview**
In traditional systems, poor process management or memory leaks can cause pipeline stalls, race conditions, or system crashes. The Cargo Management System mitigates this by:

1. **Process State Tracking:** Managing job queues and process life cycles using robust Process Control Blocks (PCBs) during context switches.


2. **Optimized CPU Allocation:** Utilizing time-shared **Round Robin (RR)** and preemptive **Shortest Remaining Time First (SRTF)** scheduling algorithms to minimize turnaround and waiting times.


3. **Active Memory Guard:** Simulating page table tracking and **FIFO Page Replacement** to handle memory constraints and calculate page faults accurately.



🏗️ **Architecture**

* **Backend / Core Engine:** Python / C++ (Simulating OS modules, scheduling logic, and memory frames).
* **Frontend / Interface:** React (Vite) / Tailwind CSS for visual simulation dashboards.
* **OS Principles:** Process Control, Paging, Deadlock Avoidance, and Inter-Process Communication (IPC).



🚀 **Quick Start**

### Prerequisites

* Python 3.10+
* Node.js 18+

### 1. Backend Simulation Setup

```bash
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
python main.py --simulate=cargo-schedulers

```

### 2. Frontend Dashboard Setup

```bash
cd frontend
npm install
npm run dev

```

The application will be accessible at `http://localhost:3000`.

📖 **Documentation & Test Benchmarks**

* **CPU Scheduling Simulation:** Verified against test metrics (e.g., Round Robin with Time Quantum = $2\text{ ms}$, SRTF completing at $25\text{ ms}$ with an average turnaround of $11\text{ ms}$).


* **Memory Management:** FIFO page replacement trackers logging exact memory frames and page faults.



⚖️ **License**
Proprietary - Internal Academic & System Engineering Use Only.
