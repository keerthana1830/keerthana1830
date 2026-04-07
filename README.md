<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
    <title>Keerthana R · Embedded & AI Engineer</title>
    <!-- Google Fonts + Font Awesome -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,600;14..32,700;14..32,800&family=JetBrains+Mono:wght@400;500;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: #0a0c10;
            font-family: 'Inter', 'Segoe UI', sans-serif;
            color: #eef2ff;
            line-height: 1.5;
            scroll-behavior: smooth;
        }

        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #11161f;
        }
        ::-webkit-scrollbar-thumb {
            background: #3b4b6e;
            border-radius: 12px;
        }

        .container {
            max-width: 1280px;
            margin: 0 auto;
            padding: 2rem 1.8rem 4rem;
        }

        /* ASCII header glow */
        .ascii-art {
            font-family: 'JetBrains Mono', monospace;
            font-size: clamp(0.55rem, 2.5vw, 0.85rem);
            line-height: 1.2;
            white-space: pre;
            color: #b9e6ff;
            text-shadow: 0 0 3px #2d8fbb33;
            background: #01010140;
            padding: 1rem 0.5rem;
            border-radius: 32px;
            overflow-x: auto;
            text-align: center;
            letter-spacing: 0.5px;
        }

        .glow-text {
            background: linear-gradient(135deg, #c0e0ff, #7cb8e4);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            font-weight: 600;
        }

        .badge-pill {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            background: #12161fcc;
            backdrop-filter: blur(4px);
            border: 1px solid #2d4059;
            border-radius: 100px;
            padding: 0.4rem 1rem;
            font-size: 0.85rem;
            font-weight: 500;
            transition: all 0.2s;
        }

        .badge-pill i {
            font-size: 1rem;
            color: #7aa9dd;
        }

        .section-title {
            font-size: 1.8rem;
            font-weight: 700;
            letter-spacing: -0.3px;
            margin: 2rem 0 1.5rem 0;
            border-left: 5px solid #2d7f9e;
            padding-left: 1rem;
            display: flex;
            align-items: center;
            gap: 12px;
        }
        .section-title i {
            font-size: 1.8rem;
            color: #56b4e9;
        }

        .terminal-card {
            background: #0c0f15e6;
            backdrop-filter: blur(2px);
            border: 1px solid #232834;
            border-radius: 24px;
            padding: 1.5rem;
            margin: 1rem 0;
            transition: transform 0.2s ease, border-color 0.2s;
            box-shadow: 0 12px 24px -12px rgba(0,0,0,0.5);
        }
        .terminal-card:hover {
            border-color: #3f6792;
        }

        .cmd-line {
            font-family: 'JetBrains Mono', monospace;
            color: #9dc3e6;
            font-size: 1rem;
            margin-bottom: 1rem;
            display: flex;
            align-items: center;
            gap: 8px;
            flex-wrap: wrap;
        }
        .cmd-prompt {
            color: #5dc9a0;
        }

        .skills-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 0.8rem;
            margin: 1.2rem 0 0.5rem;
        }
        .skill-tag {
            background: #11161f;
            padding: 0.45rem 1rem;
            border-radius: 40px;
            font-size: 0.8rem;
            font-weight: 500;
            font-family: 'JetBrains Mono', monospace;
            border: 1px solid #28303e;
            transition: all 0.2s;
        }
        .skill-tag:hover {
            background: #1a2538;
            border-color: #4b7aa1;
            transform: translateY(-2px);
        }

        .table-highlight {
            background: #0f131c;
            border-radius: 24px;
            overflow: hidden;
            border: 1px solid #252e3c;
        }
        .table-highlight table {
            width: 100%;
            border-collapse: collapse;
        }
        .table-highlight th, .table-highlight td {
            padding: 1rem 1.2rem;
            text-align: left;
            border-bottom: 1px solid #202630;
        }
        .table-highlight th {
            background: #0b0f16;
            color: #9fc9ff;
            font-weight: 600;
        }
        .medal {
            font-weight: 800;
            font-size: 1.2rem;
        }

        .tech-stack-badge {
            display: inline-flex;
            flex-wrap: wrap;
            gap: 0.6rem;
            margin-top: 0.8rem;
        }

        .quote-box {
            background: linear-gradient(135deg, #0a111c, #03070f);
            border-radius: 32px;
            padding: 1.6rem 2rem;
            text-align: center;
            border: 1px solid #2e3b4e;
            margin: 2rem 0 1rem;
            font-style: italic;
            font-size: 1.15rem;
            font-weight: 400;
        }

        footer {
            text-align: center;
            margin-top: 3.5rem;
            padding-top: 2rem;
            border-top: 1px solid #1e2632;
            font-size: 0.85rem;
            color: #8595aa;
        }

        a {
            color: #a0c6f0;
            text-decoration: none;
            transition: color 0.2s;
        }
        a:hover {
            color: white;
            text-decoration: underline;
        }

        .flex-between {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            align-items: center;
            gap: 1rem;
        }

        @media (max-width: 720px) {
            .container {
                padding: 1rem 1.2rem 2rem;
            }
            .section-title {
                font-size: 1.5rem;
            }
            .ascii-art {
                font-size: 0.48rem;
            }
        }
        .blinking-cursor {
            background-color: #6bb5e0;
            width: 10px;
            height: 1.2rem;
            display: inline-block;
            animation: blink 1s step-end infinite;
            margin-left: 3px;
        }
        @keyframes blink {
            0%, 100% { opacity: 1; }
            50% { opacity: 0; }
        }
        .status-led {
            display: inline-block;
            width: 10px;
            height: 10px;
            border-radius: 50%;
            background-color: #3fe0a0;
            box-shadow: 0 0 6px #3fe0a0;
            margin-right: 8px;
        }
        .icon-spacing i {
            margin-right: 6px;
        }

        /* Enhanced highlight row */
        .highlight-row {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
            justify-content: space-between;
            margin-top: 1rem;
        }
        .stat-badge {
            background: #0e121b;
            border-radius: 1.5rem;
            padding: 0.5rem 1.2rem;
            border: 1px solid #2a3442;
            font-size: 0.85rem;
        }
        .stat-badge i {
            margin-right: 6px;
            color: #5f9bc2;
        }
    </style>
</head>
<body>
<div class="container">

    <!-- ASCII with dynamic feel -->
    <div align="center">
        <div class="ascii-art">
██╗  ██╗███████╗███████╗██████╗ ████████╗██╗  ██╗ █████╗ ███╗   ██╗ █████╗    ██████╗ 
██║ ██╔╝██╔════╝██╔════╝██╔══██╗╚══██╔══╝██║  ██║██╔══██╗████╗  ██║██╔══██╗  ██╔══██╗
█████╔╝ █████╗  █████╗  ██████╔╝   ██║   ███████║███████║██╔██╗ ██║███████║  ██████╔╝
██╔═██╗ ██╔══╝  ██╔══╝  ██╔══██╗   ██║   ██╔══██║██╔══██║██║╚██╗██║██╔══██║  ██╔══██╗
██║  ██╗███████╗███████╗██║  ██║   ██║   ██║  ██║██║  ██║██║ ╚████║██║  ██║  ██║  ██║
╚═╝  ╚═╝╚══════╝╚══════╝╚═╝  ╚═╝   ╚═╝   ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═══╝╚═╝  ╚═╝  ╚═╝  ╚═╝
        </div>
        <div style="margin-top: 0.5rem;">
            <span class="badge-pill"><i class="fas fa-microchip"></i> Computer & Communication Engineering</span>
            <span class="badge-pill"><i class="fas fa-robot"></i> Embedded Systems · IoT · AI</span>
        </div>
        <p style="margin: 1rem 0 0.2rem; font-size: 1.05rem; max-width: 700px;">
            <i class="fas fa-cogs"></i> <span class="glow-text">Building hardware-integrated systems that bridge the physical and digital worlds.</span>
        </p>
        <div style="margin: 1rem 0;">
            <a href="https://linkedin.com/in/keerthanar18" target="_blank"><i class="fab fa-linkedin" style="font-size: 1.6rem; margin: 0 8px;"></i></a>
            <a href="mailto:keerthanarajkumar11@gmail.com"><i class="fas fa-envelope" style="font-size: 1.6rem; margin: 0 8px;"></i></a>
            <span style="margin-left: 12px;"><i class="fas fa-eye"></i> <span style="font-family: monospace;">active · embedded edge</span></span>
        </div>
    </div>

    <!-- $ whoami enhanced section -->
    <div class="terminal-card">
        <div class="cmd-line"><span class="cmd-prompt">$</span> <span style="color:#ffbc6e;">whoami</span><span class="blinking-cursor"></span></div>
        <div style="display: flex; flex-wrap: wrap; gap: 1rem; align-items: flex-start;">
            <div style="flex: 2;">
                <p style="font-size: 1.05rem; margin-bottom: 0.5rem;"><span class="status-led"></span> <strong>Keerthana R</strong> <span style="color:#aac8e0;">(she/her)</span></p>
                <p>Hi, I'm a passionate engineering student with a strong pull towards the intersection of embedded hardware and intelligent software. I enjoy designing systems that are not just smart, but <strong>useful</strong>: from IoT-based healthcare monitors to AI-driven agriculture automation.</p>
                <p style="margin-top: 0.8rem;">When I'm not wiring sensors or flashing firmware, I'm training models, writing papers, or competing in hackathons.</p>
                <div class="highlight-row" style="margin-top: 1rem;">
                    <span class="stat-badge"><i class="fas fa-trophy"></i> 3x Hackathon Winner</span>
                    <span class="stat-badge"><i class="fas fa-file-alt"></i> Published Researcher (ICRTICC'25)</span>
                    <span class="stat-badge"><i class="fas fa-microchip"></i> 5+ Embedded prototypes</span>
                </div>
            </div>
        </div>
    </div>

    <!-- $ ls ./skills with tree-like style -->
    <div class="terminal-card">
        <div class="cmd-line"><span class="cmd-prompt">$</span> ls ./skills --tree</div>
        <div style="font-family: 'JetBrains Mono', monospace; font-size: 0.9rem;">
            <div><span style="color:#75b5e3;">├── hardware/</span></div>
            <div style="margin-left: 1.5rem;"><span style="color:#b3cde0;">│   ├── microcontrollers</span>    <span class="skill-tag" style="margin-left: 12px;">ESP32</span> <span class="skill-tag">STM32</span> <span class="skill-tag">Arduino</span></div>
            <div style="margin-left: 1.5rem;"><span style="color:#b3cde0;">│   ├── protocols</span>           <span class="skill-tag" style="margin-left: 12px;">I2C</span> <span class="skill-tag">SPI</span> <span class="skill-tag">UART</span> <span class="skill-tag">CAN</span></div>
            <div style="margin-left: 1.5rem;"><span style="color:#b3cde0;">│   └── platforms</span>           <span class="skill-tag">Raspberry Pi</span> <span class="skill-tag">Linux</span> <span class="skill-tag">RTOS</span></div>
            <div><span style="color:#75b5e3;">├── software/</span></div>
            <div style="margin-left: 1.5rem;"><span style="color:#b3cde0;">│   ├── languages</span>           <span class="skill-tag">C</span> <span class="skill-tag">C++</span> <span class="skill-tag">Python</span></div>
            <div style="margin-left: 1.5rem;"><span style="color:#b3cde0;">│   ├── ml_frameworks</span>       <span class="skill-tag">TensorFlow</span> <span class="skill-tag">scikit-learn</span></div>
            <div style="margin-left: 1.5rem;"><span style="color:#b3cde0;">│   ├── data_tools</span>          <span class="skill-tag">NumPy</span> <span class="skill-tag">Pandas</span> <span class="skill-tag">Matplotlib</span></div>
            <div style="margin-left: 1.5rem;"><span style="color:#b3cde0;">│   └── databases</span>           <span class="skill-tag">MongoDB</span> <span class="skill-tag">MySQL</span> <span class="skill-tag">SQLite</span></div>
            <div><span style="color:#75b5e3;">└── devops/</span></div>
            <div style="margin-left: 1.5rem;"><span style="color:#b3cde0;">    ├── version_control</span>     <span class="skill-tag">Git</span> <span class="skill-tag">GitHub</span></div>
            <div style="margin-left: 1.5rem;"><span style="color:#b3cde0;">    └── containers</span>          <span class="skill-tag">Docker</span></div>
        </div>
    </div>

    <!-- Highlights Table (Awards & Achievements) -->
    <div class="section-title"><i class="fas fa-medal"></i> `$ cat ./highlights.log`</div>
    <div class="table-highlight">
        <table>
            <thead>
                <tr><th>Place</th><th>Event</th><th>Details</th></tr>
            </thead>
            <tbody>
                <tr><td class="medal" style="color:#FFD966;">🥇 1st</td><td>InstaVenture AI Hackathon</td><td>CED, Anna University</td></tr>
                <tr><td class="medal" style="color:#C0C0C0;">🥈 2nd</td><td>SRISHTI 2025</td><td>National Level Project Exhibition</td></tr>
                <tr><td class="medal" style="color:#CD7F32;">🏅 4th</td><td>TNWISE Hackathon</td><td>₹10,000 prize</td></tr>
                <tr><td><i class="fas fa-file-pdf"></i> 📄 Published</td><td>ICRTICC 2025</td><td>Smart Cart System — Research Paper</td></tr>
            </tbody>
        </table>
    </div>

    <!-- Enhanced Tech Stack with JSON preview and badges -->
    <div class="section-title"><i class="fas fa-code-branch"></i> `$ cat ./tech_stack.json`</div>
    <div class="terminal-card">
        <div style="background:#0a0e16; border-radius: 18px; padding: 1rem; font-family: 'JetBrains Mono', monospace; font-size: 0.8rem;">
            {
            <div style="margin-left: 1.2rem;">"languages":   ["C", "C++", "Python"],</div>
            <div style="margin-left: 1.2rem;">"ml":          ["TensorFlow", "scikit-learn", "NumPy", "Pandas", "Matplotlib"],</div>
            <div style="margin-left: 1.2rem;">"hardware":    ["ESP32", "STM32", "Arduino", "Raspberry Pi"],</div>
            <div style="margin-left: 1.2rem;">"protocols":   ["I2C", "SPI", "UART", "CAN"],</div>
            <div style="margin-left: 1.2rem;">"databases":   ["MongoDB", "MySQL", "SQLite"],</div>
            <div style="margin-left: 1.2rem;">"devops":      ["GitHub", "Docker"],</div>
            <div style="margin-left: 1.2rem;">"os":          ["Linux", "RTOS"]</div>
            }
        </div>
        <div class="tech-stack-badge" style="margin-top: 1.2rem;">
            <span class="skill-tag"><i class="fab fa-python"></i> Python</span>
            <span class="skill-tag"><i class="fas fa-microchip"></i> C++/Embedded</span>
            <span class="skill-tag"><i class="fas fa-brain"></i> TensorFlow</span>
            <span class="skill-tag"><i class="fas fa-database"></i> MongoDB</span>
            <span class="skill-tag"><i class="fab fa-docker"></i> Docker</span>
            <span class="skill-tag"><i class="fab fa-github"></i> GitHub Actions</span>
            <span class="skill-tag"><i class="fas fa-chart-line"></i> Pandas</span>
            <span class="skill-tag"><i class="fas fa-microphone-alt"></i> I2C/SPI</span>
        </div>
    </div>

    <!-- Tech Stack Icons Row (clean inline) -->
    <div style="display: flex; flex-wrap: wrap; gap: 0.5rem; margin: 0.5rem 0 1rem;">
        <img src="https://img.shields.io/badge/c-%2300599C.svg?style=flat-square&logo=c&logoColor=white" alt="C">
        <img src="https://img.shields.io/badge/c++-%2300599C.svg?style=flat-square&logo=c%2B%2B&logoColor=white" alt="C++">
        <img src="https://img.shields.io/badge/python-3670A0?style=flat-square&logo=python&logoColor=ffdd54" alt="Python">
        <img src="https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=flat-square&logo=TensorFlow&logoColor=white" alt="TF">
        <img src="https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=flat-square&logo=scikit-learn&logoColor=white" alt="sklearn">
        <img src="https://img.shields.io/badge/numpy-%23013243.svg?style=flat-square&logo=numpy&logoColor=white" alt="numpy">
        <img src="https://img.shields.io/badge/pandas-%23150458.svg?style=flat-square&logo=pandas&logoColor=white" alt="pandas">
        <img src="https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=flat-square&logo=Matplotlib&logoColor=black" alt="matplotlib">
        <img src="https://img.shields.io/badge/-Arduino-00979D?style=flat-square&logo=Arduino&logoColor=white" alt="Arduino">
        <img src="https://img.shields.io/badge/-Raspberry_Pi-C51A4A?style=flat-square&logo=Raspberry-Pi" alt="RPi">
        <img src="https://img.shields.io/badge/docker-%230db7ed.svg?style=flat-square&logo=docker&logoColor=white" alt="docker">
        <img src="https://img.shields.io/badge/github-%23121011.svg?style=flat-square&logo=github&logoColor=white" alt="github">
        <img src="https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=flat-square&logo=mongodb&logoColor=white" alt="mongodb">
        <img src="https://img.shields.io/badge/mysql-4479A1.svg?style=flat-square&logo=mysql&logoColor=white" alt="mysql">
        <img src="https://img.shields.io/badge/sqlite-%2307405e.svg?style=flat-square&logo=sqlite&logoColor=white" alt="sqlite">
    </div>

    <!-- Fortune / Quote with dynamic refresh -->
    <div class="quote-box" id="quoteBox">
        <i class="fas fa-terminal" style="margin-right: 10px; opacity: 0.7;"></i> 
        <span id="dynamicQuote">Loading wisdom...</span>
        <div style="margin-top: 12px;"><i class="fas fa-sync-alt" style="font-size: 0.7rem; opacity: 0.5;"></i> <span style="font-size: 0.7rem;">dev inspiration · reloads every visit</span></div>
    </div>

    <!-- Extra project spotlight / embedded highlight -->
    <div class="terminal-card">
        <div class="cmd-line"><span class="cmd-prompt">$</span> git log --oneline --grep="feature" -n 3</div>
        <div style="font-family: 'JetBrains Mono', monospace; font-size: 0.85rem;">
            <div><span style="color:#9ec184;">✦ a1b2c3d</span> : IoT Patient Health Monitoring with realtime alerts (ESP32 + TensorFlow Lite)</div>
            <div><span style="color:#9ec184;">✦ d4e5f6g</span> : AgriSense: AI-driven soil nutrient predictor & automated irrigation</div>
            <div><span style="color:#9ec184;">✦ h7i8j9k</span> : Smart Cart System | frictionless billing + RFID | Research paper @ ICRTICC'25</div>
        </div>
        <div style="margin-top: 1rem; font-size: 0.8rem; border-left: 2px solid #2f698b; padding-left: 12px;">
            <i class="fas fa-flask"></i> <strong>Current focus:</strong> Real-time Edge AI for predictive maintenance & low-power wide-area networks.
        </div>
    </div>

    <footer>
        <i class="fas fa-microchip"></i> Keerthana R · Embedded & AI systems · <i class="far fa-copyright"></i> 2025 · Open for collaborations & research
        <div style="margin-top: 0.8rem;">
            <a href="#"><i class="fab fa-github"></i> github/keerthana1830</a> &nbsp;|&nbsp;
            <a href="#"><i class="fab fa-linkedin"></i> linkedin.com/in/keerthanar18</a>
        </div>
    </footer>
</div>

<script>
    // Fortune quotes collection (inspiring + tech related)
    const quotes = [
        "The best way to predict the future is to invent it. — Alan Kay",
        "Hardware and software: two sides of the same intelligent coin.",
        "Any sufficiently advanced technology is indistinguishable from magic. — Arthur C. Clarke",
        "Embed every system with empathy and robustness.",
        "Talk is cheap. Show me the firmware. — inspired by Linus Torvalds",
        "Innovation happens at the intersection of bits and atoms.",
        "Keep it simple, but not simpler. — Einstein",
        "Don't just connect things, connect possibilities. — IoT mindset",
        "AI without embedded is just theory; embedded without AI is just switches.",
        "Code is poetry, hardware is sculpture."
    ];
    function setRandomQuote() {
        const randomIndex = Math.floor(Math.random() * quotes.length);
        const quoteElem = document.getElementById('dynamicQuote');
        if (quoteElem) {
            quoteElem.innerHTML = `“ ${quotes[randomIndex]} ”`;
        }
    }
    setRandomQuote();

    // subtle dynamic year update & terminal cursor blink effect (already css)
    // add interactive effect on skill tags
    const skillTags = document.querySelectorAll('.skill-tag');
    skillTags.forEach(tag => {
        tag.addEventListener('click', function() {
            this.style.backgroundColor = '#1f3348';
            setTimeout(() => {
                this.style.backgroundColor = '#11161f';
            }, 200);
        });
    });
</script>
</body>
</html>
