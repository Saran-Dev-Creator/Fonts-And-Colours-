<head>
  <title>My Cool Website</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="https://fonts.googleapis.com/css2?family=Poppins&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      background-color: #f8f9fa;
      color: #222;
      text-align: center;
      padding: 20px;
    }
    h1 {
      animation: fadeIn 2s ease-in-out;
    }
    @keyframes fadeIn {
      from {opacity: 0;}
      to {opacity: 1;}
    }
    img {
      width: 100%;
      max-width: 400px;
      border-radius: 8px;
    }
    input, textarea {
    width: 90%;
      padding: 10px;
      margin: 5px 0;
      font-size: 16px;
      border: 1px solid #ccc;
      border-radius: 6px;
    }
    button {
      padding: 10px 20px;
      font-size: 16px;
      background-color: #00b894;
      color: white;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      transition: 0.3s ease;
    }
    button:hover {
      background-color: #019875;
    }
    a {
      color: #0984e3;
      text-decoration: none;
      font-weight: bold;
    }
    a:hover {
      text-decoration: underline;
    }
   </style>
</head>

<body>
  <button onclick="toggleTheme()" id="theme-toggle">🌙 Dark Mode</button>
  <h1>Welcome to My Website</h1>
  <p>This site supports dark mode!</p>

  <script>
    function toggleTheme() {
      const body = document.body;
      const button = document.getElementById("theme-toggle");

      body.classList.toggle("dark-mode");

      if (body.classList.contains("dark-mode")) {
        button.textContent = "☀️ Light Mode";
      } else {
        button.textContent = "🌙 Dark Mode";
      }
    }
  </script>
</body>
