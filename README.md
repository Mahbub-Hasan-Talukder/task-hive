# nstu-codebreakers

## Team Members
- Mahbub-Hasan-Talukder (Team Leader)
- 1Shishir
- Tahsin007

## Mentor
- chisty2996

## Project Description
# TASK-HIVE

A robust task management and project collaboration Flutter application with Supabase integration.


> **Screenshots**: 
<p align="center">
  <img src="https://github.com/user-attachments/assets/091d6919-d2d1-4e29-bbe7-664d40be7499" width="220" height="480">
  <img src="https://github.com/user-attachments/assets/a9d276ed-4f40-4334-b2b4-b67f938e21b0" width="220" height="480">
  <img src="https://github.com/user-attachments/assets/f25dd44d-4f34-4f37-a93f-19bf99be00fc" width="220" height="480">
  <img src="https://github.com/user-attachments/assets/6aadb3c4-8d05-4009-a0b9-a1f16376da0f" width="220" height="480">
</p>
## Overview

TASK-HIVE is a comprehensive project and task management solution that enables teams to efficiently collaborate on projects, track progress, and manage workloads. Built with Flutter and backed by Supabase, it offers a seamless experience across multiple platforms.

## Features

### Authentication Module

- **Secure Login System**:
  - Email/password authentication
  - Form validation with real-time feedback
  - Secure password storage with encryption

- **Signup Process**:
  - Email verification
  - Password strength requirements
  - User profile creation

- **Password Recovery**:
  - Email-based recovery workflow
  - Secure token-based reset mechanism
  - Expiring reset links for security

### Project Dashboard

- **Project Management**:
  - Grid and list view options for projects
  - Project cards with progress indicators
  - Color-coded project categorization
  - Search and filter functionality
  - Project creation with custom templates

- **Quick Actions**:
  - Create new project
  - Pin important projects
  - Archive completed projects
  - Project analytics summary

### Task Management System

- **Kanban Board**:
  - Column-based task organization:
    - To-Do
    - In Progress
    - Done
    - Blocked
  - Drag-and-drop functionality
  - Collapsible columns
  - Task count indicators

- **Task Details**:
  - Title and subtitle fields
  - Rich text description
  - Due date with reminder options
  - Priority levels (Low, Medium, High, Urgent)
  - Custom labels and tags
  - Checklists for subtasks

- **Task Assignment**:
  - User assignment with avatars
  - Multiple assignees support
  - Notification system for assignments
  - Workload visibility

- **Attachments**:
  - Multiple file uploads
  - Image previews
  - Storage quotas
  - File versioning

### User Profile Management

- **Profile Features**:
  - Personal information management
  - Profile picture upload
  - Role-based permissions
  - Activity history and statistics
  - Notification preferences
  - Theme settings

## Technical Implementation

### Frontend Architecture

TASK-HIVE implements a clean architecture pattern with:

- **Presentation Layer**: Flutter UI components with Material Design 3
- **Business Logic Layer**: BLoC pattern for state management
- **Domain Layer**: Core business logic and models
- **Data Layer**: Repository pattern for data access

### Backend Integration

- **Supabase Integration**:
  - Real-time data synchronization
  - PostgreSQL database
  - Row-level security (RLS) policies
  - Supabase Auth for authentication
  - Supabase Storage for file management


## Database Structure

TASK-HIVE uses the following Supabase tables:

- **Users**: Stores user profiles and authentication data
- **Projects**: Contains project metadata and ownership information
- **Tasks**: Manages task details including status, priority, and due dates
- **Task Assignees**: Tracks assignment of tasks to team members
- **Attachments**: Stores file metadata for task attachments

## Project Structure

The project follows a modular structure:

- **Core**: Configuration, constants, utilities, and error handling
- **Data**: Models, repositories, and data sources
- **Domain**: Business logic, entities, and use cases
- **Presentation**: UI components, screens, and state management
  - **Authentication Screens**: Login, signup, password recovery
  - **Dashboard**: Project overview and management
  - **Project Screens**: Task board and project details
  - **Task Management**: Task creation and editing
  - **Profile**: User profile management

## Dependencies

Key Flutter packages used:

- **State Management**: flutter_bloc, equatable
- **Supabase**: supabase_flutter
- **UI Components**: flutter_svg, cached_network_image, shimmer
- **Forms**: form_field_validator
- **Utilities**: intl, flutter_dotenv, logger
- **File Handling**: path_provider, file_picker


## Performance Features

- Lazy loading for efficient data fetching
- Local caching for offline access
- Background synchronization
- Optimized image loading
- Efficient state management

## Security

- JWT-based authentication
- Secure data storage
- Input validation and sanitization
- Supabase Row Level Security policies
- Encrypted data transmission

## Future Enhancements

- Team collaboration features
- Advanced reporting and analytics
- Calendar integration
- Time tracking
