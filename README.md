<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Tourism Planner - Login</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background: linear-gradient(135deg, #2193b0, #6dd5ed);
        }

        .login-container {
            width: 380px;
            background: white;
            padding: 35px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
        }

        .login-container h1 {
            text-align: center;
            color: #2193b0;
            margin-bottom: 10px;
        }

        .login-container p {
            text-align: center;
            color: #666;
            margin-bottom: 25px;
        }

        .input-group {
            margin-bottom: 18px;
        }

        .input-group label {
            display: block;
            margin-bottom: 7px;
            font-weight: bold;
            color: #333;
        }

        .input-group input {
            width: 100%;
            padding: 12px;
            border: 1px solid #ccc;
            border-radius: 8px;
            font-size: 15px;
            outline: none;
        }

        .input-group input:focus {
            border-color: #2193b0;
        }

        .login-btn {
            width: 100%;
            padding: 13px;
            border: none;
            border-radius: 8px;
            background: #2193b0;
            color: white;
            font-size: 16px;
            font-weight: bold;
            cursor: pointer;
        }

        .login-btn:hover {
            background: #176f86;
        }

        .register {
            text-align: center;
            margin-top: 20px;
        }

        .register a {
            color: #2193b0;
            text-decoration: none;
            font-weight: bold;
        }

        .register a:hover {
            text-decoration: underline;
        }
    </style>
</head>

<body>

    <div class="login-container">

        <h1>Tourism Planner</h1>
        <p>Login to plan your journey</p>

        <form onsubmit="login(event)">

            <div class="input-group">
                <label for="email">Email</label>
                <input
                    type="email"
                    id="email"
                    placeholder="Enter your email"
                    required>
            </div>

            <div class="input-group">
                <label for="password">Password</label>
                <input
                    type="password"
                    id="password"
                    placeholder="Enter your password"
                    required>
            </div>

            <button type="submit" class="login-btn">
                Login
            </button>

        </form>

        <div class="register">
            <p>Don't have an account?
                <a href="register.html">Register</a>
            </p>
        </div>

    </div>

    <script>
        function login(event) {
            event.preventDefault();

            const email = document.getElementById("email").value;
            const password = document.getElementById("password").value;

            // Demo login
            if (email === "admin@gmail.com" && password === "1234") {
                alert("Login successful!");
                window.location.href = "home.html";
            } else {
                alert("Invalid email or password!");
            }
        }
    </script>

</body>
</html># TourismPlanner
