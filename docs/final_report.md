This is the initial structure that can be changed to fit the final report requirements!!!

# Final report

---

## **Distri-place**
_Group 7 / Distributed Systems Course / 15.12.2025_

---

## **Table of Contents**
- [1. Introduction](#1-introduction)  
- [2. Project Goals and Core Functionality](#2-project-goals-and-core-functionality)  
- [3. Design Principles](#3-design-principles)  
  - [3.1 System Architecture](#31-system-architecture)  
  - [3.2 Processes and Components](#32-processes-and-components)  
  - [3.3 Communication Model](#33-communication-model)  
  - [3.4 Mapping of Design to Source Code](#34-mapping-of-design-to-source-code)  
- [4. System Functionalities](#4-system-functionalities)  
  - [4.1 Global State Management](#41-global-state-management)  
  - [4.2 Consistency and Synchronization](#42-consistency-and-synchronization)  
  - [4.3 Consensus Mechanism](#43-consensus-mechanism)  
  - [4.4 Fault Tolerance and Recovery](#44-fault-tolerance-and-recovery)  
- [5. Scalability Evaluation](#5-scalability-evaluation)  
- [6. Performance Evaluation](#6-performance-evaluation)  
  - [6.1 Performance Metrics](#61-performance-metrics)  
  - [6.2 Experimental Setup](#62-experimental-setup)  
  - [6.3 Performance Results](#63-performance-results)  
  - [6.4 Performance Improvements](#64-performance-improvements)  
- [7. Key Enablers and Lessons Learned](#7-key-enablers-and-lessons-learned)  
- [8. Team Contributions](#8-team-contributions)  
- [9. Appendices](#9-appendices)  
  - [A. Major Design Changes](#a-major-design-changes)  
  - [B. Code References](#b-code-references)  
  - [C. Additional Figures, Logs, or Data](#c-additional-figures-logs-or-data)

---

# **1. Introduction**
This is the final report of our project Distri-place. Distri-place is a shared canvas app that allows users to distributedly work on the same graphical canvas to create works of art.

In this report we will discuss the project design and implementation goals and technology from the lens of implementing a working distributed system. We go into the core functionality and give a detailed review of how key distributed system elements such as leader election, consistency and fault tolerance are implemented, what are the roles of different nodes in our system and much more.

---

# **2. Project Goals and Core Functionality**

**2.1 Project Objectives**
- The project objective was to be a shared canvas that works seamlessly with multitude of users each working on the canvas in real time. The distributed aspects of the project that we mainly were focusing on were replication among multiple nodes and availability, so that the users are always able to connect to our system.
  
**2.2 Core Features**
- Distributed systems elements are mostly implemented via RAFT-algorithm. We concluded after our initial design that with RAFT the project gets the key features that we expect from the distributed system. Those were the consistency and global synchronization, consensus via leader election and fault tolerance in case of errors happening that might compromise the current leader.

**2.3 Potential Applications / Services Built on This Project**

---

# **3. Design Principles**

## **3.1 System Architecture**
- Overview diagram  
- Components and responsibilities  

## **3.2 Processes and Components**
- Node roles  
- Local vs distributed components  

## **3.3 Communication Model**
- Protocols used  
- Message types  
- Network topology  

## **3.4 Mapping of Design to Source Code**
- Where to find architectural decisions in the code  
- Important modules and functions  

---

# **4. System Functionalities**

## **4.1 Global State Management**

## **4.2 Consistency and Synchronization**

## **4.3 Consensus Mechanism**

## **4.4 Fault Tolerance and Recovery**

---

# **5. Scalability Evaluation**

---

# **6. Performance Evaluation**

## **6.1 Performance Metrics**

## **6.2 Experimental Setup**

## **6.3 Performance Results**

## **6.4 Performance Improvements**

---

# **7. Key Enablers and Lessons Learned**

---

# **8. Appendices**

