# Tailwind-CSS.Project

✅ Folder Structure (Recommended):

portfolio/
│
├── index.html
├── /images/
│   └── avatar.png (or use placeholder from online)
├── /pages/
│   └── optional sub-pages if needed
└── /README.md


---

✅ index.html Template

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Your Name | Portfolio</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <!-- Optional: Heroicons -->
  <script src="https://unpkg.com/feather-icons"></script>
</head>
<body class="bg-white text-gray-800 scroll-smooth">

  <!-- Navbar -->
  <header class="bg-gray-100 shadow-md sticky top-0 z-50">
    <nav class="max-w-6xl mx-auto flex justify-between items-center p-4">
      <div class="text-xl font-bold">Your Name</div>
      <ul class="flex space-x-6 font-medium">
        <li><a href="#home" class="hover:text-blue-500">Home</a></li>
        <li><a href="#about" class="hover:text-blue-500">About</a></li>
        <li><a href="#projects" class="hover:text-blue-500">Projects</a></li>
        <li><a href="#contact" class="hover:text-blue-500">Contact</a></li>
      </ul>
    </nav>
  </header>

  <!-- Home Section -->
  <section id="home" class="min-h-screen flex flex-col justify-center items-center bg-gray-50 text-center px-4">
    <img src="/images/avatar.png" alt="Profile Picture" class="w-32 h-32 rounded-full mb-4" />
    <h1 class="text-4xl font-bold">Hi, I'm Your Name</h1>
    <p class="text-xl mt-2 text-blue-600">Web Developer & Designer</p>
    <p class="mt-4 italic text-gray-600">"Designing the web, one line at a time."</p>
    <a href="/your_resume.pdf" download class="mt-6 inline-block bg-blue-600 text-white px-6 py-2 rounded-lg hover:bg-blue-700 transition">
      Download Resume
    </a>
  </section>

  <!-- About Me Section -->
  <section id="about" class="py-16 bg-white px-4 max-w-5xl mx-auto">
    <h2 class="text-3xl font-bold text-center mb-8">About Me</h2>
    <div class="grid md:grid-cols-2 gap-8">
      <div>
        <p class="mb-4">I am a passionate front-end developer with a love for clean code, responsive design, and user-friendly web interfaces. My goal is to build efficient and elegant websites that solve real problems.</p>
        <p>I enjoy learning new technologies and constantly improving my skills.</p>
      </div>
      <div>
        <h3 class="text-xl font-semibold mb-2">Skills</h3>
        <ul class="list-disc list-inside space-y-1">
          <li>HTML</li>
          <li>CSS & Tailwind CSS</li>
          <li>JavaScript</li>
          <li>Git & GitHub</li>
        </ul>
        <h3 class="text-xl font-semibold mt-6 mb-2">Education</h3>
        <ul class="space-y-2">
          <li><strong>B.Sc. Computer Science</strong> – XYZ University (2020–2023)</li>
          <li><strong>Web Development Bootcamp</strong> – Online Course (2023)</li>
        </ul>
      </div>
    </div>
  </section>

  <!-- Projects Section -->
  <section id="projects" class="py-16 bg-gray-50 px-4 max-w-6xl mx-auto">
    <h2 class="text-3xl font-bold text-center mb-10">Projects</h2>
    <div class="grid md:grid-cols-3 gap-6">
      <!-- Project Card -->
      <div class="bg-white p-4 rounded-lg shadow hover:shadow-lg hover:scale-105 transition">
        <img src="https://via.placeholder.com/300x200" alt="Project Screenshot" class="rounded mb-4" />
        <h3 class="text-xl font-semibold">Project One</h3>
        <p class="text-sm text-gray-600 mb-2">A responsive website for showcasing portfolios. Built using HTML, Tailwind, and JS.</p>
        <a href="https://github.com/your/project1" target="_blank" class="text-blue-600 text-sm">View on GitHub</a>
      </div>
      <!-- Repeat for other projects -->
      <div class="bg-white p-4 rounded-lg shadow hover:shadow-lg hover:scale-105 transition">
        <img src="https://via.placeholder.com/300x200" alt="Project Screenshot" class="rounded mb-4" />
        <h3 class="text-xl font-semibold">Project Two</h3>
        <p class="text-sm text-gray-600 mb-2">An interactive to-do app with local storage support. Built using vanilla JavaScript.</p>
        <a href="https://github.com/your/project2" target="_blank" class="text-blue-600 text-sm">View on GitHub</a>
      </div>
      <div class="bg-white p-4 rounded-lg shadow hover:shadow-lg hover:scale-105 transition">
        <img src="https://via.placeholder.com/300x200" alt="Project Screenshot" class="rounded mb-4" />
        <h3 class="text-xl font-semibold">Project Three</h3>
        <p class="text-sm text-gray-600 mb-2">Fake News Detection web app using ML model. Built with Python & Gradio frontend.</p>
        <a href="https://github.com/your/project3" target="_blank" class="text-blue-600 text-sm">View on GitHub</a>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="py-16 bg-white px-4 max-w-xl mx-auto">
    <h2 class="text-3xl font-bold text-center mb-8">Contact Me</h2>
    <form class="space-y-4">
      <input type="text" placeholder="Your Name" class="w-full border border-gray-300 rounded p-2 focus:outline-none focus:ring-2 focus:ring-blue-500" required />
      <input type="email" placeholder="Your Email" class="w-full border border-gray-300 rounded p-2 focus:outline-none focus:ring-2 focus:ring-blue-500" required />
      <textarea placeholder="Your Message" rows="5" class="w-full border border-gray-300 rounded p-2 focus:outline-none focus:ring-2 focus:ring-blue-500" required></textarea>
      <button type="submit" class="bg-blue-600 text-white px-6 py-2 rounded hover:bg-blue-700 transition">Send</button>
    </form>
    <!-- Optional: Social Media -->
    <div class="flex justify-center mt-6 space-x-4">
      <a href="#"><i data-feather="linkedin"></i></a>
      <a href="#"><i data-feather="github"></i></a>
      <a href="#"><i data-feather="twitter"></i></a>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-gray-100 text-center py-4 text-sm text-gray-500">
    &copy; 2025 Your Name. All rights reserved.
  </footer>

  <script>feather.replace()</script>
</body>
</html>


---

✅ README.md (Short Experience Paragraph)

# My Portfolio Website

This project is a personal portfolio website built using only **HTML and Tailwind CSS**. It includes fully responsive sections such as Home, About Me, Projects, and Contact. I learned how to effectively use Tailwind’s utility classes, responsive grids, and layout components. I also gained a better understanding of structuring HTML semantically and making the site mobile-friendly. Overall, this project helped strengthen my front-end development and design skills.




