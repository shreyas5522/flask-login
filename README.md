# Flask Login System

This project is a Flask web application with user authentication features. It allows users to register, log in, and log out securely. The application uses Flask-Login, Flask-SQLAlchemy, and Flask-WTF for session management, database interactions, and form handling, respectively.

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/shreyas5522/flask-login.git
    ```

2. Navigate to the project directory:

    ```bash
    cd flask-login
    ```

3. Create a virtual environment (optional but recommended):

    ```bash
    python -m venv venv
    ```

4. Activate the virtual environment:

    - On Windows:

        ```bash
        venv\Scripts\activate
        ```

    - On macOS/Linux:

        ```bash
        source venv/bin/activate
        ```

5. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

## Database Setup

1. Create a MySQL database:

    ```bash
    mysql -u your_username -p
    ```

2. Create the database:

    ```sql
    CREATE DATABASE IF NOT EXISTS login;
    USE login;
    ```

3. Create the users table:

    ```sql
    CREATE TABLE IF NOT EXISTS users (
        id INT AUTO_INCREMENT PRIMARY KEY,
        username VARCHAR(20) UNIQUE NOT NULL,
        password VARCHAR(60) NOT NULL
    );
    ```

4. Exit the MySQL shell:

    ```sql
    exit
    ```

## Running the Application

1. Make sure your virtual environment is activated.

2. Run the Flask application:

    ```bash
    python app.py
    ```

3. Open your web browser and navigate to `http://127.0.0.1:5000/`.

4. You can register, log in, and enjoy the features of the Flask Login System.

## Notes

- Make sure you have MySQL installed and running before creating the database.
- Adjust the database connection URI in `app.py` if necessary.
- Customize the project according to your needs.
