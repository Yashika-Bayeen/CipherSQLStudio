# CipherSQLStudio 
This is a prototype for a SQL learning interface. It focuses on the core functionality of executing queries against a live database and displaying results.
---
## Project Overview
* **Database:** Used SQLite instead of PostgreSQL for easier setup and portability.
* **Architecture:** Developed as a single-page application rather than a multi-page assignment listing.
* **Editor:** Used a standard HTML text area for query input.
* **Security:** Query sanitization is not currently implemented; the engine runs raw SQL directly.

## Technology Stack
**Frontend:** React.js
**Backend:** Node.js with Express
**Database:** SQLite3
**Communication:** Axios (REST API)

## Installation and Setup
1. Backend Setup
Navigate to the backend folder and install the necessary dependencies:

```bash
cd backend
npm install
Initialize the Database: You must create the sandbox data before running the server:
```bash
node seed.js

Start the Server:
```bash
node server.js

The backend will run on http://localhost:5000.

2. Frontend Setup
Open a new terminal, navigate to the frontend folder, and install the dependencies:

```bash
cd frontend
npm install
Start the Application:

```bash
npm start
The application should open automatically at http://localhost:3000.

* **Usage Instructions**
Once the app loads, you will see a default query: SELECT * FROM employees;.

Click the "Run Query" button.

The results from the sandbox.db file will appear in the table below.

If you enter an invalid query (e.g., SELECT * FROM non_existent_table), an error message from the SQLite engine will be displayed.
