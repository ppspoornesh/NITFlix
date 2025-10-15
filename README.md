NITFlix (internally known as BookMyNIT) is a modern, robust, and scalable seat reservation system designed for managing movie or event ticket bookings. Leveraging the power of Google Firebase, this project offers real-time seat availability tracking and efficient data management, making it perfect for deploying a reliable ticketing solution for a cinema, theater, or institutional event.

**Key Features
Real-time Seat Tracking: Utilizes Firebase Firestore to provide instantaneous updates on seat availability, preventing double-bookings.

Flexible Seating Maps: Easily configure complex seating layouts using the included populateSeats.js script.

Scalable Backend: Built on Node.js and Firebase Admin SDK for a fast and reliable server-side foundation.

Dedicated Setup Script: Includes a utility (populateSeats.js) to quickly initialize the database with a predefined show and seat arrangement.

**Tech Stack
The core of NITFlix is built using the following technologies:

Category	Technology	Purpose
Backend	Node.js	JavaScript runtime environment for the server-side logic.
Database	Firebase Firestore	NoSQL cloud database for real-time data synchronization.
Authentication	Firebase Admin SDK	Securely interacts with the Firebase project and services.

Export to Sheets
Setup and Installation
Follow these steps to set up the project locally.

Prerequisites
Node.js (LTS version recommended)

A Firebase Project (Google Cloud Project)

1. Clone the Repository
Bash

git clone <your-repository-url>
cd NITFlix
2. Install Dependencies
Install the required packages listed in package.json:

Bash

npm install
3. Configure Firebase Admin Credentials
This project requires a Firebase Service Account Key to initialize the Admin SDK and connect to your Firestore database.

Go to your Firebase Project Console.

Navigate to Project settings > Service accounts.

Click Generate new private key and download the JSON file.

Rename the downloaded file to serviceAccountKey.json and place it in the root directory of this project.

4. Populate Seating Data
Run the utility script to initialize a sample show and populate the seat structure in your Firestore database.

Bash

node populateSeats.js
Note: You can customize the showId and seatLayout variables inside populateSeats.js to match your specific event structure before running the script.

***Contribution
Contributions are welcome! If you have suggestions or want to improve the project, please open an issue or submit a pull request.
