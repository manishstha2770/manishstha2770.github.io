
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Cybersecurity | Cloud Security Portfolio</title>

<meta name="description"
content="Cybersecurity, Security Operations, AWS, Azure and AI portfolio.">

<style>
:root {
  --bg: #080e18;
  --surface: #101b2b;
  --surface2: #142437;
  --accent: #00e5a0;
  --text: #eaf2fa;
  --muted: #9db0c4;
  --border: #26394e;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  background: var(--bg);
  color: var(--text);
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.7;
}

a {
  color: inherit;
  text-decoration: none;
}

button {
  cursor: pointer;
  font: inherit;
}

.container {
  width: min(1120px, 90%);
  margin: auto;
}

section {
  padding: 90px 0;
  scroll-margin-top: 75px;
}

.section-title {
  font-size: 32px;
  color: var(--accent);
  margin-bottom: 18px;
}

.section-intro {
  max-width: 750px;
  color: var(--muted);
  margin-bottom: 30px;
}

/* NAVIGATION */

header {
  position: sticky;
  top: 0;
  z-index: 100;
  background: rgba(8,14,24,.96);
  border-bottom: 1px solid var(--border);
}

.navbar {
  min-height: 72px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 20px;
}

.logo {
  color: var(--accent);
  font-size: 21px;
  font-weight: bold;
}

.nav-links {
  display: flex;
  gap: 22px;
  flex-wrap: wrap;
}

.nav-links a {
  color: var(--muted);
  font-size: 14px;
}

.nav-links a:hover {
  color: var(--accent);
}

/* HERO */

