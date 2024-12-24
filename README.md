# TeamSync: Collaborative Project Tracker

## Overview
TeamSync is a project management tool designed to help teams track and manage their work efficiently. The app integrates with GitHub to monitor task completions via commit messages, ensuring tasks are completed on schedule.

## Features
- **Multiple Projects Management**: Handle multiple projects with distinct tasks and team members.
- **Task Tracking**: Track task progress through GitHub commits.
- **Reminders**: Automated email reminders for overdue tasks.
- **Delay Functionality**: Easily reschedule tasks and adjust project timelines.

## Tech Stack
- **Frontend**: HTML, CSS, JavaScript
- **Backend**: Python (Flask or Django)
- **Database**: SQLite or PostgreSQL
- **APIs**: GitHub REST API for commit tracking, Python `smtplib` for email notifications.

## Setup
1. Clone the repository:
   ```
   git clone https://github.com/DavidHua04/TeamSync-CollaborativeProjectTracker.git
   ```
2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
3. Run the application:
   ```
   python run.py
   ```

## Contribution
Contributions are welcome! Please fork the project and submit a pull request with your improvements.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
