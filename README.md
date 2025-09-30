<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Bech.co - Marketing Agency</title>
  <style>
    body, html {
      margin: 0;
      padding: 0;
      font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
      background-color: #0b1c0b;
      color: #f0f0f0;
      height: 100%;
    }

    header {
      background-color: #1a2e1a;
      padding: 15px 30px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    header h1 {
      margin: 0;
      font-size: 1.8em;
      color: #a4c639;
      cursor: pointer;
    }

    nav {
      display: flex;
      gap: 20px;
    }

    nav button {
      background: none;
      border: 2px solid #a4c639;
      padding: 8px 16px;
      border-radius: 5px;
      cursor: pointer;
      font-size: 1em;
      color: #f0f0f0;
      transition: all 0.3s ease;
    }

    nav button:hover {
      background-color: #a4c639;
      color: #0b1c0b;
    }

    section {
      display: none;
      padding: 50px 20px;
      min-height: 100vh;
      text-align: center;
    }

    section.active {
      display: block;
    }

    #home {
      background: url('db738d1a519b8af43dea7ea2a9e1b15e.jpg') center/cover no-repeat,
                  url('MoonSwatch-With-Camera.webp') center/cover no-repeat;
      position: relative;
      color: white;
    }

    #home::before {
      content: "";
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      background: rgba(0, 0, 0, 0.6);
    }

    #home .content {
      position: relative;
      z-index: 1;
      top: 40%;
      transform: translateY(-40%);
    }

    #our-work .gallery {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      margin-top: 30px;
    }

    #our-work .gallery img {
      max-width: 350px;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.7);
      transition: transform 0.3s ease;
    }

    #our-work .gallery img:hover {
      transform: scale(1.05);
    }

    footer {
      background-color: #1a2e1a;
      color: #f0f0f0;
      text-align: center;
      padding: 20px;
    }
  </style>
</head>
<body>
  <header>
    <h1 onclick="showSection('home')">Bech.co</h1>
    <nav>
      <button onclick="showSection('home')">Home</button>
      <button onclick="showSection('about')">About Us</button>
      <button onclick="showSection('clients')">Clients</button>
      <button onclick="showSection('our-work')">Our Work</button>
    </nav>
  </header>

  <!-- Home Section -->
  <section id="home" class="active">
    <div class="content">
      <h2>Welcome to Bech.co</h2>
      <p>Your Partner in Promotional Marketing & Creative Growth</p>
    </div>
  </section>

  <!-- About Section -->
  <section id="about">
    <h2>About Us</h2>
    <p>
      Bech.co is a dynamic platform dedicated to revolutionizing how businesses scale their reach and how skilled individuals monetize their influence. 
      We seamlessly connect companies with a vetted network of freelance product promoters, videographers, and brand advocates ready to drive targeted awareness and sales. 
      Our mission is to dismantle traditional marketing barriers by providing a transparent, efficient, and performance-driven marketplace where companies can easily find the perfect voice for their product, 
      and promoters can connect with impactful, relevant opportunities. <br><br>
      At Bech.co, we're not just a connector; we're building the future of decentralized, results-focused marketing.
    </p>
  </section>

  <!-- Clients Section -->
  <section id="clients">
    <h2>Our Clients</h2>
    <p>We proudly work with leading brands:</p>
    <ul style="list-style: none; padding: 0; font-size: 1.2em;">
      <li>✔ Titan</li>
      <li>✔ Tanishq</li>
      <li>✔ Rolex</li>
      <li>✔ Jacob & Co.</li>
    </ul>
  </section>

  <!-- Our Work Section -->
  <section id="our-work">
    <h2>Our Work</h2>
    <p>Here’s a showcase of our photography and promotional projects:</p>
    <div class="gallery">
      <img src="Rolex-watches-for-man-Australia_480x480.webp" alt="Rolex Watch">
      <img src="alagna-valsesia-december-3-2022-260nw-2246669183.webp" alt="Watch in Mountains">
      <img src="maxresdefault.jpg" alt="Tanishq Jewelry">
    </div>
  </section>

  <footer>
    <p>&copy; 2025 Bech.co | Marketing & Promotions</p>
  </footer>

  <script>
    function showSection(sectionId) {
      document.querySelectorAll("section").forEach(sec => sec.classList.remove("active"));
      document.getElementById(sectionId).classList.add("active");
    }
  </script>
</body>
</html>
