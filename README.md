<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Meta Garments — garment supply and apparel solutions for businesses.">
  <title>Meta Garments | Garment Supply</title>

  <style>
    :root {
      --navy: #172b3a;
      --blue: #29485c;
      --cream: #f5f3ee;
      --white: #ffffff;
      --text: #202b33;
      --muted: #68737b;
      --border: #e2e5e5;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, Helvetica, sans-serif;
      color: var(--text);
      background: var(--white);
      line-height: 1.7;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    .container {
      width: min(1120px, 90%);
      margin: auto;
    }

    header {
      background: var(--white);
      border-bottom: 1px solid var(--border);
    }

    nav {
      min-height: 76px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 24px;
      flex-wrap: wrap;
      padding: 16px 0;
    }

    .logo {
      font-size: 23px;
      font-weight: 800;
      letter-spacing: 1px;
      color: var(--navy);
    }

    .logo span {
      display: block;
      font-size: 10px;
      letter-spacing: 3px;
      color: var(--muted);
      font-weight: 500;
    }

    .nav-links {
      display: flex;
      flex-wrap: wrap;
      gap: 22px;
      font-size: 13px;
      font-weight: 600;
    }

    .nav-links a:hover,
    .text-link:hover {
      color: #52758b;
    }

    .hero {
      background: var(--navy);
      color: var(--white);
      padding: 105px 0 100px;
    }

    .eyebrow {
      text-transform: uppercase;
      letter-spacing: 3px;
      font-size: 11px;
      font-weight: 700;
      margin-bottom: 18px;
      color: #b9ccd6;
    }

    h1 {
      max-width: 760px;
      font-size: clamp(38px, 6vw, 68px);
      line-height: 1.12;
      letter-spacing: -1.5px;
      margin-bottom: 24px;
    }

    .hero p {
      max-width: 590px;
      color: #d8e1e6;
      font-size: 17px;
      margin-bottom: 30px;
    }

    .button {
      display: inline-block;
      padding: 12px 20px;
      background: var(--white);
      color: var(--navy);
      font-weight: 700;
      font-size: 13px;
      border: 1px solid var(--white);
      transition: 0.2s;
    }

    .button:hover {
      background: #e8edf0;
    }

    .button-outline {
      background: transparent;
      color: var(--white);
      margin-left: 8px;
    }

    section {
      padding: 78px 0;
      scroll-margin-top: 20px;
    }

    .section-heading {
      max-width: 650px;
      margin-bottom: 32px;
    }

    .section-heading .eyebrow {
      color: #617a89;
      margin-bottom: 10px;
    }

    h2 {
      font-size: clamp(28px, 4vw, 42px);
      line-height: 1.2;
      color: var(--navy);
      margin-bottom: 16px;
    }

    .section-heading p,
    .section-copy {
      color: var(--muted);
      font-size: 15px;
    }

    .about-grid,
    .factory-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 42px;
      align-items: center;
    }

    .feature-panel {
      min-height: 270px;
      background: var(--cream);
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 35px;
      text-align: center;
    }

    .feature-panel strong {
      display: block;
      color: var(--navy);
      font-size: 22px;
      margin-bottom: 8px;
    }

    .feature-panel p {
      color: var(--muted);
      font-size: 13px;
    }

    .text-link {
      display: inline-block;
      margin-top: 22px;
      font-size: 13px;
      font-weight: 700;
      color: var(--navy);
      border-bottom: 1px solid #a9b5bc;
      padding-bottom: 4px;
    }

    .catalogue {
      background: var(--cream);
    }

    .product-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 20px;
    }

    .product-card {
      background: var(--white);
      border: 1px solid var(--border);
      padding: 28px;
    }

    .product-number {
      color: #7a8d98;
      font-size: 12px;
      letter-spacing: 2px;
      margin-bottom: 22px;
    }

    .product-card h3 {
      font-size: 19px;
      color: var(--navy);
      margin-bottom: 10px;
    }

    .product-card p {
      font-size: 14px;
      color: var(--muted);
    }

    .customise {
      background: var(--white);
    }

    .customise-box {
      background: #edf1f2;
      padding: 38px;
      border-left: 4px solid var(--blue);
    }

    .customise-box h3 {
      font-size: 23px;
      color: var(--navy);
      margin-bottom: 10px;
    }

    .customise-box p {
      color: var(--muted);
      max-width: 700px;
    }

    .factory {
      background: var(--cream);
    }

    .factory-panel {
      background: #dfe5e6;
      min-height: 270px;
      padding: 30px;
      display: flex;
      flex-direction: column;
      justify-content: center;
    }

    .factory-panel strong {
      font-size: 22px;
      color: var(--navy);
      margin-bottom: 8px;
    }

    .contact-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 35px;
    }

    .contact-card {
      padding: 26px;
      border: 1px solid var(--border);
    }

    .contact-card h3 {
      color: var(--navy);
      margin-bottom: 8px;
    }

    .contact-card p {
      color: var(--muted);
      font-size: 14px;
    }

    footer {
      background: var(--navy);
      color: var(--white);
      padding: 28px 0;
      font-size: 12px;
    }

    .footer-inner {
      display: flex;
      justify-content: space-between;
      gap: 15px;
      flex-wrap: wrap;
    }

    footer p {
      color: #c6d2d9;
    }

    @media (max-width: 720px) {
      nav {
        align-items: flex-start;
      }

      .nav-links {
        gap: 12px 16px;
      }

      .hero {
        padding: 75px 0;
      }

      section {
        padding: 55px 0;
      }

      .about-grid,
      .factory-grid,
      .contact-grid {
        grid-template-columns: 1fr;
      }

      .product-grid {
        grid-template-columns: 1fr;
      }

      .button-outline {
        margin: 10px 0 0;
      }

      .customise-box {
        padding: 25px;
      }
    }
  </style>
