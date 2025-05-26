<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
      Responsive Landing Page 
  <link rel="stylesheet" href="style.css" />
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet" />
</head>
<body>
  <header>
    <div class="container">
      <div class="logo">
        <img src="https://via.placeholder.com/120x40?text=LOGO" alt="Logo" />
      </div>
      <nav>
        <ul class="nav-links">
          <li><a href="#">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Our Services</a></li>
          <li><a href="#">Contact/help</a></li>
        </ul>
        <div class="menu-toggle" id="menu-toggle">&#9776;</div>
      </nav>
    </div>
  </header>

  <section class="hero">
    <div class="container hero-content">
      <h1>Welcome to Our Website</h1>
      <p>This is the responsive landing page,tried to add the navigation buttons too.</p>
      <a href="#" class="btn">Get Started</a>
    </div>
  </section>

  <footer>
    <div class="container">
      <p>© 2025 Your Company. All rights reserved.</p>
      <div class="social-links">
        <a href="#">🌐 Email = tusharsarang222@gmail.com</a>
        <a href="#">🐦 Location = Kolkata </a>
        <a href="#">📘 Facebook = Tushar_Sarang </a>
      </div>
    </div>
  </footer>

/* Header */
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

/* Hero Section */
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

/* Footer */
footer {
  background: #333;
  color: #fff;
  text-align: center;
  padding: 20px 0;
}
footer .social-links a {
  color: #fff;
  margin: 0 10px;
  font-size: 18px;
  text-decoration: none;
  transition: color 0.3s;
}
footer .social-links a:hover {
  color: #007bff;
}

/* Responsive */
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