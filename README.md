# **Admin Dashboard - Role-Based Access Control (RBAC)**

This project demonstrates a modern **Admin Dashboard** for managing users, roles, and permissions using **Role-Based Access Control (RBAC)**. The application enables administrators to manage user roles, creators to manage posts, and users to explore and interact with content. Built with React, the project emphasizes intuitive design, role-based functionalities, and modern web development practices.

---

## **Table of Contents**
1. [Project Overview](#project-overview)  
2. [Features](#features)  
3. [Technologies Used](#technologies-used)  
4. [Project Structure](#project-structure)  
5. [State Management](#state-management)  
6. [Routing and Permissions](#routing-and-permissions)  
7. [How to Run the Project](#how-to-run-the-project)  

---

## **Project Overview**

The Admin Dashboard enables:
- **Admin Features**: Manage users, toggle roles, and assign permissions.
- **Creator Features**: Create and manage posts.
- **User Features**: View posts and interact with creators by following/unfollowing them.

The application implements RBAC principles for secure and efficient role-based navigation and functionality.

---

## **Features**

### **Admin Features**
- **Role Management**: Assign or toggle roles for users.
- **User Management**: Add, edit, or delete users.

### **Creator Features**
- **Post Creation**: Create and edit posts with a rich text editor.
- **Post History**: View a list of previously created posts.

### **User Features**
- **Post Viewing**: Browse posts created by creators.
- **Follow Creators**: Follow or unfollow creators.

### **Shared Features**
- **Protected Routes**: Restrict access based on user roles.
- **Optimized UI**: Includes responsive design, shimmer loading effects, and debounced inputs.

---

## **Technologies Used**
- **React**: Frontend library for building the user interface.
- **React Context API**: Global state management.
- **React Router**: Navigation and protected routes.
- **Tailwind CSS**: Modern, responsive design.
- **TinyMCE**: Rich text editor for post creation.
- **Debounce**: Efficient input handling.
- **Shimmer Effect**: Adds skeleton loading effects.

---

## **Project Structure**

```bash
src/
├── components/         # Reusable components
│   ├── forms/          # Login and add-user forms
│   ├── CreatorNav/     # Navbar for creators
│   ├── Shimmer/        # Loading animation
│   ├── UserNav/        # Navbar for users
├── context/            # Context API for global state
│   ├── AuthContext/    # Manages authentication
│   ├── BlogContext/    # Handles blog data
├── pages/              # Individual pages
│   ├── Dashboard/      # Admin dashboard
│   ├── Following/      # User follow/unfollow page
│   ├── PastBlogs/      # Creator's post history
│   ├── Unauthorized/   # Unauthorized access page
│   ├── UserDashboard/  # User's main dashboard
│   ├── Write/          # Creator's post creation page
├── utils/              # Helper functions
│   ├── reducer.js      # Reducer logic for state updates
├── App.jsx             # Main application component
├── protectedRoute.jsx  # Logic for protected routes
