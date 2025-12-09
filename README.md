# Jewel Aura

A modern e-commerce platform for buying and selling jewelry, built as part of Year 1 Semester 2 Web Based Application Development coursework.

## 📋 Table of Contents

- [About](#about)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Configuration](#configuration)
- [Database Setup](#database-setup)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Authors](#authors)

## 🎯 About

Jewel Aura is a comprehensive jewelry e-commerce platform that allows users to buy and sell jewelry online. The platform provides a seamless experience for customers to browse services, manage their accounts, and interact with the jewelry marketplace.

## ✨ Features

- **User Authentication**: Secure sign-up and sign-in functionality
- **Buy & Sell**: Platform for buying and selling jewelry
- **User Profile**: Personal profile management
- **Services**: Browse and explore jewelry services
- **Contact System**: Contact form for customer inquiries
- **Admin Panel**: Administrative interface for managing users and content
- **Responsive Design**: Mobile-friendly interface
- **Legal Pages**: Privacy Policy, Terms & Conditions, and Refund Policy

## 🛠️ Tech Stack

- **Frontend**: HTML5, CSS3
- **Backend**: PHP
- **Database**: MySQL
- **Server**: Apache (XAMPP/WAMP/LAMP)

## 📦 Prerequisites

Before you begin, ensure you have the following installed:

- [XAMPP](https://www.apachefriends.org/) (or WAMP/LAMP) - PHP development environment
- MySQL Server
- A modern web browser (Chrome, Firefox, Safari, Edge)
- PHP 7.4 or higher
- MySQL 5.7 or higher

## 🚀 Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/jewel-aura-2023.git
   cd jewel-aura-2023
   ```

2. **Start XAMPP/WAMP/LAMP**

   - Start Apache and MySQL services from your control panel

3. **Move project to web server directory**

   - **XAMPP**: Copy the project folder to `C:\xampp\htdocs\` (Windows) or `/Applications/XAMPP/htdocs/` (macOS)
   - **WAMP**: Copy to `C:\wamp64\www\`
   - **LAMP**: Copy to `/var/www/html/`

4. **Access the application**
   - Open your browser and navigate to: `http://localhost/jewel-aura-2023/`

## ⚙️ Configuration

### Database Configuration

1. **Update database credentials** in `connection.php`:

   ```php
   $hostName = "localhost";
   $dbUser = "root";
   $dbPassword = "";  // Update with your MySQL password if set
   $dbName = "jewel_aura_db";
   ```

2. **Update credentials** in `actions.php` and `contactActions.php` if needed

## 🗄️ Database Setup

1. **Open phpMyAdmin**

   - Navigate to `http://localhost/phpmyadmin`

2. **Create the database**

   - Click on "New" to create a new database
   - Name it: `jewel_aura_db`
   - Select collation: `utf8mb4_general_ci`

3. **Import the database schema**

   - Select the `jewel_aura_db` database
   - Click on "Import" tab
   - Choose the `database.sql` file from the project root
   - Click "Go" to import

   Alternatively, you can run the SQL commands directly:

   ```sql
   CREATE DATABASE jewel_aura_db;
   USE jewel_aura_db;
   -- Then run the SQL commands from database.sql
   ```

## 📖 Usage

### For Users

1. **Sign Up**: Navigate to `signup.html` to create a new account
2. **Sign In**: Use `signin.html` to log into your account
3. **Browse Services**: Explore available jewelry services
4. **Buy/Sell**: Access buy and sell features through the navigation
5. **Contact**: Use the contact form for inquiries
6. **Profile**: Manage your profile information

### For Administrators

1. Navigate to `admin/index.php` to access the admin panel
2. Manage users through `admin/users.php`
3. Edit content through `admin/edit.php`

## 📁 Project Structure

```
jewel-aura-2023/
│
├── admin/                 # Admin panel files
│   ├── edit.php          # Edit functionality
│   ├── index.php         # Admin dashboard
│   └── users.php         # User management
│
├── css/                  # Stylesheets
│   ├── contact.css       # Contact page styles
│   └── style.css         # Main stylesheet
│
├── img/                  # Images and media files
│   └── [various images]  # Product images, logos, etc.
│
├── actions.php           # User registration/login actions
├── contactActions.php    # Contact form handler
├── connection.php        # Database connection
├── database.sql          # Database schema
│
├── index.html            # Homepage
├── about.html            # About page
├── services.html         # Services page
├── buy.html              # Buy jewelry page
├── sell.html             # Sell jewelry page
├── contact.html          # Contact page
├── signin.html           # Sign in page
├── signup.html           # Sign up page
├── profile.html          # User profile page
├── privacy.html          # Privacy policy
├── terms.html            # Terms and conditions
├── Refund Policy.html    # Refund policy
│
└── README.md             # This file
```

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is created for educational purposes as part of Year 1 Semester 2 Web Based Application Development coursework.

## 👥 Authors

- **Development Team** - Year 1 Semester 2 Web Based Application Development

## 🙏 Acknowledgments

- Course instructors and teaching staff
- Open source community for inspiration and resources

---

**Note**: This is an educational project. Ensure you follow best practices for security, especially regarding password hashing, SQL injection prevention, and input validation before deploying to production.
