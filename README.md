<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hacker Etis Hub</title>
  <style>
    body {
      margin: 0;
      font-family: "Courier New", monospace;
      background: #0d0d0d;
      color: #e0e0e0;
      display: flex;
      flex-direction: column;
      min-height: 100vh;
    }
    header {
      padding: 15px;
      text-align: center;
      background: #111;
      font-size: 1.4rem;
      font-weight: bold;
      letter-spacing: 2px;
      color: #00ff88;
    }
    nav {
      display: flex;
      justify-content: space-around;
      background: #1a1a1a;
      padding: 12px;
      position: sticky;
      top: 0;
      z-index: 100;
    }
    nav a {
      color: #00ff88;
      text-decoration: none;
      font-size: 1rem;
    }
    section {
      flex: 1;
      padding: 20px;
      text-align: center;
    }
    h2 {
      margin-bottom: 10px;
      color: #00ffcc;
    }
    .card {
      background: #1a1a1a;
      margin: 12px auto;
      padding: 15px;
      border-radius: 10px;
      max-width: 500px;
      box-shadow: 0 0 10px #00ff88;
      text-align: left;
    }
    footer {
      text-align: center;
      padding: 12px;
      background: #111;
      font-size: 0.85rem;
      color: #888;
    }
    /* Search box */
    .search-box {
      margin: 15px auto;
      text-align: center;
    }
    input[type="text"] {
      padding: 10px;
      width: 90%;
      max-width: 400px;
      border-radius: 8px;
      border: 1px solid #00ff88;
      background: #0d0d0d;
      color: #00ff88;
      font-size: 1rem;
    }
    ul {
      padding-left: 20px;
    }
  </style>
</head>
<body>
  <header>💻 Hacker Etis Hub</header>

  <nav>
    <a href="#roadmap">Roadmap</a>
    <a href="#skills">Skills</a>
    <a href="#resources">Resources</a>
    <a href="#etika">Etika</a>
  </nav>

  <section id="roadmap">
    <h2>🚀 Roadmap Belajar</h2>
    <div class="card">
      <ul>
        <li>1. Belajar Linux & Command Line</li>
        <li>2. Networking & Protocols</li>
        <li>3. Web Security (OWASP Top 10)</li>
        <li>4. OSINT & Forensics</li>
        <li>5. Ethical Hacking Labs</li>
        <li>6. Bug Bounty & Legal Practice</li>
      </ul>
    </div>
  </section>

  <section id="skills">
    <h2>🛠️ Skills</h2>
    <div class="search-box">
      <input type="text" id="searchInput" placeholder="Cari skill...">
    </div>
    <div class="card" id="skillList">
      <p>- Linux & Terminal</p>
      <p>- Jaringan & Server</p>
      <p>- Web Exploitation</p>
      <p>- OSINT & Investigasi</p>
      <p>- Digital Forensics</p>
      <p>- Reverse Engineering</p>
      <p>- Cryptography</p>
      <p>- Cloud Security</p>
    </div>
  </section>

  <section id="resources">
    <h2>📚 Resources</h2>
    <div class="card">
      <p><a href="https://tryhackme.com" target="_blank">TryHackMe</a> → Belajar interaktif</p>
      <p><a href="https://www.hackthebox.com/" target="_blank">HackTheBox</a> → Tantangan nyata</p>
      <p><a href="https://owasp.org" target="_blank">OWASP</a> → Standar keamanan web</p>
      <p><a href="https://overthewire.org/wargames/" target="_blank">OverTheWire</a> → Game pembelajaran</p>
    </div>
  </section>

  <section id="etika">
    <h2>⚖️ Etika & Legal</h2>
    <div class="card">
      <p>🔒 Gunakan skill hacking hanya untuk tujuan pembelajaran & keamanan.</p>
      <p>❌ Jangan menyerang sistem tanpa izin.</p>
      <p>✅ Latihan di lab legal, bug bounty, atau simulasi.</p>
    </div>
  </section>

  <footer>
    © 2025 Hacker Etis Hub | Belajar Aman & Legal
  </footer>

  <script>
    // Fitur pencarian skill
    const searchInput = document.getElementById("searchInput");
    const skillList = document.getElementById("skillList");
    const skills = Array.from(skillList.getElementsByTagName("p"));

    searchInput.addEventListener("keyup", function() {
      let filter = searchInput.value.toLowerCase();
      skills.forEach(skill => {
        if (skill.textContent.toLowerCase().includes(filter)) {
          skill.style.display = "";
        } else {
          skill.style.display = "none";
        }
      });
    });
  </script>
</body>
</html>
