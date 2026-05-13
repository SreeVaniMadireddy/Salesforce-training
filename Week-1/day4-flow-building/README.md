Day 4 – Flow Builder

#What is Flow Builder?

Flow Builder is a Salesforce automation tool used to create business workflows without writing code. It helps automate repetitive tasks like updating records, sending notifications, creating tasks, and guiding users through screens. Businesses use Flow Builder to improve productivity, reduce manual work, and avoid human errors.


---

#Types of Flows

##1. Screen Flow

Screen Flow is a type of flow that interacts with users through screens. It is used when user input is required.

###Example:

A student registration form where users enter their details.

###Features:

Requires user interaction

Displays screens and forms

Collects data from users

Used for guided processes



---

##2. Record-Triggered Flow

Record-Triggered Flow runs automatically when a record is created, updated, or deleted.

###Example:

Automatically sending a fee reminder email when the due date is near.

###Features:

Runs automatically

No manual action required

Used for automation processes

Helps maintain consistency



---

#Automation Ideas for College Management System
##1. Auto Email After Student Registration
###Automation Process
When a student completes registration, Salesforce automatically sends a confirmation email with registration details.
###Why Automation Helps
Automation saves staff time and ensures every student instantly receives confirmation without manual effort.
##2. Auto Generate Student ID
###Automation Process
After admission approval, the system automatically creates a unique student ID for the student.
###Why Automation Helps
It reduces human errors, avoids duplicate IDs, and speeds up the admission process.
##3. Auto Update Available Seats
###Automation Process
Whenever a student joins or leaves a course, the system automatically updates the remaining seat count.
###Why Automation Helps
It keeps records accurate in real time and helps students know seat availability immediately.
##4. Notify Faculty When Course is Full
###Automation Process
When the maximum number of students join a course, Salesforce automatically sends a notification to faculty members.
###Why Automation Helps
It helps faculty manage classes better and prevents over-enrollment issues.
##5. Automatic Fee Reminder
###Automation Process
Before the fee deadline, the system automatically sends reminder emails or messages to students.
###Why Automation Helps
It reduces late payments, decreases manual follow-up work, and improves fee collection efficiency.
##6. Automatic Attendance Alert
###Automation Process
If a student’s attendance goes below the required percentage, the system automatically sends a warning message.
###Why Automation Helps
It helps students improve attendance early and reduces manual monitoring by faculty.
##7. Exam Result Notification
###Automation Process
When exam results are published, Salesforce automatically notifies students through email or SMS.
###Why Automation Helps
Students receive updates quickly without waiting for manual announcements.
##8. Library Due Date Reminder
###Automation Process
Before the return date of a borrowed book, the system automatically sends reminders to students.
###Why Automation Helps
It reduces late returns and helps manage library resources efficiently.

----

#Flow Design Thinking

##Selected Automation:

Automatic Fee Reminder System

##Flow Process:

Fee Due Date Near
        ↓
Check Student Payment Status
        ↓
Has Student Paid?
   ↓ Yes          ↓ No
  End        Send Reminder Email

Explanation:

The flow automatically checks whether a student has paid the fee. If the payment is not completed, Salesforce sends a reminder email automatically.

---

#Manual vs Automated Process

##Process Chosen:

Student Fee Reminder

##Manual Process

Staff members manually check fee records and send reminder messages or emails individually to students.

##Problems in Manual Process

Time consuming

Chances of missing some students

Human errors may occur

Requires continuous monitoring


##Automated Process Using Salesforce

Salesforce automatically checks fee due dates and sends reminder emails to students whose payments are pending.

Benefits of Automation

Faster process

Reduces human effort

Improves accuracy

Saves time

Increases productivity



---

#Reflection – Why Automation Matters in Enterprise Systems

Automation is important because it helps companies save time, reduce repetitive work, improve accuracy, and increase productivity. It allows employees to focus on important business tasks instead of doing repetitive manual work. Automation also improves consistency, customer experience, and overall efficiency in enterprise systems.


---

#Reflective Questions

##1. Why do companies automate workflows?

Companies automate workflows to save time, reduce errors, improve efficiency, and increase productivity.

##2. What problems happen with manual processes?

Manual processes are slow, repetitive, error-prone, and require more human effort.

##3. Difference between Screen Flow and Record Triggered Flow?

Screen Flow requires user interaction, while Record Triggered Flow runs automatically in the background.

##4. Why is no-code automation powerful?

No-code automation allows businesses to automate processes quickly without requiring programming knowledge.

##5. When should automation be avoided?

Automation should be avoided for processes that require human judgment, creativity, or complex decision-making.

##6. How does automation improve consistency and productivity?

Automation performs tasks the same way every time, reducing errors and helping employees complete work faster.


---

#Conclusion

Through this Day 4 Flow Builder activity, I learned how Salesforce automates business workflows using no-code tools. I understood different flow types, automation logic, record updates, and how automation improves efficiency in enterprise systems.
