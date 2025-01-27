User Management Web Application

Overview

This project is a User Management Web Application built using HTML, CSS, and JavaScript. The application allows users to perform CRUD (Create, Read, Update, Delete) operations on user data. User details are fetched from an external API, and options are provided to edit, delete, or add new users through interactive forms.


Features

1. Fetch and Display Users

    Users are fetched dynamically from the JSONPlaceholder API.
    Each user is displayed as a card, showing the following details:
    ID
    First Name
    Last Name
    Email
    Department (default: Software).

2. Edit User

    Clicking the Edit button saves the user details to localStorage and redirects to an edit form (editForm.html).

3. Delete User

    Clicking the Delete button saves the user details to localStorage and redirects to a delete confirmation page (deleteForm.html).

4. Add User

    The Add User button redirects to an add user form (addUser.html).

5. Error Handling

    If the API fetch fails, the application redirects the user to an error page (error.html).

    File Structure

.
├── index.html              # Main entry point of the application
├── editForm.html           # Page for editing user details
├── deleteForm.html         # Page for deleting user details
├── addUser.html            # Page for adding new users
├── error.html              # Error page
├── README.md               # Project documentation

Technologies Used

    HTML5: Structure and layout of the application.
    CSS3: Styling using a clean and modern design (Google Fonts and custom styles).
    JavaScript: Core functionality for dynamically managing user data.
    JSONPlaceholder API: Simulated user data source.

How to Run

    Clone or download the repository.
    Open the index.html file in your browser.
    Ensure an active internet connection to fetch data from the JSONPlaceholder API.

Key JavaScript Functions

1. createAppendUserCard(userDetails)

    Dynamically creates user cards and appends them to the main container.

2. openEditForm(userDetails)

    Saves user details to localStorage and redirects to the edit form.

3. openDeletePage(userDetails)

    Saves user details to localStorage and redirects to the delete page.

4. API Fetch Logic

    Fetches user data from https://jsonplaceholder.typicode.com/users.

    Transforms the API response to match the application format.

    Handles errors by redirecting to the error page.
