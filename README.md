#About the project:

This project appears to be an Employee Review Management System designed to facilitate assigning and tracking employee reviews within an organization. The application likely involves two types of users: an admin and employees, each with access to their respective dashboards. The primary functionality revolves around assigning performance reviews from one employee (reviewer) to another (reviewee) and providing feedback on the reviewee’s performance.

Key Features of the Project:
Employee Management:

Fetch and display a list of employees.
Use a service (EmployeeService) to retrieve employee data from a backend API or service.
Employees can select another employee from the list as the reviewee.

Review Assignment:
Employees can assign reviews to their colleagues.
A logged-in employee (reviewer) can choose a colleague (reviewee) and provide feedback.
The review assignment is handled via an AssignReviewService, which sends data (reviewer, reviewee, and feedback) to the backend.

Feedback System:
A feedback field allows the reviewer to write comments about the reviewee.
Validation ensures that both the reviewee and feedback are selected before submission.

Logged-in User Information:
The system tracks the logged-in user (loggedInUserId) and displays their name as the reviewer in the UI.
This is dynamically fetched from the employee data and displayed in the review assignment form.

UI and Design:
The project utilizes Angular Material components for a modern UI experience, including form fields, buttons, select boxes, and toolbars.
Key components like mat-form-field, mat-select, and mat-button are used to create a responsive and user-friendly interface.

Navigation:
Employees and admins can navigate between different parts of the application, such as dashboards and review assignment pages.
There is functionality to return to the employee dashboard after completing tasks.

Modular Design:
The project is organized into components such as ReviewListComponent, AdminDashboardComponent, and EmployeeDashboardComponent.
Each component serves a specific purpose within the system, ensuring modularity and maintainability.

Routing and Navigation:
Angular routing is used to manage page navigation, including links to the employee and admin dashboards.

Backend Integration (via Services):
The system interacts with backend services (AssignReviewService, EmployeeService) to fetch data and assign reviews.
This integration is crucial for persisting review assignments and managing employee data.

Technical Stack:
Angular: Used for the frontend UI and application logic.
Angular Material: Provides pre-built UI components for a polished user experience.
Services: Angular services (AssignReviewService, EmployeeService) handle backend communication for fetching employee data and assigning reviews.
Routing: Angular’s routing module is employed to switch between different components and dashboards.

Possible Use Cases:
Employee Performance Review: Allow employees to give feedback to their peers or subordinates.
Admin Review Monitoring: Admins can track who is reviewing whom and monitor feedback within the organization.
Self-Review for Logged-In User: A logged-in employee can view their own details, assign reviews, and see who is reviewing them.

Typical Workflow:
Login: The employee logs in, and their user ID is stored.
Dashboard Access: The employee can access the review page from their dashboard.
Assign a Review: The employee selects a colleague as the reviewee, provides feedback, and submits the review.
Data Storage: The review and feedback are sent to the backend for storage and analysis.
Review List: Admins or employees with certain permissions may view assigned reviews.

In summary, this project helps to manage employee reviews in a structured and organized way, allowing team members to provide feedback on each other's performance while maintaining a smooth and interactive user experience with Angular Material components.


# EmployeeFeedback

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 18.2.9.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.dev/tools/cli) page.
