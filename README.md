TrueValue-Shop/
├── index.html           → Startseite (öffentlich)
├── admin.html           → Admin-Panel (einfach geschützt)
├── style.css            → Komplettes Design (grün, modern, responsive)
├── /assets
│   ├── logo.png         → Dein Logo (eingebunden)
│   └── product1.jpg     → Beispielproduktbilder
└── README.md            → Anleitung für GitHub Pages Upload
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>True Value Shop</title>
  <link rel="stylesheet" href="style.css" />
  <link rel="icon" type="image/png" href="assets/logo.png" />
</head>
<body>
  <header>
    <img src="assets/logo.png" alt="True Value Logo" class="logo" />
    <nav>
      <a href="#products">Products</a>
      <a href="admin.html">Admin</a>
    </nav>
  </header>

  <main>
    <section class="hero">
      <h1>Welcome to True Value</h1>
      <p>Trust Once, Buy Again – Quality you can count on!</p>
    </section>

    <section id="products" class="products">
      <h2>Our Products</h2>
      <div class="product-grid">
        <div class="product">
          <img src="assets/product1.jpg" alt="Product 1">
          <h3>Product Title</h3>
          <p>$19.99</p>
          <a href="https://www.aliexpress.com/" target="_blank" class="btn">Buy Now</a>
        </div>
        <!-- Weitere Produkte hier einfach duplizieren -->
      </div>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 True Value. All rights reserved.</p>
  </footer>
</body>
</html>
body {
  margin: 0;
  font-family: 'Segoe UI', sans-serif;
  background-color: #e9f7ef;
  color: #1b4332;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #fff;
  padding: 1rem 2rem;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

.logo {
  height: 50px;
}

nav a {
  margin-left: 20px;
  text-decoration: none;
  color: #1b4332;
  font-weight: bold;
}

.hero {
  text-align: center;
  padding: 3rem 1rem;
}

.products {
  padding: 2rem;
}

.product-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 2rem;
  justify-content: center;
}

.product {
  background: #fff;
  border-radius: 10px;
  padding: 1rem;
  text-align: center;
  box-shadow: 0 4px 6px rgba(0,0,0,0.1);
  max-width: 200px;
}

.product img {
  width: 100%;
  border-radius: 5px;
}

.btn {
  display: inline-block;
  margin-top: 10px;
  padding: 0.5rem 1rem;
  background-color: #2d6a4f;
  color: white;
  border-radius: 5px;
  text-decoration: none;
}

footer {
  text-align: center;
  padding: 1rem;
  background-color: #d8f3dc;
  margin-top: 2rem;
}
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Admin Panel</title>
  <link rel="stylesheet" href="style.css">
  <script>
    const password = "admin123";
    function checkLogin() {
      const input = prompt("Enter admin password:");
      if (input !== password) {
        alert("Access Denied.");
        window.location.href = "index.html";
      }
    }
    window.onload = checkLogin;
  </script>
</head>
<body>
  <header>
    <h1 style="margin: 0;">Admin Panel</h1>
  </header>
  <main style="padding: 2rem;">
    <h2>Welcome, Admin!</h2>
    <p>Here you can manage products manually or update content.</p>
    <p>(Diese Version ist statisch – für echte Funktionen brauchst du z. B. Firebase oder ein CMS.)</p>
  </main>
</body>
</html>
# True Value – Dropshipping Shop

## Anleitung zum Veröffentlichen (kostenlos):

1. Gehe zu https://github.com und erstelle ein neues Repository (z. B. `truevalue-shop`)
2. Lade alle Dateien (`index.html`, `style.css`, `admin.html`, Ordner `assets/`) hoch
3. Gehe zu **Settings > Pages**, wähle „Branch: `main` / Ordner: `/root`“
4. Fertig! Deine Seite ist live unter: `https://<dein-username>.github.io/truevalue-shop/`
