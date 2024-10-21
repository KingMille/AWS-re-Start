AWS re/Start Project: Web App with Amazon Aurora Database
Overview
This project is part of my AWS re/Start course, where I built a web application integrated with a database using Amazon Aurora. The goal was to create a functional web app hosted on Amazon EC2 that interacts with a database to store and retrieve user data. It was a great opportunity to deepen my understanding of cloud computing, database management, and server configuration.

Project Structure
EC2 Instance: Set up to host the web application, providing the necessary environment for app deployment.
Amazon Aurora Database: Used for data storage, allowing the web app to interact with a scalable database instance.
Web Application: Developed using HTML and PHP, enabling users to add and view data such as names and addresses.
Software Installed:
Apache Server: For serving the web app.
MariaDB: Database server for interacting with Amazon Aurora.
MySQL CLI: Command-line tool for direct database management.
Features
User Input Form: A simple HTML form that allows users to input their name and address, which is then stored in the Amazon Aurora database.
Data Retrieval: Users can view the stored data directly from the web app interface.
Database Management: Ability to manage and manipulate the database directly using MySQL commands within the EC2 instance.
Challenges & Solutions
Permission Issues: Encountered permission errors while modifying files within the EC2 instance. Resolved these by adjusting user permissions to allow necessary modifications.
Database Connectivity: Configured the web app to securely connect with the Amazon Aurora database, ensuring smooth data flow between the app and database.
