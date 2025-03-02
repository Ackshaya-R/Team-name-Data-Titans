1. Project Title:
    AI-Driven Non-Invasive Health Monitoring System with Smart Chatbot  

2. Overview :
• Monitoring glucose, cholesterol, and hemoglobin levels traditionally requires blood tests, which can be invasive, time-consuming, and uncomfortable for many individuals. 
Regular health check-ups become difficult due to the need for laboratory tests and professional assistance.
• We are developing a non-invasive health monitoring system that uses saliva & sweat analysis to detect blood glucose, hemoglobin, and cholesterol levels. 
• This system eliminates the need for needle-based blood tests and provides a painless, real-time health tracking solution. 
• An AI chatbot will provide health tips, diet suggestions, and answer queries, making health monitoring easy and painless. 

3. Technologies Used: 
• Java - programming language. 
• Swing (GUI) - Utilized to make buttons, text fields, and windows. 
• MySQL (Database) - Keeps health data. 
• JDBC (Database Connection) - Bridges Java and MySQL. 
• NLP Simple Chatbot - Makes use of keywords such as "exercise" and "diet" to provide health advice.

4. Setup the Environment
• Install Java (JDK 8 or above).
• Install MySQL and set up the database.
• Ensure you have JDBC Driver for MySQL.

5. Configure the Database
• Open MySQL and create a database:
       CREATE DATABASE HEALTHs;
• Use the following table structure:
    CREATE TABLE users (
    id INT PRIMARY KEY,
    name VARCHAR(255),
    sodium FLOAT,
    potassium FLOAT,
    lactose FLOAT,
    glucose FLOAT,
    hemoglobin FLOAT,
    cholesterol FLOAT
);

6. Configure Database Credentials
• Open Health.java
• Update these lines with your MySQL details:
   private static final String URL = "jdbc:mysql://localhost:3306/HEALTHs";
   private static final String USER = "root";  // Update if needed
   private static final String PASSWORD = "yourpassword";  // Set your password

7. Compile and Run the Program
• Open the project in any Java IDE (Eclipse, IntelliJ, or VS Code).
• Compile and run the Health.java file.

8. Using the Application
• Enter ID, Name, and health values (Sodium, Potassium, Lactose).
• Click Check to calculate Glucose, Hemoglobin, and Cholesterol levels.
• The results will be displayed in a new window.
• Data is automatically saved to the database.

9. Chatbot Feature
• Type health-related queries in the chatbot (e.g., "glucose," "diet," "cholesterol").
• The bot will provide relevant health tips.

10. Features:  
• Sensor-Based Health Analysis 
• AI-Powered Prediction 
• User-Friendly Data Entry 
• Secure User Login 
• AI Chatbot Support  
• Database Storage & Management

11. Technical Workflow: 
• Sensors detect sodium, potassium, and lactose concentrations from sweat or saliva. 
• Software calculates glucose, cholesterol, and hemoglobin based on medically approved formulas. 
• Predicted values are stored in a database. 
• The users can log in with their username and password to monitor their health history 
in the long term. 
• The system allows users to compare past and present health records for better monitoring. 
• The NLP- driven chatbot gives tips on health based on predicted values and responds to user questions regarding diet, exercise and overall health. 

12. Future Enhancement:
The system currently utilizes Natural Language Processing(NLP) to have the chatbot offer health-related recommendations. 
This will be complemented in the future with an AI-based doctor consultation feature, enabling users to consult doctors directly within the app if their estimated glucose, cholesterol, or hemoglobin
levels are High.
