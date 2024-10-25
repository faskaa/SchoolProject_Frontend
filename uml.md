@startuml

entity Student {
    +student_id: INT [PK]
    --
    first_name: VARCHAR
    last_name: VARCHAR
    email: VARCHAR
    faculty: VARCHAR
    course: INT
    status: VARCHAR
}

entity Teacher {
    +teacher_id: INT [PK]
    --
    first_name: VARCHAR
    last_name: VARCHAR
    subject: VARCHAR
    status: VARCHAR
}

entity Program {
    +program_id: INT [PK]
    --
    name: VARCHAR
    faculty: VARCHAR
    duration: VARCHAR
    credits: INT
    status: VARCHAR
}

entity Application {
    +application_id: INT [PK]
    --
    student_id: INT [FK]
    program_id: INT [FK]
    date: DATE
    status: VARCHAR
}

entity Inquiry {
    +inquiry_id: INT [PK]
    --
    name: VARCHAR
    email: VARCHAR
    subject: VARCHAR
    message: TEXT
    date: DATE
    status: VARCHAR
}

entity Event {
    +event_id: INT [PK]
    --
    name: VARCHAR
    date: DATE
    location: VARCHAR
    participants: INT
    status: VARCHAR
}

entity Club {
    +club_id: INT [PK]
    --
    name: VARCHAR
    description: TEXT
    members: INT
    foundation_date: DATE
    status: VARCHAR
}

entity News {
    +news_id: INT [PK]
    --
    title: VARCHAR
    content: TEXT
    date: DATE
    category: VARCHAR
    status: VARCHAR
}

entity File {
    +file_id: INT [PK]
    --
    name: VARCHAR
    type: VARCHAR
    size: VARCHAR
    upload_date: DATE
}

entity Page {
    +page_id: INT [PK]
    --
    name: VARCHAR
    url: VARCHAR
    content: TEXT
    last_updated: DATE
    status: VARCHAR
}

entity Gallery {
    +gallery_id: INT [PK]
    --
    title: VARCHAR
    description: TEXT
    file_path: VARCHAR
}

entity Schedule {
    +schedule_id: INT [PK]
    --
    class: VARCHAR
    day: VARCHAR
    start_time: TIME
    end_time: TIME
    subject: VARCHAR
    teacher_id: INT [FK]
    room: VARCHAR
}

Student ||--o{ Application : applies
Program ||--o{ Application : offers
Teacher ||--o{ Schedule : teaches
Student ||--o{ Event : participates
Student ||--o{ Club : joins

@enduml
