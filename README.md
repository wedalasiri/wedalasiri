
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <title>Wed Alasiri | Portfolio</title>

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

  <link
    href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap"
    rel="stylesheet"
  >

  <style>

    :root {
      --bg: #0f0f12;
      --card: #1a1b20;
      --muted: #9aa0a6;
      --text: #ffffff;
      --primary: #1da1f2;
      --radius: 20px;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: 'Inter', sans-serif;
      background: var(--bg);
      color: var(--text);
    }

    .container {
      max-width: 1200px;
      margin: auto;
      padding: 40px 20px;
      display: grid;
      gap: 24px;
    }

    .grid {
      display: grid;
      gap: 24px;
    }

    .grid-2 {
      grid-template-columns: 2fr 1fr;
    }

    .grid-3 {
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    }

    .card {
      background: var(--card);
      border-radius: var(--radius);
      padding: 24px;
    }

    h1,
    h2,
    h3 {
      margin: 0 0 12px;
    }

    p,
    li {
      color: var(--muted);
      line-height: 1.6;
    }

    ul {
      padding-left: 18px;
      margin: 0;
    }

    /* PROFILE IMAGE */

    .avatar img {
      max-width: 200px;
      width: 100%;
      height: auto;
      border-radius: 0;
      display: block;
    }

    /* BUTTONS */

    .contact-btn {
      background: var(--primary);
      border: none;
      color: #fff;
      padding: 10px 16px;
      border-radius: 999px;
      cursor: pointer;
      font-weight: 600;
      text-decoration: none;
      display: inline-block;
    }

    .contact-btn:hover {
      opacity: 0.85;
    }

    /* ICON CARDS */

    .icon-card {
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 40px;
    }

    /* HERO */

    .hero-text {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: flex-start;
      text-align: left;
    }

    .section-title {
      margin-bottom: 18px;
    }

    /* =========================================
       PROJECTS
    ========================================= */

    /* =========================================
   PROJECTS
========================================= */

.projects {
  align-items: stretch;
}

.project-card {
  background: #1a1b20;
  border-radius: 20px;
  padding: 16px;

  display: flex;
  flex-direction: column;

  gap: 12px;

  height: 100%;
}

/* ALL APP / PROJECT IMAGES — EXACT SAME SIZE */

.projects img {
  width: 100%;
  aspect-ratio: 1 / 1;
  height: auto;
  object-fit: contain;
  border-radius: 14px;
  margin-bottom: 4px;
  display: block;
  background: transparent;
  flex-shrink: 0;
}

.project-card h3 {
  margin: 0;
}

