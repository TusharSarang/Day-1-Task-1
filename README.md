<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Responsive Landing Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet" />

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Poppins', sans-serif;
      background: #f9f9f9;
      color: #333;
    }
    .container {
      max-width: 1100px;
      margin: auto;
      padding: 0 20px;
    }

    header {
      background: #fff;
      box-shadow: 0 2px 5px rgba(0,0,0,0.05);
      position: sticky;
      top: 0;
      z-index: 1000;
    }
    header .container {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 15px 0;
    }
    .logo img {
      height: 40px;
    }
    nav ul {
      list-style: none;
      display: flex;
      gap: 20px;
    }
    nav a {
      text-decoration: none;
      color: #333;
      font-weight: 500;
      transition: color 0.3s;
    }
    nav a:hover {
      color: #007bff;
    }
    .menu-toggle {
      display: none;
      font-size: 24px;
      cursor: pointer;
    }

    .hero {
      background: #007bff;
      color: #fff;
      padding: 100px 20px;
      text-align: center;
    }
    .hero h1 {
      font-size: 2.5rem;
      margin-bottom: 15px;
    }
    .hero p {
      font-size: 1.2rem;
      margin-bottom: 25px;
    }
    .btn {
      padding: 12px 25px;
      background: #fff;
      color: #007bff;
      text-decoration: none;
      border-radius: 5px;
      font-weight: 600;
      transition: background 0.3s;
    }
    .btn:hover {
      background: #f2f2f2;
    }

    footer {
      background: #333;
      color: #fff;
      text-align: center;
      padding: 20px 0;
    }
    footer .social-links a {
      color: #fff;
      margin: 0 10px;
      font-size: 14px;
      text-decoration: none;
    }
    footer .social-links a:hover {
      color: #007bff;
    }

    @media (max-width: 768px) {
      nav ul {
        flex-direction: column;
        background: #fff;
        position: absolute;
        top: 60px;
        right: 0;
        width: 200px;
        display: none;
        border: 1px solid #ddd;
      }
      nav ul.active {
        display: flex;
      }
      .menu-toggle {
        display: block;
      }
    }
  </style>
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
        <a href="mailto:tusharsarang222@gmail.com">📧 tusharsarang222@gmail.com</a>
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