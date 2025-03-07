# CampusConnect-WebApp

CampusConnect is a comprehensive Event Management System built with **Django** that streamlines the creation, management, and approval of events within an organization or institution. It enhances collaboration between users and administrators through an intuitive interface and automated email notifications. 

---

## Features

### User Features
- **Create Events**: Users can create events with details such as title, description, date & time, location, and an optional event photo.
- **Update Events**: Users can update their own events while ensuring unauthorized edits are prevented.
- **Event Approval Workflow**: Events created by users require administrator approval to be published.

### Admin Features
- **Event Notifications**:
  - New event creation triggers an email notification to the admin/superuser with detailed event information for review.
  - Updates to existing events also notify the admin.
- **Approval/Disapproval Notifications**:
  - Admins can approve or reject events. The respective user is notified via email about the status of their event.

### Email Notifications
- **Automated Emails**:
  - Emails are sent for key actions using Django's `send_mail`.
  - Emails include detailed event information such as title, description, date & time, location, and more.

---

## Technologies Used
- **Backend**: Django (Python)
- **Frontend**: Django Templates (HTML, CSS)
- **Database**: SQLite (default Django database)
- **Email Integration**: SMTP with Django's email utilities
