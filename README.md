# Fullstack User Authentication and Dashboard Backend Template

## Overview

This is the **Django backend** for a full-stack template that includes user creation, user login, and OAuth login with GitHub. It serves as a starting point for full-stack projects requiring user authentication and is ready to be scaled. This backend is designed to work seamlessly with a **React** frontend.

The frontend for this template, built with React, can be found [here](https://github.com/Nivix047/oauth-django-frontend).

## Features

- **User Registration**: Allows users to create new accounts with secure password handling.
- **User Login**: Authenticates users with password credentials and returns a token.
- **OAuth Login**: Provides GitHub OAuth login integration.
- **Token-Based Authentication**: Utilizes Django REST Framework's token authentication for secure API access.
- **CORS Configuration**: Handles CORS requests to allow communication with frontend applications.

## Tech Stack

### Backend:

- **Django**: Python web framework for handling user authentication, session management, and APIs.
- **Django REST Framework**: For building RESTful APIs and managing token-based authentication.
- **Django Social Auth**: For handling OAuth logins, specifically GitHub OAuth.
- **PostgreSQL**: As the database backend (can be changed as needed).
- **Python-Decouple**: For managing environment variables.

### Frontend:

- The frontend (not included in this repo) is built with **React** and **Material-UI (MUI)**. You can find the frontend repository [here](https://github.com/your-frontend-repo).

## Getting Started

- Make sure to set up your `.env` file with the required environment variables such as `SECRET_KEY`, `DATABASE` credentials, and OAuth credentials.
- Install the necessary dependencies.

## Deployment

To deploy both the frontend and backend on the same EC2 instance using Docker:

- Containerize the Backend: Create a Dockerfile for the Django backend and build the image.
- Deploy on EC2: After containerizing, deploy the backend on an EC2 instance, ensuring it's configured to connect with your frontend.
