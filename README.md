<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Stellah Wycliff - Portfolio</title>
  <style>
    :root {
      --primary-color: #006d77;
      --secondary-color: #83c5be;
      --accent-color: #ff6b6b;
      --background-color: #edf6f9;
      --text-color: #2f3e46;
    }

    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      margin: 0;
      padding: 0;
      background-color: var(--background-color);
      color: var(--text-color);
    }

    header {
      background-color: var(--primary-color);
      color: white;
      padding: 30px 0;
      text-align: center;
    }

    nav ul {
      list-style: none;
      padding: 0;
      margin: 10px 0;
    }

    nav ul li {
      display: inline;
      margin: 0 15px;
    }

    nav ul li a {
      color: white;
      text-decoration: none;
      font-weight: bold;
    }

    section {
      padding: 40px 20px;
      max-width: 900px;
      margin: auto;
      background-color: white;
      margin-bottom: 25px;
      border-radius: 10px;
      box-shadow: 0 3px 10px rgba(0, 0, 0, 0.05);
    }

    h2 {
      color: var(--primary-color);
      border-left: 6px solid var(--accent-color);
      padding-left: 10px;
    }

    ul {
      padding-left: 20px;
    }

    .project {
      background-color: var(--secondary-color);
      color: white;
      padding: 15px;
      border-left: 5px solid var(--accent-color);
      margin-bottom: 20px;
      border-radius: 5px;
    }

    form {
      display: grid;
      gap: 15px;
      max-width: 500px;
    }

    input, textarea {
      padding: 10px;
      font-size: 1em;
      width: 100%;
      border: 1px solid #ccc;
      border-radius: 4px;
    }

    button {
      background-color: var(--accent-color);
      color: white;
      border: none;
      padding: 10px;
      font-size: 1em;
      border-radius: 4px;
      cursor: pointer;
    }

    button:hover {
      background-color: #e05656;
    }

    footer {
      text-align: center;
      padding: 20px;
      background-color: var(--primary-color);
      color: white;
    }

    @media (max-width: 600px) {
      nav ul li {
        display: block;
        margin: 10px 0;
      }
    }
  </style>
</head>
<body>

  <!-- Header Section -->
  <header>
    <h1>Stellah Wycliff</h1>
    <p>Junior Data Analyst at KRA | Aspiring Software Engineer</p>
    <nav>
      <ul>
        <li><a href="#about">About</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#education">Education</a></li>
        <li><a href="#reviews">Review</a></li>
      </ul>
    </nav>
  </header>

  <!-- About Section -->
  <section id="about">
    <h2>About Me</h2>
    <p>
      Hello! I'm Stellah Wycliff, a Junior Data Analyst currently working at the Kenya Revenue Authority (KRA).
      I’m passionate about data and technology, and I’m currently sharpening my skills in software engineering with a focus on mobile app development under PowerLearnProject (PlP) Academy.
      My mission is to make sense of data and build digital solutions that improve lives.
    </p>
  </section>

  <!-- Skills Section -->
  <section id="skills">
    <h2>Skills</h2>
    <ul>
      <li>Python</li>
      <li>SQL</li>
      <li>Excel</li>
      <li>Power BI</li>
      <li>Tableau</li>
      <li>Data Cleaning, Analysis & Visualization</li>
      <li>Report Development & Dashboard Design</li>
    </ul>
  </section>

  <!-- Projects Section -->
  <section id="projects">
    <h2>Projects</h2>
    <div class="project">
      <h3>Electronic Waste Management at ICT Authority Kenya</h3>
      <p>
        I contributed by designing a dashboard to visualize the status of electronic devices at the E-Waste center—those received, repaired, and reused.
        Technologies used include Power BI, Excel, and Python.
        I was contributed in designing the E-waste Logo and manual which were adopted by the company and are in use up todate. This upskilled me in terms of graphic designing and documentation.
      </p>
    </div>
  </section>

  <!-- Education Section -->
  <section id="education">
    <h2>Education</h2>
    <p><strong>Bachelor's Degree in Mathematics and Computer Science</strong><br>Muranga University of Technology, 2016–2020</p>
    <p><strong>Professional Certificate in Software Engineeringtrong><br>XYZ University, 2025</p>
  </section>

  <!-- Review Section -->
  <section id="reviews">
    <h2>Leave a Review</h2>
    <form onsubmit="submitReview(event)">
      <label for="name">Your Name:</label>
      <input type="text" id="name" required>

      <label for="email">Your Email:</label>
      <input type="email" id="email" required>

      <label for="review">Your Review:</label>
      <textarea id="review" rows="4" required></textarea>

      <button type="submit">Submit Review</button>
    </form>
    <div id="review-msg" style="margin-top: 15px; color: green;"></div>
  </section>

  <!-- Footer -->
  <footer>
    &copy; 2025 Stellah Wycliff | All rights reserved.
  </footer>

  <!-- JavaScript -->
  <script>
    function submitReview(event) {
      event.preventDefault();
      const name = document.getElementById("name").value;
      document.getElementById("review-msg").textContent = `Thanks for your feedback, ${name}!`;

      // Clear form
      document.getElementById("name").value = "";
      document.getElementById("email").value = "";
      document.getElementById("review").value = "";
    }
  </script>
</body>
</html>
