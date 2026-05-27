<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mihreteab Niguse | Portfolio</title>
    <style>
        /* Global Styles */
        :root {
            --bg-color: #0f172a;
            --card-bg: #1e293b;
            --text-main: #f8fafc;
            --text-muted: #94a3b8;
            --accent: #38bdf8;
            --border: #334155;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-main);
            line-height: 1.6;
        }

        .container {
            max-width: 1000px;
            margin: 0 auto;
            padding: 2rem;
        }

        /* Navigation */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.5rem 0;
            border-bottom: 1px solid var(--border);
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--accent);
        }

        .nav-links a {
            color: var(--text-muted);
            text-decoration: none;
            margin-left: 1.5rem;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: var(--accent);
        }

        /* Hero Section */
        header {
            padding: 5rem 0;
            text-align: center;
        }

        header h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        header h1 span {
            color: var(--accent);
        }

        header p {
            font-size: 1.2rem;
            color: var(--text-muted);
            max-width: 600px;
            margin: 0 auto 2rem auto;
        }

        /* Section Layouts */
        section {
            padding: 4rem 0;
            border-bottom: 1px solid var(--border);
        }

        h2 {
            font-size: 2rem;
            margin-bottom: 2rem;
            position: relative;
            display: inline-block;
        }

        h2::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: -5px;
            width: 50%;
            height: 3px;
            background-color: var(--accent);
        }

        /* Grid Layouts */
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .card {
            background-color: var(--card-bg);
            padding: 2rem;
            border-radius: 8px;
            border: 1px solid var(--border);
            transition: transform 0.3s, border-color 0.3s;
        }

        .card:hover {
            transform: translateY(-5px);
            border-color: var(--accent);
        }

        .card h3 {
            margin-bottom: 1rem;
            color: var(--accent);
        }

        /* Skills Tag Style */
        .skills-list {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            list-style: none;
        }

        .skills-list li {
            background-color: rgba(56, 189, 248, 0.1);
            color: var(--accent);
            padding: 0.4rem 0.8rem;
            border-radius: 4px;
            font-size: 0.9rem;
            font-weight: 500;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 2rem 0;
            color: var(--text-muted);
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

    <div class="container">
        <!-- Navigation -->
        <nav>
            <div class="logo">MN.</div>
            <div class="nav-links">
                <a href="#about">About</a>
                <a href="#focus">Focus Areas</a>
                <a href="#projects">Projects</a>
                <a href="#skills">Skills</a>
            </div>
        </nav>

        <!-- Hero / Header -->
        <header>
            <h1>Hi, I'm <span>Mihreteab Niguse</span></h1>
            <p>Computer Science Student | Systems & AI Infrastructure Enthusiast</p>
        </header>

        <!-- About Section -->
        <section id="about">
            <h2>About Me</h2>
            <p style="color: var(--text-muted); font-size: 1.1rem; max-width: 800px;">
                I am a passionate Computer Science student dedicated to exploring how hardware interfaces with software and how massive modern data structures scale. From writing optimized, low-level assembly code to evaluating enterprise-grade AI infrastructure, I enjoy digging deep into technical complexities to find elegant solutions.
            </p>
        </section>

        <!-- Focus Areas -->
        <section id="focus">
            <h2>Areas of Interest</h2>
            <div class="grid">
                <div class="card">
                    <h3>Systems Programming</h3>
                    <p style="color: var(--text-muted);">Fascinated by computer architecture, microprocessor internals (like the 8086), segmentation models, and memory management mechanics.</p>
                </div>
                <div class="card">
                    <h3>AI & Vector Infrastructure</h3>
                    <p style="color: var(--text-muted);">Researching scalability in similarity searches, vector databases, and modern indexing algorithms like HNSW and DiskANN.</p>
                </div>
            </div>
        </section>

        <!-- Projects Section -->
        <section id="projects">
            <h2>Featured Projects</h2>
            <div class="grid">
                <div class="card">
                    <h3>Vector Database Performance Benchmark</h3>
                    <p style="color: var(--text-muted); margin-bottom: 1rem;">A comparative research study evaluating Pinecone and Weaviate for similarity searches at scale, measuring latency, throughput, and costs.</p>
                </div>
                <div class="card">
                    <h3>Computer Graphics Transformation Engine</h3>
                    <p style="color: var(--text-muted); margin-bottom: 1rem;">Implemented 3D transformation matrices including scaling, rotation, translation, and surface modeling techniques.</p>
                </div>
                <div class="card">
                    <h3>Student Advisory Expert System</h3>
                    <p style="color: var(--text-muted); margin-bottom: 1rem;">Developed a rule-based advisor application tailored to streamline academic planning and decision-making workflows.</p>
                </div>
            </div>
        </section>

        <!-- Skills Section -->
        <section id="skills">
            <h2>Core Technical Skills</h2>
            <ul class="skills-list">
                <li>x86 Assembly (8086)</li>
                <li>Computer Architecture</li>
                <li>Vector Databases (Pinecone, Weaviate)</li>
                <li>3D Computer Graphics</li>
                <li>HTML5 & CSS3</li>
                <li>Expert Systems (AI)</li>
            </ul>
        </section>

        <!-- Footer -->
        <footer>
            <p>&copy; 2026 Mihreteab Niguse. Built with code clarity and precision.</p>
        </footer>
    </div>

</body>
</html>
