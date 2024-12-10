# University Timetable Web Application

This project is a Flask web application that dynamically displays a university timetable based on the student's level. It connects to a PostgreSQL database, allowing filtering of courses by levels (`Level 1`, `Level 2`, `Level 3`) and is containerized using Docker.

---

## Features
- **Dynamic Timetable:** Displays a filtered timetable for selected levels.
- **Database Integration:** PostgreSQL database stores course data.
- **Docker Support:** Fully containerized for easy deployment.
- **Web Interface:** User-friendly interface to select and view timetables.

---

## Technologies Used
- **Backend:** Python, Flask
- **Database:** PostgreSQL
- **Containerization:** Docker, Docker Compose
- **Frontend:** HTML, CSS

---

## Prerequisites
1. **Install Docker:** Download and install Docker from [Docker's website](https://www.docker.com/).
2. **Git Installed:** Ensure Git is installed.

---

## Getting Started
### Step 1: Clone the Repository
```bash
git clone <repository_url>
cd <repository_name>


here is the all commands that i used 


cd "C:\Users\hp\Downloads\PostgreSQL\pgsql\bin"

pg_ctl -D "C:\Users\hp\Downloads\PostgreSQL\pgsql\data" start

psql -h localhost -U postgres


CREATE DATABASE asad;

CREATE TABLE timetable (
    id SERIAL PRIMARY KEY,
    course_name VARCHAR(100),
    level VARCHAR(50),
    day VARCHAR(20),
    time_slot VARCHAR(50),
    room VARCHAR(50)
);

INSERT INTO timetable (course_name, level, day, time_slot, room)
VALUES
    ('Global Social Problems', 'level 1', 'Wednesday', '11:30 AM - 01:50 PM', 'Room A'),
    ('IT Project Management, 'level 2', 'Monday', '09:00 AM - 11:20 AM', 'Room B'),
    ('Systems Analysis and Design', 'level 3', 'Friday', '09:00 AM - 11:20 PM', 'Room C'),
    ('Computer Architecture', 'level 1', 'Friday', '11:30 AM - 01:50 PM', 'Room D'),
    ('Management Theory', 'level 2', 'Monday', '11:30 AM - 01:50 PM', 'Room E'),
    ('Principles of Programming', 'level 1', 'Wednesday', '09:00 AM - 11:20 AM', 'Room F');







docker-compose up --build

docker-compose logs web

docker-compose logs db




docker exec -it final-db-1 bash
psql -U postgres -d asad



\dt


CREATE TABLE timetable (
    id SERIAL PRIMARY KEY,
    course_name VARCHAR(100),
    level VARCHAR(50),
    day VARCHAR(20),
    time_slot VARCHAR(50),
    room VARCHAR(50)
);


INSERT INTO timetable (course_name, level, day, time_slot, room)
VALUES

    ('Social Engineering', 'Level 2', 'Friday', '11:30 AM - 01:50 PM', 'Room 408'),
    ('Computer Languages', 'Level 1', 'Friday', '09:00 AM - 11:20 AM', 'Room 115'),
    ('Operating Systems', 'Level 2', 'Wednesday', '11:30 AM - 01:50 PM', 'Room 114'),
    ('Contemporary Europe', 'Level 3', 'Monday', '11:30 AM - 01:50 PM', 'WebNet+'),
    ('Introduction to Ethics', 'Level 1', 'Wednesday', '09:00 AM - 11:20 AM', 'Room 403'),
    ('Survey of Economics', 'Level 3', 'Monday', '09:00 AM - 11:20 AM', 'Room 406'),
    ('Mathematics for Computer', 'Level 1', 'Monday', '12:30 PM - 03:20 PM', 'Room 307'),
    ('Marketing', 'Level 2', 'Friday', '12:30 PM - 03:20 PM', 'WebNet+'),
    ('Descriptive Statistics', 'Level 3', 'Thursday', '12:30 PM - 03:20 PM', 'WebNet+'),
    ('Computer Programming II', 'Level 2', 'Wednesday', '09:30 AM - 12:20 PM', 'Room 114'),
    ('Financial Accounting I', 'Level 1', 'Monday', '09:30 AM - 12:20 PM', 'Room 229'),
    ('Network Principles', 'Level 3', 'Wednesday', '12:30 PM - 03:20 PM', 'Room 304');
    ('Global Social Problems', 'level 1', 'Wednesday', '11:30 AM - 01:50 PM', 'Room A'),
    ('IT Project Management, 'level 2', 'Monday', '09:00 AM - 11:20 AM', 'Room B'),
    ('Systems Analysis and Design', 'level 3', 'Friday', '09:00 AM - 11:20 PM', 'Room C'),
    ('Computer Architecture', 'level 1', 'Friday', '11:30 AM - 01:50 PM', 'Room D'),
    ('Management Theory', 'level 2', 'Monday', '11:30 AM - 01:50 PM', 'Room E'),
    ('Principles of Programming', 'level 1', 'Wednesday', '09:00 AM - 11:20 AM', 'Room F');


SELECT * FROM timetable;

docker-compose down
docker-compose up --build
