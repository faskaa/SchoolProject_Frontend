# Database Diagram

## Tables and Relationships

### Student
- **student_id**: INT [PK]
- first_name: VARCHAR
- last_name: VARCHAR
- email: VARCHAR
- faculty: VARCHAR
- course: INT
- status: VARCHAR

### Teacher
- **teacher_id**: INT [PK]
- first_name: VARCHAR
- last_name: VARCHAR
- subject: VARCHAR
- status: VARCHAR

### Program
- **program_id**: INT [PK]
- name: VARCHAR
- faculty: VARCHAR
- duration: VARCHAR
- credits: INT
- status: VARCHAR

### Application
- **application_id**: INT [PK]
- student_id: INT [FK]
- program_id: INT [FK]
- date: DATE
- status: VARCHAR

### Inquiry
- **inquiry_id**: INT [PK]
- name: VARCHAR
- email: VARCHAR
- subject: VARCHAR
- message: TEXT
- date: DATE
- status: VARCHAR

### Event
- **event_id**: INT [PK]
- name: VARCHAR
- date: DATE
- location: VARCHAR
- participants: INT
- status: VARCHAR

### Club
- **club_id**: INT [PK]
- name: VARCHAR
- description: TEXT
- members: INT
- foundation_date: DATE
- status: VARCHAR

### News
- **news_id**: INT [PK]
- title: VARCHAR
- content: TEXT
- date: DATE
- category: VARCHAR
- status: VARCHAR

### File
- **file_id**: INT [PK]
- name: VARCHAR
- type: VARCHAR
- size: VARCHAR
- upload_date: DATE

### Page
- **page_id**: INT [PK]
- name: VARCHAR
- url: VARCHAR
- content: TEXT
- last_updated: DATE
- status: VARCHAR

### Gallery
- **gallery_id**: INT [PK]
- title: VARCHAR
- description: TEXT
- file_path: VARCHAR

### Schedule
- **schedule_id**: INT [PK]
- class: VARCHAR
- day: VARCHAR
- start_time: TIME
- end_time: TIME
- subject: VARCHAR
- teacher_id: INT [FK]
- room: VARCHAR

## Relationships

- **Student** applies to **Program** through **Application**.
- **Teacher** teaches **Schedule**.
- **Student** participates in **Event**.
- **Student** joins **Club**.
