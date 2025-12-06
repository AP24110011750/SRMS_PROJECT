# SRMS_PROJECT
STUDENT LOGIN AND MANAGEMENT SYSTEM (C)

This project is a terminal-based Student Login and Management System written in C. It supports three user roles: admin, staff, and guest. Each role has different levels of access and permissions. The program stores login credentials and student information in text files for simplicity.

FEATURES

Authentication

Users log in using a username and password.

Supports three roles: admin, staff, guest.

Password input is hidden using '*' characters.

Role-Based Access

ADMIN can:

Add student

Display all students

Search student

Update student

Delete student

Logout

STAFF can:

Add student

Display students

Search student

Update student

Logout

GUEST can:

Display students

Search student

Logout

DATA STORAGE

credentials.txt (used for login)
Format:
username password role

Example:
admin admin123 admin
staff1 staff123 staff
guest1 guest123 guest

students.txt (stores student records)
Format:
roll name mark

Example:
1 Alice 89.50
2 Bob 76.00
3 Charlie 92.25

HOW THE SYSTEM WORKS

User enters username and password.

Program validates them using the credentials.txt file.

Depending on the role, the user is taken to Admin Menu, Staff Menu, or Guest Menu.

All student-related operations are performed using students.txt.

Update and delete operations use a temporary file to rewrite updated data.

COMPILATION AND RUNNING

Linux or macOS or MinGW (gcc):

gcc main.c -o student_system
./student_system

Windows (MSVC):

cl main.c
main.exe

REQUIRED FILES

Create credentials.txt in the same folder:

admin admin123 admin
staff1 staff123 staff
guest1 guest123 guest

Optionally create an empty students.txt file.

LIMITATIONS

Passwords are stored as plain text.

Student names with spaces may not display correctly.

No validation for incorrect numeric inputs.

Text files can be edited manually (not secure).

No sorting or advanced filtering.

POSSIBLE FUTURE IMPROVEMENTS

Password encryption

Use of structs and binary files

Better validation

Sorting and filtering options

Graphical interface

Multiple search options such as search by roll number

AUTHOR

V.VANI
