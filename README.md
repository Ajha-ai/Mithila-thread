# Mithila-thread<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>MithilaThread</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600&family=Inter&display=swap" rel="stylesheet">
  <style>
    :root {
      --primary-color: #ff7043;
      --dark: #222;
      --light: #fafafa;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Inter', sans-serif;
      background-color: var(--light);
      color: var(--dark);
      line-height: 1.6;
    }

    header {
      background-color: white;
      padding: 20px 40px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      border-bottom: 1px solid #ddd;
      position: sticky;
      top: 0;
      z-index: 999;
    }

    header h1 {
      font-family: 'Playfair Display', serif;
      font-size: 28px;
      color: var(--primary-color);
    }

    nav a {
      margin: 0 15px;
      text-decoration: none;
      color: var(--dark);
      font-weight: 500;
      transition: color 0.3s ease;
    }

    nav a:hover {
      color: var(--primary-color);
    }

    .hero {
      background: linear-gradient(rgba(0,0,0,0.4), rgba(0,0,0,0.4)), url('hero-image.jpg') no-repeat center center/cover;
      height: 90vh;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      color: #fff;
      animation: fadeIn 2s ease-in;
    }

    .hero h2 {
      font-size: 48px;
      background-color: rgba(0, 0, 0, 0.5);
      padding: 20px 30px;
      border-radius: 8px;
      max-width: 90%;
    }

    .products {
      padding: 60px 40px;
      background-color: var(--light);
    }

    .products h3 {
      text-align: center;
      font-size: 32px;
      margin-bottom: 40px;
    }

    .product-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 30px;
    }

    .product {
      background-color: white;
      border-radius: 12px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.08);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      overflow: hidden;
      text-align: center;
    }

    .product img {
      width: 100%;
      height: 300px;
      object-fit: cover;
    }

    .product h4 {
      padding: 15px;
      font-size: 18px;
    }

    .product:hover {
      transform: translateY(-5px);
      box-shadow: 0 10px 20px rgba(0,0,0,0.1);
    }

    footer {
      background-color: var(--dark);
      color: #eee;
      text-align: center;
      padding: 30px 10px;
      font-size: 14px;
    }

    @keyframes fadeIn {
      0% { opacity: 0; transform: translateY(20px); }
      100% { opacity: 1; transform: translateY(0); }
    }

    @media (max-width: 600px) {
      .hero h2 {
        font-size: 32px;
        padding: 15px 20px;
      }

      header {
        flex-direction: column;
        align-items: flex-start;
      }

      nav {
        margin-top: 10px;
      }

      nav a {
        display: inline-block;
        margin: 10px 10px 0 0;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>MithilaThread</h1>
    <nav>
      <a href="#">Home</a>
      <a href="#">Shop</a>
      <a href="#">About</a>
      <a href="#">Contact</a>
    </nav>
  </header>

  <section class="hero">
    <h2>Wear the Story of Mithila</h2>
  </section>

  <section class="products">
    <h3>Featured Products</h3>
    <div class="product-grid">
      <div class="product">
        <img src="tshirt.jpg" alt="Mithila Art T-Shirt">
        <h4>Mithila Art T-Shirt</h4>
      </div>
      <div class="product">
        <img src="hoodie.jpg" alt="Mithila Art Hoodie">
        <h4>Mithila Art Hoodie</h4>
      </div>
      <div class="product">
        <img src="denim.jpg" alt="Mithila Denim Jacket">
        <h4>Mithila Denim Jacket</h4>
      </div>
    </div>
  </section>

  <footer>
    &copy; 2025 MithilaThread — Where Tradition Meets Style.
  </footer>

</body>
</html>
