# Travlr

# Architecture

In this project, I used multiple types of frontend development approaches. On the customer-facing side, I used Express with HTML templates and JavaScript to render pages dynamically from the server. This approach reloads pages when navigating between views and relies on server-side rendering. For the administrative side, I used a Single-Page Application (SPA) built with Angular. Unlike traditional Express-rendered pages, the SPA loads once and dynamically updates content without refreshing the page. This made the admin interface faster and more interactive. The backend uses MongoDB, a NoSQL database. MongoDB stores data in flexible, document-based JSON-like structures rather than fixed relational tables. This worked well for the project because trip data can evolve over time, and MongoDB allows schema flexibility. It also integrates smoothly with Node.js and Express through Mongoose, making data modeling and queries straightforward.

# Functionality

JSON is a lightweight data format used to structure and transmit data between the frontend and backend. While JSON looks similar to JavaScript objects, it is strictly a data format and does not include functions or executable code. In this project, JSON connects the Angular frontend to the Express backend by sending and receiving trip data through API endpoints. For example, when a trip is requested, the backend sends trip information as JSON, and Angular parses and displays it in the UI. During development, I refactored code by separating concerns into controllers, models, and routes on the backend. On the frontend, I reused Angular components for listing trips and editing trips instead of duplicating code. Reusable UI components improve efficiency, make updates easier, and reduce bugs because changes only need to be made in one place. This also improves scalability if new features are added later.

# Testing

API testing was done using tools like Postman to verify that each endpoint functioned correctly. I tested GET, POST, PUT, and DELETE methods to ensure full CRUD functionality. Each endpoint represents a specific resource path, such as /api/trips or /api/trips/:tripId. Methods define what action is performed on that resource, such as retrieving data or updating it. After implementing authentication for the admin side, testing became more complex because protected routes required valid login credentials and tokens. This added an additional security layer that had to be verified. Understanding endpoints, HTTP methods, and security layers helped me see how frontend and backend systems communicate securely in a full stack application.

# Reflection

This course significantly strengthened my understanding of full stack development. I learned how frontend and backend systems connect through APIs, how databases integrate into applications, and how authentication adds security to web systems. I developed stronger skills in JavaScript, Angular, Express, MongoDB, and RESTful API design. Completing this project made me more confident in building and debugging full stack applications. These skills are directly applicable to roles in software engineering and backend development, and they make me a stronger candidate in the tech field because I now understand both client-side and server-side architecture.
