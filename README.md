ai-attendance-system

Face recognition-based attendance system using OpenCV and PostgreSQL.

This project automates the daily attendance process by recognizing students' or employees' faces in real-time and securely logging their presence into a PostgreSQL database.

🚀 Features

Real-time Face Recognition: Detects and identifies multiple faces instantly using OpenCV.

Automated Database Logging: Marks attendance automatically in a PostgreSQL database with timestamps.

Proxy Prevention: Ensures high accuracy to prevent duplicate or proxy attendance.

Easy Management: Simple interface to register new users and view daily attendance records.

🛠️ Tech Stack

Programming Language: Python 3.x

Computer Vision: OpenCV, face_recognition

Database: PostgreSQL

Libraries: psycopg2 (PostgreSQL adapter), numpy, pandas

⚙️ Installation & Setup

Follow these steps to set up the project on your local machine:

1. Clone the repository

git clone https://github.com/vaishnavig8276/ai-attendance-system.git
cd ai-attendance-system


2. Create a Virtual Environment (Recommended)

# For Windows
python -m venv venv
venv\Scripts\activate

# For macOS/Linux
python3 -m venv venv
source venv/bin/activate


3. Install Dependencies

pip install -r requirements.txt


4. PostgreSQL Database Setup

Make sure you have PostgreSQL installed and running.

Create a new database named attendance_db.

Update your database credentials (username, password) in the project's configuration file (e.g., config.py or .env).

Run the initial script to create the necessary tables:

python setup_database.py


5. Run the Application

python main.py


📂 Project Structure

Here is an overview of the project's directory structure:

ai-attendance-system/
│
├── main.py                  # Main entry point of the application
├── requirements.txt         # List of Python dependencies
├── README.md                # Project documentation
├── .env                     # Environment variables and DB credentials
│
├── src/                     # Source code for the application
│   ├── face_detection.py    # Logic for OpenCV face detection and encoding
│   └── db_handler.py        # PostgreSQL connection and CRUD operations
│
├── dataset/                 # Folder to store registered user images
│   ├── User_1/
│   └── User_2/
│
└── database/                # Database related scripts
    └── setup_database.py    # Script to create initial tables


🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

📝 License

This project is open-source and available under the MIT License.
