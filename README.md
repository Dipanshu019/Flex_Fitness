Flex Fitness - Gym Management System

• Table of Contents

- About The Project
- Features
- Technologies Used
- Getting Started
- Prerequisites
- Installation
- Usage
- Contact

• About The Project
 - Flex Fitness is a comprehensive web-based Gym Management System developed using PHP and MySQL. It aims to streamline the day-to-day operations of a fitness center, making it easier to manage members, subscriptions, trainers, classes, payments, and more. This system provides an intuitive interface for gym administrators, staff, and potentially members.

Key Goals:

Automate membership management.

Efficiently track payments and dues.

Organize classes and trainer schedules.

Provide insightful reports for business analysis.

Improve overall gym operational efficiency.

• Features
Here are some of the core features of the Flex Fitness Gym Management System:

Dashboard: An overview for administrators/staff with key metrics.

Member Management:

Add, edit, view, and delete member profiles.

Search and filter members.

Member activity tracking (e.g., check-ins/outs).

Subscription & Payment Management:

Define various membership plans (monthly, quarterly, annual, etc.).

Assign and renew member subscriptions.

Record and track payment history.

Generate payment receipts.

Trainer Management:

Add, edit, and manage trainer profiles.

Assign trainers to specific classes or members.

Class & Schedule Management:

Create and manage fitness classes (Yoga, Zumba, HIIT, etc.).

Set up class schedules and assign trainers.

Reporting:

Generate reports on memberships, payments, and attendance.

User Roles (Admin/Staff):

Different access levels for administrators and general staff.

Notifications (Optional):

Email/SMS reminders for membership expiry, upcoming classes.

Attendance Tracking (Optional):

System for members to mark attendance (e.g., manual or integrated with a barcode scanner).

• Technologies Used
Backend:

PHP [Version, e.g., 8.x]

MySQL / MariaDB

Frontend:

HTML5

CSS3 ([e.g., Tailwind CSS, Bootstrap, or custom CSS])

JavaScript ([e.g., jQuery, Vanilla JS])

Web Server:

Apache / Nginx

Database Management:

phpMyAdmin (or similar)

Other (Optional):

[Composer for dependency management, if used]

[Any other libraries/frameworks like PHPMailer, Chart.js etc.]

• Getting Started
To get a local copy up and running, follow these simple steps.

• Prerequisites
Before you begin, ensure you have the following installed on your system:

PHP: [e.g., PHP 8.0 or higher]

MySQL / MariaDB: Database server

Web Server: Apache or Nginx (e.g., part of XAMPP, WAMP, MAMP)

Composer: (Optional, if your project uses PHP dependencies managed by Composer)

sudo apt install composer (for Ubuntu/Debian)

[Link to Composer installation guide if needed]

• Installation
Clone the repository:

git clone https://github.com/Dipanshu019/Flex_Fitness.git
cd Flex_Fitness

Configure Web Server:

Place the Flex_Fitness directory in your web server's document root (e.g., htdocs for XAMPP, www for WAMP, /var/www/html for Apache on Linux).

Ensure your web server is configured to serve PHP files from this directory. You might need to set up a virtual host for cleaner URLs.

Database Setup:

Open your MySQL client (e.g., phpMyAdmin, MySQL Workbench, or command line).

Create a new database for the project:

CREATE DATABASE `flex_fitness_db`;

(Optional: You can replace flex_fitness_db with your preferred database name.)

Import the provided database schema. You should find a .sql file in the project.

# From the project root, assuming your SQL file is named `database.sql`
mysql -u your_db_username -p flex_fitness_db < database.sql

Alternatively, use phpMyAdmin to import the database.sql file.

Database Configuration (PHP):

Navigate to the [your_project_root]/config or [your_project_root]/includes directory.

Locate the database configuration file, typically named db_config.php, config.php, or similar.

Open this file and update the following details to match your database credentials:

<?php
// Example db_config.php content
define('DB_SERVER', 'localhost');
define('DB_USERNAME', 'your_db_username'); // e.g., root
define('DB_PASSWORD', 'your_db_password'); // e.g., "" for XAMPP root
define('DB_NAME', 'flex_fitness_db');

// Create connection
$link = mysqli_connect(DB_SERVER, DB_USERNAME, DB_PASSWORD, DB_NAME);

// Check connection
if($link === false){
    die("ERROR: Could not connect. " . mysqli_connect_error());
}
?>

Replace your_db_username and your_db_password with your actual MySQL credentials.

Install PHP Dependencies (if using Composer):

If your project uses Composer, navigate to the project root directory and run:

composer install

• Usage
After successful installation, you can access the application through your web browser:

Open your web browser and go to http://localhost/Flex_Fitness (or your configured virtual host URL, e.g., http://flexfitness.local).

Default Login Credentials:

Admin Username: admin

Admin Password: password (or admin123)

Note: It is highly recommended to change these default credentials immediately after your first login for security reasons.

Explore the different sections of the dashboard to:

Add new members and manage their details.

Create new subscription plans and assign them.

Process and track payments.

Manage trainers and their schedules.

Add and schedule classes.

View various reports to monitor gym performance.

• Contact

Dipanshu - deeputawar14@gmail.com
Project Link: https://github.com/Dipanshu019/Flex_Fitness
