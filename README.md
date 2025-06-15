# 2code
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>KINZA BATOOL Portfolio</title>
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
    <img src="data:image/jpeg;base64,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" alt="Profile Picture" class="profile-pic" /> 
    <h2 class="section-title">Welcome! I'm Kinza 👩‍💻</h2>
    <p style="text-align: center; max-width: 700px; margin: auto;">
    Hi! I’m a BS Data Science student and a Web Developer who loves building websites and working with data. I enjoy making clean and creative web pages using HTML, CSS, JavaScript, and React. At the same time, I’m learning how to understand and use data to solve real-life problems with tools like Python and machine learning.

I like mixing both my skills — design and logic — to create smart and user-friendly websites. My goal is to keep learning and build projects that are both useful and fun!
    </p>
    <p class="tagline">"Designing digital experiences that are clean, elegant, and efficient."</p>
    <div class="links" style="text-align:center;">
      <a href="https://github.com/KinzaBatool-coder" target="_blank">GitHub</a>
      <a href="https://www.linkedin.com/in/kinza-batool-95079a301?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app" target="_blank">LinkedIn</a>
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

      <!-- ✅ New Cartoon Animation Skill -->
      <div class="skill-card"><img src="https://cdn-icons-png.flaticon.com/512/3135/3135789.png" /><h4>Cartoon Animation</h4></div>
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

      <!-- ✅ New Cartoon Adventure Project -->
      <div class="project-card">
        <h4>Small Girl Adventure Cartoon</h4>
        <p>Created an engaging cartoon animation featuring a small girl on a jungle adventure using animation tools and web integration techniques. Designed characters, background, and movement logic.</p>
      </div>
    </div>

    <div class="buttons">
      <button onclick="showPage('intro')">⬅ Back to Introduction</button>
    </div>
  </section>

  <footer>
    &copy; 2025 Kinza Batool | Designed with ❤️ <br>
    📧 Personal Email: batool084@gmail.com | ☎ Contact: 03121306469 <br>
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
