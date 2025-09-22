# Mergington High School Activities

A comprehensive FastAPI web application for managing extracurricular activities at Mergington High School. The system allows teachers to manage student registrations and provides students with easy access to view and explore available activities.

## Features

### For Students
- **Browse Activities**: View all available extracurricular activities with detailed information
- **Search & Filter**: Find activities using search or filter by:
  - Category (Sports, Arts, Academic, Community, Technology)
  - Day of the week (Monday through Sunday)
  - Time period (Before School, After School, Weekend)
- **Activity Details**: See comprehensive information including:
  - Activity descriptions and schedules
  - Current enrollment and available spots
  - Participant lists
  - Capacity indicators with visual progress bars

### For Teachers
- **Authentication System**: Secure login system for teachers and administrators
- **Student Registration**: Register students for activities via email
- **Student Management**: Remove students from activities when needed
- **Real-time Updates**: View current enrollment status and manage capacity

### Technical Features
- **RESTful API**: FastAPI backend with comprehensive endpoints
- **Real-time Filtering**: Client-side and server-side filtering capabilities
- **Responsive Design**: Mobile-friendly interface with modern UI components
- **Modal Interfaces**: Clean registration and login forms
- **Database Integration**: MongoDB for persistent data storage
- **Multiple Time Periods**: Support for before school (6:00-8:00 AM), after school (3:00-6:00 PM), and weekend activities

## Activity Categories

The system automatically categorizes activities into:
- **Sports**: Soccer Team, Basketball Team, Morning Fitness
- **Arts**: Art Club, Drama Club, Creative activities
- **Academic**: Math Club, Science Olympiad, Debate Team, Chess Club
- **Technology**: Programming Class, Weekend Robotics Workshop
- **Community**: Various community service activities

## API Endpoints

- `GET /activities` - Retrieve all activities with optional filtering
- `GET /activities/days` - Get available activity days
- `POST /activities/{activity_name}/signup` - Register a student for an activity
- `POST /activities/{activity_name}/unregister` - Remove a student from an activity
- `POST /auth/login` - Teacher authentication
- `GET /auth/check-session` - Validate teacher session

## Development Guide

For detailed setup and development instructions, please refer to our [Development Guide](../docs/how-to-develop.md).
