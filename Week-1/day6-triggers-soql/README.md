Day 6 — Triggers & SOQL
# 1. What is SOQL?

SOQL (Salesforce Object Query Language) is the query language used in Salesforce to retrieve data from Salesforce objects.

It is similar to SQL, but SOQL is specially designed for Salesforce data.

## SOQL helps developers:

> Fetch records
> Filter data
> Sort records
> Retrieve related object data
> Build automation logic
# Example
SELECT Name, Email FROM Contact
This query retrieves the Name and Email fields from the Contact object.
# 2. What is an Apex Trigger?

An Apex Trigger is a piece of code that runs automatically when certain events happen in Salesforce.

## Triggers execute before or after actions like:

> Insert
> Update
> Delete
> Undelete

Triggers help automate business processes and enforce business rules.

## Example Use Cases
> Send notifications after record creation
> Prevent invalid data from saving
> Automatically update related records
> Create audit logs
> Maintain data consistency
# 3. Difference
## Flow vs Trigger
| Flow                              | Trigger                          |
| --------------------------------- | -------------------------------- |
| Declarative automation            | Programmatic automation          |
| Built using drag-and-drop tools   | Written using Apex code          |
| Easier for admins                 | Requires developers              |
| Best for simple automation        | Best for complex logic           |
| Faster to build                   | More flexible and powerful       |
| Less technical knowledge required | Strong coding knowledge required |
## Conclusion

Flows are preferred for simple business automation, while Triggers are used for advanced logic and complex system behavior.
| Before Trigger                                     | After Trigger                                       |
| -------------------------------------------------- | --------------------------------------------------- |
| Runs before data is saved                          | Runs after data is saved                            |
| Used for validation and modifying values           | Used for actions after save                         |
| Faster because changes happen before database save | Used when record ID is needed                       |
| Commonly used to update field values               | Commonly used for notifications and related records |
## Example
### Before Trigger

Automatically format a phone number before saving.

### After Trigger

Send a welcome email after a customer record is created.
# 4. Trigger Use Cases (5 Examples)
## 1. Automatic Welcome Email

When a new customer account is created, the system automatically sends a welcome email.

## 2. Prevent Invalid Data

If a user enters a negative salary value, the trigger prevents the record from saving.

## 3. Update Related Records

When an Opportunity is closed, the related Account status is automatically updated.

## 4. Create Audit Logs

Whenever important fields are changed, the system stores old and new values for tracking.

## 5. Inventory Management

When a product order is placed, stock quantity automatically decreases.

# 5. Query Examples
## Example 1
English Idea

Get all customers from Hyderabad.

### SOQL:
SELECT Name FROM Account WHERE BillingCity = 'Hyderabad'
## Example 2
English Idea

Find all contacts with Gmail accounts.

### SOQL:
SELECT Name, Email FROM Contact WHERE Email LIKE '%gmail.com'
## Example 3SELECT Name, CreatedDate FROM Lead ORDER BY CreatedDate DESC
English Idea

Retrieve all opportunities with amount greater than 1 lakh.

### SOQL:
SELECT Name, Amount FROM Opportunity WHERE Amount > 100000
## Example 4
English Idea

Get recently created leads.

### SOQL:
SELECT Name, CreatedDate FROM Lead ORDER BY CreatedDate DESC
## Example 5
English Idea

Find all active customers.

### SOQL:
SELECT Name FROM Account WHERE Active__c = true
6. Reflection

Enterprise systems react automatically to data changes because businesses need real-time automation.

Modern companies handle thousands or millions of records daily. Manual monitoring is impossible.

Triggers and automation systems help:

Maintain data accuracy
Reduce human effort
Improve speed
Enforce business rules
Keep systems synchronized
Provide instant responses to events

For example:

Banks detect suspicious transactions instantly
E-commerce systems update inventory automatically
CRM systems send notifications immediately
Healthcare systems alert doctors about emergencies

This event-driven behavior makes enterprise systems intelligent and efficient.

# Reflective Questions
## 1. Why do systems need triggers?

Systems need triggers to automatically respond to important events without human intervention. They improve efficiency, accuracy, and consistency.

## 2. Difference between polling and event-driven systems?
Polling System

The system continuously checks for changes repeatedly.

Event-Driven System

The system reacts only when an event occurs.

Event-driven systems are faster and more efficient because they avoid unnecessary checking.

## 3. Why are database queries important?

Database queries help retrieve useful business information quickly.

Without queries, organizations cannot analyze customers, sales, reports, or operations effectively.

## 4. When should Flows be preferred over Triggers?

Flows should be preferred when:

Automation is simple
No advanced coding is needed
Admins need to maintain the logic
Faster development is required

Triggers should only be used for complex business logic.

## 5. What problems happen if automation logic becomes too complex?

Complex automation can cause:

Slow performance
Difficult debugging
Confusing business processes
System errors
Maintenance challenges
Unexpected automation conflicts
## 6. Why should developers think carefully before automating actions?

Automation directly affects business operations and customer data.

Poor automation can create incorrect updates, duplicate records, system failures, or bad customer experiences.

Developers must ensure automation is reliable, efficient, and aligned with business requirements.

# End of Day Outcome

After completing this task, I now understand:

How Salesforce queries data using SOQL
How event-driven systems work
What Apex Triggers do
Difference between declarative and programmatic automation
How enterprise systems react intelligently to data changes


