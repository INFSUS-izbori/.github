### WebApp

-   **Description:** This web application provides a platform for managing political candidates and parties for an election. Users can view, create, edit, and delete candidates and parties. The application features a responsive user interface built with React and Tailwind CSS, and it communicates with a backend API to handle data persistence.
-   **Features:**
    -   User-friendly interface for managing candidates and parties.
    -   Real-time data updates and synchronization.
    -   Secure authentication and authorization.
    -   Responsive design for seamless use on various devices.

### WebAPI

-   **Description:** This project is a Web API for managing political parties and their candidates. It allows for CRUD (Create, Read, Update, Delete) operations on both parties and candidates, built with ASP.NET Core for high performance and scalability.
-   **Features:**
    -   Comprehensive CRUD operations for political parties and candidates.
    -   Secure endpoints with token-based authentication.
    -   Detailed logging and error handling.

## Technologies Used

Our projects leverage a modern technology stack:

-   **Frontend (WebApp):** React, Tailwind CSS, JavaScript/TypeScript
-   **Backend (WebAPI):** ASP.NET Core, C#, Entity Framework Core
-   **Database:** PostgreSQL (or your preferred database)
-   **DevOps:** Docker, GitHub Actions

## Using WebApp and WebAPI Together

To use the `webapp` and `webapi` together, follow these general steps:

1.  **Set up the WebAPI:**

    -   Clone the `webapi` repository.
    -   Follow the setup instructions in its README to get the API running locally or deploy it to a server.
    -   Ensure the API endpoints are accessible.

2.  **Configure the WebApp:**

    -   Clone the `webapp` repository.
    -   In the `webapp`'s configuration files, update the API endpoint URLs to point to your running `webapi` instance.
    -   Follow the setup instructions in its README to build and run the `webapp`.

3.  **Usage:**
    -   Once both applications are running and the `webapp` is configured to communicate with the `webapi`, you can start using the `webapp`.
    -   The `webapp` will make requests to the `webapi` to fetch and manipulate data, providing a user-friendly interface for the functionalities offered by the API.
    -   **Example Workflow:** A user logs into the WebApp. To display a list of political parties, the WebApp sends a GET request to the `/api/parties` endpoint of the WebAPI. The WebAPI retrieves the data from the database and returns it to the WebApp, which then renders the list to the user.
