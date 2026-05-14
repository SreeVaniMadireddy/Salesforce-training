# Day 5 – Apex Introduction

## 1. What is Apex?

Apex is a programming language used in Salesforce to add custom business logic and automation that cannot be handled fully using clicks or configuration tools.

It is similar to Java and runs on the Salesforce platform.

Apex helps developers:

- Automate complex processes
- Validate business rules
- Integrate external systems
- Perform calculations
- Create custom workflows
- Handle advanced logic

Example:
If a college wants to automatically block students with unpaid fees from registering for exams, Apex can handle that logic.

---

# 2. Difference

## Flow vs Apex

| Flow | Apex |
|---|---|
| No-code / low-code tool | Programming language |
| Built using drag-and-drop | Written using code |
| Easy for admins | Used by developers |
| Good for simple automation | Good for complex automation |
| Faster to build | More flexible and powerful |
| Limited for advanced logic | Can handle advanced conditions and integrations |

---

## Configuration vs Coding

| Configuration | Coding |
|---|---|
| Uses clicks and settings | Uses programming |
| Faster and easier | Requires developer knowledge |
| Limited flexibility | Highly customizable |
| Best for simple business rules | Best for complex business logic |
| Easier to maintain | Requires testing and debugging |

---

# 3. Real Examples Where Apex Is Needed

## Example 1: Automatic Scholarship Eligibility

If a student's attendance is above 90% and CGPA is above 8.5, Apex automatically marks them eligible for scholarships.

---

## Example 2: Fee Due Restriction

Apex blocks hall ticket generation if pending fee amount is greater than a certain limit.

---

## Example 3: External Payment Integration

Apex connects Salesforce with external payment gateways to verify fee payments automatically.

---

# 4. Integrated System Design

# College Management System

## CRM

CRM helps manage relationships between:

- Students
- Faculty
- Parents
- Administration

The system stores and tracks all interactions and academic activities.

---

## Objects

Custom Objects used:

| Object Name | Purpose |
|---|---|
| Student | Stores student details |
| Faculty | Stores faculty information |
| Course | Stores course data |
| Attendance | Stores attendance records |
| Fee | Stores fee details |
| Scholarship | Stores scholarship information |
| Exam | Stores exam details |

---

## Relationships

| Relationship | Type |
|---|---|
| Student → Course | Many-to-One |
| Student → Attendance | One-to-Many |
| Student → Fee | One-to-Many |
| Faculty → Course | One-to-Many |

Relationships help connect related data together.

---

## Validation Rules

Validation rules ensure correct data entry.

Examples:

- Attendance cannot exceed 100%
- Fee amount cannot be negative
- Student ID must follow proper format
- CGPA must be between 0 and 10

---

## Flow

Flows automate simple processes.

Examples:

- Send email after student registration
- Update attendance percentage automatically
- Notify students about fee due dates
- Create welcome messages

---

## Apex

Apex handles advanced business logic.

Examples:

- Scholarship eligibility calculation
- Automatic semester promotion
- Prevent exam registration for low attendance
- Integration with payment systems

---

# 5. Pseudocode Examples

## Scholarship Eligibility Logic

```text
IF attendance > 90
AND CGPA > 8.5
THEN
    Eligible = TRUE
ELSE
    Eligible = FALSE
# Fee Due Restriction
IF pending_fee > 5000
THEN
    Block Hall Ticket
ELSE
    Allow Hall Ticket
# Attendance Warning System
IF attendance_percentage < 75
THEN
    Send Warning Email
# 6. Reflection

Enterprise systems eventually need programming because every business has unique requirements that cannot always be handled using only no-code tools.

In the beginning, configuration tools like Flows and Validation Rules are enough for simple tasks. But as the system grows, business processes become more complex and require custom logic.

Apex helps developers build scalable and flexible solutions for real-world problems such as advanced automation, integrations, calculations, and security handling.

This helped me understand that Salesforce is not only about clicks and configuration, but also about solving business problems using the right balance of no-code and programming.

---

# Reflective Questions

## 1. Why is Apex needed if Salesforce already has Flows?

Flows are useful for simple automation, but Apex is needed for complex business logic, integrations, advanced calculations, and large-scale data processing.

---

## 2. When should developers prefer no-code solutions?

Developers should prefer no-code solutions when the requirement is simple, easy to maintain, and can be solved using existing Salesforce tools.

---

## 3. What problems require custom programming?

Problems involving:
- Complex calculations
- External system integrations
- Advanced validations
- Dynamic business rules
- Large data operations

usually require custom programming using Apex.

---

## 4. Why is business logic important in enterprise systems?

Business logic ensures that organizational rules, processes, and policies are correctly followed inside the system.

It helps maintain accuracy, consistency, and automation in business operations.

---

## 5. Why should developers avoid unnecessary coding?

Unnecessary coding increases:
- Complexity
- Maintenance effort
- Chances of bugs
- Testing time

Using simpler no-code solutions whenever possible makes systems easier to manage.

---

## 6. How does programming increase flexibility?

Programming allows developers to:
- Create custom features
- Handle complex requirements
- Integrate external platforms
- Build scalable solutions

This makes enterprise systems more powerful and adaptable to changing business needs.