.hero {
  min-height: 85vh;
  display: flex;
  align-items: center;
  background:
    radial-gradient(circle at 85% 35%,
    #123d39 0%, transparent 45%),
    var(--bg);
}

.hero-grid {
  display: grid;
  grid-template-columns: 1.3fr 1fr;
  align-items: center;
  gap: 50px;
}

.eyebrow {
  color: var(--accent);
  font-family: monospace;
  margin-bottom: 15px;
}

.hero h1 {
  font-size: clamp(36px, 5vw, 64px);
  line-height: 1.15;
  margin-bottom: 20px;
}

.accent {
  color: var(--accent);
}

.hero-description {
  color: var(--muted);
  font-size: 17px;
  max-width: 630px;
}

.buttons {
  display: flex;
  gap: 14px;
  flex-wrap: wrap;
  margin-top: 28px;
}

.btn {
  display: inline-block;
  padding: 12px 22px;
  background: var(--accent);
  color: #061710;
  border: 1px solid var(--accent);
  border-radius: 7px;
  font-weight: bold;
  transition: .2s;
}

.btn:hover {
  transform: translateY(-3px);
  opacity: .9;
}

.btn-outline {
  background: transparent;
  color: var(--accent);
}

/* TERMINAL */

.terminal {
  border: 1px solid #285a51;
  border-radius: 12px;
  background: #07121d;
  overflow: hidden;
  box-shadow: 0 20px 65px #0005;
}

.terminal-header {
  padding: 13px 17px;
  background: #152435;
  display: flex;
  align-items: center;
  gap: 8px;
}

.dot {
  width: 10px;
  height: 10px;
  border-radius: 50%;
}

.red { background: #ff5f57; }
.yellow { background: #febc2e; }
.green { background: #28c840; }

.terminal-title {
  margin-left: 10px;
  color: var(--muted);
  font-size: 12px;
}

.terminal-body {
  padding: 25px;
  font-family: monospace;
  font-size: 14px;
  line-height: 2;
}

.command {
  color: var(--accent);
}

.output {
  color: #c4d7e7;
}

/* CARDS */

.grid {
  display: grid;
  grid-template-columns:
    repeat(auto-fit, minmax(245px, 1fr));
  gap: 22px;
}

.card {
  padding: 26px;
  background: var(--surface);
  border: 1px solid var(--border);
  border-radius: 12px;
  transition: .25s;
}

.card:hover {
  transform: translateY(-5px);
  border-color: var(--accent);
}

.card-icon {
  font-size: 30px;
  margin-bottom: 15px;
}

.card h3 {
  font-size: 19px;
  margin-bottom: 12px;
}

.card p {
  color: var(--muted);
  font-size: 14px;
}

.tags {
  margin-top: 18px;
}

.tag {
  display: inline-block;
  color: var(--accent);
  background: #173c38;
  padding: 5px 10px;
  margin: 4px 4px 4px 0;
  border-radius: 5px;
  font-size: 12px;
}

/* ABOUT */

.about-grid {
  display: grid;
  grid-template-columns: 1.5fr 1fr;
  gap: 35px;
  align-items: start;
}

.about-text p {
  color: var(--muted);
  margin-bottom: 18px;
}

.info-box {
  background: var(--surface);
  padding: 25px;
  border: 1px solid var(--border);
  border-radius: 12px;
}

.info-row {
  padding: 12px 0;
  border-bottom: 1px solid var(--border);
}

.info-row:last-child {
  border-bottom: 0;
}

.info-label {
  color: var(--accent);
  font-size: 13px;
}

.info-value {
  display: block;
  margin-top: 3px;
}

/* CERTIFICATIONS */

.cert-status {
  display: inline-block;
  margin-top: 15px;
  border: 1px solid var(--border);
  padding: 5px 12px;
  border-radius: 20px;
  color: var(--muted);
  font-size: 12px;
}

/* PROJECTS */

.project-card {
  display: flex;
  flex-direction: column;
}

.project-card .tags {
  margin-top: auto;
  padding-top: 20px;
}

.project-link {
  display: inline-block;
  margin-top: 18px;
  color: var(--accent);
  font-weight: bold;
  font-size: 14px;
}

/* CONTACT */

.contact-section {
  text-align: center;
  background: linear-gradient(
    180deg, var(--bg), #0e242b
  );
}

.contact-section p {
  color: var(--muted);
  max-width: 650px;
  margin: 0 auto;
}

.contact-section .buttons {
  justify-content: center;
}

/* FOOTER */

footer {
  padding: 25px 0;
  border-top: 1px solid var(--border);
  color: var(--muted);
  text-align: center;
  font-size: 13px;
}

/* SCROLL REVEAL */

.reveal {
  opacity: 0;
  transform: translateY(20px);
  transition: opacity .6s, transform .6s;
}

.reveal.visible {
  opacity: 1;
  transform: translateY(0);
}

/* MOBILE */

@media (max-width: 800px) {
  .hero-grid,
  .about-grid {
    grid-template-columns: 1fr;
  }

  .hero {
    padding: 75px 0;
  }

  section {
    padding: 65px 0;
  }

  .navbar {
    flex-direction: column;
    padding: 15px 0;
  }

  .nav-links {
    justify-content: center;
    gap: 12px;
  }

  .hero h1 {
    font-size: 40px;
  }
}

@media (prefers-reduced-motion: reduce) {
  html { scroll-behavior: auto; }

  .reveal {
    opacity: 1;
    transform: none;
  }
}
</style>
</head>

<body>

<!-- NAVIGATION -->

<header>
  <nav class="container navbar">
    <a class="logo" href="#home">
      &lt;CyberPortfolio /&gt;
    </a>

    <div class="nav-links">
      <a href="#about">About</a>
      <a href="#skills">Skills</a>
      <a href="#certifications">Certifications</a>
      <a href="#projects">Projects</a>
      <a href="#education">Education</a>
      <a href="#contact">Contact</a>
    </div>
  </nav>
</header>

<main>

<!-- HERO -->

<section id="home" class="hero">
  <div class="container hero-grid">

    <div>
      <p class="eyebrow">
        $ Welcome to my cybersecurity portfolio
      </p>

      <h1>
        Hi, I'm <span class="accent">YOUR NAME</span>
        <br>
        Cybersecurity &
        <span class="accent">Cloud Security</span>
      </h1>

      <p class="hero-description">
        Cybersecurity student and aspiring Cloud Security
        Engineer specializing in Security Operations,
        Microsoft Azure, AWS Cloud, threat detection,
        identity security, and AI-powered automation.
      </p>

      <div class="buttons">
        <a class="btn" href="#projects">
          Explore My Projects
        </a>
        <a class="btn btn-outline" href="#contact">
          Contact Me
        </a>
      </div>
    </div>

    <div class="terminal">
      <div class="terminal-header">
        <span class="dot red"></span>
        <span class="dot yellow"></span>
        <span class="dot green"></span>
        <span class="terminal-title">security@portfolio</span>
      </div>

      <div class="terminal-body">
        <div class="command">$ whoami</div>
        <div class="output">
          Cybersecurity Student
        </div>

        <div class="command">$ cat interests.txt</div>
        <div class="output">
          Security Operations<br>
          Cloud Security Engineering<br>
          AWS & Microsoft Azure<br>
          AI-Powered Threat Detection
        </div>

        <div class="command">$ status</div>
        <div class="output">
          Learning. Building. Securing.
        </div>

        <div class="command">$ _</div>
      </div>
    </div>

  </div>
</section>

<!-- ABOUT -->

<section id="about">
  <div class="container reveal">

    <h2 class="section-title">01. About Me</h2>

    <div class="about-grid">
      <div class="about-text">
        <p>
          I am a cybersecurity student with a strong
          interest in security operations, cloud
          infrastructure protection, and security
          automation.
        </p>

        <p>
          My focus includes Microsoft Sentinel,
          Microsoft Entra ID, Azure security,
          AWS security services, incident response,
          threat hunting, and identity management.
        </p>

        <p>
          I am especially interested in combining
          artificial intelligence with security
          operations to improve incident triage,
          alert investigation, and response workflows.
        </p>

        <p>
          My career goal is to become a Cloud Security
          Engineer and contribute to building secure,
          resilient, and automated cloud environments.
        </p>
      </div>

      <div class="info-box">
        <div class="info-row">
          <span class="info-label">Career Focus</span>
          <span class="info-value">
            Cloud Security Engineer
          </span>
        </div>

        <div class="info-row">
          <span class="info-label">Specialization</span>
          <span class="info-value">
            Security Operations & Cloud
          </span>
        </div>

        <div class="info-row">
          <span class="info-label">Platforms</span>
          <span class="info-value">
            Microsoft Azure & AWS
          </span>
        </div>

        <div class="info-row">
          <span class="info-label">Interests</span>
          <span class="info-value">
            AI Security Automation
          </span>
        </div>
      </div>
    </div>

  </div>
</section>

<!-- SKILLS -->

<section id="skills">
  <div class="container reveal">

    <h2 class="section-title">02. Technical Skills</h2>

    <p class="section-intro">
      Technologies and security concepts that form
      my cloud security and SOC learning path.
    </p>

    <div class="grid">

      <article class="card">
        <div class="card-icon">🛡️</div>
        <h3>Security Operations</h3>
        <p>
          Security monitoring, investigation,
          threat detection, and incident response.
        </p>
        <div class="tags">
          <span class="tag">Microsoft Sentinel</span>
          <span class="tag">SIEM</span>
          <span class="tag">KQL</span>
          <span class="tag">Threat Hunting</span>
          <span class="tag">Incident Response</span>
          <span class="tag">MITRE ATT&CK</span>
        </div>
      </article>

      <article class="card">
        <div class="card-icon">☁️</div>
        <h3>Microsoft Azure</h3>
        <p>
          Azure administration, identity management,
          cloud monitoring, and access security.
        </p>
        <div class="tags">
          <span class="tag">Azure VMs</span>
          <span class="tag">Entra ID</span>
          <span class="tag">Azure RBAC</span>
          <span class="tag">Azure Monitor</span>
          <span class="tag">Azure Policy</span>
          <span class="tag">Azure CLI</span>
        </div>
      </article>

      <article class="card">
        <div class="card-icon">🌐</div>
        <h3>AWS Cloud Security</h3>
        <p>
          Cloud infrastructure, access management,
          auditing, and security monitoring.
        </p>
        <div class="tags">
          <span class="tag">AWS IAM</span>
          <span class="tag">EC2</span>
          <span class="tag">S3</span>
          <span class="tag">CloudTrail</span>
          <span class="tag">CloudWatch</span>
          <span class="tag">Security Hub</span>
        </div>
      </article>

      <article class="card">
        <div class="card-icon">🤖</div>
        <h3>AI & Security Automation</h3>
        <p>
          Applying AI, scripting, and automation
          concepts to security workflows.
        </p>
        <div class="tags">
          <span class="tag">AI Practitioner</span>
          <span class="tag">Python</span>
          <span class="tag">REST APIs</span>
          <span class="tag">LLMs</span>
          <span class="tag">AI Triage</span>
          <span class="tag">Automation</span>
        </div>
      </article>

      <article class="card">
        <div class="card-icon">🔐</div>
        <h3>Identity & Access Security</h3>
        <p>
          Identity governance, authentication,
          authorization, and least privilege.
        </p>
        <div class="tags">
          <span class="tag">IAM</span>
          <span class="tag">MFA</span>
          <span class="tag">RBAC</span>
          <span class="tag">Conditional Access</span>
          <span class="tag">Zero Trust</span>
        </div>
      </article>

      <article class="card">
        <div class="card-icon">💻</div>
        <h3>Tools & Technologies</h3>
        <p>
          Tools for cloud administration,
          scripting, and technical projects.
        </p>
        <div class="tags">
          <span class="tag">Git</span>
          <span class="tag">GitHub</span>
          <span class="tag">Linux</span>
          <span class="tag">PowerShell</span>
          <span class="tag">AWS CLI</span>
          <span class="tag">VS Code</span>
        </div>
      </article>

    </div>
  </div>
</section>

<!-- CERTIFICATIONS -->

<section id="certifications">
  <div class="container reveal">

    <h2 class="section-title">
      03. Certifications & Learning
    </h2>

    <p class="section-intro">
      My professional certification learning path.
      Update the statuses below to reflect your
      actual exam and certification progress.
    </p>

    <div class="grid">

      <article class="card">
        <div class="card-icon">🏅</div>
        <h3>CompTIA Security+</h3>
        <p>
          Core cybersecurity concepts, security
          architecture, risk management,
          and security operations.
        </p>
        <span class="cert-status">Status: Update</span>
      </article>

      <article class="card">
        <div class="card-icon">☁️</div>
        <h3>AWS Certified Cloud Practitioner</h3>
        <p>
          AWS cloud concepts, security,
          services, and cloud fundamentals.
        </p>
        <span class="cert-status">Status: Update</span>
      </article>

      <article class="card">
        <div class="card-icon">🤖</div>
        <h3>AWS Certified AI Practitioner</h3>
        <p>
          Artificial intelligence,
          machine learning, and generative AI
          fundamentals on AWS.
        </p>
        <span class="cert-status">Status: Update</span>
      </article>

      <article class="card">
        <div class="card-icon">🔷</div>
        <h3>Microsoft AZ-104</h3>
        <p>
          Microsoft Azure Administrator:
          compute, networking, storage,
          identity, and governance.
        </p>
        <span class="cert-status">Status: Update</span>
      </article>

      <article class="card">
        <div class="card-icon">🔒</div>
        <h3>Microsoft Security Certification</h3>
        <p>
          Microsoft cloud security and identity.
          Replace with your verified exam code
          and certification title.
        </p>
        <span class="cert-status">Status: Update</span>
      </article>

    </div>
  </div>
</section>

<!-- PROJECTS -->

<section id="projects">
  <div class="container reveal">

    <h2 class="section-title">
      04. Cybersecurity Projects
    </h2>

    <p class="section-intro">
      Project concepts for my cybersecurity
      portfolio. Replace these with completed
      implementations and repository links.
    </p>

    <div class="grid">

      <article class="card project-card">
        <div class="card-icon">🚨</div>
        <h3>AI-Powered SOC Triage Engine</h3>

        <p>
          A proposed security automation project
          connecting Microsoft Sentinel with
          AI-assisted incident analysis.
          The goal is to enrich security alerts,
          classify incidents, and provide
          investigation recommendations.
        </p>

        <div class="tags">
          <span class="tag">Microsoft Sentinel</span>
          <span class="tag">Python</span>
          <span class="tag">AI</span>
          <span class="tag">KQL</span>
        </div>
      </article>

      <article class="card project-card">
        <div class="card-icon">☁️</div>
        <h3>AWS Security Monitoring Lab</h3>

        <p>
          A cloud security lab concept using
          AWS CloudTrail, CloudWatch, IAM,
          and security monitoring services
          to investigate cloud activity
          and identify suspicious behavior.
        </p>

        <div class="tags">
          <span class="tag">AWS</span>
          <span class="tag">CloudTrail</span>
          <span class="tag">CloudWatch</span>
          <span class="tag">IAM</span>
        </div>
      </article>

      <article class="card project-card">
        <div class="card-icon">🔐</div>
        <h3>Azure Identity Security Lab</h3>

        <p>
          An Azure identity management lab
          exploring Microsoft Entra ID,
          role-based access control,
          least privilege, and
          identity security practices.
        </p>

        <div class="tags">
          <span class="tag">Azure</span>
          <span class="tag">Entra ID</span>
          <span class="tag">RBAC</span>
          <span class="tag">IAM</span>
        </div>
      </article>

      <article class="card project-card">
        <div class="card-icon">🔎</div>
        <h3>Microsoft Sentinel Detection Lab</h3>

        <p>
          A proposed SIEM project to explore
          KQL queries, security analytics,
          log investigation, and incident
          detection within Microsoft Sentinel.
        </p>

        <div class="tags">
          <span class="tag">SIEM</span>
          <span class="tag">KQL</span>
          <span class="tag">Azure Monitor</span>
        </div>
      </article>

    </div>
  </div>
</section>

<!-- EDUCATION -->

<section id="education">
  <div class="container reveal">

    <h2 class="section-title">05. Education</h2>

    <div class="card">
      <div class="card-icon">🎓</div>

      <h3>Webster University</h3>

      <p>
        Graduate Student | Cybersecurity Focus
      </p>

      <p>
        St. Louis, Missouri, United States
      </p>

      <div class="tags">
        <span class="tag">Cybersecurity</span>
        <span class="tag">Information Security</span>
        <span class="tag">Cloud Security</span>
        <span class="tag">Risk Management</span>
      </div>
    </div>

  </div>
</section>

<!-- CONTACT -->

<section id="contact" class="contact-section">
  <div class="container reveal">

    <h2 class="section-title">
      06. Let's Connect
    </h2>

    <p>
      I am interested in opportunities involving
      cloud security engineering, security
      operations, threat detection, and
      AI-powered cybersecurity automation.
    </p>

    <div class="buttons">
      <a class="btn"
         href="mailto:your.email@example.com">
        Email Me
      </a>

      <a class="btn btn-outline"
         href="https://github.com/YOUR_USERNAME"
         target="_blank"
         rel="noopener noreferrer">
        GitHub
      </a>

      <a class="btn btn-outline"
         href="https://www.linkedin.com/in/YOUR_USERNAME/"
         target="_blank"
         rel="noopener noreferrer">
        LinkedIn
      </a>
    </div>

  </div>
</section>

</main>

<!-- FOOTER -->

<footer>
  <div class="container">
    © <span id="year"></span>
    YOUR NAME | Cybersecurity & Cloud Security
    Portfolio
  </div>
</footer>

<!-- JAVASCRIPT -->

<script>
document.getElementById("year").textContent =
  new Date().getFullYear();

const elements = document.querySelectorAll(".reveal");

if ("IntersectionObserver" in window) {
  const observer = new IntersectionObserver(
    (entries) => {
      entries.forEach((entry) => {
        if (entry.isIntersecting) {
          entry.target.classList.add("visible");
          observer.unobserve(entry.target);
        }
      });
    },
    { threshold: 0.1 }
  );

  elements.forEach((element) => {
    observer.observe(element);
  });
} else {
  elements.forEach((element) => {
    element.classList.add("visible");
  });
}
</script>

</body>
</html>
