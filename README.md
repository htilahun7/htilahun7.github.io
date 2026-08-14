<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hailu Tilahun Kebede | Animal Breeding & Climate Resilience Specialist</title>
    <style>
        :root {
            --primary: #0f382c;
            --accent: #2d6a4f;
            --light-accent: #e8f5e9;
            --text-dark: #1f2937;
            --text-light: #6b7280;
            --bg-light: #f8faf9;
            --white: #ffffff;
            --shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', system-ui, -apple-system, sans-serif;
        }

        body {
            color: var(--text-dark);
            background-color: var(--bg-light);
            line-height: 1.6;
        }

        /* Navigation */
        nav {
            background: var(--white);
            box-shadow: var(--shadow);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .nav-container {
            max-width: 1100px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 1.5rem;
        }

        .logo {
            font-weight: 700;
            font-size: 1.2rem;
            color: var(--primary);
            text-decoration: none;
        }

        .nav-links a {
            color: var(--text-dark);
            text-decoration: none;
            margin-left: 1.5rem;
            font-weight: 500;
            font-size: 0.95rem;
            transition: color 0.2s;
        }

        .nav-links a:hover {
            color: var(--accent);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, var(--primary) 0%, #1b4332 100%);
            color: var(--white);
            padding: 5rem 1.5rem;
            text-align: center;
        }

        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }

        .hero h1 {
            font-size: 2.8rem;
            font-weight: 800;
            margin-bottom: 1rem;
            line-height: 1.2;
        }

        .hero p {
            font-size: 1.25rem;
            color: #d8f3dc;
            margin-bottom: 2rem;
        }

        .btn-group {
            display: flex;
            gap: 1rem;
            justify-content: center;
            flex-wrap: wrap;
        }

        .btn {
            padding: 0.8rem 1.6rem;
            border-radius: 6px;
            font-weight: 600;
            text-decoration: none;
            transition: all 0.2s;
        }

        .btn-primary {
            background-color: #52b788;
            color: var(--primary);
        }

        .btn-primary:hover {
            background-color: #74c69d;
        }

        .btn-outline {
            border: 2px solid var(--white);
            color: var(--white);
        }

        .btn-outline:hover {
            background: rgba(255, 255, 255, 0.1);
        }

        /* Main Container */
        .container {
            max-width: 1100px;
            margin: 3rem auto;
            padding: 0 1.5rem;
        }

        .section-title {
            text-align: center;
            font-size: 2rem;
            color: var(--primary);
            margin-bottom: 2.5rem;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 50px;
            height: 4px;
            background: var(--accent);
            margin: 0.5rem auto 0;
            border-radius: 2px;
        }

        /* Card Grids */
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
            margin-bottom: 4rem;
        }

        .card {
            background: var(--white);
            padding: 2rem;
            border-radius: 8px;
            box-shadow: var(--shadow);
            border-top: 4px solid var(--accent);
            transition: transform 0.2s;
        }

        .card:hover {
            transform: translateY(-5px);
        }

        .card h3 {
            color: var(--primary);
            font-size: 1.25rem;
            margin-bottom: 0.8rem;
        }

        .card p {
            color: var(--text-light);
            font-size: 0.95rem;
        }

        /* Showcase List */
        .showcase-item {
            background: var(--white);
            padding: 1.5rem;
            border-radius: 8px;
            box-shadow: var(--shadow);
            margin-bottom: 1rem;
            display: flex;
            flex-direction: column;
        }

        .showcase-title {
            font-weight: 700;
            font-size: 1.1rem;
            color: var(--primary);
        }

        .showcase-sub {
            color: var(--text-light);
            font-size: 0.9rem;
            margin-top: 0.2rem;
        }

        /* Badges */
        .badge-container {
            display: flex;
            flex-wrap: wrap;
            gap: 0.6rem;
            margin-top: 1rem;
        }

        .badge {
            background: var(--light-accent);
            color: var(--primary);
            padding: 0.4rem 0.8rem;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 600;
        }

        /* Footer */
        footer {
            background: var(--primary);
            color: #d8f3dc;
            text-align: center;
            padding: 2rem 1.5rem;
            margin-top: 4rem;
        }

        footer a {
            color: var(--white);
            text-decoration: underline;
        }
    </style>
