
CREATE DATABASE <database_name>;
SHOW DATABASES;
CONNECT <database_name>;
CREATE TABLE <table_name_in_plural> (); 
INSERT INTO <table_name_in_plural>
(columns)
VALUES (values);

Utility Commands
\! cls 
mysqldump -u root -p --databases library_db > C:\Users\Admin\Documents\dev\DEV-IT30A\backups\08182026_library_db.sql
mysqldump -u root -p --databases library_db > "C:\Users\Admin\Documents\dev\DEV-IT30A\backups\%date:~-4%_%date:~4,2%_%date:~7,2%_%time:~0,2%_%time:~3,2%_%time:~6,2%_library_db.sql"

ALTER TABLE students ADD COLUMN students_created_at TIMESTAMP NULL DEFAULT NULL;
UPDATE students SET students_created_at = CURRENT_TIMESTAMP WHERE students_created_at IS NULL;
ALTER TABLE students MODIFY COLUMN students_created_at TIMESTAMP NOT NULL DEFAULT CURRENT_TIMESTAMP;

INSERT INTO students (student_first_name,student_last_name,student_course_)
    -> VALUES ("ERON", "MOQUETE","BSIT");
    