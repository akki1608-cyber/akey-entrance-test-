# Let's create the final animated index.html file content for Ankit's AKEY Entrance Test website.
index_html_content = """<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>AKEY Entrance Test</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: linear-gradient(135deg, #1e3c72, #2a5298);
      color: white;
      height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      animation: fadeIn 2s ease-in-out;
    }

    @keyframes fadeIn {
      0% { opacity: 0; transform: translateY(-20px); }
      100% { opacity: 1; transform: translateY(0); }
    }

    h1 {
      font-size: 3rem;
      margin-bottom: 10px;
      animation: pulse 2s infinite;
    }

    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.05); }
      100% { transform: scale(1); }
    }

    p {
      font-size: 1.2rem;
      max-width: 700px;
      margin: 0 auto 30px;
    }

    .btn-group {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
      justify-content: center;
    }

    a.btn {
      background: #ffffff;
      color: #2a5298;
      text-decoration: none;
      padding: 12px 25px;
      border-radius: 8px;
      font-weight: bold;
      transition: 0.3s ease;
    }

    a.btn:hover {
      background: #f1f1f1;
      transform: scale(1.05);
    }

    .logo {
      width: 100px;
      margin-bottom: 20px;
    }

    footer {
      position: absolute;
      bottom: 10px;
      font-size: 0.8rem;
      color: #ccc;
    }
  </style>
</head>
<body>

  <!-- Placeholder for logo -->
  <img src="logo.png" alt="AKEY Logo" class="logo" />

  <h1>🧠 AKEY Entrance Test</h1>
  <p>
    “Not your marks, your mind matters.”<br>
    AKEY is a unique entrance test based on <strong>real-life situations, logical reasoning, critical thinking</strong> and <strong>problem-solving ability</strong>. Not mugging, but mindset!
  </p>

  <div class="btn-group">
    <a href="login.html" class="btn">Login / Register</a>
    <a href="test.html" class="btn">Start Test</a>
    <a href="result-login.html" class="btn">Check Results</a>
  </div>

  <footer>© 2025 AKEY Entrance Test. All rights reserved.</footer>
</body>
</html>
"""

# Save this as index.html to share with the user
file_path = "/mnt/data/index.html"
with open(file_path, "w") as f:
    f.write(index_html_content)

file_path
