<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hailu Tilahun Kebede | Animal Scientist & Climate Specialist</title>
    <style>
        :root {
            --primary: #0f382c;
            --accent: #2d6a4f;
            --accent-light: #52b788;
            --light-bg: #f4f8f5;
            --card-bg: #ffffff;
            --text-main: #1f2937;
            --text-sub: #4b5563;
            --border: #d8f3dc;
            --shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.05), 0 2px 4px -1px rgba(0, 0, 0, 0.03);
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', system-ui, -apple-system, sans-serif;
        }

        body {
            color: var(--text-main);
            background-color: var(--light-bg);
            line-height: 1.6;
        }

        /* Navigation */
        nav {
            background: var(--primary);
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: var(--shadow);
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
            font-size: 1.15rem;
            color: #ffffff;
            text-decoration: none;
        }

        .nav-links a {
            color: #d8f3dc;
            text-decoration: none;
            margin-left: 1.2rem;
            font-weight: 500;
            font-size: 0.9rem;
            transition: color 0.2s;
        }

        .nav-links a:hover {
            color: #ffffff;
        }

        /* Hero Header */
        .hero {
            background: linear-gradient(135deg, var(--primary) 0%, #1b4332 100%);
            color: #ffffff;
            padding: 4.5rem 1.5rem;
            text-align: center;
        }

        .hero-container {
            max-width: 900px;
            margin: 0 auto;
        }

        .hero h1 {
            font-size: 2.6rem;
            font-weight: 800;
            margin-bottom: 0.5rem;
            letter-spacing: -0.5px;
        }

        .hero h2 {
            font-size: 1.2rem;
            color: var(--accent-light);
            font-weight: 600;
            margin-bottom: 1.2rem;
        }

        .hero p {
            font-size: 1.05rem;
            color: #e8f5e9;
            line-height: 1.7;
            margin-bottom: 2rem;
        }

        .btn-group {
            display: flex;
            gap: 1rem;
            justify-content: center;
            flex-wrap: wrap;
        }

        .btn {
            padding: 0.75rem 1.5rem;
            border-radius: 6px;
            font-weight: 600;
            text-decoration: none;
            font-size: 0.95rem;
            transition: all 0.2s;
        }

        .btn-primary {
            background-color: var(--accent-light);
            color: var(--primary);
        }

        .btn-primary:hover {
            background-color: #74c69d;
        }

        .btn-outline {
            border: 2px solid #ffffff;
            color: #ffffff;
        }

        .btn-outline:hover {
            background: rgba(255, 255, 255, 0.1);
        }

        /* Container & Sections */
        .container {
            max-width: 1100px;
            margin: 3rem auto;
            padding: 0 1.5rem;
        }

        section {
            margin-bottom: 4rem;
        }

        .section-title {
            text-align: center;
            font-size: 1.8rem;
            color: var(--primary);
            margin-bottom: 2rem;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 50px;
            height: 3px;
            background: var(--accent);
            margin: 0.5rem auto 0;
            border-radius: 2px;
        }

        /* Grids and Cards */
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 1.5rem;
        }

        .card {
            background: var(--card-bg);
            padding: 1.8rem;
            border-radius: 8px;
            box-shadow: var(--shadow);
            border-top: 4px solid var(--accent);
        }

        .card h3 {
            color: var(--primary);
            font-size: 1.2rem;
            margin-bottom: 0.8rem;
        }

        .card p {
            color: var(--text-sub);
            font-size: 0.95rem;
        }

        .card ul {
            list-style: none;
            margin-top: 0.5rem;
        }

        .card ul li {
            position: relative;
            padding-left: 1.2rem;
            margin-bottom: 0.4rem;
            font-size: 0.92rem;
            color: var(--text-main);
        }

        .card ul li::before {
            content: '•';
            color: var(--accent);
            font-weight: bold;
            position: absolute;
            left: 0;
        }

        /* Tags and Badges */
        .tag-cloud {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            justify-content: center;
            margin-top: 1rem;
        }

        .tag {
            background: #e8f5e9;
            color: var(--primary);
            padding: 0.4rem 0.9rem;
            border-radius: 20px;
            font-size: 0.88rem;
            font-weight: 600;
            border: 1px solid var(--border);
        }

        /* Text Block Styling */
        .text-block {
            background: var(--card-bg);
            padding: 2rem;
            border-radius: 8px;
            box-shadow: var(--shadow);
            color: var(--text-main);
            font-size: 1rem;
            line-height: 1.7;
        }

        /* Footer */
        footer {
            background: var(--primary);
            color: #d8f3dc;
            text-align: center;
            padding: 2.5rem 1.5rem;
            margin-top: 4rem;
        }

        footer a {
            color: #ffffff;
            text-decoration: underline;
        }
    </style>
