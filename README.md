Doctorly Calendar API
This project is a backend API for managing scheduling within a doctor's practice. It provides endpoints for creating, updating, and deleting events, managing attendees, and searching for events.

Prerequisites
Before running this project, ensure you have the following installed:

.NET 6 SDK
Visual Studio 2022 or Visual Studio Code
SQL Server
Installation
Clone this repository to your local machine.
bash
Copy code
git clone https://github.com/BrianlerouxUtlra/doctorly.git
Open the solution (DoctorlyCalendar.sln) in Visual Studio.

Build the solution to restore NuGet packages and build the project.

Database Setup
Open SQL Server Management Studio (SSMS).

Create a new database named DoctorlyCalendarDB.

Run the SQL script DatabaseScript.sql located in the Database folder to create the necessary tables and seed initial data.

Configuration
Update the connection string in appsettings.json located in the Doctorly.API_ project to point to your SQL Server instance.
json
Copy code
"ConnectionStrings": {
  "DefaultConnection": "Server=Doctorly;Database=DoctorlyCalendarDB;Trusted_Connection=True;"
}
Running the Project
Set the Doctorly.API_ project as the startup project.

Press F5 or click the "Start" button in Visual Studio to run the project.

The API will start and be accessible at http://localhost:xxxx(availalbe port).

API Documentation
After running the project, navigate to http://localhost:{yourPort}/swagger in your web browser to view the Swagger documentation.
Usage
Use a REST client like Postman or Swagger UI to interact with the API endpoints.

Refer to the Swagger documentation for detailed information on available endpoints and their usage.
