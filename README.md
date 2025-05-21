<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>One Humanity: Stand for Ukraine</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Roboto', sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f9f9f9;
      color: #333;
    }
    header {
      background-image: url('https://upload.wikimedia.org/wikipedia/commons/9/9b/Kyiv_after_Russian_invasion_February_2022_02.jpg');
      background-size: cover;
      background-position: center;
      color: black;
      text-align: center;
      padding: 100px 20px;
    }
    header h1 {
      font-size: 3em;
    }
    header p {
      font-size: 1.5em;
      margin-top: 20px;
    }
    .cta-button {
      margin-top: 30px;
      padding: 15px 30px;
      font-size: 1em;
      background-color: #007BFF;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      text-decoration: none;
    }
    .section {
      padding: 60px 20px;
      max-width: 1000px;
      margin: auto;
    }
    .section h2 {
      text-align: center;
      margin-bottom: 30px;
    }
    .impact-stats, .partners, .donation-options {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-around;
      text-align: center;
    }
    .card {
      flex: 1 1 250px;
      background: white;
      margin: 15px;
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }
    footer {
      background-color: #222;
      color: white;
      text-align: center;
      padding: 20px;
    }
  </style>
</head>
<body>

  <h1 id="title">Translate</h1>
  <p id="description">This is a multilingual website.</p>

  <label for="language">Choose Language:</label>
  <select id="language" onchange="translatePage()">
    <option value="en">English</option>
    <option value="es">Español</option>
    <option value="fr">Français</option>
  </select>

  <script>
    const translations = {
      en: {
        title: "Welcome",
        description: "This is a multilingual website example."
      },
      es: {
        title: "Bienvenido",
        description: "Este es un ejemplo de sitio web multilingüe."
      },
      fr: {
        title: "Bienvenue",
        description: "Ceci est un exemple de site Web multilingue."
      }
    };

    function translatePage() {
      const lang = document.getElementById("language").value;
      document.getElementById("title").innerText = translations[lang].title;
      document.getElementById("description").innerText = translations[lang].description;
    }
  </script>

  <header>
    <h1>Give Hope. Heal Lives. Help Ukraine.</h1>
    <p>Join us in providing urgent relief to those affected by the conflict in Ukraine.</p>
    <a href="#donate" class="cta-button">Donate Now</a>
  </header>

  <section class="section">
    <h2>Our Mission</h2>
    <p>We are a global movement delivering emergency aid, shelter, medical care, and hope to war victims in Ukraine. Together, we can make a difference—one life at a time.</p>
  </section>

  <section class="section">
    <h2>Impact So Far</h2>
    <div class="impact-stats">
      <div class="card">
        <h3>100,000+</h3>
        <p>Families supported with food and shelter</p>
      </div>
      <div class="card">
        <h3>50,000+</h3>
        <p>Individuals provided with trauma care</p>
      </div>
      <div class="card">
        <h3>$5M+</h3>
        <p>Raised through global donations</p>
      </div>
    </div>
  </section>

  <section class="section">
    <h2>Trusted Partners</h2>
    <div class="partners">
      <div class="card">
        <h3>UNICEF</h3>
        <p>Protecting children in crisis</p>
      </div>
      <div class="card">
        <h3>IRC</h3>
        <p>Emergency relief on the ground</p>
      </div>
      <div class="card">
        <h3>Doctors Without Borders</h3>
        <p>Medical assistance for victims</p>
      </div>
    </div>
  </section>

  <section id="donate" class="section">
    <h2>How to Donate</h2>
    <div class="donation-options">
      <div class="card">
        <h3>Online</h3>
        <p>Donate via Stripe, PayPal, Apple Pay, Google Pay</p>
      </div>
      <div class="card">
        <h3>Crypto</h3>
        <p>Accepting BTC, ETH, USDT with secure conversion</p>
      </div>
      <div class="card">
        <h3>Bank Transfer</h3>
        <p>Use Wise or SEPA for low-fee transfers</p>
      </div>
    </div>
  </section>

  <footer>
    <p>&copy; 2025 One Humanity. All rights reserved.</p>
  </footer>
</body>
</html>
