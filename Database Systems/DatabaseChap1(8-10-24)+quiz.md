
# Cheat Sheet: Database Environment and Development Process

## 1. Key Terms
- **Database**: An organized collection of logically related data.
- **Data**: Raw, unprocessed facts (e.g., numbers, text, images).
  - **Structured Data**: Data with a predefined format (e.g., numbers, dates).
  - **Unstructured Data**: Data without a predefined format (e.g., videos, images).
- **Information**: Data that has been processed to give meaning or aid decision-making.
- **Metadata**: Data that describes other data (e.g., data types, field sizes, relationships).

## 2. Problems with File Processing Systems
- **Program-Data Dependence**: Each program stores its own data structure, leading to duplication.
- **Duplication of Data**: Data stored in multiple places, wasting space and risking inconsistency.
- **Limited Data Sharing**: No centralized control makes sharing between systems hard.
- **Program Maintenance**: Changes to data format require changes to every related program.

## 3. Database Approach
- **Centralized Data**: All data is stored in a single repository.
- **Controlled Access**: Managed by a **Database Management System (DBMS)**, improving consistency and security.
- **Program-Data Independence**: Data is separated from programs, reducing the need for frequent updates to programs when data changes.
- **Advantages**:
  - Improved data consistency and sharing.
  - Reduced duplication.
  - Better decision-making due to centralized access.

## 4. Database Models and Relationships
- **Data Model**: A graphical representation of data, showing relationships between entities.
- **Entities**: Objects (people, places, things) stored in the database.
- **Relationships**: Define how entities are related (e.g., one-to-many or many-to-many).

## 5. Development Approaches
- **System Development Life Cycle (SDLC)**: A structured, step-by-step process for system development. Stages include planning, analysis, design, implementation, and maintenance.
- **Prototyping**: An iterative approach to system development with quick prototypes and frequent user feedback.

## 6. Database Schema
- **External Schema**: Defines how users view the data.
- **Conceptual Schema**: The overall structure of the data and its relationships.
- **Internal Schema**: Physical storage structure and how data is stored.

## 7. Evolution of Database Systems
- **Key Drivers**: Need for program-data independence, more complex data, ease of access, and better decision support systems.
- **Types**:
  - Personal databases.
  - Client-server databases.
  - Enterprise databases (ERP, Data Warehousing).

---

# Quiz

1. **What is an advantage of the database approach?**
   a) Duplication of data  
   b) Centralized control of data  
   c) Program-data dependence  
   d) Limited data sharing

2. **What is metadata?**
   a) Data about users  
   b) Data describing other data  
   c) Data stored in images  
   d) Data for system operations

3. **Which of the following is a disadvantage of the file processing system?**
   a) Centralized control  
   b) Program-data independence  
   c) Duplication of data  
   d) Easy data sharing

4. **What is program-data independence?**
   a) Separation of programs and data, reducing maintenance costs  
   b) Data stored in different files for each program  
   c) A single copy of data for multiple programs  
   d) Program requiring frequent updates

5. **Which of these describes the relationship between entities in a database?**
   a) Program-data independence  
   b) Prototyping  
   c) One-to-many or many-to-many  
   d) File processing
