# LifeFence

LifeFence is a geofencing-driven faculty attendance management system, designed to automate the attendance process using real-time location data. The project utilizes a Python FastAPI backend, a Flutter frontend, and integrates with the Supabase database to provide a seamless and efficient attendance management solution.

## Prerequisites

Ensure you have the following installed on your system:

- Python 3.12+
- Poetry (for dependency management)
- Supabase account & project setup
- Supabase CLI (for managing the database)

## Tech Stack

- **Backend**:
  - [Python](https://www.python.org/)
  - [FastAPI](https://fastapi.tiangolo.com/)
  - [Supabase](https://supabase.io/)
- **Frontend**:

  - [Flutter](https://flutter.dev/)

- **Database**:
  - Supabase (PostgreSQL)

## Project Structure

The project is organized into three main directories:

- **lifefence-backend**:
  The Python FastAPI backend responsible for handling the geofencing logic, user authentication, and API services. It integrates with the Supabase database for data storage and retrieval.

- **lifefence-frontend**:
  The Flutter frontend that provides a cross-platform interface (Android, iOS, Web) for users to interact with the attendance system, view geofencing zones, and track attendance.

- **literature-review**:
  This directory contains research materials, literature surveys, and documentation regarding geofencing technology and its applications in real-world scenarios.

## Project Features

- **Geofencing API**: Determine when a faculty member enters or exits a geofenced zone.
- **Attendance Tracking**: Automate attendance marking based on real-time location data.
- **Authentication**: JWT-based user authentication and authorization.
- **Supabase Integration**: Seamless integration with the Supabase database for storing user data, attendance logs, and geofencing information.
- **Automated Attendance**: Automatically marks attendance based on the user's location within predefined geofencing zones.
- **Real-time Location Tracking**: Tracks the real-time location of users to ensure accurate attendance records.
- **Cross-platform Support**: Provides a seamless user experience across Android, iOS, and web platforms.
- **User Authentication**: Secure authentication mechanism to ensure only authorized users can access the system.
- **Comprehensive Reports**: Generates detailed attendance reports and analytics for faculty and administrators.
- **Scalable Architecture**: Built with scalability in mind to accommodate growing numbers of users and geofencing zones.

## Installation

### Backend Setup

1. **Clone the Repository**

   ```bash
   git clone https://github.com/your-org/lifefence-backend.git
   cd lifefence-backend
   ```

2. **Install Dependencies**
   Using Poetry to install required dependencies:

   ```bash
   poetry install
   ```

3. **Setup Environment Variables**

   Create a `.env` (make a copy of the `.env.example` and add the required parameters) file in the root directory and add the following environment variables:

   ```env
   DATABASE_URL=<your-database-url>
   JWT_SECRET=""<your-jwt-secret>
   ```

4. **Run Database Migrations**
   Use the Supabase CLI or direct SQL scripts to set up your database schema.

   If you're using Supabase CLI:

   ```bash
   supabase db push
   ```

5. **Start the Backend**
   Start the FastAPI development server:

   ```bash
   poetry run uvicorn app.main:app --reload
   ```

   The API will be available at `http://localhost:8000`.

### API Documentation

Once the server is running, you can access the interactive API documentation (Swagger UI) at:

```
http://localhost:8000/docs
```

### Deployment

Pull the pre-built docker image

```bash
docker pull kreativethinker/lifefence-backend:latest
```

Deploy using:

```bash
docker run kreativethinker/lifefence-backend
```

### Running Tests

To run the test suite using `pytest` and `pytest-asyncio`, run:

```bash
poetry run pytest
```

### Supabase Configuration

- **Supabase** is used for data storage. Ensure your Supabase instance has the necessary schema and tables for the application (e.g., users, attendance logs, geofenced areas).
- More details on Supabase configuration and database schema will be found in the `docs/` directory.

## Project Structure

```
lifefence-backend/
├── .github/
│   └── workflows/           # Workflows and github actions
├── app/
│   ├── api/                 # API routes
│   ├── models/              # Pydantic models and Tortoise ORM models
│   ├── utils/               # Business logic (geofencing, attendance tracking)
│   ├── config.py            # Stores server configuration
│   └── main.py              # FastAPI app entry point
├── Dockerfile               # Dockerfile for deployment
├── .env.example             # Example environment variables file
├── poetry.lock              # Poetry lock
├── pyproject.toml           # Poetry configuration
└── README.md                # This file
```

### Literature Review

For research and documentation purposes, refer to the materials available in the `literature-review` folder. This includes:

- Literature surveys on geofencing technology
- Research papers and related articles
- Future prospects and system enhancements

## Contributing

We welcome contributions! Please follow these steps for making contributions:

1. Fork the repository
2. Create a new branch for your feature or bugfix
3. Submit a pull request with a clear description of your changes

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
