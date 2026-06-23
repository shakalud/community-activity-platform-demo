# Architecture

## Overview

The platform was designed as a self-hosted FastAPI web application running behind Nginx on a Linux VPS.

The system used separate production and laboratory environments to safely test changes before deployment.

## Main Components

- FastAPI backend
- SQLite database
- Jinja2 templates
- Discord OAuth authentication
- Role-based access control
- Audit logging
- Image upload workflow
- Nginx reverse proxy
- systemd service management
- Backup automation

## Environment Model

- Production environment for real users
- Laboratory environment for testing new features
- Separate configuration files
- Separate services
- Separate domains
- Backup and restore workflow

## Security Model

Access was controlled through Discord OAuth and internal role mapping.

Roles included:

- Owner
- Admin
- Member

Each role had different permissions for viewing, editing and administrative actions.