.project-card p {
  margin: 0;
}
    /* TAGS */

    .tags {
      margin-top: 4px;
    }

    .tags span {
      display: inline-block;

      background: #2a2b31;

      padding: 6px 10px;

      border-radius: 999px;

      font-size: 12px;

      margin: 6px 6px 0 0;

      color: #d8d8d8;
    }

    /* PROJECT BUTTONS */

    .project-links {
      display: flex;
      flex-wrap: wrap;

      gap: 8px;

      margin-top: auto;

      padding-top: 4px;
    }

    .project-btn {
      background: var(--primary);

      color: white;

      text-decoration: none;

      padding: 8px 13px;

      border-radius: 999px;

      font-size: 13px;

      font-weight: 600;

      display: inline-block;
    }

    .project-btn.secondary {
      background: #2a2b31;
    }

    .project-btn:hover {
      opacity: 0.85;
    }

    /* =========================================
       EXPERIENCE
    ========================================= */

    .experience-item {
      padding: 18px 0;

      border-bottom: 1px solid #2a2b31;
    }

    .experience-item:last-child {
      border-bottom: none;
    }

    .experience-title {
      font-size: 18px;

      font-weight: 600;

      margin-bottom: 5px;
    }

    .experience-date {
      color: var(--primary);

      font-size: 13px;

      margin-bottom: 12px;
    }

    /* =========================================
       EDUCATION
    ========================================= */

    .education-list {
      display: grid;

      gap: 14px;
    }

    .education-item {
      background: #202126;

      border-radius: 14px;

      padding: 18px;

      display: flex;

      align-items: center;

      gap: 18px;
    }

    /* EDUCATION LOGO BOX */

    .education-logo {
      width: 80px;

      height: 80px;

      min-width: 80px;

      background: #ffffff;

      border-radius: 14px;

      display: flex;

      align-items: center;

      justify-content: center;

      overflow: hidden;
    }

    /* ALL EDUCATION LOGOS SAME SIZE */

    .education-logo img {
      width: 70px;

      height: 70px;

      object-fit: contain;

      display: block;
    }

    .education-info {
      flex: 1;
    }

    .education-info h3 {
      margin: 0 0 6px;
    }

    .education-date {
      color: var(--primary);

      font-size: 13px;
    }

    /* =========================================
       SKILLS
    ========================================= */

    .skill-group {
      margin-bottom: 18px;
    }

    .skill-group:last-child {
      margin-bottom: 0;
    }

    .skill-group h4 {
      margin: 0 0 8px;

      font-size: 15px;
    }

    /* =========================================
       LANGUAGE BUTTON
    ========================================= */

    .lang-btn {
      position: fixed;

      top: 20px;

      right: 20px;

      background: #2a2b31;

      color: #fff;

      border: none;

      padding: 8px 14px;

      border-radius: 999px;

      cursor: pointer;

      font-weight: 600;

      z-index: 999;
    }

    .lang-btn:hover {
      background: #3a3b42;
    }

    /* =========================================
       FOOTER
    ========================================= */

    footer {
      text-align: center;

      color: var(--muted);

      font-size: 14px;

      margin-top: 40px;
    }

    /* =========================================
       MOBILE
    ========================================= */

    @media (max-width: 700px) {

      .grid-2 {
        grid-template-columns: 1fr;
      }

      .container {
        padding: 25px 15px;
      }

      .avatar img {
        max-width: 150px;
      }

      h1 {
        font-size: 30px;
      }

      .education-item {
        align-items: flex-start;
      }

      .education-logo {
        width: 70px;
        height: 70px;
        min-width: 70px;
      }

      .education-logo img {
        width: 60px;
        height: 60px;
      }

      .projects img {
        height: 200px;
      }

    }

  </style>
</head>

