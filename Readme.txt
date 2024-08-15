User Authentication System

Overview

This is a simple user authentication system built with PHP and MySQL. It allows users to register, log in, and log out of the system. The project demonstrates basic functionalities of user management, including secure password handling and session management.

Features

Registration: Allows new users to create an account with a username and password. Passwords are hashed for security.
Login: Users can log in with their credentials. Passwords are verified using hashing.
Logout: Users can log out, which destroys their session and returns them to the login page.
Session Management: Tracks logged-in users and displays a personalized welcome message.

Installation

1. Clone the Repository

   bash
   git clone https://github.com/yourusername/your-repository-name.git
   

2. Navigate to the Project Directory

   bash
   cd your-repository-name
   

3. Set Up the Database

   Import the provided SQL schema into your MySQL database. You can use a tool like phpMyAdmin or run the SQL commands manually.
   Ensure that the `user_system` database exists and has a `users` table with `username` and `password` fields.

4. Configure Database Connection

   Open `index.php` and update the database connection parameters to match your MySQL server setup:
   
     php
     $servername = "localhost";
     $username = "root";
     $password = "";
     $dbname = "user_system";
     

5. Deploy the Application

    Place the project files on your web server.
    Ensure PHP and MySQL are properly configured on the server.

Usage

1. Access the Application

   Open your web browser and navigate to the location where you deployed the application.

2. Register a New User

    Enter a desired username and password in the registration form and submit.
    If registration is successful, a confirmation message will be displayed.

3. Log In

    Use the registered username and password to log in.
    On successful login, you'll be redirected to a welcome page with a logout option.

4. Log Out

    Click the "Logout" link to end the session and return to the login page.

Security Considerations

 Password Hashing: Passwords are hashed using PHP's `password_hash()` and verified with `password_verify()`, ensuring secure password storage.
 Session Management: Sessions are used to manage user login states and are properly destroyed on logout.

Contributing

Feel free to fork the repository, make improvements, and submit pull requests. Contributions are welcome.

