# Healthcare-Information-Tool
The system is production-ready with security features like SQL injection protection, XSS prevention, and secure session management. All user inputs are stored in the database, and admins can manage the symptom database dynamically through the web interface.
Complete System Overview

Database & Backend
database_setup.sql: Complete MySQL schema with tables for users, symptoms, sessions, and admin users
config.php: Database configuration and helper functions
api/submit_symptoms.php: REST API endpoint for storing user submissions

User Interface
symptom_checker_with_db.html: Updated frontend that connects to the database
symptom_checker.html: Original standalone version (for reference)

Admin System
admin_login.php: Secure admin authentication
admin_dashboard.php: Main dashboard with statistics and recent activity
admin_symptoms.php: Complete symptom management (add/edit/delete)
admin_logout.php: Secure logout functionality

🚀 Key Features

For Users:
Symptom collection form with demographics
Educational information about each symptom
Emergency detection and warnings
Data stored securely in database

For Admins:
Secure login system (admin/admin123)
Dashboard with real-time statistics
Manage symptoms dynamically
View user submissions and patterns
Activity logging for security

Database Features:
Structured SQL with proper relationships
JSON storage for flexible symptom arrays
Emergency case tracking
Audit trails with timestamps
Soft deletes for data integrity

�� Setup Instructions
Set up your web server (Apache/Nginx with PHP)
Import the database: mysql -u root -p < database_setup.sql
Configure database in config.php
Access the system:
User interface: symptom_checker_with_db.html
Admin panel: admin_login.php

