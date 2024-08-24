- Authentication
     1.POST /auth/register: Registers a new user. Requires user details such as username, email, and password.
     2.POST /auth/login: Authenticates a user and provides an access token for subsequent requests. Requires user credentials (e.g., email and password).
     3.POST /auth/logout: Logs out a user and invalidates their access token.
  
-Users
    1.GET /users/: Retrieves a list of all users.
    2.GET /users/{user_id}: Retrieves detailed information about a specific user by their user ID.
  
-Projects
    1.GET /projects/: Retrieves a list of all projects.
    2.POST /projects/: Creates a new project. Requires project details (e.g., name, description).
    3.GET /projects/{project_id}: Retrieves detailed information about a specific project by its project ID.
    4.PUT /projects/{project_id}: Updates the details of a specific project. Requires project details (e.g., name, description).
    5.DELETE /projects/{project_id}: Deletes a specific project by its project ID.
    
-Tasks
    1.GET /tasks/: Retrieves a list of all tasks.
    2.POST /tasks/: Creates a new task. Requires task details (e.g., title, description, due date).
    3.GET /tasks/{task_id}: Retrieves detailed information about a specific task by its task ID.
    4.PUT /tasks/{task_id}: Updates the details of a specific task. Requires task details (e.g., title, description, status).
    5.DELETE /tasks/{task_id}: Deletes a specific task by its task ID.
    
-Comments
    1.POST /tasks/{task_id}/comments/: Adds a comment to a specific task. Requires comment content.
    2.GET /tasks/{task_id}/comments/: Retrieves a list of comments for a specific task.

- Plugins
    1.POST /plugins/: Creates a new plugin. Requires plugin details (e.g., name, configuration).
    2.GET /plugins/: Retrieves a list of all plugins.
    3.PUT /plugins/{plugin_id}: Updates the details of a specific plugin by its plugin ID. Requires plugin details.
    4.DELETE /plugins/{plugin_id}: Deletes a specific plugin by its plugin ID.
