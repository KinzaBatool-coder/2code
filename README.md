# 2code
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Kinza Batool Portfolio</title>
  <style>
    * {margin: 0; padding: 0; box-sizing: border-box; scroll-behavior: smooth;}
    body {font-family: 'Segoe UI', sans-serif; background: #f0f4f8; color: #2c3e50;}
    header {background: #34495e; color: #ecf0f1; padding: 1.5rem; text-align: center; position: sticky; top: 0; z-index: 1000;}
    nav a {color: #ecf0f1; margin: 0 15px; text-decoration: none; font-weight: 500; transition: color 0.3s;}
    nav a:hover {color: #f39c12;}
    section {padding: 3rem 1rem; max-width: 1100px; margin: auto; display: none;}
    section.active {display: block;}
    .profile-pic {width: 150px; border-radius: 50%; display: block; margin: 1.5rem auto; border: 3px solid #34495e;}
    .tagline {font-style: italic; color: #7f8c8d; margin: 1rem 0; text-align: center;}
    .links a {display: inline-block; margin: 0.5rem 10px; color: #2980b9; text-decoration: none; font-weight: 500;}
    .section-title {text-align: center; font-size: 2.2rem; margin-bottom: 2rem; color: #2c3e50;}
    .skills-container {display: flex; flex-wrap: wrap; gap: 1rem; justify-content: center;}
    .skill-card {background: white; border-radius: 12px; box-shadow: 0 2px 10px rgba(0,0,0,0.1); padding: 1rem; width: 200px; text-align: center; transition: transform 0.3s;}
    .skill-card:hover {transform: translateY(-5px);}
    .skill-card img {width: 50px; height: 50px; margin-bottom: 10px;}
    .projects-container {display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 1.5rem;}
    .project-card {background: white; padding: 1.5rem; border-radius: 12px; box-shadow: 0 0 10px rgba(0,0,0,0.1); transition: transform 0.3s;}
    .project-card:hover {transform: translateY(-5px);}
    .project-card h4 {margin-bottom: 0.5rem; color: #2980b9;}
    .project-card p {font-size: 0.95rem; color: #555;}
    .buttons {text-align: center; margin-top: 2rem;}
    button {padding: 10px 20px; font-size: 16px; border: none; background: #2980b9; color: white; cursor: pointer; border-radius: 5px; margin: 5px; transition: background 0.3s;}
    button:hover {background: #1f6391;}
    footer {text-align: center; padding: 1.5rem; background: #34495e; color: #ecf0f1; margin-top: 3rem; font-size: 0.9rem;}
    @media (max-width: 600px) {.skills-container {flex-direction: column; align-items: center;}}
  </style>
</head>
<body>
  <header>
    <h1>Kinza Batool</h1>
    <nav>
      <a href="#" onclick="showPage('intro')">Introduction</a>
      <a href="#" onclick="showPage('skills')">Skills & Projects</a>
    </nav>
  </header>

  <section id="intro" class="active">
    <img src="mypic.jpg" alt="Profile Picture" class="profile-pic" />
    <h2 class="section-title">Welcome! I'm Kinza 👩‍💻</h2>
    <p style="text-align: center; max-width: 700px; margin: auto;">
      I am an enthusiastic Web Developer and a dedicated BS Data Science student. My journey revolves around transforming creative ideas into functional and elegant digital solutions. With a keen interest in front-end development and a growing knowledge of back-end technologies, I strive to build user-friendly, accessible, and modern web applications.
    </p>
    <p class="tagline">"Designing digital experiences that are clean, elegant, and efficient."</p>
    <div class="links" style="text-align:center;">
      <a href="https://github.com/Muqadas-g" target="_blank">GitHub</a>
      <a href="https://www.linkedin.com/in/kinza-batool-95079a301?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app target="_blank">LinkedIn</a>
    </div>
    <div class="buttons">
      <button onclick="showPage('skills')">➡ Go to Skills & Projects</button>
    </div>
  </section>

  <section id="skills">
    <h2 class="section-title">💻 Technical Skills</h2>
    <div class="skills-container">
      <div class="skill-card"><img src="https://cdn-icons-png.flaticon.com/512/732/732212.png"/><h4>HTML</h4></div>
      <div class="skill-card"><img src="https://cdn-icons-png.flaticon.com/512/732/732190.png"/><h4>CSS</h4></div>
      <div class="skill-card"><img src="https://cdn-icons-png.flaticon.com/512/5968/5968292.png"/><h4>JavaScript</h4></div>
      <div class="skill-card"><img src="https://cdn-icons-png.flaticon.com/512/1126/1126012.png"/><h4>React</h4></div>
      <div class="skill-card"><img src="https://cdn-icons-png.flaticon.com/512/5968/5968350.png"/><h4>Python</h4></div>
      <div class="skill-card"><img src="https://cdn-icons-png.flaticon.com/512/226/226777.png"/><h4>Java</h4></div>
      <div class="skill-card"><img src="https://cdn-icons-png.flaticon.com/512/6132/6132222.png"/><h4>C</h4></div>
      <div class="skill-card"><img src="https://cdn-icons-png.flaticon.com/512/2772/2772128.png"/><h4>MySQL</h4></div>
    </div>

    <h2 class="section-title" style="margin-top: 3rem;">🚀 Projects Showcase</h2>
    <div class="projects-container">
      <div class="project-card">
        <h4>Fitness Gym</h4>
        <p>Developed a Gym e-commerce site using HTML and CSS, featuring a clean dark mode interface to improve the user browsing experience.</p>
      </div>
      <div class="project-card">
        <h4>Portfolio Website</h4>
        <p>A responsive and elegant personal portfolio designed to showcase technical skills and remote internship work in a professional layout.</p>
      </div>
    </div>
    <div class="buttons">
      <button onclick="showPage('intro')">⬅ Back to Introduction</button>
    </div>
  </section>

  <footer>
    &copy; 2025 Kinza Batool | Designed with ❤️ <br>
    📧 Personal Email: batool084@gmail.com | ☎ Contact: 0311-3014709 <br>
    💼 Remote Intern @ CoreTech Innovations <br>
    📩 Internship Email: hr@coretechio.com | ☎ HR: 0309-1800187
  </footer>

  <script>
    function showPage(pageId) {
      document.querySelectorAll('section').forEach(section => {
        section.classList.remove('active');
      });
      document.getElementById(pageId).classList.add('active');
    }
  </script>
</body>
</html>
