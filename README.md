# WorkLoop — Real-Time Team Collaboration Platform

<div align="center">

![WorkLoop Banner](https://img.shields.io/badge/WorkLoop-Realtime%20Collaboration%20Platform-blueviolet?style=for-the-badge)

A modern **Slack-inspired realtime collaboration and messaging platform** built using the **MERN Stack**, **Socket.IO**, and **Cloudinary**.

Designed for teams to communicate through workspaces, channels, direct messages, thread replies, notifications, file sharing, and smart reminder-based messaging.

</div>

---

# Live Demo

## Frontend

```txt[
https://workloop-realtime-chat.vercel.app/
```

## Backend

```txt
https://workloop-realtime-chat.onrender.com
```

---

# Project Introduction

WorkLoop is a full-stack realtime collaboration platform inspired by applications like Slack and Microsoft Teams.

The application allows users to:

* Create workspaces
* Create channels
* Chat in realtime
* Send direct messages
* Share files
* Reply in threads
* React to messages
* Receive notifications
* Track online users
* Set priority-based reminder messages

The goal of this project is to simulate how modern team communication platforms work while keeping the architecture beginner-friendly, scalable, and clean.

---

# Main Features

## Authentication System

* User Registration
* User Login
* JWT Authentication
* Protected Routes
* Persistent Login
* Logout Functionality

---

## Workspace Management

* Create workspaces
* Add workspace members
* Workspace-based communication
* Member role handling

---

## Channel System

* Public channels
* Private channels
* Channel-based realtime messaging
* Channel member management

---

## Real-Time Messaging

* Instant message delivery
* Channel messaging
* Direct messaging
* Auto-scroll latest messages
* Live message synchronization using Socket.IO

---

## Thread Reply System

* Reply to specific messages
* Dedicated thread panel
* Realtime thread updates
* Organized conversation structure

---

## Direct Messaging

* One-to-one private conversations
* Realtime direct messaging
* Direct message notifications

---

## File Sharing

* Upload files
* Share images/documents/PDFs
* Cloudinary file storage
* Realtime file message updates

---

## Reactions System

* Emoji reactions
* Add/remove reactions
* Realtime reaction synchronization

---

## Notifications System

* Message notifications
* Direct message notifications
* Thread reply notifications
* Reminder notifications
* Read/unread notification handling

---

# Unique Feature — Smart Priority + Reminder Messaging

One of the unique features of WorkLoop is the **Priority + Reminder Messaging System**.

Users can send messages with:

* LOW priority
* MEDIUM priority
* HIGH priority

Users can also schedule reminder times for important messages.

Example:

```txt
Complete frontend testing before tomorrow.
Priority: HIGH
Reminder Time: 10:00 PM
```

When reminder time arrives:

* Notification is generated
* Reminder appears in reminders section
* User receives reminder alert

This makes WorkLoop more practical for team productivity and task-oriented communication.

---

# Tech Stack

## Frontend

* React
* React Router DOM
* Redux Toolkit
* Axios
* Socket.IO Client
* Vite
* Common reusable styling system (`common.js`)

---

## Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* Socket.IO
* JWT Authentication
* bcryptjs
* Multer
* Cloudinary
* Redis
* Cookie Parser
* dotenv

---

# Real-Time Features

WorkLoop uses **Socket.IO** for realtime communication.

Implemented realtime features include:

* Channel messaging
* Direct messaging
* Thread replies
* Reactions
* Online/offline user tracking
* Notifications
* Live UI updates

Socket rooms used:

```txt
channel-channelId
dm-user1-user2
user-userId
workspace-workspaceId
```

This allows messages and notifications to update instantly without refreshing the page.

---

# Project Architecture

The project follows a clean full-stack architecture.

## Frontend

Frontend handles:

* UI rendering
* Global state management
* Socket listeners
* API communication
* Routing
* Responsive layouts

Main reusable components:

* MessageInput
* MessageList
* MessageItem
* ThreadPanel
* NotificationPanel
* Sidebar

---

## Backend

Backend handles:

* Authentication
* API validation
* Database operations
* Socket events
* Notifications
* File uploads
* Reminder scheduling

Main backend modules:

* Authentication APIs
* Workspace APIs
* Channel APIs
* Message APIs
* Notification APIs
* Socket events

---

# Project Folder Structure

```txt
WorkLoop/
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── store/
│   │   ├── sockets/
│   │   ├── styles/
│   │   ├── routes/
│   │   ├── utils/
│   │   ├── App.jsx
│   │   └── main.jsx
│
├── backend/
│   ├── APIs/
│   ├── models/
│   ├── sockets/
│   ├── config/
│   ├── middlewares/
│   ├── server.js
│   └── README.md
│
└── README.md
```

---

# Frontend Highlights

* Responsive chat UI
* Sticky message input
* Realtime updates
* Thread sidebar
* Notification badges
* Modern workspace layout
* Reusable styling architecture

Detailed frontend documentation:


---

# Backend Highlights

* JWT authentication
* MongoDB schema design
* Socket.IO realtime architecture
* Cloudinary file handling
* Reminder scheduling system
* Notification system
* Role-based validation

Detailed backend documentation:


---

# Database Models

Main MongoDB models:

* UserModel
* WorkspaceModel
* ChannelModel
* MessageModel
* NotificationModel

The database stores:

* Users
* Workspaces
* Channels
* Messages
* File URLs
* Reactions
* Notifications
* Reminder data

---

# Screenshots

## Login Page

*Add screenshot here*

---

## Workspace Dashboard

*Add screenshot here*

---

## Realtime Channel Chat

*Add screenshot here*

---

## Thread Reply Panel

*Add screenshot here*

---

## Notifications Panel

*Add screenshot here*

---

# Installation Guide

## Clone Repository

```bash
git clone https://github.com/WorkLoop-Developers/workloop-realtime-chat.git
```

---

# Frontend Setup

## Navigate to frontend

```bash
cd frontend
```

## Install dependencies

```bash
npm install
```

## Run frontend

```bash
npm run dev
```

Frontend runs on:

```txt
http://localhost:5173
```

---

# Backend Setup

## Navigate to backend

```bash
cd backend
```

## Install dependencies

```bash
npm install
```

## Run backend

```bash
npm run dev
```

Backend runs on:

```txt
http://localhost:5000
```

---

# Environment Variables

## Frontend `.env`

```env
VITE_API_URL=http://localhost:5000
```

---

## Backend `.env`

```env
PORT=5000

DB_URL=your_mongodb_connection_string

SECRET_KEY=your_secret_key

CLIENT_URL=http://localhost:5173

CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

REDIS_URL=redis://localhost:6379
```

---

# Deployment

## Frontend Deployment

* Vercel

## Backend Deployment

* Render

## Database

* MongoDB Atlas

## File Storage

* Cloudinary

---

# Common Features Implemented

* Authentication
* Protected Routes
* Realtime Communication
* Online/Offline Presence
* File Uploads
* Notifications
* Reactions
* Thread Replies
* Message Editing
* Soft Delete Messages
* Reminder Messaging
* Responsive UI

---

# Future Improvements

Possible future enhancements:

* Typing indicators
* Voice messages
* Video calls
* Dark mode
* Message bookmarking
* Advanced search
* Rich text editor
* Push notifications
* Pinned messages
* AI-based message suggestions

---

# Team Members

Add your team member names here:

```txt
1. Your Name
2. Team Member Name
3. Team Member Name
4. Team Member Name
```

---

# Mentor Viva / Project Explanation

### What is WorkLoop?

WorkLoop is a realtime collaboration platform where users can communicate through workspaces, channels, direct messages, thread replies, and notifications.

---

### What is the unique feature?

The Smart Priority + Reminder Messaging System.

---

### Why did we use Socket.IO?

Socket.IO allows messages and updates to appear instantly without refreshing the page.

---

### Why did we use Cloudinary?

Cloudinary stores uploaded files while MongoDB stores only file metadata and URLs.

---

### Why did we use Redux Toolkit?

Redux Toolkit manages global application state efficiently across the application.

---

# Final Summary

WorkLoop is a modern realtime collaboration platform built using the MERN Stack and Socket.IO.

The project combines:

* Realtime communication
* File sharing
* Notifications
* Thread conversations
* Direct messaging
* Smart reminder-based messaging
* Responsive UI architecture

This project helped us understand:

* Full-stack architecture
* Realtime systems
* Socket.IO communication
* Authentication
* Database design
* API handling
* State management
* Modern frontend development

The application is designed to be beginner-friendly while still implementing important real-world collaboration features used in professional messaging platforms.

---

<div align="center">

### WorkLoop — Connect • Collaborate • Communicate

</div>
