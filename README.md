# constructors.co.ke
engineering
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Authentic Constructors Kenya</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

  <style>
    :root {
      --yellow: #ffc107;
      --black: #000;
      --white: #fff;
      --gray-light: #f4f4f4;

      --primary: #00553A;
      --accent: #F9A825;
      --bg: #f4f6f8;
      --text: #333;
    }

    /* RESET & BASE */
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      font-family: Arial, sans-serif;
      color: var(--black);
      background: var(--gray-light);
      line-height: 1.6;
    }
    a { text-decoration: none; }
    ul { list-style: none; }

    /* CUSTOM HEADER */
    .custom-header .container {
      padding: 40px 20px;
      background: #fff;
      border-radius: 12px;
      box-shadow: 0 0 20px rgba(0,0,0,0.1);
      animation: fadeIn 1.2s ease-out;
      text-align: center;
      margin: 20px auto 0;
      max-width: 800px;
    }

    .custom-header h1 {
      font-size: 2.4em;
      color: var(--primary);
      margin-bottom: 10px;
    }

    .custom-header h2 {
      font-size: 1.4em;
      color: var(--accent);
      margin-bottom: 15px;
    }

    .custom-header i {
      font-size: 48px;
      color: var(--accent);
      margin-bottom: 15px;
      animation: bounce 2s infinite;
    }

    /* NAVIGATION */
    .nav-toggle {
      display: none;
      font-size: 1.8rem;
      background: none;
      color: var(--yellow);
      border: none;
      cursor: pointer;
      margin: 20px auto;
      display: block;
    }

    nav.nav {
      text-align: center;
      background: var(--black);
      overflow: hidden;
      max-height: 0;
      transition: max-height 0.4s ease-in-out, opacity 0.4s ease, transform 0.3s ease;
      opacity: 0;
      transform: translateY(-10px);
      pointer-events: none;
    }

    nav.nav.active {
      max-height: 500px;
      opacity: 1;
      transform: translateY(0);
      pointer-events: auto;
    }

    nav.nav ul {
      display: flex;
      flex-direction: column;
      padding: 10px;
    }

    nav.nav li {
      margin: 10px 0;
    }

    nav.nav a {
      color: var(--yellow);
      font-weight: bold;
      transition: opacity 0.2s;
    }

    nav.nav a:hover { opacity: 0.7; }

    @media (min-width: 769px) {
      .nav-toggle {
        display: none;
      }

      nav.nav {
        max-height: none !important;
        opacity: 1 !important;
        transform: none !important;
        pointer-events: auto !important;
      }

      nav.nav ul {
        flex-direction: row;
        justify-content: center;
        flex-wrap: wrap;
      }

      nav.nav li {
        margin: 0 10px;
      }
    }

    /* SECTION STYLING */
    section {
      background: var(--white);
      margin: 40px auto;
      padding: 20px;
      max-width: 800px;
      border-left: 5px solid var(--yellow);
      border-radius: 4px;
      opacity: 0;
      animation: fadeIn 1s forwards;
    }
    section:nth-of-type(1) { animation-delay: 0.3s; }
    section:nth-of-type(2) { animation-delay: 0.6s; }
    section:nth-of-type(3) { animation-delay: 0.9s; }
    section:nth-of-type(4) { animation-delay: 1.2s; }
    section:nth-of-type(5) { animation-delay: 1.5s; }
    section:nth-of-type(6) { animation-delay: 1.8s; }
    section:nth-of-type(7) { animation-delay: 2.1s; }
    section:nth-of-type(8) { animation-delay: 2.4s; }
    section:nth-of-type(9) { animation-delay: 2.7s; }
    section:nth-of-type(10){ animation-delay: 3.0s; }
    section:nth-of-type(11){ animation-delay: 3.3s; }
    section:nth-of-type(12){ animation-delay: 3.6s; }

    section h2 {
      font-size: 1.4rem;
      color: var(--black);
      border-bottom: 2px solid var(--yellow);
      display: inline-flex;
      align-items: center;
      padding-bottom: 4px;
      margin-bottom: 15px;
    }

    .icon {
      width: 32px;
      height: 32px;
      margin-right: 8px;
    }

    .section-image {
      width: 100%;
      border-radius: 4px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      margin: 12px 0;
    }

    ul.details { margin-left: 20px; list-style: disc; }

    /* CONTACT BUTTON */
    .contact {
      text-align: center;
      margin: 60px 0;
      animation: fadeIn 1s forwards;
      animation-delay: 4s;
    }

    .whatsapp-link {
      display: inline-block;
      background: var(--yellow);
      color: var(--black);
      padding: 15px 30px;
      font-size: 1.1rem;
      border-radius: 4px;
      font-weight: bold;
      box-shadow: 0 2px 6px rgba(0,0,0,0.2);
      animation: bounce 2s infinite;
    }

    /* ANIMATIONS */
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to   { opacity: 1; transform: translateY(0); }
    }

    @keyframes bounce {
      0%,100% { transform: translateY(0); }
      50% { transform: translateY(-6px); }
    }
  </style>
