# convergense

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>UniSchedule Login</title>
    <link rel="stylesheet" href="css/style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>

<body class="fade-in">
    <div class="login-screen">
        <div class="login-grid glass-card floating-card">

            <!-- Left Side: Form -->
            <div class="login-form-area">
                <h1 class="auth-title">UniSchedule</h1>
                <p class="auth-subtitle">University Automated Timetable System</p>

                <form onsubmit="return authenticate(event)">
                    <div class="form-group">
                        <label>Select Role</label>
                        <select id="role" class="form-control" required>
                            <option value="Admin">Admin</option>
                            <option value="Student">Student</option>
                            <option value="Faculty">Faculty</option>
                        </select>
                    </div>

                    <div class="form-group">
                        <label>Username / ID</label>
                        <input type="text" id="username" class="form-control" placeholder="Enter user ID" required>
                    </div>

                    <div class="form-group">
                        <label>Password</label>
                        <input type="password" id="password" class="form-control" placeholder="Enter password" required>
                    </div>

                    <button type="submit" class="btn btn-primary"
                        style="width: 100%; margin-top: 1.5rem; padding: 1rem;">
                        Login to Portal <i class="fas fa-arrow-right"></i>
                    </button>
                </form>
            </div>

            <!-- Right Side: Info -->
            <div class="login-info-area">
                <h3><i class="fas fa-key"></i> System Access Credentials</h3>

                <div class="cred-box">
                    <p style="margin-bottom: 5px;"><i class="fas fa-shield-alt"></i> <strong>Admin:</strong> admin /
                        admin123</p>
                    <p style="margin-bottom: 5px;"><i class="fas fa-graduation-cap"></i> <strong>Student:</strong>
                        student / student123</p>
                    <p><i class="fas fa-chalkboard-teacher"></i> <strong>Faculty:</strong> faculty01 / faculty123</p>
                </div>

                <div style="margin-top: 2rem;">
                    <h4><i class="fas fa-info-circle"></i> Access Notes</h4>
                    <ul style="padding-left: 1.5rem; font-size: 0.9rem; line-height: 1.8;">
                        <li>Admin has full access to the system backend.</li>
                        <li>Student account is restricted to read-only views.</li>
                        <li>Faculty can view schedules and apply for leave.</li>
                    </ul>
                </div>
            </div>

        </div>
    </div>

    <script src="js/script.js"></script>
</body>

</html>
