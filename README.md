# WhatsApp Database
This project contains SQL scripts for creating tables and populating data in a WhatsApp-like database. The database includes tables for users, groups, group members, chats, statuses, status_view. It also includes an Entity Relationship Diagram (ERD) showing the relationships between tables and a view to see the sender name, receiver name, messages sent between them with timestamps.

### Prerequisites
SQL Server or any other relational database management system
Knowledge of SQL language
Getting Started
Create a database in your SQL Server or any other relational database management system.

### Run the SQL scripts :
**Scripts.sql**  which contains 6 tables and 1 view as follows: 
.`Users`
`Groups`
`GroupMembers`
`Chats`
`Statuses`
`Status_Views`
`ChatDetails`

Check the tables and data in the database to make sure they have been created and populated correctly.

# Entity Relationship Diagram
Here is an Entity Relationship Diagram (ERD) that shows the relationships between tables in the database:
<img width="625" alt="doc" src="https://user-images.githubusercontent.com/54138835/216763100-1d1db83f-1c7b-4f01-9c65-aac72488299a.PNG">


**Users table**:  contains information about each user, including their UserID, UserName, and PhoneNumber.

**Groups table**:  contains information about each group, including their GroupID and GroupName.

**GroupMembers table**:  links users and groups, connecting a user to the groups they are a member of.

**Chats table**:  contains information about each chat, including the ChatID, SenderID, ReceiverID, Message, and Timestamp.

**Status table**:  contains information about each status, including the UserID, StatusID, and Number of views. 

**Status_View**:  contains information about each status viewed, including the UserID, StatusID,   ViewID and isViewed?. 

### View
The ChatDetails view is created to see the sender name, receiver name, messages sent between them with timestamps. This view joins the Chats table with the Users table to display the sender and receiver names instead of their UserIDs.

## Conclusion
This project provides a basic foundation for creating a WhatsApp-like database, including tables for users, groups, group members, status, status_views and chats. The ERD and view provide an overview of the relationships between tables and a convenient way to see the sender name, receiver name, messages sent between them with timestamps.




