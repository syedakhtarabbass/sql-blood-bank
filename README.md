Blood Bank Management System (Python + MySQL)

This project is a simple command-line Blood Bank Management System built using Python and MySQL. It allows registering blood donors, handling blood donation requests, viewing donors based on blood group, and deleting records.
It’s designed for beginners learning database connectivity with Python.

______________________________________________
📌 Features
1. Donor Registration
Add new donors with details such as:
Donor ID
Name
Date of Birth
Aadhar Number
Blood Group
Phone Number
Gmail
Address

2. Blood Donation Request
Register a patient who needs a specific blood group with:
Patient ID
Name
Phone Number
Required Blood Group
Age
Hospital Details

3. View Donors
Search and display donors by blood group.

5. Delete Records
Delete donor data
Delete patient request data
______________________________________________
🗄️ Database Requirement

Create a MySQL database named blood_bank with at least these tables:

Table: donors
Column Name	Type
DonorId	VARCHAR / INT
Name	VARCHAR
DOB	DATE
Aadhar	VARCHAR
Blood_Group	VARCHAR
Phone	VARCHAR
Gmail	VARCHAR
Address	VARCHAR
Table: donor_details

(Your project’s reduced donor table)

Table: anemic_patient
Column Name	Type
PatientId	VARCHAR / INT
Name	VARCHAR
Phone	VARCHAR
BloodGroup	VARCHAR
Age	INT
Hospital	VARCHAR
____________________________________________
⚙️ Installation & Setup
1. Install Required Python Modules
pip install mysql-connector-python

2. Configure MySQL
Update your MySQL credentials inside the script:
-------------------------------------------
con = mysql.connector.connect(
    host="localhost",
    user="root",
    password="YOUR_PASSWORD",
    database="blood_bank"
)
-------------------------------------------
4. Run the Program
python main.py