</head>

<body>

  <header>
    <nav class="container">
      <a href="#home" class="logo">
        META GARMENTS
        <span>GARMENT SUPPLY</span>
      </a>

      <div class="nav-links">
        <a href="#home">Home</a>
        <a href="#about">About Us</a>
        <a href="#products">Products</a>
        <a href="#customise">Customisation</a>
        <a href="#factory">Manufacturing</a>
        <a href="#contact">Contact</a>
      </div>
    </nav>
  </header>

  <main>
    <section class="hero" id="home">
      <div class="container">
        <p class="eyebrow">META GARMENTS · BUSINESS ENQUIRIES</p>

        <h1>Garments made around your business requirements.</h1>

        <p>
          Explore our garment range, learn about our business,
          and get in touch with us to discuss your apparel requirements.
        </p>

        <a class="button" href="#products">Explore Products</a>
        <a class="button button-outline" href="#contact">Contact Us</a>
      </div>
    </section>

    <section id="about">
      <div class="container about-grid">
        <div>
          <div class="section-heading">
            <p class="eyebrow">ABOUT META GARMENTS</p>
            <h2>A business built around garment requirements.</h2>
          </div>

          <p class="section-copy">
            Meta Garments is an apparel business focused on garment
            supply and business enquiries. We aim to make it easier
            for buyers to explore products, discuss specifications,
            and communicate their requirements directly with our team.
          </p>

          <a class="text-link" href="#contact">Learn More About Us →</a>
        </div>

        <div class="feature-panel">
          <div>
            <strong>Meta Garments</strong>
            <p>Apparel · Products · Business Enquiries</p>
          </div>
        </div>
      </div>
    </section>

    <section class="catalogue" id="products">
      <div class="container">
        <div class="section-heading">
          <p class="eyebrow">OUR PRODUCTS</p>
          <h2>Explore our garment range.</h2>
          <p>
            Discover the types of garments we offer. Contact us
            to discuss product details and specific requirements.
          </p>
        </div>

        <div class="product-grid">
          <article class="product-card">
            <p class="product-number">PRODUCT CATEGORY 01</p>
            <h3>Formal Shirts</h3>
            <p>Explore shirt options and discuss fabric, colour and design requirements.</p>
            <a class="text-link" href="#contact">Enquire About Shirts →</a>
          </article>

          <article class="product-card">
            <p class="product-number">PRODUCT CATEGORY 02</p>
            <h3>T-Shirts</h3>
            <p>Discuss available styles, fabrics and requirements for your order.</p>
            <a class="text-link" href="#contact">Enquire About T-Shirts →</a>
          </article>

          <article class="product-card">
            <p class="product-number">PRODUCT CATEGORY 03</p>
            <h3>Other Garments</h3>
            <p>Contact us to discuss other garment categories and specifications.</p>
            <a class="text-link" href="#contact">Make an Enquiry →</a>
          </article>
        </div>

        <a class="text-link" href="#contact">Interested in more products? Contact Us →</a>
      </div>
    </section>

    <section class="customise" id="customise">
      <div class="container">
        <div class="customise-box">
          <p class="eyebrow">GARMENT CUSTOMISATION</p>
          <h3>Have a specific garment in mind?</h3>
          <p>
            Tell us about your preferred fabric, colour, design and
            other requirements. Our team can discuss the available
            options with you.
          </p>
          <a class="text-link" href="#contact">Discuss Your Requirements →</a>
        </div>
      </div>
    </section>

    <section class="factory" id="factory">
      <div class="container factory-grid">
        <div>
          <div class="section-heading">
            <p class="eyebrow">OUR OPERATIONS</p>
            <h2>Learn more about our garment operations.</h2>
          </div>

          <p class="section-copy">
            Interested in learning more about how we work?
            Contact us to discuss our operations and the processes
            relevant to your requirements.
          </p>

          <a class="text-link" href="#contact">Learn More About Our Operations →</a>
        </div>

        <div class="factory-panel">
          <strong>Inside Meta Garments</strong>
          <p>Manufacturing photographs and videos can be added here when ready.</p>
        </div>
      </div>
    </section>

    <section id="contact">
      <div class="container">
        <div class="section-heading">
          <p class="eyebrow">CONTACT</p>
          <h2>Let's discuss your requirements.</h2>
          <p>
            Contact our team to enquire about products,
            garment specifications or potential business opportunities.
          </p>
        </div>

        <div class="contact-grid">
          <div class="contact-card">
            <h3>Business Email</h3>
            <p>Add your official Meta Garments email address before publishing.</p>
          </div>

          <div class="contact-card">
            <h3>Phone & WhatsApp</h3>
            <p>Add your business contact number before publishing.</p>
          </div>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="container footer-inner">
      <strong>META GARMENTS</strong>
      <p>© <span id="year"></span> Meta Garments. All rights reserved.</p>
    </div>
  </footer>

  <script>
    document.getElementById("year").textContent = new Date().getFullYear();
  </script>

</body>
</html>
