# Day4-LeProject
Site like figma (the code is there take it if u want)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>eLearning CUTM</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Inter', sans-serif;
      background: #fff;
      color: #333;
    }
    header {
      position: fixed;
      width: 100%;
      top: 0;
      left: 0;
      z-index: 1000;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem 2rem;
      background: white;
      border-bottom: 1px solid #ddd;
    }
    nav a {
      margin: 0 0.75rem;
      text-decoration: none;
      color: #333;
      font-weight: 500;
      cursor: pointer;
    }
    .hero {
      margin-top: 80px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      background: linear-gradient(to right, #fef3c7, #d1fae5);
      padding: 3rem 2rem;
    }
    .hero h1 {
      font-size: 2.5rem;
      margin-bottom: 1rem;
    }
    .hero button {
      background: #f97316;
      border: none;
      padding: 0.75rem 1.5rem;
      color: white;
      font-size: 1rem;
      border-radius: 5px;
      cursor: pointer;
    }
    .categories {
      padding: 2rem;
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
      gap: 1.5rem;
    }
    .category-card {
      border: 1px solid #eee;
      border-radius: 10px;
      padding: 1rem;
      text-align: center;
      box-shadow: 0 1px 3px rgba(0,0,0,0.05);
    }
    .category-card img {
      width: 40px;
      height: 40px;
    }
    .footer {
      padding: 2rem;
      background: #f9fafb;
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
    }
    .footer div {
      margin: 1rem;
      min-width: 200px;
    }
    .container {
      max-width: 1200px;
      margin: 2rem auto;
      display: flex;
      gap: 2rem;
    }
    .sidebar {
      flex: 1;
    }
    .courses {
      flex: 3;
    }
    .course-card {
      display: flex;
      gap: 1rem;
      margin-bottom: 2rem;
      padding: 1rem;
      border: 1px solid #eee;
      border-radius: 10px;
      box-shadow: 0 2px 4px rgba(0,0,0,0.05);
    }
    .course-card img {
      width: 200px;
      border-radius: 8px;
    }
    .course-info h3 {
      margin: 0;
      font-size: 1.25rem;
    }
    .course-info p {
      margin: 0.5rem 0;
      color: #666;
    }
    .page {
      display: none;
    }
    .active {
      display: block;
    }
  </style>
</head>
<body>
  <header>
    <div><strong>📘 ELearning CUTM</strong></div>
    <nav>
      <a onclick="showPage('home')">Home</a>
      <a onclick="showPage('courses')">Courses</a>
      <a href="#">Blog</a>
      <a href="#">Pages</a>
      <a href="#">Login / Register</a>
    </nav>
  </header>

  <!-- PAGINA HOME -->
  <section id="home" class="page active">
    <section class="hero">
      <div>
        <h1>Build Skills With Online Course</h1>
        <p>Empower your future—one lesson at a time!</p>
        <button>Post Comment</button>
      </div>
      <img src="https://img.freepik.com/premium-photo/beautiful-student-girl-wearing-backpack-holding-notebook-isolated-white-background_264197-17092.jpg?w=360" alt="Hero Image" style="border-radius: 1rem;"/>
    </section>

    <section class="categories">
      <div class="category-card"><img src="https://img.icons8.com/fluency/48/000000/paint-palette.png"><div>Art & Design<br><small>69 Courses</small></div></div>
      <div class="category-card"><img src="https://img.icons8.com/fluency/48/000000/code.png"><div>Development<br><small>69 Courses</small></div></div>
      <div class="category-card"><img src="https://img.icons8.com/fluency/48/000000/conference-call.png"><div>Communication<br><small>69 Courses</small></div></div>
      <div class="category-card"><img src="https://img.icons8.com/fluency/48/000000/video-call.png"><div>Videography<br><small>69 Courses</small></div></div>
      <div class="category-card"><img src="https://img.icons8.com/fluency/48/000000/camera.png"><div>Photography<br><small>69 Courses</small></div></div>
      <div class="category-card"><img src="https://img.icons8.com/fluency/48/000000/marketing.png"><div>Marketing<br><small>69 Courses</small></div></div>
      <div class="category-card"><img src="https://img.icons8.com/fluency/48/000000/document.png"><div>Content Writing<br><small>69 Courses</small></div></div>
      <div class="category-card"><img src="https://img.icons8.com/fluency/48/000000/accounting.png"><div>Finance<br><small>69 Courses</small></div></div>
      <div class="category-card"><img src="https://img.icons8.com/fluency/48/000000/microscope.png"><div>Science<br><small>69 Courses</small></div></div>
      <div class="category-card"><img src="https://img.icons8.com/fluency/48/000000/network-card.png"><div>Network<br><small>69 Courses</small></div></div>
    </section>

    <footer class="footer">
      <div>
        <h4>ELearn CUTM</h4>
        <p>God is good!!!</p>
      </div>
      <div>
        <h4>GET HELP</h4>
        <p>Contact<br>FAQs<br>Support</p>
      </div>
      <div>
        <h4>PROGRAMS</h4>
        <p>Art & Design<br>Languages<br>IT & Software</p>
      </div>
      <div>
        <h4>CONTACT US</h4>
        <p>911 Street, City<br>+123 456 7890<br>email@911.com</p>
      </div>
    </footer>
  </section>

  <!-- PAGINA COURSES -->
  <section id="courses" class="page">
    <div class="container" style="margin-top: 100px;">
      <div class="sidebar">
        <h3>Filters</h3>
        <ul>
          <li>Photography (15)</li>
          <li>Art & Design (15)</li>
          <li>Marketing (15)</li>
        </ul>
      </div>

      <div class="courses">
        <h2>All Courses</h2>

        <div class="course-card">
          <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTDtCsOo_nSpeOLOc1MTE7n7mr7JoPBcafq2w&s" alt="Course 1">
          <div class="course-info">
            <h3>Create An LMS Website </h3>
            <p>2 Weeks · 30 Students · All Levels · 50 Lessons</p>
            <p style="color: green;"><strong>$50 Free</strong></p>
          </div>
        </div>

        <div class="course-card">
          <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ_fer_rs1GpVgSe82LQuE0XB-7FkoTDNw2xg&s" alt="Course 2">
          <div class="course-info">
            <h3>Create An HTML Website </h3>
            <p>2 Weeks · 15 Students · All Levels · 40 Lessons</p>
            <p style="color: green;"><strong>$30 Free</strong></p>
          </div>
        </div>

        <div class="course-card">
          <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTbDc7Ugp5YrYWh5n9ssqYZ-VkmnFRvgllhew&s" alt="Course 3">
          <div class="course-info">
            <h3>Create An Figma Project </h3>
            <p>2 Weeks · 45 Students · All Levels · 30 Lessons</p>
            <p style="color: green;"><strong>$20 Free</strong></p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <script>
    function showPage(id) {
      document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
      document.getElementById(id).classList.add('active');
    }
  </script>
</body>
</html>
