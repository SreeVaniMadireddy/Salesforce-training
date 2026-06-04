# Salesforce Summer Program - Day 14

## Objective

Learn how enterprise systems use Flow Builder, branching logic, approval workflows, and governance to ensure controlled and secure business operations.

---

# Task 1: Multi-Level Approval Design

## Course Creation Approval Workflow

### Approval Process

1. Faculty submits a new course proposal.
2. Head of Department (HOD) reviews the proposal.
3. Academic Dean approves the course.
4. Principal gives final approval.

### After Approval

- Course is added to the Course Catalog.
- Faculty receives a confirmation notification.

### After Rejection

- Proposal is returned with comments.
- Faculty can modify and resubmit.

---

## Faculty Leave Request Approval Workflow

### Approval Process

1. Faculty submits a leave request.
2. HOD reviews the request.
3. Principal approves if the leave exceeds predefined limits.

### After Approval

- Leave status changes to Approved.
- Attendance and workload records are updated.

### After Rejection

- Faculty receives a rejection notification with the reason.

---

## Student Scholarship Request Approval Workflow

### Approval Process

1. Student submits a scholarship application.
2. Scholarship Committee verifies eligibility.
3. Finance Department reviews funding availability.
4. Principal provides final approval.

### After Approval

- Scholarship amount is allocated.
- Student receives approval notification.

### After Rejection

- Application status changes to Rejected.
- Student receives feedback.

---

## Budget Approval Workflow

### Approval Process

1. Department submits a budget request.
2. Finance Officer reviews the request.
3. Finance Manager approves the budget.
4. Principal provides final approval.

### After Approval

- Budget is allocated.
- Department receives confirmation.

### After Rejection

- Request is returned with remarks for revision.

---

# Task 2: Branching Flow Logic

## Attendance Monitoring Workflow

### Decision Point

Check student attendance percentage.

### Branch 1: Attendance Below 75%

#### Action Triggered

- Send warning email to the student.
- Advise attendance improvement.

### Branch 2: Attendance Below 60%

#### Action Triggered

- Notify parents or guardians.
- Schedule a counseling session.

### Branch 3: Attendance Below 50%

#### Action Triggered

- Escalate the issue to administration.
- Generate a disciplinary review request.

### Workflow Benefits

- Early identification of attendance issues.
- Automated communication.
- Reduced manual monitoring effort.
- Improved student accountability.

---

# Task 3: Governance Thinking

## Why Can't Enterprise Systems Allow Everyone to Directly Change Important Records?

### Security

- Sensitive information must be protected from unauthorized access.

### Prevention of Misuse

- Users may intentionally or accidentally modify critical records.

### Approval Control

- Important business actions require verification before execution.

### Business Risk Reduction

- Incorrect changes can cause financial loss, compliance violations, and operational disruptions.

### Auditability

- Every change must be traceable for accountability and compliance.

---

# Task 4: Reflection

## Why Do Enterprises Require Controlled Workflows Instead of Unrestricted Actions?

Controlled workflows ensure:

- Proper authorization before actions are executed.
- Compliance with organizational policies.
- Reduction of errors and fraudulent activities.
- Clear accountability through approval tracking.
- Consistent and reliable business processes.
- Better governance and risk management.

Without controlled workflows, organizations may face security breaches, data inconsistencies, financial losses, and regulatory issues.

---

# Key Learnings

- Understanding of Approval Workflows.
- Design of Multi-Level Approval Processes.
- Implementation of Branching Flow Logic.
- Importance of Governance in Enterprise Systems.
- Role of Controlled Workflows in Business Operations.
- Enterprise-Level Process Automation Concepts.

---

# Revision Questions and Answers

## 1. Why are approval workflows important?

Approval workflows ensure that critical actions are reviewed and authorized before execution, reducing errors and risks.

## 2. Why do businesses require governance?

Governance provides control, accountability, security, and compliance across business operations.

## 3. What are branching workflows?

Branching workflows use decision points to direct different actions based on specific conditions.

## 4. Why should automation follow business rules?

Business rules ensure automation aligns with organizational policies and objectives.

## 5. Why are decision nodes important in flows?

Decision nodes allow workflows to take different paths based on conditions and outcomes.

## 6. Why should enterprises restrict sensitive operations?

Restrictions protect critical data, prevent misuse, and maintain system integrity.

## 7. Why are approvals important in large organizations?

Approvals provide accountability, verification, and controlled decision-making.

## 8. Why should workflows be auditable?

Auditable workflows help track actions, ensure compliance, and support investigations when needed.
