# Event Management Database System

A comprehensive relational database system designed to manage events, attendees, organizers, registrations, and related information for an event management platform.

## Project Overview

This project implements a normalized relational database for managing events and their related entities. It's designed to handle event creation, attendee registration, ticketing, payment processing, and feedback collection.

## Database Tables

The system includes the following core entities:

- **Event** - Event details and information
- **Attendee** - Attendee profiles and demographics
- **Attendee Contact** - Contact information for attendees
- **Organizer** - Event organizer information
- **Organizer Email** - Email addresses for organizers
- **Organizer Phone** - Phone numbers for organizers
- **Venue** - Event venue details
- **Registration** - Attendee registration records
- **Ticket** - Ticket information and allocation
- **Payment** - Payment transaction records
- **Feedback** - Attendee feedback and reviews

## Features

 Normalized database schema following best practices  
 Comprehensive entity relationships  
 Support for multiple contact methods (email, phone)  
 Payment and ticketing integration  
 Feedback and review system  
Scalable design for multiple events and attendees  

## Project Structure

```
├── sql files/              # SQL scripts for table creation
│   ├── event.sql
│   ├── attendee.sql
│   ├── attendee_contact.sql
│   ├── organizer.sql
│   ├── organizer_email.sql
│   ├── organizer_phone.sql
│   ├── venue.sql
│   ├── registration.sql
│   ├── ticket.sql
│   ├── payment.sql
│   └── feedback.sql
├── diagrams/               # Database schema diagrams
│   └── Database Schema.pdf
├── docs/                   # Project documentation
│   ├── GroupWork_EventManagement_DB.docx
│   └── Normalization steps.docx
└── README.md              # This file
```

## Database Setup

### Prerequisites
- SQL Server / MySQL / PostgreSQL (depending on your system)
- Database management tool (SQL Server Management Studio, MySQL Workbench, pgAdmin, etc.)

### Installation

1. Create a new database for the project
2. Execute the SQL files in the following order:
   ```sql
   event.sql
   attendee.sql
   attendee_contact.sql
   organizer.sql
   organizer_email.sql
   organizer_phone.sql
   venue.sql
   registration.sql
   ticket.sql
   payment.sql
   feedback.sql
   ```

3. Verify all tables are created successfully

## Database Schema

The database follows normalization best practices (3NF). See `diagrams/Database Schema.pdf` for the complete Entity-Relationship Diagram (ERD).

Key relationships:
- **Events** are organized by **Organizers** and held at **Venues**
- **Attendees** register for **Events** and receive **Tickets**
- **Payments** are processed for ticket purchases
- **Feedback** is collected from attendees after events

## Documentation

- **GroupWork_EventManagement_DB.docx** - Comprehensive project documentation
- **Normalization steps.docx** - Detailed normalization process and decisions

## Team

This is a group project for the Database Systems course at Strathmore University (First Year).

## Course Information

- **Institution**: Strathmore University
- **Course**: Database Systems
- **Level**: First Year
- **Project Type**: Group Work

## License

This project is created for educational purposes.

## Notes

- All SQL scripts are designed to be compatible with standard SQL syntax
- Adjust script syntax if using a specific database management system
- Review the normalization documentation for understanding design decisions
- Refer to the database schema diagram for visual representation of relationships

---

For questions or contributions, please contact the project team or submit issues through the repository.
