# System Design

## System Architecture Diagram
[https://github.com/Teersingh/TaskManagerPlan/blob/main/System%20Design.pdf]

## Database Schema
[https://github.com/Teersingh/TaskManagerPlan/blob/main/Database%20Schema.docx]

### Tables
1. Users
2. Projects
3. Tasks
4. Comments/Notifications
5. Plugin




## API Structure
Endpoints:
Authentication:
POST /auth/register
POST /auth/login
POST /auth/logout
Users:
GET /users/
GET /users/{user_id}
Projects:
GET /projects/
POST /projects/
GET /projects/{project_id}
PUT /projects/{project_id}
DELETE /projects/{project_id}
Tasks:
GET /tasks/
POST /tasks/
GET /tasks/{task_id}
PUT /tasks/{task_id}
DELETE /tasks/{task_id}
Comments:
POST /tasks/{task_id}/comments/
GET /tasks/{task_id}/comments/
Notifications:
GET /notifications/
Plugins:
POST /plugins/
GET /plugins/
PUT /plugins/{plugin_id}
DELETE /plugins/{plugin_id}


## Real-time Communication Mechanism
We will use WebSockets for real-time updates. 
WebSockets used to push real-time updates to clients when tasks are created, updated, or deleted. WebSocket connections will be managed using Django Channels WebSocket capabilities.

