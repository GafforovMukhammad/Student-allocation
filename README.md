# Student-allocation
https://popsql.com/queries/-NqHww5ou_nGkgPCQusc/untitled-query-2024-02-10-1717
DROP TABLE student;
CREATE TABLE student(
    student_id INT AUTO_INCREMENT,
    name VARCHAR(20),
    major VARCHAR(70) DEFAULT 'undecided',
    PRIMARY KEY(student_id)
);

-- SELECT * FROM student;
INSERT INTO student(name, major) VALUES('Mukhammad', 'Biology');
INSERT INTO student(name, major) VALUES('Abdulaziz', 'Computer Science');
INSERT INTO student(name, major) VALUES('Amir', 'International  Relations');
INSERT INTO student(name, major) VALUES('John', 'Economics');


UPDATE student
SET major = 'Business'
WHERE major = 'International relation' or major = 'Economics';
SELECT * FROM  student;

**Description**
--This SQL script initializes a simple database table named student with columns for student_id, name, and major. The student_id is set as an auto-incrementing integer acting as the primary key. The name column holds the name of each student, while the major column denotes their chosen field of study, defaulted to 'undecided' if not specified.

Commands in the Script
CREATE TABLE student: Defines the structure of the student table with appropriate column names and data types.
INSERT INTO student: Inserts records into the student table with specified name and major.
UPDATE student: Updates the major column for certain students where their major is either 'International relation' or 'Economics', setting it to 'Business'.
SELECT * FROM student: Displays all records from the student table after the update operation.
This script can be used as a basis for setting up a student database within a larger database management system.