</head>
<body>

    <!-- Website Navigation -->
    <nav>
        <div class="nav-container">
            <a href="#" class="logo">Hailu Tilahun Kebede</a>
            <div class="nav-links">
                <a href="#about">About</a>
                <a href="#expertise">Expertise</a>
                <a href="#impact">Areas of Impact</a>
                <a href="#partnerships">Partnerships</a>
                <a href="#research">Research</a>
                <a href="#projects">Projects</a>
                <a href="#contact">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Header Hero -->
    <header class="hero" id="home">
        <div class="hero-container">
            <h1>Hailu Tilahun Kebede</h1>
            <h2>Animal Scientist | Researcher | Climate & Sustainable Development Specialist</h2>
            <p>Bridging animal science, agricultural innovation, climate action, biodiversity conservation, carbon finance, sustainable development, and international markets to develop practical solutions for resilient communities, sustainable livelihoods, and a greener future.</p>
            <div class="btn-group">
                <a href="#contact" class="btn btn-primary">Contact Me</a>
                <a href="#impact" class="btn btn-outline">Explore Areas of Impact</a>
            </div>
        </div>
    </header>

    <div class="container">

        <!-- About Summary -->
        <section id="about">
            <h2 class="section-title">Overview</h2>
            <div class="text-block">
                <p>I operate at the intersection of livestock genomics, climate finance, regenerative agriculture, and market linkages. By integrating rigorous scientific research with practical community-based development, my work aims to transform climate action into economic value for local communities and global partners alike.</p>
            </div>
        </section>

        <!-- Expertise Section -->
        <section id="expertise">
            <h2 class="section-title">Expertise</h2>
            <div class="grid">

                <div class="card">
                    <h3>Animal Science & Livestock</h3>
                    <ul>
                        <li>Animal Breeding & Genetics</li>
                        <li>Livestock Genomics & GWAS</li>
                        <li>Genetic Resource Conservation</li>
                        <li>Sustainable Livestock Production</li>
                        <li>Climate-Resilient Livestock Systems</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>Climate, Carbon & Sustainable Finance</h3>
                    <ul>
                        <li>Carbon Credit Development</li>
                        <li>Climate Finance</li>
                        <li>Climate Mitigation</li>
                        <li>Climate Adaptation</li>
                        <li>Climate-Smart Agriculture</li>
                        <li>Climate-Resilient Development</li>
                        <li>Environmental and Sustainable Investment</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>Biodiversity, Agroforestry & Nature</h3>
                    <ul>
                        <li>Biodiversity Conservation</li>
                        <li>Agroforestry</li>
                        <li>Ecosystem Restoration</li>
                        <li>Sustainable Land Management</li>
                        <li>Regenerative Agriculture</li>
                        <li>Nature-Based Solutions</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>Agriculture & Food Systems</h3>
                    <ul>
                        <li>Sustainable Agriculture</li>
                        <li>Agroecology</li>
                        <li>Agricultural Research & Innovation</li>
                        <li>Sustainable Food Systems</li>
                        <li>Community-Based Agriculture</li>
                        <li>Climate-Smart Production Systems</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>Coffee & International Trade</h3>
                    <ul>
                        <li>Coffee Farming and Production</li>
                        <li>Ethiopian Coffee Value Chains</li>
                        <li>Coffee Quality and Market Development</li>
                        <li>Coffee Export</li>
                        <li>International Market Linkage</li>
                        <li>Agricultural Investment and Trade Partnerships</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>Research & Inclusive Development</h3>
                    <ul>
                        <li>Agricultural Research & Data Analysis</li>
                        <li>Scientific Innovation & Technology Transfer</li>
                        <li>Evidence-Based Development</li>
                        <li>Youth Empowerment & Women’s Inclusion</li>
                        <li>Capacity Building & International Partnerships</li>
                        <li>Sustainable Livelihood Development</li>
                    </ul>
                </div>

            </div>
        </section>

        <!-- Areas of Impact Section -->
        <section id="impact">
            <h2 class="section-title">Areas of Impact</h2>
            <div class="grid">

                <div class="card">
                    <h3>Climate & Carbon</h3>
                    <p>Developing practical approaches to carbon markets, climate finance, mitigation, adaptation, and climate-resilient development, with a focus on creating environmental and economic value.</p>
                </div>

                <div class="card">
                    <h3>Biodiversity & Nature</h3>
                    <p>Supporting biodiversity conservation, agroforestry, ecosystem restoration, sustainable land management, and nature-based solutions that strengthen ecological resilience and community livelihoods.</p>
                </div>

                <div class="card">
                    <h3>Sustainable Agriculture</h3>
                    <p>Promoting climate-smart agriculture, agroecology, regenerative production, sustainable livestock systems, and resilient food value chains.</p>
                </div>

                <div class="card">
                    <h3>Livestock Science & Genetics</h3>
                    <p>Applying expertise in animal breeding, genetics, genomics, GWAS, genetic-resource conservation, and sustainable livestock production to improve productivity and resilience.</p>
                </div>

                <div class="card">
                    <h3>Coffee & International Markets</h3>
                    <p>Connecting Ethiopia’s agricultural potential with international markets through sustainable coffee production, value-chain development, export, investment, and international commercial partnerships.</p>
                </div>

                <div class="card">
                    <h3>Community & Inclusive Development</h3>
                    <p>Working with communities, youth, women, institutions, researchers, governments, and international partners to transform knowledge and resources into inclusive and sustainable development outcomes.</p>
                </div>

            </div>
        </section>

        <!-- Partnerships Section -->
        <section id="partnerships">
            <h2 class="section-title">Partnerships</h2>
            <div class="text-block" style="text-align: center;">
                <p style="margin-bottom: 1.5rem;"><strong>I work with:</strong></p>
                <div class="tag-cloud" style="margin-bottom: 2rem;">
                    <span class="tag">Universities & Research Institutions</span>
                    <span class="tag">Government Institutions</span>
                    <span class="tag">International Organizations</span>
                    <span class="tag">Development Partners</span>
                    <span class="tag">NGOs & Civil Society</span>
                    <span class="tag">Private-Sector Companies</span>
                    <span class="tag">Investors & Financial Institutions</span>
                    <span class="tag">Agricultural Producers & Cooperatives</span>
                    <span class="tag">Climate & Carbon-Market Actors</span>
                    <span class="tag">International Buyers & Trading Partners</span>
                    <span class="tag">Youth & Community Networks</span>
                </div>

                <p style="margin-bottom: 0.5rem;"><strong>Partnership Focus:</strong></p>
                <p style="color: var(--accent); font-weight: 600;">
                    Research | Climate Action | Agriculture | Biodiversity | Carbon Finance | Investment | Trade | Innovation | Community Development
                </p>
            </div>
        </section>

        <!-- Research Section -->
        <section id="research">
            <h2 class="section-title">Research</h2>
            <div class="text-block">
                <p>My research and professional interests focus on the relationship between animal science, agricultural productivity, genetics, climate resilience, biodiversity, sustainable land use, and community development.</p>
                <p style="margin-top: 1rem;">The goal is to generate evidence and innovations that can be translated into practical solutions for farmers, communities, institutions, and international development partners.</p>
            </div>
        </section>

        <!-- Projects Section -->
        <section id="projects">
            <h2 class="section-title">Projects & Initiatives</h2>
            <div class="card">
                <p style="margin-bottom: 1rem;">My project interests and initiatives focus on driving practical impact across multiple domains:</p>
                <div class="tag-cloud" style="justify-content: flex-start;">
                    <span class="tag">Climate-Smart Agriculture</span>
                    <span class="tag">Sustainable Livestock Development</span>
                    <span class="tag">Animal Breeding & Genetic Improvement</span>
                    <span class="tag">Biodiversity Conservation</span>
                    <span class="tag">Agroforestry & Ecosystem Restoration</span>
                    <span class="tag">Carbon-Credit Development</span>
                    <span class="tag">Climate Finance</span>
                    <span class="tag">Climate Mitigation & Adaptation</span>
                    <span class="tag">Sustainable Coffee Production</span>
                    <span class="tag">Coffee Export & Market Linkage</span>
                    <span class="tag">Agricultural Investment</span>
                    <span class="tag">Community-Based Development</span>
                    <span class="tag">Youth & Women Empowerment</span>
                    <span class="tag">International R&D Partnerships</span>
                </div>
            </div>
        </section>

        <!-- Collaboration Call to Action -->
        <section>
            <h2 class="section-title">Collaboration</h2>
            <div class="text-block" style="text-align: center;">
                <h3 style="color: var(--primary); font-size: 1.4rem; margin-bottom: 1rem;">Let's Build Sustainable Solutions Together</h3>
                <p style="margin-bottom: 1.5rem;">I welcome collaboration with research institutions, universities, governments, development organizations, investors, private-sector companies, agricultural organizations, climate and carbon-market partners, and international buyers.</p>
                <p style="margin-bottom: 2rem;">Together, we can connect science, innovation, finance, nature, agriculture, and international markets to create measurable environmental, social, and economic impact.</p>
                
                <div class="tag-cloud">
                    <span class="tag">Research Collaboration</span>
                    <span class="tag">Strategic Partnership</span>
                    <span class="tag">Investment</span>
                    <span class="tag">Climate Finance</span>
                    <span class="tag">Agricultural Trade</span>
                    <span class="tag">International Market Linkage</span>
                </div>
            </div>
        </section>

    </div>

    <!-- Contact & Footer -->
    <footer id="contact">
        <h2 style="font-size: 1.5rem; margin-bottom: 0.5rem; color: #ffffff;">Contact Hailu Tilahun Kebede</h2>
        <p style="margin-bottom: 1rem;">📍 Addis Ababa, Ethiopia | 📱 (+251) 910204390</p>
        <p>Email: <a href="mailto:hailshtilahun@gmail.com">hailshtilahun@gmail.com</a></p>
        <p style="margin-top: 2rem; font-size: 0.85rem; opacity: 0.8;">&copy; 2026 Hailu Tilahun Kebede. All Rights Reserved.</p>
    </footer>

</body>
</html>
