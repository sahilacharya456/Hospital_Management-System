Hospital Management System (DSA-Based) — Full Overview
This C++ project is a console-based hospital management system built using Data Structures like:

Doubly Linked Lists (for patients and feedbacks)

Stacks (for lab reports)

Queues/Priority Queues (for emergency patients)

Binary Search Trees (BST) (for managing doctors)

Graph (Dijkstra’s Algorithm) (for ambulance routing)

📋 Main Functional Areas
🔐 1. Login System
Admin login (Admin / 123)

User access (no login required)

🧑‍⚕️ 2. Patient Management
a. Add New Patients
Captures all info: name, ID, age, CNIC, timings, ward, bed, department

Stored in a doubly linked list

b. View & Search Patients
Search by name or ID

View categorized by department (ENT, Eye, Skin, Cardiac)

c. Discharge Patients
Removes patient from the list (FIFO approach)

d. Generate Discharge Report
Final report with cost based on lab or emergency usage

🚨 3. Emergency Ward Management
Emergency patients are prioritized by age using a priority queue

Functions:

AddEmergencyPatients()

dischargeEmergencyPatients()

displayEmergencyPatients()

🧪 4. Laboratory System
Patients added to lab test queue (stack-based)

Supports tests like: CBC, Creatinine, Lipid, X-ray, Ultrasound

Functions:

pushPatientLaboratory() → adds test request

popPatientLaboratory() → removes after test

displayLaboratory() → views current queue

👨‍⚕️ 5. Doctor Management
Uses BST (Binary Search Tree) for efficient storage/search by ID or name

Each doctor has availability status based on patients attended

Functions:

insertDoc() → Adds to BST if available

displayDoctor() → Inorder traversal

deleteDoc() → Removes (free) doctor

search() → Searches doctor by ID or name

🚑 6. Ambulance System with Dijkstra’s Algorithm
Uses an adjacency matrix graph with 7 hospitals

Calculates shortest path from a chosen hospital to others

Function:

dijkstra()

⭐ 7. Feedback System
Feedbacks stored using a doubly linked list

Users can:

Add a feedback (addFeedback())

View all feedbacks (displayFeedBack())

👨‍💼 8. User Portal
Allows basic users (non-admin) to:

Search patients

Request appointments

Leave/view feedback

Search doctors

📌 Data Structures Used
Feature	Data Structure Used
Normal Patients	Doubly Linked List
Emergency Patients	Priority Queue (age)
Lab Test Queue	Stack
Feedback	Doubly Linked List
Doctors	Binary Search Tree
Ambulance Routes	Graph + Dijkstra Algo

📈 Summary
This project provides a complete simulation of a hospital’s backend logic with:

Multi-role access (Admin/User)

Patient and doctor record systems

Emergency and lab handling

Feedback collection

Route optimization via graph algorithm
