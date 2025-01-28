<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Portfolio</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, sans-serif;
    }

    .navbar {
      display: flex;
      justify-content: space-around;
      align-items: center;
      background-color: #11e747;
      padding: 1rem;
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    .navbar button {
      background-color: #03090b;
      color: #0fe1e8;
      border: none;
      padding: 1rem 1rem;
      border-radius: 1px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    .navbar button:hover {
      background-color: #7cbb1e;
    }

    .tab-content {
      display: none;
      padding: 4rem;
      text-align: center;
    }

    .tab-content.active {
      display: block;
    }

    .home-section {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 2rem;
    }

    .home-section img {
      width: 200px;
      height: 200px;
      border-radius: 50%;
      object-fit: cover;
    }

    .home-section p {
      font-size: 1.2rem;
      max-width: 600px;
    }
  </style>
</head>
<body>
  <div class="navbar">
    <button onclick="showTab('home')">Home</button>
    <button onclick="showTab('about')">About Me</button>
    <button onclick="showTab('skills')">Skills</button>
    <button onclick="showTab('achievements')">Achievements</button>
    <button onclick="showTab('contact')">Contact</button>
  </div>

  <div id="home" class="tab-content active">
    <div class="home-section">
      <h1>Welcome to My Portfolio</h1>
      <img src="Jaanu img.jpg" >
      <p>Hello! I am jahnavi , a passionate developer with a all round knowledge. Welcome to my portfolio where you can explore my skills, achievements, and get to know me better!</p>
    </div>
  </div>

  <div id="about" class="tab-content">
    <h2>About Me</h2>
    <p>This section contains information about me.</p>
    <p> i am a b.tech student from khit institute and i completed compoter science degree</p>
    <p> my age is 21</p>
    <p> i want to work as a software dveloper</p>
  </div>

  <div id="skills" class="tab-content">
    <h2>Skills</h2>
    <p>Here are some of my technical skills.</p>
    <p> i am a full stack developer</p>
    <p> i am a skilled python programmer</p>
  </div>

  <div id="achievements" class="tab-content">
    <h2>Achievements</h2>
    <p>Here are my achievements.</p>
    <p>i am an ethical hacker from anonymous group</p>

  </div>

  <div id="contact" class="tab-content">
    <h2>Contact</h2>
    <p>Feel free to get in touch!</p>
    <p>mobile no: 9391545519</p>
    <p>gmail id:218x1a0510@khitguntur.ac.in</p>
  </div>

  <script>
    function showTab(tabId) {
      const tabs = document.querySelectorAll('.tab-content');
      tabs.forEach(tab => tab.classList.remove('active'));
      document.getElementById(tabId).classList.add('active');
    }
  </script>
</body>
</html>
