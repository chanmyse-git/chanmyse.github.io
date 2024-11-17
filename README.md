<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Login Page</title>
  <style>
    body {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #f5f5f5;
    }
    .login-container {
      text-align: center;
      background-color: white;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    }
    .login-container input[type="text"],
    .login-container input[type="password"] {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    .login-container button {
      width: 100%;
      padding: 10px;
      background-color: #007bff;
      color: white;
      border: none;
      border-radius: 5px;
      font-size: 16px;
      cursor: pointer;
    }
    .login-container button:hover {
      background-color: #0056b3;
    }
    .login-container a {
      display: block;
      margin-top: 15px;
      color: #007bff;
      text-decoration: none;
      font-size: 14px;
    }
    .login-container a:hover {
      text-decoration: underline;
    }
  </style>
</head>
<body>
  <div class="login-container">
    <h2>Login</h2>
    <input type="text" id="userId" placeholder="Enter your ID">
    <input type="password" id="password" placeholder="Enter your Password">
    <button onclick="login()">Login</button>
    <a href="forgot-password.html">Forgot Password?</a>
  </div>

  <script>
    function login() {
      const userId = document.getElementById('userId').value;
      const password = document.getElementById('password').value;
      alert(`ID: ${userId}\nPassword: ${password}`);
      // Add login logic here
    }
  </script>
</body>
</html>
