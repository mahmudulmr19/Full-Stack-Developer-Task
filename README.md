### Full-Stack Developer Task: Advanced Todo Application using Express, TypeScript, tRPC, and Next.js

#### Objective:

Create an advanced full-stack Todo application with a backend that allows users to create, read, update, and delete todos, and a frontend to interact with this backend. The backend should be built using Express, TypeScript, and tRPC, while the frontend should use Next.js and TypeScript.

#### Requirements:

### Backend

1. **Setup:**

   - Initialize a new Node.js project.
   - Configure TypeScript.
   - Set up Express and tRPC.

2. **Endpoints:**

   - `POST /todos`: Create a new todo.
   - `GET /todos`: Get a list of all todos with optional filtering by completion status.
   - `GET /todos/:id`: Get a specific todo by its ID.
   - `PUT /todos/:id`: Update a specific todo by its ID.
   - `DELETE /todos/:id`: Delete a specific todo by its ID.

3. **Todo Model:**

   - Each todo should have the following fields:
     - `id`: string (UUID)
     - `title`: string
     - `description`: string
     - `completed`: boolean
     - `createdAt`: Date
     - `updatedAt`: Date

4. **Implementation Details:**

   - Use tRPC to define and implement the endpoints.
   - Use an in-memory data store (a simple array) to manage todos.
   - Implement middleware to log each request with its method and URL.
   - Add input validation for all endpoints using Zod (or similar validation library).
   - Implement pagination for the `GET /todos` endpoint.
   - Implement filtering for the `GET /todos` endpoint to allow users to filter todos by their completion status (`completed` or `not completed`).

5. **Additional Features:**

   - Implement a mechanism to simulate database errors and ensure proper error handling and responses.
   - Ensure concurrency control for update operations (optimistic locking).

### Frontend

1. **Setup:**

   - Initialize a new Next.js project.

2. **Functionality:**

   - Fetch todos from the backend with filtering and pagination.
   - Create, read, update, and delete todos using the backend API.
   - Handle loading and error states appropriately.

3. **UI/UX:**

   - Use a modern CSS framework (e.g., Tailwind CSS) for styling.
   - Ensure the application is responsive and accessible.

#### Deliverables:

- A GitHub repository with the complete project, including both frontend and backend.
- Clear instructions on how to run the project locally.
- A brief document explaining the approach and any assumptions made.
