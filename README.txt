Django Authentication App
This is a Django web application that provides user authentication and authorization functionality.
 It includes views and templates for user registration, login, logout, password change, and password reset.

Installation
-Clone this repository to your local machine.
-Navigate to the project directory and create a virtual environment for the application:
    python3 -m venv env
-Activate the virtual environment:
    source env/bin/activate
-Install the required packages:
    pip install -r requirements.txt
-Create the database tables:
    python manage.py migrate
-Set up the SMTP email server in the settings.py file.
 In the EMAIL_BACKEND setting, set the value to 'django.core.mail.backends.smtp.EmailBackend'.
 Then set the EMAIL_HOST, EMAIL_PORT, EMAIL_USE_TLS, EMAIL_HOST_USER, and
 EMAIL_HOST_PASSWORD settings to the values for your SMTP email server.
 OR you can use any other third party mail servers.
-Start the development server:
    python manage.py runserver

Usage:
-User Registration
    To register a new user, navigate to the registration page at http://localhost:8000/accounts/register/.
    Fill out the registration form with a valid email address and password.
    Upon successful registration, you will be redirected to the login page.

-User Login
    To log in, navigate to the login page at http://localhost:8000/accounts/login/.
    Enter your email address and password and click the "Login" button.
    If your credentials are valid, you will be redirected to the dashboard.

-User Logout
    To log out, click the "Logout" link in the top navigation bar.
    You will be redirected to the login page.

-Password Change
    To change your password, click the "Change Password" link in the top navigation bar.
    Enter your current password and your new password in the form and click the "Change Password" button.
    If your current password is valid and your new password meets the password requirements,
     your password will be changed and you will be redirected to the login page.

-Password Reset
    If you forget your password, you can request a password reset by clicking the "Forgot Password?" link on the login page.
    Enter your email address in the form and click the "Reset Password" button.
    If the email address is associated with a valid user account,
    an email will be sent to that address with instructions for resetting your password.
    Follow the instructions in the email to reset your password.

-Credits
    This Django Authentication App was created by H.LAKSHMAN.
     If you have any questions or feedback, please contact me at lakshman.vaibhav007@gmail.com.