
 # Attendease - Face Recognition Attendance System

Attendease is an automated attendance management system using face recognition technology. It provides different interfaces for students, teachers, and administrators to manage attendance records efficiently.

## Features

- **Face Recognition Attendance**: Automatically marks attendance using computer vision
- **Multi-role Access**:
  - Students can view their attendance records
  - Teachers can view and manage class attendance
  - Admins can manage students, teachers, and timetables
- **Timetable Integration**: Smart attendance marking based on class schedules
- **Late Detection**: Identifies latecomers automatically
- **Comprehensive Reporting**: Generates attendance statistics and reports

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/Attendease-Attendance-Management-System.git


Install dependencies:

bash
pip install -r requirements.txt
Set up the database 

Run the application:

bash

python src/main.py

Database Setup

This repository includes database schema files but no actual student/teacher data. 

The empty_database.db file shows the expected structure

Modify timetable/timetable.json to set up your class schedule

Add your own icons to the icons/ folder

The system will automatically create an attendance/ directory for CSV records

Usage

 Main Menu: Choose your role (Student, Teacher, Admin)
 Student Login: View your attendance records
 Teacher Login: View and manage class attendance
 Admin Panel: Manage all system data and settings


# Database Structure

This describes the database schema for the Attendease system. Note that the repository contains only the database structure without any actual student or teacher data.

## Tables

### 1. students

| Column      | Type        | Description                     |
|-------------|-------------|---------------------------------|
| roll_no     | TEXT (PK)   | Student roll number             |
| name        | TEXT        | Student name                    |
| age         | INTEGER     | Student age                     |
| gender      | TEXT        | Gender (Male/Female/Other)      |
| department  | TEXT        | Department/Class                |
| image       | BLOB        | Student photo (optional)        |
| password    | TEXT        | Hashed password                 |

### 2. teachers

| Column      | Type        | Description                     |
|-------------|-------------|---------------------------------|
| teacher_id  | TEXT (PK)   | Teacher ID                      |
| name        | TEXT        | Teacher name                    |
| subject     | TEXT        | Subject taught                  |
| password    | TEXT        | Hashed password                 |

### 3. admin

| Column      | Type        | Description                     |
|-------------|-------------|---------------------------------|
| admin_id    | TEXT (PK)   | Admin ID                        |
| name        | TEXT        | Admin name                      |
| password    | TEXT        | Hashed password                 |


