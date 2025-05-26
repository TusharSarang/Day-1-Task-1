<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Responsive Landing Page</title>
  <link rel="stylesheet" href="style.css" />
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet" />
</head>
<body>

  <!-- Header -->
  <header>
    <div class="container">
      <div class="logo">
        <img src="64F4ACE5-2E5F-4054-AC84-2C0ABE4C967C.png" alt="Logo" />
      </div>
      <nav>
        <ul class="nav-links">
          <li><a href="#">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Services</a></li>
          <li><a href="#">Contact</a></li>
        </ul>
        <div class="menu-toggle" id="menu-toggle">&#9776;</div>
      </nav>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="hero">
    <div class="container">
      <h1>Welcome to Our Website</h1>
      <p>Your journey to awesome web experiences starts here.</p>
      <a href="#" class="btn">Get Started</a>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <div class="container">
      <p>© 2025 Your Company. All rights reserved.</p>
      <div class="social-links">
        <a href="mailto:your-email@example.com">📧 your-email@example.com</a>
        <a href="#">📍 Kolkata</a>
      </div>
    </div>
  </footer>

  <!-- Mobile Nav Script -->
  <script>
    const toggle = document.getElementById("menu-toggle");
    const navLinks = document.querySelector(".nav-links");
    toggle.addEventListener("click", () => {
      navLinks.classList.toggle("active");
    });
  </script>
</body>
</html>