</head>
<body>

  <header class="custom-header">
    <div class="container">
      <i class="fas fa-building"></i>
      <h1>Authentic Constructors</h1>
      <h2>Building Services and Consultation</h2>
      <p>Delivering quality, structure, and style — from blueprint to finish.</p>
    </div>
  </header>

  <button class="nav-toggle" aria-label="Toggle navigation">&#9776;</button>
  <nav class="nav">
    <ul>
      <li><a href="#drawing">Drawing</a></li>
      <li><a href="#interior">Interior</a></li>
      <li><a href="#construction">Construction</a></li>
      <li><a href="#welding">Welding</a></li>
      <li><a href="#bending">Bar Bending</a></li>
      <li><a href="#landscape">Landscaping</a></li>
      <li><a href="#painting">Painting</a></li>
      <li><a href="#drainage">Drainage</a></li>
      <li><a href="#carbo">Paving</a></li>
      <li><a href="#plumbing">Plumbing</a></li>
      <li><a href="#carpentry">Carpentry</a></li>
    </ul>
  </nav>

  <section id="drawing">
    <h2><img src="icons/blueprint.svg" alt="blueprint icon" class="icon" /> Building Drawing</h2>
    <img src="images/building-drawing.jpg" alt="Ground and Roof Plans" class="section-image" />
    <p>Detailed CAD layouts for ground floor and roof plans to guide construction.</p>
  </section>

  <section id="interior">
    <h2><img src="icons/interior.svg" alt="interior icon" class="icon" /> Interior Design</h2>
    <img src="images/interior-design.jpg" alt="Interior Visualization" class="section-image" />
    <p>3D mockups, material palettes, lighting and furniture schemes crafted to your style.</p>
  </section>

  <section id="construction">
    <h2><img src="icons/crane.svg" alt="crane icon" class="icon" /> Construction Works</h2>
    <img src="images/construction-works.jpg" alt="On-site Construction" class="section-image" />
    <p>Full turnkey structural and architectural execution with expert crews and KOLIDA tools.</p>
  </section>

  <section id="welding">
    <h2><img src="icons/welding.svg" alt="welding icon" class="icon" /> Welding & Fabrication</h2>
    <img src="images/welding-fabrication.jpg" alt="Steel Welding" class="section-image" />
    <ul class="details">
      <li>40×40×3 mm mild SHS</li>
      <li>3 mm steel plates per spec</li>
      <li>75×75×3 mm structural SHS</li>
      <li>Certified welders & machinery</li>
    </ul>
  </section>

  <section id="bending">
    <h2><img src="icons/rebar.svg" alt="rebar icon" class="icon" /> Bar Bending Schedule</h2>
    <img src="images/bar-bending.jpg" alt="Bar Bending Schedule" class="section-image" />
    <p>Precision bending schedules aligned with structural drawings for safe reinforcement.</p>
  </section>

  <section id="landscape">
    <h2><img src="icons/landscape.svg" alt="landscape icon" class="icon" /> Landscaping</h2>
    <img src="images/landscaping.jpg" alt="Garden Landscaping" class="section-image" />
    <p>Design and install lush gardens, walkways & irrigation for a sustainable outdoor space.</p>
  </section>

  <section id="painting">
    <h2><img src="icons/paint-roller.svg" alt="paint icon" class="icon" /> Painting</h2>
    <img src="images/painting.jpg" alt="Wall Painting" class="section-image" />
    <p>Durable, high-coverage finishes using ORCO & Dorcor for interior and exterior surfaces.</p>
  </section>

  <section id="drainage">
    <h2><img src="icons/drain.svg" alt="drain icon" class="icon" /> Drainage & Sanitation</h2>
    <img src="images/drainage-sanitation.jpg" alt="Drainage Pipes" class="section-image" />
    <p>Robust KENSPLASTIC/PVC piping and Gravena fittings for leak-proof, reliable drainage.</p>
  </section>

  <section id="carbo">
    <h2><img src="icons/paving.svg" alt="paving icon" class="icon" /> Carbo Paving</h2>
    <img src="images/carbo-paving.jpg" alt="Interlocking Pavers" class="section-image" />
    <p>Premium MasterPac interlocking pavers for driveways, patios, and pedestrian areas.</p>
  </section>

  <section id="plumbing">
    <h2><img src="icons/plumbing.svg" alt="plumbing icon" class="icon" /> Plumbing</h2>
    <img src="images/plumbing.jpg" alt="Plumbing Installation" class="section-image" />
    <p>Complete piping, fixtures, and water-management solutions for any project size.</p>
  </section>

  <section id="carpentry">
    <h2><img src="icons/woodwork.svg" alt="carpentry icon" class="icon" /> Carpentry</h2>
    <img src="images/carpentry.jpg" alt="Custom Carpentry" class="section-image" />
    <p>Custom woodwork, cabinetry and finish carpentry by Assinia Group & AGI craftsmen.</p>
  </section>

  <div class="contact">
    <a href="https://wa.me/254700557010" target="_blank" class="whatsapp-link">
      Chat on WhatsApp: 0700 557 010
    </a>
  </div>

  <script>
    const toggleBtn = document.querySelector('.nav-toggle');
    const nav = document.querySelector('nav.nav');

    toggleBtn.addEventListener('click', () => {
      nav.classList.toggle('active');
    });
  </script>
</body>
</html>
