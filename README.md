# STUDENT-INFORMATION-DASHBOARD-
Creating a 2nd year mini project for my college about student information database , designed to efficiently manage and display student data. It integrates a user-friendly interface with a robust database system to store, retrieve, and update student information in real-time.
   student login #student login interface
   Frontend #html
   
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vel Tech High Tech Login</title>
    <link rel="stylesheet" href="style.css">
    <!-- Font Awesome for icons (optional, but good for username/password icons) -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
<body>
    <div class="background-image"></div>
    <div class="login-container">
        <div class="logo-section">
          
            <img src="veltech_logo.jpg"alt="Vel Tech Logo" class="logo" >
            <p class="college-name">Vel Tech High Tech</p>
        </div>
        <div class="login-form-section">
            <h2>WELCOME TO VTHT</h2>
            <div class="input-group">
                <i class="fas fa-user"></i>
                <input type="text" placeholder="VH.no">
            </div>
            <div class="input-group">
                <i class="fas fa-lock"></i>
                <input type="password" placeholder="DOB">
            </div>
            <button class="login-button">LOGIN</button>
            <p class="admin-login-link">Admin Login</p>
            <button class="admin.in-button">ADMIN</button>
        </div>
    </div>
</body>
</html>
#student login interface
#css
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap');

body {
    margin: 0;
    font-family: 'Poppins', sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background-color: #f0f2f5; /* Fallback background color */
    overflow: hidden; /* Prevent scroll if image is larger */
}

.background-image {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-image: url('veltech_college_background.jpg'); /* Replace with your actual image path */
    background-size: cover;
    background-position: center;
    filter: blur(3px) brightness(0.7); /* Adjust blur and brightness to make login clearer */
    z-index: -1;
}

.login-container {
    display: flex;
    background: rgba(255, 255, 255, 0.2); /* Glassmorphism background */
    border-radius: 20px;
    box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
    backdrop-filter: blur(10px);
    -webkit-backdrop-filter: blur(10px);
    border: 1px solid rgba(255, 255, 255, 0.18);
    padding: 30px;
    width: 800px; /* Adjust width as needed */
    max-width: 90%;
    color: white; /* Text color for glassmorphism effect */
    position: relative;
}

.logo-section {
    flex: 1;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background: linear-gradient(135deg, #6a11cb 0%, #2575fc 100%); /* Gradient background for logo section */
    border-radius: 15px;
    padding: 20px;
    margin-right: 30px;
}

.logo {
    width: 120px; /* Adjust logo size */
    height: 120px;
    margin-bottom: 15px;
}

.college-name {
    font-size: 1.2em;
    font-weight: 600;
    text-align: center;
    color: white;
}

.login-form-section {
    flex: 2;
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding-left: 20px;
}

.login-form-section h2 {
    text-align: center;
    margin-bottom: 30px;
    font-size: 2em;
    color: white;
    font-weight: 600;
}

.input-group {
    position: relative;
    margin-bottom: 25px;
    display: flex;
    align-items: center;
}

.input-group i {
    position: absolute;
    left: 15px;
    color: rgba(255, 255, 255, 0.8);
    font-size: 1.1em;
}

.input-group input {
    width: calc(100% - 70px); /* Adjust width considering icon and padding */
    padding: 15px 15px 15px 50px; /* Adjust padding for icon */
    border: none;
    border-radius: 10px;
    background: rgba(255, 255, 255, 0.1); /* Semi-transparent input background */
    color: white;
    font-size: 1em;
    outline: none;
    transition: background 0.3s ease;
}

.input-group input::placeholder {
    color: rgba(255, 255, 255, 0.7);
}

.input-group input:focus {
    background: rgba(255, 255, 255, 0.2);
}

.login-button {
    width: 100%;
    padding: 15px;
    border: none;
    border-radius: 10px;
    background: linear-gradient(to right, #ee0979, #ff6a00); /* Gradient for login button */
    color: white;
    font-size: 1.1em;
    font-weight: 600;
    cursor: pointer;
    transition: transform 0.2s ease-in-out;
    margin-top: 20px;
}

.login-button:hover {
    transform: translateY(-2px);
}

.admin-login-link {
    text-align: center;
    margin-top: 20px;
    font-size: 0.9em;
    color: rgba(255, 255, 255, 0.9);
}

.admin-login-link a {
    color: white;
    text-decoration: none;
    font-weight: 600;
}

.admin-login-link a:hover {
    text-decoration: underline;
}

/* Responsive adjustments */
@media (max-width: 768px) {
    .login-container {
        flex-direction: column;
        padding: 20px;
        width: 95%;
    }

    .logo-section {
        margin-right: 0;
        margin-bottom: 20px;
        padding: 15px;
    }

    .login-form-section {
        padding-left: 0;
    }

    .logo {
        width: 100px;
        height: 100px;
    }

    .login-form-section h2 {
        font-size: 1.8em;
    }
}
