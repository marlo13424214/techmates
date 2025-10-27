<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Techmates – PC & Handy Support</title>
  <style>
    :root {
      --accent: #c77dff;
      --text: #ffffff;
      --card: #1a152d;
      --button: #9b59b6;
      --button-glow: #c77dff;
    }

    * {
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: var(--bg);
      color: var(--text);
      overflow-x: hidden;
    }

    .announcement {
      background-color: #3a2f50;
      color: #ffd700;
      text-align: center;
      padding: 15px 20px;
      font-size: 1rem;
      box-shadow: 0 0 10px rgba(255, 215, 0, 0.3);
    }

    header {
      background-color: var(--card);
      padding: 60px 20px 30px;
      text-align: center;
    }

    .profile-pic {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      border: 3px solid var(--accent);
      object-fit: cover;
      margin-bottom: 20px;
      box-shadow: 0 0 15px var(--button-glow);
    }

    h1 {
      font-size: 2.8rem;
      color: var(--accent);
      margin-bottom: 10px;
    }

    .typewriter {
      font-size: 1.3rem;
      height: 30px;
      color: var(--text);
    }

    main {
      max-width: 900px;
      margin: 40px auto;
      background: var(--card);
      padding: 40px;
      border-radius: 14px;
      box-shadow: 0 0 30px rgba(199, 125, 255, 0.2);
      animation: fadeInUp 1.5s ease-out;
    }

    h2 {
      color: var(--accent);
      font-size: 1.8rem;
      margin-top: 30px;
    }

    ul {
      list-style: none;
      padding: 0;
      margin: 20px 0;
    }

    ul li {
      margin: 12px 0;
      padding-left: 1.2em;
      position: relative;
      opacity: 0;
      animation: fadeIn 1s forwards;
    }

    ul li::before {
      content: "•";
      position: absolute;
      left: 0;
      color: var(--accent);
    }

    ul li:nth-child(1) { animation-delay: 0.2s; }
    ul li:nth-child(2) { animation-delay: 0.4s; }
    ul li:nth-child(3) { animation-delay: 0.6s; }
    ul li:nth-child(4) { animation-delay: 0.8s; }
    ul li:nth-child(5) { animation-delay: 1s; }

    .button {
      display: inline-block;
      padding: 14px 30px;
      margin-top: 30px;
      background: var(--button);
      color: white;
      font-weight: bold;
      border-radius: 6px;
      text-decoration: none;
      transition: 0.3s ease;
      box-shadow: 0 0 15px var(--button-glow);
      border: none;
      cursor: pointer;
    }

    .button:hover {
      background: var(--button-glow);
      color: black;
      box-shadow: 0 0 25px var(--button-glow);
    }

    img.main-img {
      max-width: 100%;
      border-radius: 12px;
      margin-top: 40px;
      box-shadow: 0 0 20px rgba(199, 125, 255, 0.3);
    }

    form {
      margin-top: 30px;
    }

    input, textarea {
      width: 100%;
      padding: 12px;
      margin: 10px 0;
      border: none;
      border-radius: 8px;
      background-color: #2b2344;
      color: white;
      font-size: 1rem;
    }

    input::placeholder, textarea::placeholder {
      color: #aaa;
    }

    footer {
      text-align: center;
      color: #aaa;
      margin: 60px 0 20px;
      font-size: 0.9rem;
    }

    @keyframes fadeInUp {
      from { opacity: 0; transform: translateY(40px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>
  <div class="announcement">
    🚧 <strong>Hinweis:</strong> Diese Seite befindet sich im <strong>Testbetrieb</strong>.<br />
    Das Kontaktformular kann Probleme verursachen. Bitte schreiben Sie uns direkt per E-Mail an: <strong>techmates@gmail.com</strong>
  </div>

  <header>
    <img class="profile-pic" src="https://images.unsplash.com/photo-1603415526960-f7e0328c63b3?auto=format&fit=crop&w=200&q=80" alt="Profilbild" />
    <h1>Techmates</h1>
    <div class="typewriter"><span id="typeText"></span></div>
  </header>

  <main>
    <h2>Was wir können 👨‍💻👨‍💻</h2>
    <ul>
      <li>Handyhilfe (iPhone, WhatsApp, WLAN, iCloud)</li>
      <li>Windows-PC aufräumen & beschleunigen (Scripte & Tools)</li>
      <li>Eigene Software & Webseiten entwickeln</li>
      <li>Technik verständlich für jedes Alter erklären</li>
      <li>Ultrasaubere Lösungen mit Stil & Animation</li>
    </ul>

    <h2>Kontakt 📧</h2>
    <p>E-Mail: <strong>techmates@gmail.com</strong></p>

    <form action="mailto:techmates@gmail.com" method="post" enctype="text/plain">
      <h2>Schreib uns direkt:</h2>
      <input type="text" name="name" placeholder="Dein Name" required />
      <input type="email" name="email" placeholder="Deine E-Mail" required />
      <textarea name="message" rows="5" placeholder="Was sollen wir für dich tun?" required></textarea>
      <button type="submit" class="button">Senden</button>
    </form>

    <img class="main-img" src="https://images.unsplash.com/photo-1555617970-611e4c1f3b8f?auto=format&fit=crop&w=900&q=80" alt="Technik Symbolbild" />
  </main>

  <footer>
    &copy; 2025 Techmates – Powered by Marlo & Crew 💜
  </footer>

  <script>
    const textElement = document.getElementById("typeText");
    const texts = ["Hallo...", "Wir sind die Techmates.", "Wir helfen mit Technik.", "PCs. Handys. Skripte.", "Zuverlässig. Schnell. Stark."];
    let textIndex = 0;
    let charIndex = 0;
    let deleting = false;

    function type() {
      const current = texts[textIndex];
      const visible = current.substring(0, charIndex);
      textElement.textContent = visible;

      if (!deleting && charIndex < current.length) {
        charIndex++;
        setTimeout(type, 90);
      } else if (deleting && charIndex > 0) {
        charIndex--;
        setTimeout(type, 50);
      } else {
        deleting = !deleting;
        if (!deleting) textIndex = (textIndex + 1) % texts.length;
        setTimeout(type, 700);
      }
    }
    type();
  </script>
</body>
</html>
