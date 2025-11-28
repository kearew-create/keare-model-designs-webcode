<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="Keare Model Designs – Custom apparel and branding for expressive, inclusive fashion." />
  <title>Keare Model Designs</title>
  <style>
    :root {
      --black: #111111;
      --gold: #d4af37;
      --pink: #ff4081;
    }

    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: var(--black);
      color: white;
    }

    header, footer {
      background: var(--black);
      color: var(--gold);
      padding: 1em;
      text-align: center;
    }

    nav a {
      margin: 0 1em;
      color: var(--pink);
      text-decoration: none;
      font-weight: bold;
    }

    nav a:hover {
      color: var(--gold);
    }

    main {
      padding: 2em;
      background: #222;
    }

    section {
      margin-bottom: 2em;
      background: #333;
      padding: 1.5em;
      border-radius: 8px;
      border: 2px solid var(--gold);
    }

    h1, h2 {
      color: var(--gold);
    }

    form input, form select {
      display: block;
      margin: 0.5em 0;
      padding: 0.5em;
      width: 100%;
      max-width: 400px;
      border: 1px solid var(--gold);
      border-radius: 4px;
    }

    .cta {
      background: var(--pink);
      color: white;
      padding: 0.75em 1.5em;
      border: none;
      cursor: pointer;
      font-weight: bold;
      border-radius: 4px;
    }

    .cta:hover {
      background: var(--gold);
      color: var(--black);
    }
  </style>
</head>
<body>
  <header>
    <h1>Keare Model Designs</h1>
    <nav>
      <a href="#about">About</a>
      <a href="#shop">Shop</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <main>
    <section id="about">
      <h2>About Us</h2>
      <p>We create custom apparel and branding that celebrates identity, style, and representation.</p>
    </section>
<section id="shop">
  <h2>Featured Products</h2>
  <p>Explore our expressive fashion line — designed for real people with bold vision.</p>

  <div class="product-grid">
    <div class="product-card">
      <img src="images/shirt.jpg" alt="Custom Gold Logo Shirt" />
      <h3>Gold Logo Tee</h3>
      <p>Bold identity on soft cotton.</p>
      <button class="cta">Add to Cart</button>
    </div>

    <div class="product-card">
      <img src="images/hoodie.jpg" alt="Pink Accent Hoodie" />
      <h3>Pink Accent Hoodie</h3>
      <p>Comfort meets expressive style.</p>
      <button class="cta">Add to Cart</button>
    </div>

    <div class="product-card">
      <img src="images/cap.jpg" alt="Black & Gold Cap" />
      <h3>Black & Gold Cap</h3>
      <p>Minimalist design with luxury detail.</p>
      <button class="cta">Add to Cart</button>
    </div>
  </div>
</section>

    <section id="shop">
      <h2>Featured Products</h2>
      <p>Explore our expressive fashion line — designed for real people with bold vision.</p>
      <button class="cta">Shop Now</button>
    </section>

    <section id="contact">
      <h2>Contact Us</h2>
      <form id="contactForm">
        <label for="username">Username (max 10 characters):</label>
        <input type="text" id="username" name="username" />

        <label for="phone">Phone Number:</label>
        <input type="text" id="phone" name="phone" />

        <label for="age">Your Age:</label>
        <input type="number" id="age" name="age" />

        <button type="submit" class="cta">Submit</button>
      </form>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 Keare Model Designs</p>
  </footer>

  <script>
    const form = document.getElementById("contactForm");
    const ageInput = document.getElementById("age");
    let userAgeValid = false;
    const validColor = "#c8e6c9";
    const invalidColor = "#ffcdd2";

    ageInput.addEventListener("input", () => {
      const age = parseInt(ageInput.value);
      ageInput.style.backgroundColor = invalidColor;
      userAgeValid = false;
      if (age >= 15 && age <= 120) {
        ageInput.style.backgroundColor = validColor;
        userAgeValid = true;
      }
    });

    form.addEventListener("submit", (event) => {
      const username = document.getElementById("username").value;
      const phone = document.getElementById("phone").value;

      if (username.length > 10 || isNaN(phone) || phone.length < 9 || !userAgeValid) {
        console.log("Input is invalid");
        event.preventDefault();
      }
    });
  </script>
</body>
</html>

## Repo  
https://github.com/kearew-create/keare-model-designs-webcode








