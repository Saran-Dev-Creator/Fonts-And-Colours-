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
