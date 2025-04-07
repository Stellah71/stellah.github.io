<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Stellah Wycliff | Data Analyst & Software Engineer</title>
    <style>
        /* General styles */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            background-color: #f0f0f0;
        }
        header {
            background-color: #ff6f61;
            color: white;
            text-align: center;
            padding: 2em 0;
        }
        header h1 {
            margin: 0;
            font-size: 3em;
        }
        header p {
            font-size: 1.2em;
            margin: 0.5em 0;
        }
        nav {
            position: sticky;
            top: 0;
            background-color: #333;
            padding: 1em 0;
            text-align: center;
        }
        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
            font-size: 1.2em;
        }
        nav a:hover {
            text-decoration: underline;
        }

        /* Section styles */
        section {
            padding: 4em 2em;
            margin: 2em 0;
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        section h2 {
            font-size: 2.5em;
            color: #333;
        }
        section p {
            font-size: 1.2em;
            color: #555;
            line-height: 1.6;
        }

        /* About Me Section */
        #about {
            background-color: #ffebcd;
        }

        /* Projects Section */
        #projects {
            background-color: #ffdfba;
        }

        /* Contact Section */
        #contact {
            background-color: #e6f7ff;
        }

        /* Smooth Scroll and Fade-in */
        a[href^="#"] {
            transition: color 0.3s;
        }
        a[href^="#"]:hover {
            color: #ff6f61;
        }

        /* Fade-in effect for sections */
        .fade-in {
            opacity: 0;
            transition: opacity 1s ease-out;
        }

        .fade-in.visible {
            opacity: 1;
        }

        /* Media Queries */
        @media (max-width: 768px) {
            header h1 {
                font-size: 2.5em;
            }
            header p {
                font-size: 1em;
            }
            nav a {
                font-size: 1em;
            }
        }
    </style>
</head>
<body>

    <!-- Header -->
    <header>
        <h1>Stellah Wycliff</h1>
        <p>Data Analyst & Aspiring Software Engineer</p>
    </header>

    <!-- Navigation -->
    <nav>
        <a href="#about">About</a>
        <a href="#projects">Projects</a>
        <a href="#contact">Contact</a>
    </nav>

    <!-- About Section -->
    <section id="about" class="fade-in">
        <h2>About Me</h2>
        <p>Hi! I'm Stellah Wycliff, a professional Data Analyst and aspiring Software Engineer specializing in mobile app development. I'm passionate about using data to drive decisions and building solutions that make a difference. I have experience in data manipulation, analysis, visualization, and reporting findings effectively.</p>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="fade-in">
        <h2>Projects</h2>
        <h3>Electronic Waste Management Dashboard</h3>
        <p>As part of the ICT Authority Kenya's Electronic Waste Management project, I designed a dashboard that visualized the devices received at the E-Waste centre, including those that have been repaired and those reused. The dashboard was used to provide insights to stakeholders on the project’s progress.</p>
        <p><strong>Technologies Used:</strong> Power BI, Excel, Python</p>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="fade-in">
        <h2>Contact</h2>
        <p>You can reach me by email at <a href="mailto:stellahdaniel71@gmail.com">stellahdaniel71@gmail.com</a>.</p>
    </section>

    <script>
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Scroll animations for sections
        window.addEventListener('scroll', () => {
            const sections = document.querySelectorAll('.fade-in');
            sections.forEach(section => {
                const rect = section.getBoundingClientRect();
                if (rect.top >= 0 && rect.bottom <= window.innerHeight) {
                    section.classList.add('visible');
                }
            });
        });
    </script>
</body>
</html>
