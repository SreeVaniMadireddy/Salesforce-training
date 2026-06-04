# College Management System – Salesforce Mini Project

## System Overview

The College Management System is developed using Salesforce to manage students, faculty, courses, and departments. The application uses custom objects, relationships, validation rules, flows, reports, dashboards, and Apex logic to automate college operations.

---

## CRM Concepts

### Student
Stores student details such as name, email, phone number, attendance, and enrolled course.

### Faculty
Stores faculty information including name, email, phone number, and department.

### Course
Stores course information such as course name and total seats.

### Department
Stores department details such as department name and department code.

---

## Data Model

### Objects Created

#### Department
- Department Name
- Department Code

#### Faculty
- Faculty Name
- Email
- Phone
- Department (Lookup Relationship)

#### Course
- Course Name
- Total Seats

#### Student
- Student Name
- Email
- Phone
- Attendance
- Course (Lookup Relationship)

### Relationships

- Faculty → Department
- Student → Course

---

## Validation Rules

### Email Mandatory Validation

Purpose:
Ensure every student record contains an email address.

Formula:

ISBLANK(Email__c)

Error Message:

Email is mandatory.

---

## Flows

### Attendance Warning Flow

Trigger:
Student record is created or updated.

Condition:
Attendance is less than 75%.

Action:
Send warning email to the student.

### Course Registration Confirmation Flow

Trigger:
Student record is created.

Action:
Send confirmation email after successful registration.

Subject:
Course Registration Successful

Message:
You have successfully registered for the course.

---

## Apex Logic

### Course Trigger

```java
trigger CourseTrigger on Courses__c (after update) {

    for(Courses__c c : Trigger.new){

        if(c.Total_Seats__c == 0){

            System.debug('Course Full');
        }
    }
}
