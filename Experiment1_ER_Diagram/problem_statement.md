# ER Diagram Workshop – Submission Template

## Objective
To understand and apply ER modeling concepts by creating ER diagrams for real-world applications.

## Purpose
Gain hands-on experience in designing ER diagrams that represent database structure including entities, relationships, attributes, and constraints.

---


##  Scenario C: Restaurant Table Reservation & Ordering

###  Business Context
A popular restaurant wants to manage *reservations, orders, and billing*.

###  Requirements
- Customers can *reserve tables* or walk in.  
- Each reservation includes *date, time, number of guests*.  
- Customers place *food orders linked to reservations*.  
- Each order contains *multiple dishes; dishes belong to **categories* (starter, main, dessert).  
- *Bills* generated per reservation, including food and service charges.  
- *Waiters* assigned to serve reservations.  

###  ER Diagram
<img width="4512" height="2190" alt="erdplus" src="https://github.com/user-attachments/assets/d5af98b1-09fe-4d32-b84a-dca4a6968459" />

###  Entities and Attributes
| Entity    | Attributes (PK, FK) | Notes |
|-----------|----------------------|-------|
| Customer  | CustomerID (PK), Name, Contact | Makes reservations |
| Reservation | ReservationID (PK), Date, Time, Guests, CustomerID (FK), TableID (FK) | Booking info |
| Table     | TableID (PK), Capacity, Location | Dining tables |
| Order     | OrderID (PK), ReservationID (FK), Time | Linked to reservations |
| Dish      | DishID (PK), Name, Category, Price | Ordered item |
| OrderDetail | OrderID (FK), DishID (FK), Quantity | Resolves M:N |
| Bill      | BillID (PK), ReservationID (FK), Amount, ServiceCharge | Final payment |
| Waiter    | WaiterID (PK), Name | Assigned to reservations |

###  Relationships and Constraints
| Relationship | Cardinality | Participation | Notes |
|--------------|-------------|---------------|-------|
| Customer–Reservation | 1:N | Partial | A customer can have multiple reservations |
| Reservation–Table | 1:1 | Total | One reservation per table |
| Reservation–Order | 1:N | Total | Orders linked to reservation |
| Order–Dish | M:N | Total | Resolved using OrderDetail |
| Reservation–Bill | 1:1 | Total | One bill per reservation |
| Reservation–Waiter | 1:1 | Partial | Assigned waiter |

###  Assumptions
- Each reservation *occupies one table* only.  
- Bills always generated *per reservation*.  
- Service charges fixed percentage (not modeled).  

---
##  Instructions for Students
1. Complete *all three scenarios (A, B, C)*.  
2. Identify *entities, relationships, and attributes* for each scenario.  
3. Draw ER diagrams using *draw.io / diagrams.net* (or hand-drawn & scanned).  
4. Fill in *Entities, Relationships, Assumptions* tables.  
5. Export the completed Markdown (with diagrams) as a *single PDF*.  

---

  End of Submission Template# ER Diagram Workshop – Submission Template

## Objective
To understand and apply ER modeling concepts by creating ER diagrams for real-world applications.

## Purpose
Gain hands-on experience in designing ER diagrams that represent database structure including entities, relationships, attributes, and constraints.

---

# Scenario A: City Fitness Club Management

**Business Context:**  
FlexiFit Gym wants a database to manage its members, trainers, and fitness programs.

**Requirements:**  
- Members register with name, membership type, and start date.  
- Each member can join multiple programs (Yoga, Zumba, Weight Training).  
- Trainers assigned to programs; a program may have multiple trainers.  
- Members may book personal training sessions with trainers.  
- Attendance recorded for each session.  
- Payments tracked for memberships and sessions.

### ER Diagram:
*Paste or attach your diagram here*  
![ER Diagram](er_diagram_fitness.png)

### Entities and Attributes

| Entity | Attributes (PK, FK) | Notes |
|--------|--------------------|-------|
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |

### Relationships and Constraints

| Relationship | Cardinality | Participation | Notes |
|--------------|------------|---------------|-------|
|              |            |               |       |
|              |            |               |       |
|              |            |               |       |

### Assumptions
- 
- 
- 

---

# Scenario B: City Library Event & Book Lending System

**Business Context:**  
The Central Library wants to manage book lending and cultural events.

**Requirements:**  
- Members borrow books, with loan and return dates tracked.  
- Each book has title, author, and category.  
- Library organizes events; members can register.  
- Each event has one or more speakers/authors.  
- Rooms are booked for events and study.  
- Overdue fines apply for late returns.

### ER Diagram:
*Paste or attach your diagram here*  
![ER Diagram](er_diagram_library.png)

### Entities and Attributes

| Entity | Attributes (PK, FK) | Notes |
|--------|--------------------|-------|
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |

### Relationships and Constraints

| Relationship | Cardinality | Participation | Notes |
|--------------|------------|---------------|-------|
|              |            |               |       |
|              |            |               |       |
|              |            |               |       |

### Assumptions
- 
- 
- 

---

# Scenario C: Restaurant Table Reservation & Ordering

**Business Context:**  
A popular restaurant wants to manage reservations, orders, and billing.

**Requirements:**  
- Customers can reserve tables or walk in.  
- Each reservation includes date, time, and number of guests.  
- Customers place food orders linked to reservations.  
- Each order contains multiple dishes; dishes belong to categories (starter, main, dessert).  
- Bills generated per reservation, including food and service charges.  
- Waiters assigned to serve reservations.

### ER Diagram:
*Paste or attach your diagram here*  
![ER Diagram](er_diagram_restaurant.png)

### Entities and Attributes

| Entity | Attributes (PK, FK) | Notes |
|--------|--------------------|-------|
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |

### Relationships and Constraints

| Relationship | Cardinality | Participation | Notes |
|--------------|------------|---------------|-------|
|              |            |               |       |
|              |            |               |       |
|              |            |               |       |

### Assumptions
- 
- 
- 

---

## Instructions for Students

1. Complete **all three scenarios** (A, B, C).  
2. Identify entities, relationships, and attributes for each.  
3. Draw ER diagrams using **draw.io / diagrams.net** or hand-drawn & scanned.  
4. Fill in all tables and assumptions for each scenario.  
5. Export the completed Markdown (with diagrams) as **a single PDF**
