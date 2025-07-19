
Built by https://www.blackbox.ai

---

# Barakah Registration System

## Project Overview
The Barakah Registration System is a web application built using Flask that allows users to register for educational programs by entering their personal information and uploading relevant documents. The system stores user data in an Excel spreadsheet and provides functionalities for administrators to manage registrations through a dashboard.

## Installation
To set up the Barakah Registration System, follow these steps:

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd barakah-registration-system
   ```

2. Create a virtual environment and activate it:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Ensure that you have the following Python packages installed (they may also be listed in `requirements.txt`):
   - Flask
   - openpyxl
   - Werkzeug
   - reportlab

5. Run the application:
   ```bash
   python app.py
   ```

The application will start on `http://localhost:8000`.

## Usage
1. Navigate to the main page of the application at `http://localhost:8000`.
2. Fill in the registration form with the required information.
3. Upload the necessary documents (photo, family card, diploma, and birth certificate).
4. Upon submission, you will receive a success message, and your data will be saved in the linked Excel file.
5. Admins can login using the credentials and manage registrations and downloadable files from the dashboard.

## Features
- User registration with document uploads.
- Admin dashboard for managing registrations.
- Data storage in an Excel spreadsheet.
- Generate PDFs for student registration forms and records.
- User-friendly interface with success/error notifications.

## Dependencies
The application requires the following Python libraries, which can be found in the `requirements.txt` file or installed via pip:
- Flask
- openpyxl
- Werkzeug
- reportlab

Make sure to check the versions of these libraries for compatibility.

## Project Structure
The project is organized as follows:
```
barakah-registration-system/
├── app.py                     # Main application file
├── requirements.txt           # List of dependencies
├── uploads/                   # Directory for uploaded files
├── static/                    # Static files (e.g., images)
│   └── images/                # Subdirectory for image uploads
└── templates/                 # HTML templates for rendering views
    ├── index.html             # Registration form
    ├── success.html           # Success page after registration
    ├── admin_login.html       # Admin login page
    └── admin_dashboard.html    # Admin dashboard view
```

## License
This project is open-source and available under the MIT License.