</head>
<body>

    <!-- Navigation Bar -->
    <nav>
        <div class="nav-container">
            <a href="#" class="logo">Hailu Tilahun Kebede</a>
            <div class="nav-links">
                <a href="#expertise">Expertise</a>
                <a href="#partnerships">Partnerships</a>
                <a href="#research">Research</a>
                <a href="#projects">Projects</a>
                <a href="#contact">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Hero Header -->
    <header class="hero">
        <div class="hero-content">
            <h1>Advancing Animal Genetics & Sustainable Agroecology</h1>
            <p>MSc Animal Scientist bridging livestock genomic research with climate resilience, regenerative agriculture, and community development[cite: 1].</p>
            <div class="btn-group">
                <a href="mailto:hailshtilahun@gmail.com" class="btn btn-primary">Get In Touch</a>
                <a href="#research" class="btn btn-outline">Explore Research</a>
            </div>
        </div>
    </header>

    <div class="container">

        <!-- Core Expertise Section -->
        <section id="expertise">
            <h2 class="section-title">Core Expertise</h2>
            <div class="grid">
                <div class="card">
                    <h3>Genomics & Animal Breeding</h3>
                    <p>Specializing in Genome-Wide Association Studies (GWAS), phenotype characterization, and genetic data modeling using SAS, SPSS, and R[cite: 1].</p>
                </div>
                <div class="card">
                    <h3>Climate Resilience & Finance</h3>
                    <p>Developing MER frameworks for carbon credits, climate adaptation strategies, and ecosystem mitigation pathways[cite: 1].</p>
                </div>
                <div class="card">
                    <h3>Sustainable Agroecology</h3>
                    <p>Designing integrated regenerative agriculture systems combining livestock, organic farming, aquaculture, and apiculture[cite: 1].</p>
                </div>
            </div>
        </section>

        <!-- Global Partnerships Section -->
        <section id="partnerships">
            <h2 class="section-title">International Partnerships & Engagement</h2>
            <div class="grid">
                <div class="card">
                    <h3>UN Sustainable Development</h3>
                    <p>Delegate at the 12th United Nations Economic Commission for Africa (UNECA) Regional Forum on Sustainable Development[cite: 1].</p>
                </div>
                <div class="card">
                    <h3>African Union G20 Social Summit</h3>
                    <p>Official AU Delegate contributing to policy dialogues on global climate action, policy equity, and sustainable development[cite: 1].</p>
                </div>
                <div class="card">
                    <h3>Global Capacity Building</h3>
                    <p>FARM to FARM Certified (USAID) and Udacity Data/AI Specialist leading technical technology transfers[cite: 1].</p>
                </div>
            </div>
        </section>

        <!-- Research & Publications Section -->
        <section id="research">
            <h2 class="section-title">Featured Publications</h2>
            <div class="showcase-item">
                <div class="showcase-title">Assessment on Rearing and Husbandry Practices of Indigenous Goats</div>
                <div class="showcase-sub">Published in Journal of Applied Animal Research (2023) | Taylor & Francis[cite: 1]</div>
            </div>
            <div class="showcase-item">
                <div class="showcase-title">Phenotypic Characterization of Indigenous Sheep Breeds in Jimma Zone</div>
                <div class="showcase-sub">Published in Journal of Applied Animal Research (2023)[cite: 1]</div>
            </div>
            <div class="showcase-item">
                <div class="showcase-title">Phenotypic Characterization of Indigenous Goats in North Shewa Zone</div>
                <div class="showcase-sub">Published in IJRSAS (2019)[cite: 1]</div>
            </div>
        </section>

        <!-- Key Applied Projects -->
        <section id="projects">
            <h2 class="section-title">Key Projects & Initiatives</h2>
            <div class="grid">
                <div class="card">
                    <h3>Apiculture Innovation</h3>
                    <p>Principal lead in establishing university honeybee farms and evaluating modern hive technology preference[cite: 1].</p>
                </div>
                <div class="card">
                    <h3>Livestock Management Systems</h3>
                    <p>Led implementation of model cattle crushes across districts and evaluated estrus synchronization in dairy herds[cite: 1].</p>
                </div>
            </div>
        </section>

        <!-- Professional Development & Credentials -->
        <section>
            <h2 class="section-title">Credentials & Certifications</h2>
            <div class="badge-container" style="justify-content: center;">
                <span class="badge">MSc Animal Breeding & Genetics</span>[cite: 1]
                <span class="badge">BSc Animal Science</span>[cite: 1]
                <span class="badge">UNECA Delegate (2026)</span>[cite: 1]
                <span class="badge">AU G20 Social Summit Delegate (2025)</span>[cite: 1]
                <span class="badge">Udacity AI & Data Fundamentals</span>[cite: 1]
                <span class="badge">USAID FARM to FARM Certified</span>[cite: 1]
                <span class="badge">Higher Diploma in Teaching (HDP)</span>[cite: 1]
            </div>
        </section>

    </div>

    <!-- Contact & Footer -->
    <footer id="contact">
        <p style="font-size: 1.1rem; margin-bottom: 0.5rem; font-weight: 600;">Hailu Tilahun Kebede</p>
        <p>📍 Addis Ababa, Ethiopia | 📱 (+251) 910204390[cite: 1]</p>
        <p style="margin-top: 0.5rem;">Email: <a href="mailto:hailshtilahun@gmail.com">hailshtilahun@gmail.com</a>[cite: 1]</p>
        <p style="margin-top: 1.5rem; font-size: 0.85rem; opacity: 0.8;">&copy; 2026 All Rights Reserved.</p>
    </footer>

</body>
</html>
