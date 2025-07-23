# StudyPal - Student Study Management App

A comprehensive full-stack web application designed to help students manage their study time effectively.

## Features

### Frontend
- **Multilingual Support**: Arabic and English with RTL/LTR text direction
- **Theme Support**: Dark/Light mode based on device settings
- **Responsive Design**: Works on desktop, tablet, and mobile devices
- **Dashboard**: Today's schedule, pending tasks, and progress summary
- **Task Management**: Add, edit, delete tasks with priority and due dates
- **Calendar View**: Visual display of study sessions and tasks by date
- **Progress Tracking**: Weekly and monthly productivity charts
- **Authentication**: User registration and login system

### Backend
- **Secure Authentication**: JWT-based login/register/logout
- **REST API**: Complete CRUD operations for tasks
- **Calendar API**: Manage study sessions and events
- **Progress API**: Track and analyze productivity data
- **Database**: Secure data storage with user isolation
- **Security**: Protected routes and data validation

## Tech Stack

### Frontend
- React 18 with TypeScript
- React Router for navigation
- React Query for state management
- Tailwind CSS for styling
- React i18next for internationalization
- Chart.js for progress visualization
- React Hook Form for form handling

### Backend
- Node.js with Express
- MongoDB with Mongoose
- JWT for authentication
- bcrypt for password hashing
- CORS for cross-origin requests
- Express validation middleware

## Getting Started

### Prerequisites
- Node.js (v16 or higher)
- MongoDB (local or cloud instance)

### Installation

1. Clone the repository
2. Install dependencies:
   ```bash
   npm run install-deps
   ```

3. Set up environment variables:
   - Copy `.env.example` to `.env` in the server directory
   - Update the variables with your configuration

4. Start the development servers:
   ```bash
   npm run dev
   ```

This will start both the frontend (React) and backend (Express) servers concurrently.

### Build for Production

```bash
npm run build
```

## Project Structure

```
StudyPal/
├── client/          # React frontend
├── server/          # Express backend
├── package.json     # Root package.json for scripts
└── README.md        # This file
```

## API Endpoints

### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout

### Tasks
- `GET /api/tasks` - Get user tasks
- `POST /api/tasks` - Create new task
- `PUT /api/tasks/:id` - Update task
- `DELETE /api/tasks/:id` - Delete task

### Calendar
- `GET /api/calendar` - Get calendar events
- `POST /api/calendar` - Create calendar event
- `PUT /api/calendar/:id` - Update calendar event
- `DELETE /api/calendar/:id` - Delete calendar event

### Progress
- `GET /api/progress` - Get user progress data
- `POST /api/progress` - Log progress entry

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

MIT License - see LICENSE file for details
