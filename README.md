_ Hospital Database System

Project Overview
This project is a hospital database system designed to manage patients, doctors, appointments, medical records, billing, and services.  
The system helps organize hospital operations and ensures data accuracy and consistency.

Key Design Decisions
- Used separate entities for Patient, Doctor, Appointment, and Medical Record to improve organization.
- Avoided deleting data; instead used status fields (e.g., cancelled, inactive).
- Added support for real-world scenarios such as:
  - Partial payments (Payment entity)
  - Service price changes (Price History)
- Used relationships and foreign keys to maintain data integrity.

Challenges Faced
- Handling complex relationships such as the M:N relationship between Appointment and Services.
- Managing real-world scenarios such as:
  - Price changes over time
  - Doctors leaving the system
- Ensuring that no data is lost during updates or modifications.
