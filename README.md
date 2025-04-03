# LifeFence

LifeFence is a geofencing-driven faculty attendance management system, designed to automate the attendance process using real-time location data. The project utilizes a Python FastAPI backend, a Flutter frontend, and integrates with the Supabase database to provide a seamless and efficient attendance management solution.

## Project Structure

The project is organized into three main directories:

- **lifefence-backend**: 
  The Python FastAPI backend responsible for handling the geofencing logic, user authentication, and API services. It integrates with the Supabase database for data storage and retrieval.

- **lifefence-frontend**: 
  The Flutter frontend that provides a cross-platform interface (Android, iOS, Web) for users to interact with the attendance system, view geofencing zones, and track attendance.

- **literature-review**: 
  This directory contains research materials, literature surveys, and documentation regarding geofencing technology and its applications in real-world scenarios.

## Project Features

- **Automated Attendance**: Automatically marks attendance based on the user's location within predefined geofencing zones.
- **Real-time Location Tracking**: Tracks the real-time location of users to ensure accurate attendance records.
- **Cross-platform Support**: Provides a seamless user experience across Android, iOS, and web platforms.
- **User Authentication**: Secure authentication mechanism to ensure only authorized users can access the system.
- **Comprehensive Reports**: Generates detailed attendance reports and analytics for faculty and administrators.
- **Scalable Architecture**: Built with scalability in mind to accommodate growing numbers of users and geofencing zones.

## Tech Stack

- **Backend**: 
  - [Python](https://www.python.org/)
  - [FastAPI](https://fastapi.tiangolo.com/)
  - [Supabase](https://supabase.io/)
  
- **Frontend**: 
  - [Flutter](https://flutter.dev/)

- **Database**: 
  - Supabase (PostgreSQL)

## Installation

### Clone the Repository

1. Clone this repository and initialize the submodules:
    ```bash
    git clone --recurse-submodules https://github.com/KreativeThinker/lifefence.git
    cd lifefence
    ```

2. Update the submodules if necessary:
    ```bash
    git submodule update --remote
    ```

### Backend Setup

Follow the detailed instructions in the [lifefence-backend README](lifefence-backend/README.md) for setting up the FastAPI backend.

### Frontend Setup

Instructions for setting up the Flutter frontend are available in the [lifefence-frontend README](lifefence-frontend/README.md).

### Literature Review

For research and documentation purposes, refer to the materials available in the `literature-review` folder. This includes:
- Literature surveys on geofencing technology
- Research papers and related articles
- Future prospects and system enhancements

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
