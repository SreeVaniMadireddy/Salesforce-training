# Salesforce Summer Program – Day 3

# 1. Difference Between App, Object, Record, and Field

## App
An app in Salesforce is a collection of tools, tabs, and objects designed for a specific business process.

Example:
Sales App, Service App

---

## Object
An object is like a database table that stores data.

Example:
Student Object

---

## Record
A record is a single row of data stored inside an object.

Example:
Student Name = Rahul

---

## Field
A field stores one piece of information inside a record.

Example:
Student Email

---

# 2. Standard vs Custom Objects

## Standard Objects
Standard objects are already provided by Salesforce.

Examples:
- Account
- Contact
- Opportunity

---

## Custom Objects
Custom objects are created based on business requirements.

Examples:
- Student
- Faculty
- Course
- Department

---

# 3. College Management System Data Model

## Objects Used
- Student
- Faculty
- Course
- Department

---

## Relationships

### Department → Faculty
One department can have many faculty members.

Relationship Type:
Lookup Relationship

---

### Department → Course
One department can offer many courses.

Relationship Type:
Lookup Relationship

---

### Course → Student
One course can have many students.

Relationship Type:
Lookup Relationship

---

# College Data Model Diagram

![College Data Model](images/college-data-model.png)

---

# 4. Formula Fields

## Full Name
Formula combines First Name and Last Name automatically.

Why?
This reduces manual typing and avoids mistakes.

---

## Remaining Seats
Remaining Seats = Total Seats - Enrolled Students

Why?
This automatically tracks available seats in a course.

---

## Percentage
Percentage = Obtained Marks / Total Marks * 100

Why?
This avoids manual calculations and saves time.

---

# 5. Validation Rules

## Email Cannot Be Empty
Prevents saving student records without email.

Why?
Email is important for communication.

---

## Student Age Cannot Be Negative
Blocks invalid age values.

Why?
Prevents incorrect data entry.

---

## Course Seats Cannot Exceed Limit
Prevents adding students beyond course capacity.

Why?
Maintains proper seat management.

---

# 6. Reflection

Structured data helps companies organize information properly and maintain relationships between records.

It improves reporting, automation, and data accuracy.

Random spreadsheets become difficult to manage when multiple teams work together and when data becomes very large.

---

# Reflective Questions

## 1. Why can’t companies manage everything using Excel sheets?

Excel sheets become difficult to manage when data becomes very large and shared across departments.

---

## 2. Why are relationships important between objects?

Relationships connect related data and reduce duplication.

---

## 3. What problems happen if data is inconsistent?

Incorrect reports and wrong business decisions can happen.

---

## 4. Why should repetitive calculations be automated?

Automation saves time and reduces human errors.

---

## 5. Why should invalid data be blocked early?

It keeps the database accurate and reliable.

---

## 6. Why is Salesforce called a metadata-driven platform?

Salesforce allows users to build applications using configuration without heavy coding.
