Public Health Clinic Records System

Project Overview

The Public Health Clinic Records System is a relational database management project developed using MySQL. The system is designed to manage patient records, healthcare workers, appointments, visits, diagnoses, and treatments within a healthcare facility.

The project demonstrates the implementation of database concepts such as primary keys, foreign keys, relationships, data integrity, and SQL operations.

---

Project Team

Name| Student ID
Kerry Rufus Aldy Davies| 905005923
Destiny Mustapha Koroma| 905005458
Joshua Leonard Sinava Jones| 905006421

---

Database Name

public_health_clinic_records

---

Features

- Patient Management
- Health Worker Management
- Appointment Scheduling
- Visit Tracking
- Diagnosis Recording
- Treatment Management
- User Account Management
- SQL CRUD Operations (Create, Read, Update, Delete)

---

Database Structure

The system consists of six main tables:

1. Patient

Stores patient information.

Field
Patient_ID
Name
Date_Of_Birth
Gender
Phone
Address

---

2. Health_Worker

Stores information about healthcare staff.

Field
Worker_ID
Name
Role
Phone
Qualification

---

3. Appointment

Stores appointment information.

Field
Appointment_ID
Appointment_Date
Appointment_Time
Patient_ID
Health_Worker_ID
Status

---

4. Visit

Stores patient visit records.

Field
Visit_ID
Visit_Date
Reason
Patient_ID
Health_Worker_ID

---

5. Diagnosis

Stores diagnosis information.

Field
Diagnosis_ID
Diagnosis
Visit_ID
Result

---

6. Treatment

Stores treatment information.

Field
Treatment_ID
Medication
Dosage
Instructions
Diagnosis_ID

---

Relationships

- One Patient can have many Appointments.
- One Patient can have many Visits.
- One Health Worker can manage many Appointments.
- One Health Worker can attend many Visits.
- One Visit can have many Diagnoses.
- One Diagnosis can have many Treatments.

---

SQL Operations Implemented

INSERT

Used to add records into tables.

INSERT INTO Patient
(Patient_ID, Name, Date_Of_Birth, Gender, Phone, Address)
VALUES
(905001,'John Kamara','1995-03-12','Male','076123456','Freetown');

SELECT

Used to retrieve records.

SELECT * FROM Patient;

UPDATE

Used to modify records.

UPDATE Patient
SET Phone='076111111'
WHERE Patient_ID=905001;

DELETE

Used to remove records.

DELETE FROM Patient
WHERE Patient_ID=905001;

---

User Accounts

Username| Role
kerry| Administrator
destiny| Database User
joshua| Database User

---

Technologies Used

- MySQL
- phpMyAdmin
- XAMPP
- SQL
- Windows Operating System

---

Sample Record Counts

Table| Number of Records
Patient| 20
Health_Worker| 20
Appointment| 20
Visit| 20
Diagnosis| 20
Treatment| 20

---

Future Improvements

- User Authentication System
- Patient Billing Module
- Medical Report Generation
- Mobile Application Integration
- Dashboard and Analytics

---

Conclusion

The Public Health Clinic Records System successfully demonstrates the design and implementation of a relational database for healthcare record management. The system improves efficiency, data organization, and record accessibility while maintaining data integrity through the use of primary and foreign key relationships.

---

License

This project was developed for academic purposes as part of a Database Systems course.
