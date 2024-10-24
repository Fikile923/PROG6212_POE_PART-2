# PROG6212_POE_PART-2
Contract Monthly Claim System (CMCS)
Overview
This web application is designed for a fictional institution, EduTech University, allowing lecturers to submit monthly claims for their work. The system also allows program coordinators and academic managers to verify and approve or reject these claims. The application is developed using ASP.NET Core MVC, with a focus on user-friendly design and functionality.

Features
Lecturer Claim Submission:

Lecturers can submit claims including hours worked, hourly rate, and any additional notes.
Ability to upload supporting documents (PDF, DOCX, XLSX).
Real-time status tracking of claims (Pending, Approved, Rejected).
Program Coordinator and Academic Manager Verification:

Separate views for coordinators and managers to review and approve/reject claims.
Claims are displayed with all necessary details for decision-making.
File Upload:

Lecturers can upload relevant documents during claim submission.
Supported file types: PDF, DOCX, XLSX.
File size limits are implemented.
Claim Status Tracking:

Claim status is updated as it moves through the approval process.
Edit/Delete Claims:

Lecturers can edit or delete claims before they are reviewed by coordinators or managers.
Error Handling and Validation:

The system provides meaningful error messages and gracefully handles exceptions.
Unit Testing:

Key functionalities are covered with unit tests to ensure reliability.
Technologies Used
ASP.NET Core MVC
Entity Framework Core
SQL Server (for database)
HTML/CSS/JavaScript (for front-end)
Bootstrap (for responsive design)
Git/GitHub (for version control)
Prerequisites
Before running the project, ensure that you have the following installed:

.NET 6.0 SDK
SQL Server
Visual Studio 2022 (or any other code editor)
Git (for version control)

Getting Started
Follow these steps to set up the project locally:

1. Clone the repository
bash
Copy code
git clone https://github.com/yourusername/your-repository-name.git
cd your-repository-name
2. Set up the database
Update the connection string in the appsettings.json file with your SQL Server details.
json
Copy code
"ConnectionStrings": {
    "DefaultConnection": "Server=YOUR_SERVER_NAME;Database=CMCS;Trusted_Connection=True;MultipleActiveResultSets=true"
}
Run the following commands to apply migrations and set up the database:
bash
Copy code
dotnet ef database update
3. Run the application
To run the application locally:

bash
Copy code
dotnet run
Alternatively, open the project in Visual Studio and click Run.

4. Access the application
Open your web browser and go to:

arduino
Copy code
https://localhost:5001
Running Unit Tests
To run the unit tests for the application:

bash
Copy code
dotnet test
Commit History
Regular commits have been made to document the development process and implement features progressively. For more information, view the commit history.
Future Enhancements
User Authentication: Implement user authentication to restrict access to the platform based on roles (Lecturer, Coordinator, Manager).
Email Notifications: Send email notifications to lecturers and managers when the claim status is updated.
Contributing
If you'd like to contribute to the project, please fork the repository and submit a pull request.

License
This project is licensed under the MIT License.


