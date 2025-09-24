<<<<<<< HEAD
# HabbaHub - College Event Management System

<div align="center">
  <img src="frontend/public/simba.png" alt="HabbaHub Logo" width="800" />
</div>

## Overview
HabbaHub is a real-time event management platform designed specifically for college environments. It enables seamless organization and participation in college events, featuring live updates and interactive leaderboards.

## Key Features
- 🎫 Event Management & Registration
- 📢 Real-time Announcements
- 🏆 Live Leaderboard Updates
- 👥 Role-based Access Control
- 📱 Real-time Notifications
- 📊 Event Analytics

<div align="center">
  <img src="frontend/public/HabbaHub-readme-images/event-page.png" alt="Event Management" width="600" />
  <p><em>Event Management Interface</em></p>
</div>

## Technology Stack
- **Frontend**: React.js with TailwindCSS
- **Backend**: Node.js with Express.js
- **Database**: MongoDB
- **Real-time Communication**: Socket.IO
- **Authentication**: JWT-based

## Architecture
HabbaHub follows a microservice architecture with four core services:

- **Authentication Service**: User management and authentication
- **Event Service**: Event creation and management
- **Notification Service**: Real-time announcements
- **Leaderboard Service**: Participant scoring and rankings

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (v4.4 or higher)
- npm or yarn

### Installation

1. Clone the repository
```bash
git clone https://github.com/AbhishekBalija/HabbaHub.git
cd HabbaHub
```

2. Install dependencies
```bash
# Install frontend dependencies
cd frontend
npm install

# Install backend dependencies
cd ../backend
cd auth-service && npm install
cd ../event-service && npm install
cd ../notification-service && npm install
cd ../leaderboard-service && npm install
```

3. Environment Setup
```bash
# Create .env files in each service directory
# Example for auth-service:
MONGODB_URI=mongodb://localhost:27017/HabbaHub
JWT_SECRET=your_jwt_secret
PORT=8001
```

4. Start the services
```bash
# Start all services using Docker
docker-compose up

# Or start services individually
cd auth-service && npm run dev
cd event-service && npm run dev
cd notification-service && npm run dev
cd leaderboard-service && npm run dev
cd frontend && npm start
```

## User Roles

| Role | Access Level |
|------|-------------|
| Admin | Full system access, user management |
| Organizer | Event creation and management |
| Participant | Event registration and participation |

<div align="center">
  <table>
    <tr>
      <td align="center">
        <img src="frontend/public/HabbaHub-readme-images/admin-dashboard.png" alt="Admin Dashboard" width="250" /><br>
        <em>Admin Dashboard</em>
      </td>
      <td align="center">
        <img src="frontend/public/HabbaHub-readme-images/organizer-dashboard.png" alt="Organizer Dashboard" width="250" /><br>
        <em>Organizer Dashboard</em>
      </td>
      <td align="center">
        <img src="frontend/public/HabbaHub-readme-images/participant-home.png" alt="Participant View" width="250" /><br>
        <em>Participant Home</em>
      </td>
    </tr>
  </table>
</div>

## API Services

### Authentication Service (Port: 8001)
- User registration and login
- JWT token management
- Role-based access control

<div align="center">
  <img src="frontend/public/HabbaHub-readme-images/login-page.png" alt="Authentication" width="400" />
  <p><em>User Authentication Interface</em></p>
</div>

### Event Service (Port: 8002)
- Event CRUD operations
- Registration management
- Participant tracking

<div align="center">
  <img src="frontend/public/HabbaHub-readme-images/organizer-eventpage.png" alt="Event Management" width="400" />
  <p><em>Event Management Interface</em></p>
</div>

### Notification Service (Port: 8003)
- Real-time announcements
- Event updates
- System notifications

<div align="center">
  <img src="frontend/public/HabbaHub-readme-images/announcement-page.png" alt="Announcements" width="400" />
  <p><em>Announcements Interface</em></p>
</div>

### Leaderboard Service (Port: 8004)
- Score tracking
- Ranking calculations
- Achievement management

<div align="center">
  <img src="frontend/public/HabbaHub-readme-images/leaderboard-page.png" alt="Leaderboard" width="400" />
  <p><em>Leaderboard Interface</em></p>
</div>

## Real-time Features
The platform uses Socket.IO for real-time updates including:
- Live announcements
- Event status changes
- Leaderboard updates
- Registration notifications

## User Settings & Profile

<div align="center">
  <table>
    <tr>
      <td align="center">
        <img src="frontend/public/HabbaHub-readme-images/userprofile-page.png" alt="User Profile" width="250" /><br>
        <em>User Profile</em>
      </td>
      <td align="center">
        <img src="frontend/public/HabbaHub-readme-images/usersettings-page.png" alt="User Settings" width="250" /><br>
        <em>User Settings</em>
      </td>
    </tr>
  </table>
</div>

## System Administration

<div align="center">
  <table>
    <tr>
      <td align="center">
        <img src="frontend/public/HabbaHub-readme-images/admin-usermanagement.png" alt="User Management" width="250" /><br>
        <em>User Management</em>
      </td>
      <td align="center">
        <img src="frontend/public/HabbaHub-readme-images/sys-settings.png" alt="System Settings" width="250" /><br>
        <em>System Settings</em>
      </td>
    </tr>
  </table>
</div>

## Project Structure
```
HabbaHub/
├── frontend/                 # React frontend
│   ├── src/
│   │   ├── components/      # Reusable components
│   │   ├── pages/          # Page components
│   │   ├── services/       # API services
│   │   └── context/        # React context
│
├── backend/
│   ├── auth-service/       # Authentication
│   ├── event-service/      # Event management
│   ├── notification-service/ # Real-time notifications
│   ├── leaderboard-service/ # Scoring system
│   └── gateway/           # API Gateway
```

## License
This project is licensed under the MIT License - see the LICENSE file for details.
=======
# HabbaHub-Provided-by-Acharya
A web-based platform designed to simplify campus event management by enabling admins, organizers, and participants to collaborate seamlessly. Built with React.js, NestJS, and MongoDB, the system supports secure login, real-time updates using Socket.IO, task tracking, announcements, and report generation.
>>>>>>> 7c71227e48e26592a670762045ba74faf01c3a73
