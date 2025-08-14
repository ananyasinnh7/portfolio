# portfolio
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Ananya Singh — Portfolio</title>
  <meta name="description" content="Ananya Singh | CSE student | Future Fighter Pilot | Projects, skills, certifications, and contact." />

  <!-- Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Caveat:wght@600;700&family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">

  <!-- AOS Animation -->
  <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">

  <style>
    :root{
      --bg-start:#0a1022; /* deep navy */
      --bg-end:#00040a;   /* near-black */
      --ink:#ffffff;      /* white text */
      --ink-dim:#cfd6ff;  /* soft white-blue */
      --accent:#4ea8ff;   /* soft blue accent */
      --card:#0f1a33aa;   /* translucent navy */
      --glow:0 0 20px rgba(78,168,255,.4);
      --radius:16px;
      --shadow:0 12px 30px rgba(0,0,0,.35);
    }
    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{
      margin:0;
      color:var(--ink);
      background:linear-gradient(160deg, var(--bg-start), var(--bg-end));
      font-family:Inter, sans-serif;
      line-height:1.6;
    }
    .wrap{max-width:1100px; margin:auto; padding:0 20px}

    /* Navbar */
    nav{
      position:sticky; top:0; z-index:50;
      background:rgba(10,16,34,0.9);
      backdrop-filter:blur(10px);
    }
    nav .nav-inner{
      display:flex; justify-content:space-between; align-items:center;
      padding:12px 0;
    }
    nav .brand{
      font-family:Caveat, cursive; font-size:28px; font-weight:700;
    }
    nav .menu a{
      color:var(--ink); text-decoration:none;
      margin-left:18px;
    }
    nav .menu a:hover{
      color:var(--accent);
    }

    section{padding:80px 0}
    h2{
      font-family:Caveat, cursive;
      font-size:36px;
      margin-bottom:30px;
      text-align:center;
    }
    p{color:var(--ink-dim)}

    /* Typing effect */
    .typing{
      border-right: 2px solid var(--accent);
      white-space: nowrap;
      overflow: hidden;
      animation: typing 4s steps(30, end), blink 0.8s infinite;
      width: fit-content;
      margin:auto;
      font-size:20px;
    }
    @keyframes typing{
      from { width: 0 }
      to { width: 100% }
    }
    @keyframes blink{
      50% { border-color: transparent }
    }

    /* Cards */
    .cards{
      display:grid; grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
      gap:20px;
    }
    .card{
      background:var(--card);
      padding:20px;
      border-radius:var(--radius);
      box-shadow:var(--shadow);
      transition:transform .3s, box-shadow .3s;
    }
    .card:hover{
      transform:translateY(-5px);
      box-shadow:var(--glow);
    }
    .card h3{
      font-family:Caveat, cursive; font-size:24px;
    }

    /* Contact form */
    form{
      display:flex; flex-direction:column;
      gap:12px;
      max-width:500px; margin:auto;
    }
    input, textarea{
      padding:10px; border:none; border-radius:var(--radius);
      font-family:inherit;
    }
    button{
      background:var(--accent); color:#000;
      padding:10px; border:none;
      font-weight:600; border-radius:var(--radius);
      cursor:pointer;
    }
    button:hover{background:#6cbaff}
  </style>
</head>
<body>

<!-- Navbar -->
<nav>
  <div class="wrap nav-inner">
    <div class="brand">Ananya Singh</div>
    <div class="menu">
      <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#skills">Skills</a>
      <a href="#projects">Projects</a>
      <a href="#achievements">Achievements</a>
      <a href="#contact">Contact</a>
    </div>
  </div>
</nav>

<!-- Home -->
<section id="home">
  <div class="wrap" style="text-align:center">
    <h1 data-aos="fade-up">Hi, I'm Ananya Singh</h1>
    <div class="typing">CSE Student | Future Fighter Pilot | Tech Enthusiast</div>
  </div>
</section>

<!-- About -->
<section id="about">
  <div class="wrap">
    <h2 data-aos="fade-up">About Me</h2>
    <p data-aos="fade-up">
      Driven and passionate Computer Science Engineering student aspiring to serve as a Fighter Pilot one day, while leveraging technology and innovation to contribute meaningfully to society. Strong believer in using skills to make a positive impact on people's lives.
    </p>
  </div>
</section>

<!-- Skills -->
<section id="skills">
  <div class="wrap">
    <h2 data-aos="fade-up">Skills</h2>
    <div class="cards">
      <div class="card" data-aos="zoom-in">
        <h3>Programming Languages</h3>
        <p>Python, Java, C, C++</p>
      </div>
      <div class="card" data-aos="zoom-in">
        <h3>Core Areas</h3>
        <p>Data Structures & Algorithms, AI/ML, Project Management, Finance</p>
      </div>
      <div class="card" data-aos="zoom-in">
        <h3>Tools & Platforms</h3>
        <p>GitHub, Arduino, AWS Basics</p>
      </div>
    </div>
  </div>
</section>

<!-- Projects -->
<section id="projects">
  <div class="wrap">
    <h2 data-aos="fade-up">Projects</h2>
    <div class="cards">
      <div class="card" data-aos="flip-left">
        <h3>Bachpan Ki Muskaan</h3>
        <p>Social Impact Platform fostering unity in diversity across India, connecting people beyond language and cultural barriers.</p>
      </div>
      <div class="card" data-aos="flip-left">
        <h3>Food Truck Management System</h3>
        <p>End-to-end business plan with documentation, website, budget planning, timeline, and GitHub integration.</p>
      </div>
      <div class="card" data-aos="flip-left">
        <h3>Door Lock Security System</h3>
        <p>Arduino-based smart door lock with RFID authentication for enhanced security.</p>
      </div>
    </div>
  </div>
</section>

<!-- Achievements -->
<section id="achievements">
  <div class="wrap">
    <h2 data-aos="fade-up">Achievements & Activities</h2>
    <ul data-aos="fade-up">
      <li>Member of College Basketball Team</li>
      <li>Actively involved in community and social work initiatives</li>
      <li>Contributed to team-based projects and hackathons</li>
    </ul>
  </div>
</section>

<!-- Contact -->
<section id="contact">
  <div class="wrap">
    <h2 data-aos="fade-up">Contact Me</h2>
    <form id="contact-form" data-aos="fade-up">
      <input type="text" name="name" placeholder="Your Name" required />
      <input type="email" name="email" placeholder="Your Email" required />
      <textarea name="message" placeholder="Your Message" rows="5" required></textarea>
      <button type="submit">Send Message</button>
    </form>
    <p style="text-align:center;margin-top:20px;">
      <a href="https://www.linkedin.com/in/ananya-singh-b1b740294" target="_blank" style="color:var(--accent)">LinkedIn</a> |
      <a href="https://github.com/" target="_blank" style="color:var(--accent)">GitHub</a> |
      <a href="Ananya_Singh_Resume.pdf" style="color:var(--accent)">Download CV</a>
    </p>
  </div>
</section>

<!-- Scripts -->
<script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
<script>
  AOS.init({ duration: 1000, once: true });
</script>

</body>
</html>
