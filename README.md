# RaceDay

RaceDay is a full-stack, web-based event management system built for the South African road running, walking and cycling community. A lot of local events (park runs, charity walks, club races) are still run off paper registers, spreadsheets and WhatsApp groups, so this project digitises that process. Organisers can create and manage events, set up age/distance categories, and capture results. Participants can browse upcoming events, enter them, track their own results history, and (in a later part of this project) check the weather and route for race day.

This repository currently contains **Part 1** of the Portfolio of Evidence: the system planning phase. No application code has been written yet — this part is purely the ERD, the API endpoint plan, and the SQL database script, as required before Part 2 begins.

## Roles

The system has two roles, assigned to a user when they register:

- **Organiser** – creates, updates and deletes their own events, defines the age/distance categories for each event, views who has enrolled, and captures finish times and positions after the event.
- **Participant** – browses events, enrols in an event under a chosen category, and views their own enrolment and results history. Participants can't manage events or capture results for other people.

Both roles can view and update their own profile information.

## Part 1 contents (`/docs`)

- `ERD_RaceDay.png` – entity relationship diagram for the RaceDay database (6 entities: Roles, Users, Events, Categories, EventEnrolments, Results).
- `API_Endpoint_Plan.md` – full list of planned API endpoints, covering authentication, user profile, events, categories, event enrolments and results.
- `RaceDay_Database_Script.sql` – SQL Server script that creates the schema and seeds it with sample data (2 organisers, 2 participants, 3 events, categories, and enrolments).

## CI/CD

A GitHub Actions workflow runs on push and checks that the repository structure is correct (that the `/docs` folder exists and contains the required planning files).

Screenshot of a successful build:
<img width="1363" height="717" alt="image" src="https://github.com/user-attachments/assets/6c6148f5-25b9-4713-9d9b-143ace781f9c" />




## Video walkthrough

Unlisted YouTube video walking through the planning documents, the ERD decisions, the endpoint plan, and running the SQL script live in SSMS:

https://youtu.be/2loYNUHwaPg?si=6ZT5BwveyANaIagE

