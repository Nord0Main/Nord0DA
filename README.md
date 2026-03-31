<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nord0DA | AI-Powered Adventures</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root {
            --bg-dark: #0a0a0a;
            --card-bg: #161616;
            --accent: #007bff;
            --text-main: #e0e0e0;
            --text-dim: #a0a0a0;
        }

        body {
            background-color: var(--bg-dark);
            color: var(--text-main);
            font-family: 'Inter', -apple-system, sans-serif;
            margin: 0;
            line-height: 1.6;
            scroll-behavior: smooth;
        }

        /* Navigation */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 5%;
            background: rgba(10, 10, 10, 0.95);
            position: sticky;
            top: 0;
            z-index: 100;
            border-bottom: 1px solid #222;
        }

        .logo { font-size: 1.5rem; font-weight: 800; letter-spacing: 2px; color: #fff; }
        .nav-links a { color: var(--text-dim); text-decoration: none; margin-left: 20px; font-size: 0.9rem; transition: 0.3s; }
        .nav-links a:hover { color: var(--accent); }

        /* Hero Section */
        header {
            height: 80vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: radial-gradient(circle at center, #1a1a1a 0%, #0a0a0a 100%);
            padding: 0 20px;
        }

        header h1 { font-size: 4rem; margin-bottom: 10px; font-weight: 200; color: #fff; }
        header p { color: var(--text-dim); max-width: 600px; font-size: 1.2rem; }

        /* Sections */
        section { padding: 80px 10%; }
        h2 { font-size: 2.5rem; margin-bottom: 40px; text-align: center; font-weight: 300; }

        /* Adventure Grid */
        .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; }
        .card { 
            background: var(--card-bg); 
            padding: 30px; 
            border-radius: 12px; 
            border: 1px solid #222;
            transition: 0.3s;
            text-align: center;
        }
        .card:hover { border-color: var(--accent); transform: translateY(-5px); }
        .coming-soon { opacity: 0.5; font-style: italic; }

        /* Buttons */
        .btn {
            display: inline-block;
            padding: 12px 32px;
            border-radius: 6px;
            text-decoration: none;
            font-weight: 600;
            transition: 0.3s;
            cursor: pointer;
            border: none;
        }
        .btn-primary { background: var(--accent); color: #fff; }
        .btn-outline { border: 1px solid var(--accent); color: var(--accent); margin-top: 10px; }
        .btn-patreon { background: #f96854; color: #fff; }

        /* FAQ */
        .faq-item { margin-bottom: 20px; background: var(--card-bg); padding: 20px; border-radius: 8px; }
        .faq-item h3 { margin-top: 0; color: var(--accent); font-size: 1.1rem; }

        /* Footer */
        footer { padding: 40px; text-align: center; border-top: 1px solid #222; color: var(--text-dim); }

        /* Modal (Temporary Login) */
        .login-temp { text-align: center; max-width: 400px; margin: 0 auto; }
        input { 
            width: 100%; padding: 12px; margin: 8px 0; 
            background: #222; border: 1px solid #333; color: #fff; border-radius: 4px; 
        }
    </style>
</head>
<body>

<nav>
    <div class="logo">NORD0<span style="color:var(--accent)">DA</span></div>
    <div class="nav-links">
        <a href="#adventures">Adventures</a>
        <a href="#downloads">Downloads</a>
        <a href="#faq">FAQ</a>
        <a href="#support">Support</a>
        <a href="#auth" class="btn btn-outline" style="padding: 5px 15px;">Login</a>
    </div>
</nav>

<header>
    <h1>Limitless Worlds</h1>
    <p>The next generation of AI-driven text adventures. Your choices don't just change the story—they create the world.</p>
    <a href="#downloads" class="btn btn-primary" style="margin-top: 20px;">Start Your Journey</a>
</header>

<section id="adventures">
    <h2>Current Adventures</h2>
    <div class="grid">
        <div class="card">
            <i class="fas fa-dragon fa-3x" style="color:var(--accent); margin-bottom:15px;"></i>
            <h3>High Fantasy</h3>
            <p>Magic, dragons, and ancient ruins. Available now.</p>
            <span style="color:var(--accent)">Active Module</span>
        </div>
        <div class="card coming-soon">
            <i class="fas fa-rocket fa-3x" style="margin-bottom:15px;"></i>
            <h3>Sci-Fi Noir</h3>
            <p>Cybernetics and neon-soaked mysteries.</p>
            <span>Coming Soon</span>
        </div>
        <div class="card coming-soon">
            <i class="fas fa-ship fa-3x" style="margin-bottom:15px;"></i>
            <h3>High Seas</h3>
            <p>Pirates, krakens, and hidden treasures.</p>
            <span>Coming Soon</span>
        </div>
    </div>
</section>

<section id="downloads" style="background: #0f0f0f;">
    <h2>Get the Game</h2>
    <div style="text-align: center;">
        <p>Current Version: <b>v0.1.0-alpha</b></p>
        <div class="grid" style="max-width: 800px; margin: 0 auto;">
            <div class="card">
                <h3>Windows</h3>
                <a href="YOUR_LINK_HERE" class="btn btn-primary">Download .exe</a>
            </div>
            <div class="card">
                <h3>Linux / Mac</h3>
                <a href="YOUR_LINK_HERE" class="btn btn-primary">Download .zip</a>
            </div>
        </div>
    </div>
</section>

<section id="faq">
    <h2>F.A.Q.</h2>
    <div style="max-width: 700px; margin: 0 auto;">
        <div class="faq-item">
            <h3>How does the AI work?</h3>
            <p>Nord0DA uses custom-tuned LLMs to generate context-aware responses, ensuring no two adventures are ever the same.</p>
        </div>
        <div class="faq-item">
            <h3>Is it free?</h3>
            <p>The base Fantasy module is free to play during our Alpha phase. Expansion modules may require support via Patreon.</p>
        </div>
        <div class="faq-item">
            <h3>Can I play offline?</h3>
            <p>Currently, an internet connection is required to communicate with the Nord0 AI engine.</p>
        </div>
    </div>
</section>

<section id="auth" style="background: #0f0f0f;">
    <h2>Join the Archive</h2>
    <div class="card login-temp">
        <p>Login or Register to save your progress across devices.</p>
        <input type="text" placeholder="Username">
        <input type="password" placeholder="Password">
        <button class="btn btn-primary" style="width:100%; margin-top:10px;" onclick="alert('Account system coming soon!')">Login</button>
        <p style="font-size: 0.8rem; color: var(--text-dim);">Database integration in progress.</p>
    </div>
</section>

<section id="support" style="text-align: center;">
    <h2>Support Development</h2>
    <p>Help us build the ultimate AI dungeon master. Patrons get early access to new modules like Isekai and Sci-Fi.</p>
    <a href="https://www.patreon.com/c/Nord0" target="_blank" class="btn btn-patreon">
        <i class="fab fa-patreon"></i> Support Nord0 on Patreon
    </a>
</section>

<footer>
    <p>&copy; 2026 Nord0Labs. All rights reserved.</p>
</footer>

</body>
</html>
