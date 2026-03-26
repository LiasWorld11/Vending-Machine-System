# vending-Machine-System

## Project Overview
This project is a robust C++ prototype of a Vending Machine System that utilizes a custom-built Queue data structure to manage stock. Unlike standard implementations using built-in arrays, this system mimics real-world "First-In, First-Out" (FIFO) logic for dispensing items. It also features a secure Admin Inventory Module protected by a file-based login system.

## Core Functionality
- Displays up to 5 different stock items (holding up to 20 units each) in a visual grid format.
- Automated Transaction Logic:
  - Calculates total payment and issues precise refunds.
  - Features a Transaction Rollback mechanism that cancels orders and refunds money if funds are insufficient.
  - Automatically updates stock and identifies <SOLD OUT> items instantly.
- A secure module for owners to:
  - Replenish or reset stocks.
  - Modify item pricing and machine branding (titles/headers).
  - Manage machine liquidity by allocating extra funds.

## Key Technical Features
1. Custom Queue Data Structure Implementation
   - **Queue** class is implemented to manage item stock by using FIFO logic and capacity management (limited up to 20 units).
   
2. File-Based Security & Persistence
   - Automatically manages user credentials using external file storage which is records.txt and exported_records.txt.
   
3. Advanced Payment Processing
   - Include refund mechanism for real-time transactions. 

## File Structure 
| File | Description |
| :--- | :--- |
| Vending_Machine.h | Core logic for menus, payment and admin functions |
| Item.h | ADT defining item properties and queue interactions |
| Queue.h | Custom template-based Queue implementation (No built-in libraries) |
| records.txt | Stores registered administrator usernames and passwords |
| exported_records.txt | An admin function to export and audit user data |