<body>

  <button id="langToggle" class="lang-btn">
    AR
  </button>


  <main class="container">


    <!-- =========================
         HERO
    ========================== -->

    <section class="grid grid-2">

      <div class="card hero-text">

        <h1>
          HI, I’m Wed Alasiri
        </h1>

        <p>
          Software Engineer | Cybersecurity | iOS Developer
        </p>

        <p>
         Two years of hands-on experience gained through real-world projects, industry internships, and specialized training in software engineering, iOS development, and cybersecurity. Focused on building secure, scalable, and user-focused software.

        </p>

      </div>


      <div
        class="card"
        style="display:flex;justify-content:center;align-items:center"
      >

        <div class="avatar">

          <img
            src="images/wed.png"
            alt="Wed Alasiri"
          >

        </div>

      </div>

    </section>


    <!-- =========================
         CONTACT
    ========================== -->

    <section class="grid grid-3">


      <div class="card">

        <h3>
          Contact
        </h3>

        <p>
          Email: wed.alasiri2025@gmail.com
        </p>

        <p>
          Phone: +966 55 208 5766
        </p>

        <button
          class="contact-btn"
          onclick="window.location.href='mailto:wed.alasiri2025@gmail.com'"
        >
          Send an Email
        </button>

        <button
          class="contact-btn"
          style="margin-top:12px;background:#2a2b31"
          onclick="window.open('cv/Wed-Alasiri-CV.pdf','_blank')"
        >
          View My CV
        </button>

      </div>


      <!-- LINKEDIN -->

      <div
        class="card icon-card"
        style="flex-direction:column;cursor:pointer"
        onclick="window.open('https://www.linkedin.com/in/wed-alasiri-15ba242ab/','_blank')"
      >

        <img
          src="images/linkedin.png"
          alt="LinkedIn"
          style="width:64px;height:64px;margin-bottom:10px;"
        >

        <span
          style="color:var(--muted);font-size:14px"
        >
          Click to visit LinkedIn
        </span>

      </div>


      <!-- GITHUB -->

      <div
        class="card icon-card"
        style="flex-direction:column;cursor:pointer"
        onclick="window.open('https://github.com/wedalasiri/Wed-Ahmed-Alasiri','_blank')"
      >

        <img
          src="images/github.png"
          alt="GitHub"
          style="width:64px;height:64px;margin-bottom:10px;"
        >

        <span
          style="color:var(--muted);font-size:14px"
        >
          Click to visit GitHub
        </span>

      </div>

    </section>


    <!-- =========================
         ABOUT
    ========================== -->

    <section class="card">

      <h2>
        ABOUT ME
      </h2>

      <p>
        Software Engineer with practical experience building
        production-ready applications and AI-powered solutions
        through industry internships and real-world projects.
      </p>

      <p>
        Experienced in software development, application architecture,
        clean coding practices, and modern development methodologies,
        with a strong focus on delivering scalable, secure, and
        high-quality solutions.
      </p>

      <p>
        Complemented by hands-on cybersecurity experience in network
        security, vulnerability assessment, threat analysis,
        penetration testing, secure software development, and
        risk management.
      </p>

      <p>
        Continuously expanding expertise in cloud technologies and
        DevOps, including IaaS and PaaS, with a focus on integrating
        security throughout the software development lifecycle.
      </p>

    </section>


    <!-- =========================
         SKILLS
    ========================== -->

    <section class="card">

      <h2 class="section-title">
        SKILLS
      </h2>

      <div class="grid grid-2">


        <!-- CYBERSECURITY -->

        <div>

          <div class="skill-group">

            <h4>
              Cybersecurity
            </h4>

            <div class="tags">

              <span>Penetration Testing</span>
              <span>Vulnerability Assessment</span>
              <span>Threat Analysis</span>
              <span>Risk Assessment</span>
              <span>Network Security</span>
              <span>Application Security</span>
              <span>Secure Software Development</span>
              <span>Secure SDLC</span>
              <span>Incident Response</span>
              <span>Cryptography</span>

            </div>

          </div>


          <div class="skill-group">

            <h4>
              Network & Infrastructure
            </h4>

            <div class="tags">

              <span>TCP/IP</span>
              <span>DNS</span>
              <span>DHCP</span>
              <span>VPN</span>
              <span>Firewall</span>
              <span>IDS</span>
              <span>ACL</span>

            </div>

          </div>


          <div class="skill-group">

            <h4>
              Security Tools
            </h4>

            <div class="tags">

              <span>Kali Linux</span>
              <span>Metasploit</span>
              <span>Burp Suite</span>
              <span>OWASP ZAP</span>
              <span>Wireshark</span>
              <span>Nmap</span>
              <span>Splunk</span>

            </div>

          </div>

        </div>


        <!-- SOFTWARE / AI -->

        <div>

          <div class="skill-group">

            <h4>
              iOS & Software Engineering
            </h4>

            <div class="tags">

              <span>SwiftUI</span>
              <span>UIKit</span>
              <span>MVVM</span>
              <span>MVC</span>
              <span>REST APIs</span>
              <span>JSON</span>
              <span>Core Data</span>
              <span>UserDefaults</span>
              <span>Firebase</span>
              <span>Xcode</span>
              <span>Git</span>
              <span>GitHub</span>
              <span>API Integration</span>
              <span>Debugging</span>
              <span>Testing</span>

            </div>

          </div>


          <div class="skill-group">

            <h4>
              AI & Machine Learning
            </h4>

            <div class="tags">

              <span>Machine Learning</span>
              <span>Artificial Intelligence</span>
              <span>NLP</span>
              <span>Generative AI</span>
              <span>Model Development</span>
              <span>AI API Integration</span>
              <span>Core ML</span>
              <span>Create ML</span>
              <span>Recommendation Systems</span>

            </div>

          </div>


          <div class="skill-group">

            <h4>
              Cloud & DevOps
            </h4>

            <div class="tags">

              <span>DevOps Fundamentals</span>
              <span>Cloud Computing</span>
              <span>IaaS</span>
              <span>PaaS</span>
              <span>Docker</span>
              <span>AWS</span>
              <span>CI/CD</span>

            </div>

          </div>

        </div>

      </div>

    </section>


    <!-- =========================
         EXPERIENCE
    ========================== -->

    <section class="card">

      <h2 class="section-title">
        PROFESSIONAL EXPERIENCE
      </h2>


      <!-- SAUDICO -->

      <div class="experience-item">

        <div class="experience-title">
          Cyber Security & Software Development Intern
        </div>

        <div class="experience-date">
          Saudi Constructioneers Ltd. (SAUDICO) |
          March 2026 – June 2026
        </div>

        <ul>

          <li>
            Developed and integrated an attendance management
            system into the company's internal platform,
            improving operational efficiency and data accuracy.
          </li>

          <li>
            Worked across mobile development, backend integration,
            and cybersecurity projects within an enterprise environment.
          </li>

          <li>
            Conducted penetration testing and vulnerability
            assessments on web applications and networks using
            industry-standard security tools.
          </li>

          <li>
            Deployed an Intrusion Detection System (IDS) to monitor
            network traffic and detect suspicious activities.
          </li>

          <li>
            Configured firewalls, Access Control Lists (ACLs),
            and Site-to-Site VPN to strengthen network security.
          </li>

          <li>
            Built and managed core network services including
            TCP/IP, DHCP, and DNS.
          </li>

        </ul>

      </div>


      <!-- MINISTRY -->

      <div class="experience-item">

        <div class="experience-title">
          Software Engineering Intern
        </div>

        <div class="experience-date">
          Ministry of Education |
          January 2024 – July 2024
        </div>

        <ul>

          <li>
            Designed and developed a web-based platform for
            managing professional development activities.
          </li>

          <li>
            Improved database organization and reporting efficiency
            through optimized data structures and backend enhancements.
          </li>

        </ul>

      </div>

    </section>


    <!-- =========================
         EDUCATION & TRAINING
    ========================== -->

    <section class="card">

      <h2 class="section-title">
        EDUCATION & TRAINING
      </h2>


      <div class="education-list">


        <!-- EDUCATION 1 -->

        <div class="education-item">

          <div class="education-logo">

            <img
              src="https://pbs.twimg.com/profile_images/1999827624323948546/AaCdOG0F_400x400.jpg"
              alt="Tuwaiq Academy"
            >

          </div>

          <div class="education-info">

            <h3>
              Tuwaiq Academy
            </h3>

            <span class="education-date">
              Apple Developer Academy
            </span>

          </div>

        </div>


        <!-- EDUCATION 2 -->

        <div class="education-item">

          <div class="education-logo">

            <img
              src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTokxh_N2kxKvytfwlcH0th_NB5Dz-TVLTZedbA4dZwjA&s=10"
              alt="Academy of Learning"
            >

          </div>

          <div class="education-info">

            <h3>
              Academy of Learning
            </h3>

            <span class="education-date">
              July 2026
            </span>

          </div>

        </div>


        <!-- EDUCATION 3 -->

        <div class="education-item">

          <div class="education-logo">

            <img
              src="https://media.licdn.com/dms/image/v2/C4D0BAQEFDFm_LmuT5Q/company-logo_200_200/company-logo_200_200/0/1630508390505?e=2147483647&v=beta&t=Lob8GnyJUbP_T_ZaV1c4SEsP5mXkh7Wi5p6lLqJvqtY"
              alt="Education Institution"
            >

          </div>

          <div class="education-info">

            <h3>
              Princess Nourah bint Abdulrahman University
            </h3>

            <span class="education-date">
              July 2024
            </span>

          </div>

        </div>


      </div>

    </section>


    <!-- =========================
         FEATURED PROJECTS
    ========================== -->

    <section class="card">

      <h2 class="section-title">
        FEATURED PROJECTS
      </h2>


      <div class="grid grid-3 projects">


        <!-- SAFETAP -->

        <div class="project-card">

          <img
            src="images/SafeTap.png"
            alt="SafeTap"
          >

          <h3>
            SafeTap
          </h3>

          <p>
            AI-powered fraud detection application that helps
            detect fraudulent calls and messages in real time
            and explains the risk to the user.
          </p>

          <div class="tags">

            <span>SwiftUI</span>
            <span>Core ML</span>
            <span>NLP</span>
            <span>Machine Learning</span>
            <span>Cybersecurity</span>

          </div>

          <div class="project-links">

            <a
              href="https://github.com/wedalasiri"
              target="_blank"
              class="project-btn secondary"
            >
              GitHub
            </a>

          </div>

        </div>


        <!-- JISR -->

        <div class="project-card">

          <img
            src="images/Jisr.png"
            alt="Jisr"
          >

          <h3>
            Jisr | Community Integration Platform
          </h3>

          <p>
            An iOS application that helps Saudi scholarship
            students connect with others through shared interests
            and community activities.
          </p>

          <div class="tags">

            <span>SwiftUI</span>
            <span>Firebase</span>
            <span>Core ML</span>
            <span>OpenAI API</span>
            <span>3D</span>

          </div>

          <div class="project-links">

            <a
              href="https://apps.apple.com/sa/app/jisr/id6776704071"
              target="_blank"
              class="project-btn"
            >
              App Store
            </a>

            <a
              href="https://github.com/wedalasiri"
              target="_blank"
              class="project-btn secondary"
            >
              GitHub
            </a>

          </div>

        </div>


        <!-- CLUE -->

        <div class="project-card">

          <img
            src="images/clue.png"
            alt="Clue"
          >

          <h3>
            Clue
          </h3>

          <p>
            A decision-making app with two modes:
            Wisely for guided decisions and Randomly for
            instant picks when you can't decide.
          </p>

          <div class="tags">

            <span>iOS</span>
            <span>Swift</span>
            <span>Team Project</span>

          </div>

        </div>


        <!-- PRONOUNCEME -->

        <div class="project-card">

          <img
            src="images/pronounce.png"
            alt="PronounceMe"
          >

          <h3>
            PronounceMe
          </h3>

          <p>
            An iOS application supporting individuals with
            Speech Sound Disorders through interactive
            speech exercises and continuous practice.
          </p>

          <div class="tags">

            <span>iOS</span>
            <span>Swift</span>
            <span>Accessibility</span>

          </div>

        </div>


        <!-- BOARD ROOM -->

        <div class="project-card">

          <img
            src="images/boardroom.png"
            alt="Board Room"
          >

          <h3>
            Board Room
          </h3>

          <p>
            A secure SwiftUI room booking application with
            authentication and REST API integration.
          </p>

          <div class="tags">

            <span>SwiftUI</span>
            <span>REST API</span>
            <span>Authentication</span>
            <span>Security</span>

          </div>

        </div>


        <!-- JUTHOOR -->

        <div class="project-card">

          <img
            src="images/Jthoor.png"
            alt="Juthoor"
          >

          <h3>
            Juthoor | جذور
          </h3>

          <p>
            An educational game that promotes Saudi heritage
            through interactive learning experiences,
            games, and regional cultural content.
          </p>

          <div class="tags">

            <span>iOS</span>
            <span>Educational</span>
            <span>Game</span>
            <span>Saudi Culture</span>

          </div>

        </div>


      </div>

    </section>


    <!-- =========================
         CYBERSECURITY PROJECTS
    ========================== -->

    <section class="card">

      <h2 class="section-title">
        CYBERSECURITY LAB PROJECTS
      </h2>


      <div class="grid grid-3 projects">


        <!-- WEB SECURITY -->

        <div class="project-card">

          <img
            src="https://images.unsplash.com/photo-1550751827-4bd374c3f58b"
            alt="Web Security"
          >

          <h3>
            Web Vulnerability Analysis
          </h3>

          <p>
            Conducted authorized web application security testing,
            traffic interception, passive scanning, request
            analysis, and security findings documentation.
          </p>

          <div class="tags">

            <span>Burp Suite</span>
            <span>OWASP ZAP</span>
            <span>Web Security</span>
            <span>Vulnerability Assessment</span>

          </div>

        </div>


        <!-- FIREWALL -->

        <div class="project-card">

          <img
            src="https://images.unsplash.com/photo-1510511450819-1c1a7b4b6c9f"
            alt="Network Security"
          >

          <h3>
            Secure Network Using Firewall & ACL
          </h3>

          <p>
            Designed a secure network using firewall rules
            and Access Control Lists to control traffic
            between networks.
          </p>

          <div class="tags">

            <span>Firewall</span>
            <span>ACL</span>
            <span>Network Security</span>

          </div>

        </div>


        <!-- VPN -->

        <div class="project-card">

          <img
            src="https://images.unsplash.com/photo-1504639725590-34d0984388bd"
            alt="VPN"
          >

          <h3>
            Site-to-Site VPN
          </h3>

          <p>
            Implemented encrypted VPN connectivity between
            remote networks using Cisco technologies.
          </p>

          <div class="tags">

            <span>VPN</span>
            <span>Cisco</span>
            <span>Network Security</span>

          </div>

        </div>


        <!-- TCP/IP -->

        <div class="project-card">

          <img
            src="https://images.unsplash.com/photo-1504639725590-34d0984388bd"
            alt="Network Infrastructure"
          >

          <h3>
            Network Using TCP/IP, DHCP & DNS
          </h3>

          <p>
            Built a network infrastructure based on TCP/IP
            protocols with automated address allocation
            through DHCP and DNS services.
          </p>

          <div class="tags">

            <span>TCP/IP</span>
            <span>DHCP</span>
            <span>DNS</span>
            <span>Networking</span>

          </div>

        </div>


      </div>

    </section>


    <!-- =========================
         CERTIFICATIONS
    ========================== -->

    <section class="grid grid-2">


      <div class="card">

        <h3>
          Certifications
        </h3>

        <p>
          Project Management Professional (PMP)
        </p>

      </div>


      <div class="card">

        <h3>
          Languages
        </h3>

        <p>
          🇸🇦 Arabic &nbsp;&nbsp; 🇺🇸 English
        </p>

      </div>

    </section>


    <!-- =========================
         FINAL CONTACT
    ========================== -->

    <section class="card">

      <h2>
        LET'S CONNECT
      </h2>

      <p>
        Interested in software engineering, iOS development,
        cybersecurity, AI, and building secure digital products.
      </p>

      <button
        class="contact-btn"
        onclick="window.location.href='mailto:wed.alasiri2025@gmail.com'"
      >
        Get In Touch
      </button>

    </section>


    <!-- FOOTER -->

    <footer>
      © 2026 Wed Alasiri
    </footer>


  </main>


  <!-- =========================
       LANGUAGE BUTTON
  ========================== -->

  <script>

    document
      .getElementById("langToggle")
      .addEventListener("click", function () {

        alert("Arabic version coming soon.");

      });

  </script>

</body>
</html>

