## Github Group Work To-DO App
### Step 1: Define the Features and Structure
The key features to include:
- **Multiple Projects**: Each project will have its own set of tasks and coworkers.
- **Coworker Management**: Store coworker names and emails.
- **Task Management**: Each task will include:
  - Assigned coworkers.
  - Task description.
  - GitHub commit message.
  - Deadline.
  - Tags.
- **Task Tracking**: Monitor GitHub commit history for the given commit message and check if tasks are completed on time.
- **Reminders**: Send reminder emails to assigned coworkers if a task is overdue.
- **Delay Functionality**: Allow tasks to be pushed forward in case of delays.

### Step 2: Technology Stack
Based on your skill set and project requirements, here’s a recommended tech stack:
- **Frontend (UI)**:
  - **HTML/CSS** for structure and styling.
  - **JavaScript** for dynamic functionality.
  
- **Backend**:
  - **Python (Flask or Django)**: A lightweight framework like Flask could handle backend logic. Flask can interact with the GitHub API and send emails using libraries like `smtplib` or `Flask-Mail`.
  
- **Database**:
  - **SQLite or PostgreSQL**: To store coworkers, tasks, and project data.

- **GitHub API**:
  - Use the **GitHub REST API** to fetch commit history and validate whether the correct commit messages were used within the deadline.
  
- **Email Notifications**:
  - Use Python’s `smtplib` or an external service like **SendGrid** to send reminder emails when tasks are overdue.

### Step 3: GitHub API Integration
We need to:
1. **Authenticate**: Set up GitHub API authentication (OAuth or personal access tokens).
2. **Fetch Commits**: Use the API to retrieve the commit history for a specific repository. Check if any commit message matches the one assigned to the task.
3. **Deadline Checking**: Compare the commit date to the task's deadline. If no matching commit is found before the deadline, send a reminder email.

### Step 4: Building the User Interface (UI)
- **Task Overview**: Create a dashboard where users can:
  - View all tasks, filtered by project, coworker, or tags.
  - See tasks sorted by deadline, with an indicator for overdue tasks.
  
- **Add New Projects/Tasks/Coworkers**: Create forms for adding new projects, coworkers, and tasks.

### Step 5: Backend Logic for Task Management
We need to:
- **Create New Tasks**: Allow users to add tasks, assign coworkers, set a deadline, and enter the expected GitHub commit message.
- **Track Progress**: Periodically check GitHub commit history (perhaps using a cron job or scheduled task) to see if tasks are completed.

### Step 6: Implementing the Delay Button
- Implement a "delay" button that shifts all task deadlines by a specified amount of time.
- Ensure this delay applies consistently across all tasks, adjusting the schedule accordingly.

### Step 7: Testing and Deployment
- **Testing**: Make sure to test the GitHub API integration and email notification system thoroughly.
- **Deployment**: Consider deploying on a platform like **Heroku** or **AWS**.

---
