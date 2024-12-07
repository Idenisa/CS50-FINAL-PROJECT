# CS50-FINAL-PROJECT
# Medication Reminder

#### Video Demo:  [https://youtu.be/_aDOEbZT4MM]

#### Description:

LINK: http://127.0.0.1:5000/

The "Medication Reminder" web application is designed to help users manage and keep track of their medication schedules. This application ensures that users receive timely notifications to take their medications, helping them adhere to their prescribed treatment plans. The application is built using Flask for the backend, SQLite for the database, Socket.IO for real-time notifications, and a front-end comprising HTML, CSS, and JavaScript.

## Features

### Backend (Flask Application)
- **Database Initialization**:
  - The application initializes an SQLite database to store medication information. The database includes fields such as the name of the medication, dosage, frequency, start and end dates, and any additional notes.
- **Scheduler**:
  - A background scheduler checks for medications that need notifications based on their prescribed schedules. This runs every minute to ensure timely alerts.
- **Notification System**:
  - Utilizes Socket.IO to send real-time notifications to users when it's time to take their medication.

### Frontend (HTML, CSS, JavaScript)
- **User Interface**:
  - The interface includes a form to add new medications, listing sections for past, current, and upcoming medications, and real-time notifications.
- **Form Management**:
  - A form to register medications with fields for the name, dosage, frequency, start and end dates, and notes. The form supports both adding new medications and updating existing ones.
- **Medication Display**:
  - Medications are categorized and displayed based on their schedule status: past, today, and upcoming.
- **Dynamic Interactions**:
  - Users can add, edit, and delete medications. The form for adding medications can be toggled to show or hide based on user interactions.

### File Overview

- **`app.py`**:
  - Contains the main Flask application logic, including routes for adding, updating, and deleting medications. Also, handles database initialization and scheduling checks for notifications.
  
- **`index.html`**:
  - The main HTML template that structures the page, including the form for adding medications and sections for listing them. It includes necessary links to CSS and JavaScript files.

- **`styles.css`**:
  - Contains the styling for the web application, ensuring a user-friendly and visually appealing interface.

- **`app.js`**:
  - Handles the frontend logic, including form validation, sending data to the server, and managing real-time notifications.

### How to Use
1. **Register a Medication**:
   - Fill out the form with the name, dosage, frequency, start and end dates, and any notes. Click "Save Medicine" to add the medication to the database.
2. **View Medications**:
   - Medications are listed under categories: past, today, and upcoming. This helps users keep track of what has been taken and what needs to be taken.
3. **Receive Notifications**:
   - The application will send real-time notifications when it's time to take a medication based on the schedule.
4. **Update or Delete Medications**:
   - Users can edit the details of a medication or delete it from the list using the provided buttons.

### Challenges and Design Decisions
- **Date Validation**:
  - Ensured that the start date of a medication is earlier than the end date to avoid logical errors.
- **Real-time Notifications**:
  - Implemented using Socket.IO to provide instant alerts, ensuring users do not miss their medication times.
- **User Interface**:
  - Designed to be intuitive and easy to navigate, allowing users to manage their medications with minimal effort.

### Conclusion
The "Medication Reminder" application serves as a helpful tool for individuals who need assistance in managing their medication schedules. By providing timely reminders and an easy-to-use interface, it aims to improve medication adherence and overall health outcomes.

FOR THIS PROJECT I HAVE USED IA.

If you have any questions or need further assistance, feel free to reach out!

