# Multi-Tier DevSecOps Project

## _A simple multi-tier application demonstrating a Node.js API backend and a React frontend client used for a basic user management demo_

This project is designed to illustrate a typical DevSecOps-ready application structure with separate services for the frontend and backend.

## Table of Contents

Introduction
Architecture
Features
Project Structure
Prerequisites
Installation
Running the Application
Usage
Dependencies
Configuration
Examples
Troubleshooting
Contributors
License

## This repository contains a full-stack demo application composed of:

A Node.js REST API
A React frontend client
The application demonstrates how frontend and backend services interact in a multi-tier architecture.
It can be used for:
DevSecOps pipeline demonstrations
Containerization practice
CI/CD testing
Security scanning practice
Infrastructure automation demos

## Architecture

Browser
   │
   ▼
React Client (client/)
   │
   ▼
Node.js API (api/)
   │
   ▼
User Management Logic

The frontend communicates with the backend API to perform user-related operations.

## Features
Simple user management demo
Node.js API backend
React frontend
Easy local setup
Suitable for DevSecOps pipeline experiments
Modular multi-tier architecture
## Project Structure
multi-tier-devsecops-project
│
├── api/                # Node.js backend
│   ├── package.json
│   └── server files
│
├── client/             # React frontend
│   ├── package.json
│   └── React components
│
└── README.md
## Prerequisites
Before running the project, ensure you have the following installed:
Node.js (v18 or later)
npm (comes with Node.js)
Git (optional but recommended)
You can verify installations:
node -v
npm -v
## Installation

Clone the repository:
git clone <repository-url>
cd multi-tier-devsecops-project
Install dependencies for both the API and client.
Install API dependencies
cd api
npm install
Install Client dependencies
cd ../client
npm install
## Running the Application
1. Start the API Server
```
cd api
npm start
```
The backend API will start and listen for requests.

2. Start the React Client

Open a separate terminal and run:
```
cd client
npm start
```
3. Access the Application

Open your browser and navigate to:

http://localhost:3000
Usage

Once the application is running:

Open the web interface.

Interact with the user management UI.

The React client will send requests to the Node.js API.

This demonstrates frontend ↔ backend interaction in a multi-tier application.

Dependencies
Backend (API)

Typical dependencies may include:

Express

CORS

Body-parser

Frontend (Client)

Typical dependencies may include:

React

React DOM

React Scripts

(See package.json in each directory for the exact dependency list.)

Configuration

Configuration may include:

API port settings

Environment variables

Backend API URLs used by the React client

Example .env file:

PORT=5000
Examples

Example API request:

GET /users

Example response:

[
  {
    "id": 1,
    "name": "John Doe"
  }
]
Troubleshooting
Node version errors

Ensure you are using Node 18 or later:

node -v
Port already in use

If port 3000 or the API port is busy:

Stop other running servers

Change the port in configuration

Dependencies not installing

Clear npm cache and reinstall:
```
npm cache clean --force
npm install
```
Contributors
Project contributors:
Your Name: Jahangir Kabir
