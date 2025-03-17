  
  
# Secure and Intelligent E-commerce Platform with AWS AI/ML Services

## Project Overview

This project is an e-commerce platform built using Flask, integrated with AWS AI/ML services to provide a secure and intelligent shopping experience. The platform includes features such as user registration, product listing, and secure transactions.

## Features

- User authentication and authorization
- Product listing and search
- Secure transactions
- Integration with AWS AI/ML services for enhanced security and intelligence

## Setup Instructions

### Prerequisites

- Python 3.x
- Git

### Steps

1. **Clone the repository:**
    ```sh
    git clone https://github.com/JeevaByte/Secure-and-Intelligent-E-commerce-Platform-with-AWS-AI-ML-Services.git
    cd Secure-and-Intelligent-E-commerce-Platform-with-AWS-AI-ML-Services
    ```

2. **Create a virtual environment:**
    ```sh
    python -m venv env
    ```

3. **Activate the virtual environment:**
    - On Windows:
        ```sh
        env\Scripts\activate
        ```
    - On Unix or MacOS:
        ```sh
        source env/bin/activate
        ```

4. **Install the required packages:**
    ```sh
    pip install -r requirements.txt
	install the below packages if those not available in the requirements file
		Flask==2.0.1
		Flask-WTF==0.15.1
		email-validator==1.1.3
		Flask-SQLAlchemy==2.5.1
		Flask-Bcrypt==0.7.1
		click==8.0.1
		Flask==2.0.1
		Flask-Login==0.5.0
		greenlet==1.1.0
		idna==3.2
		importlib-metadata==4.6.1
		itsdangerous==2.0.1
		Jinja2==3.0.1
		MarkupSafe==2.0.1
		SQLAlchemy==1.4.22
		Werkzeug==2.0.1
		WTForms==2.3.3
		zipp==3.5.0Flask-Login==0.5.0
    ```

5. **Set environment variables:**
    - On Windows:
        ```sh
        set FLASK_APP=market.py
        set FLASK_ENV=development
        ```
    - On Unix or MacOS:
        ```sh
        export FLASK_APP=market.py
        export FLASK_ENV=development
        ```

6. **Create the SQLite database:**
    ```sh
    flask shell
    ```
    Then, in the Flask shell:
    ```python
    from market import db
    db.create_all()
    exit()
    ```

7. **Run the Flask application:**
    ```sh
    flask run
    ```

8. **Access the application:**
    Open your browser and go to [http://127.0.0.1:5000/](http://127.0.0.1:5000/).

## Challenges Encountered

### 1. Virtual Environment Activation

**Issue:** The `source` command was not recognized on Windows.

**Solution:** Used `env\Scripts\activate` instead of `source env/bin/activate`.

### 2. Missing Dependencies

**Issue:** Encountered `ModuleNotFoundError` for `email_validator`.

**Solution:** Installed the missing package using:
```sh
pip install email_validator

### 3. Git Branch Management
Issue: Needed to synchronize the main and master branches.

Solution: Used the following commands to resolve branch discrepancies:

4. Internal Server Error
Issue: Encountered an internal server error during registration.

Solution: Enabled debug mode in Flask to identify and fix the issue by modifying run.py:

5. Force Pushing to Main Branch
Issue: Updates were rejected because the tip of the current branch was behind its remote counterpart.

Solution: Used the following commands to force push the changes:

6. Database Configuration
Issue: Configuring the SQLite database and ensuring it is properly initialized.

Solution: Created the database using Flask's shell and SQLAlchemy:

Then, in the Flask shell:

7. Environment Variable Management
Issue: Setting environment variables correctly for different operating systems.

Solution: Provided specific instructions for setting environment variables on both Windows and Unix/MacOS systems.

8. Dependency Management
Issue: Ensuring all necessary packages are installed and managing dependencies.

Solution: Created a requirements.txt file and used pip install -r requirements.txt to install all required packages.

9. Debugging and Error Handling
Issue: Encountering and resolving various runtime errors and exceptions.

Solution: Enabled debug mode in Flask to get detailed error messages and stack traces, which helped in identifying and fixing issues.

10. Git Repository Management
Issue: Managing the Git repository, including handling branch discrepancies and force pushing changes.

Solution: Used Git commands to synchronize branches, resolve conflicts, and force push changes when necessary.

11. User Authentication and Security
Issue: Implementing secure user authentication and handling sensitive data.

Solution: Used Flask-Login for user authentication and Flask-Bcrypt for password hashing to ensure secure handling of user credentials.

12. Integration with AWS AI/ML Services
Issue: Integrating AWS AI/ML services for enhanced security and intelligence features.

Solution: Followed AWS documentation and used appropriate SDKs and APIs to integrate AI/ML services into the application.

13. Handling Static and Template Files
Issue: Organizing and managing static files (CSS, JS) and template files (HTML) for the Flask application.

Solution: Created appropriate directories (static and templates) and ensured Flask was configured to serve these files correctly.

14. Cross-Origin Resource Sharing (CORS)
Issue: Handling CORS issues when making API requests to external services.

Solution: Used Flask-CORS to enable CORS for the Flask application:

Then, in the application code:

15. Deployment Challenges
Issue: Deploying the Flask application to a production environment.

Solution: Followed best practices for deploying Flask applications, including using a WSGI server like Gunicorn and configuring the application for production settings.

Contributing
If you would like to contribute to this project, please fork the repository and submit a pull request. Contributions are welcome and appreciated.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Contact
For any questions or inquiries, please contact [Your Name] at [your.email@example.com].

Acknowledgements
Flask: https://flask.palletsprojects.com/
AWS AI/ML Services: https://aws.amazon.com/machine-learning/

