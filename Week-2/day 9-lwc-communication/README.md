# Day 9 - LWC Communication & Application Architecture

## Component Communication

Lightning Web Components (LWC) communicate to exchange data and coordinate actions between components.

### Parent to Child Communication
- Parent component sends data to child component using @api properties.
- Child component receives and displays the data.

Example:
Student Dashboard → Student Details Component

### Child to Parent Communication
- Child component sends data back using Custom Events.
- Parent component listens and responds to the event.

Example:
Attendance Component → Dashboard Component

### Benefits of Component Communication
- Better modularity
- Reusable components
- Easy maintenance
- Improved scalability

---

# Dashboard Design

## Student Dashboard

Components:
- Student Profile
- Attendance
- Courses
- Notifications

Communication:
- Profile component shares student data.
- Attendance component displays attendance records.
- Course component displays enrolled courses.
- Notification component displays alerts and updates.

## Faculty Dashboard

Components:
- Faculty Profile
- Course Management
- Attendance Management
- Notifications

Communication:
- Faculty manages courses and attendance.
- Notifications inform students about updates.

## Admin Dashboard

Components:
- User Management
- Course Allocation
- Reports
- System Settings

Communication:
- Admin controls users and courses.
- Reports collect data from multiple components.

---

# Data Flow Explanation

## Process Chosen: Student Registration

### UI
Student enters registration details through the user interface.

### Validation
System validates required fields and checks data format.

### Flow
Registration request is processed through Salesforce Flow.

### Apex
Apex controller handles business logic and processing.

### Database
Student information is stored in Salesforce database.

### Notification
Confirmation message or email is sent to the student.

## Complete Flow

UI → Validation → Flow → Apex → Database → Notification

The student submits information through the UI. The system validates the data, processes it using Flow and Apex, stores the information in the database, and sends a confirmation notification.

---

# Aura vs LWC

| Aura Components | Lightning Web Components (LWC) |
|----------------|--------------------------------|
| Older Framework | Modern Framework |
| More Complex | Simpler and Faster |
| Lower Performance | Better Performance |
| Proprietary Model | Based on Web Standards |
| Harder Maintenance | Easier Maintenance |

## Why Salesforce Moved from Aura to LWC

- Better performance
- Faster rendering
- Modern web standards
- Easier development
- Better maintainability
- Improved scalability

---

# Reflection

## Why do enterprise applications need modular architecture?

Enterprise applications are large and complex. Modular architecture divides the application into smaller reusable components, making development and maintenance easier.

## Why is modular architecture useful?

- Reusability
- Scalability
- Easy maintenance
- Better collaboration
- Reduced code duplication

## Why should UI and backend remain separate?

Keeping UI and backend separate improves flexibility, security, and maintainability while allowing independent development.

## Why do large systems need reusable modules?

Reusable modules reduce development time, improve consistency, and simplify maintenance.

---

# Revision Questions

### 1. Why do components communicate?
Components communicate to share data and coordinate application behavior.

### 2. Difference between parent-child communication and events?
Parent-child communication passes data directly using properties, while events allow child components to notify parent components about actions.

### 3. Why is modular architecture useful?
It improves scalability, maintainability, and code reusability.

### 4. Why did Salesforce move toward LWC?
Salesforce moved toward LWC because it provides better performance, modern web standards, and easier development.

### 5. What problems happen in tightly coupled systems?
- Difficult maintenance
- Reduced flexibility
- Poor scalability
- Increased development effort

### 6. Why is frontend architecture important?
Frontend architecture improves user experience, maintainability, and application organization.

### 7. Why should UI and backend remain separate?
To allow independent development, better security, and easier maintenance.

### 8. Why do large systems need reusable modules?
Reusable modules reduce duplication, improve consistency, and increase development efficiency.

---

# Conclusion

Today I learned how Lightning Web Components communicate, how data flows through Salesforce applications, the importance of modular architecture, and why Salesforce moved from Aura Components to Lightning Web Components.
