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

        /* Navigation Header */
        nav {
            background: var(--primary);
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: var(--shadow);
            border-bottom: 2px solid var(--accent);
        }

        .nav-container {
            max-width: 1100px;
            margin: 0 auto;
            display: flex;
            justify-content: flex-end;
            align-items: center;
            padding: 1.2rem 1.5rem;
        }

        .nav-links a {
            color: #d8f3dc;
            text-decoration: none;
            margin-left: 1rem;
            font-weight: 600;
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
            padding: 4rem 1.5rem;
            text-align: center;
        }

        .hero-container {
            max-width: 900px;
            margin: 0 auto;
        }

        .profile-img {
            width: 160px;
            height: 160px;
            border-radius: 50%;
            object-fit: cover;
            border: 4px solid var(--accent-light);
            box-shadow: 0 8px 16px rgba(0,0,0,0.25);
            margin-bottom: 1.5rem;
        }

        .hero h1 {
            font-size: 2.2rem;
            margin-bottom: 0.5rem;
            color: #ffffff;
        }

        .hero h2 {
            font-size: 1.25rem;
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

        /* Layout Container */
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

        .text-block {
            background: var(--card-bg);
            padding: 2rem;
            border-radius: 8px;
            box-shadow: var(--shadow);
            color: var(--text-main);
            font-size: 1rem;
            line-height: 1.7;
        }

        /* Footer & Social Media */
        .footer-social-title {
            color: var(--accent-light);
            font-size: 1.1rem;
            font-weight: 700;
            margin-top: 1.5rem;
            margin-bottom: 0.8rem;
        }

        .social-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 0.8rem;
            justify-content: center;
            margin-bottom: 2rem;
        }

        .social-btn {
            display: inline-flex;
            align-items: center;
            padding: 0.6rem 1.2rem;
            border-radius: 30px;
            color: #ffffff;
            font-weight: 600;
            font-size: 0.9rem;
            text-decoration: none;
            transition: transform 0.2s, opacity 0.2s;
            box-shadow: var(--shadow);
        }

        .social-btn:hover {
            transform: translateY(-2px);
            opacity: 0.9;
        }

        .social-btn.linkedin { background-color: #0a66c2; }
        .social-btn.whatsapp { background-color: #25d366; }
        .social-btn.instagram { background: linear-gradient(45deg, #f09433, #e6683c, #dc2743, #cc2366, #bc1888); }
        .social-btn.telegram { background-color: #0088cc; }
        .social-btn.facebook { background-color: #1877f2; }
        .social-btn.twitter { background-color: #1da1f2; }

        footer {
            background: var(--primary);
            color: #d8f3dc;
            text-align: center;
            padding: 3rem 1.5rem 2rem;
            margin-top: 4rem;
        }

        footer a {
            color: #ffffff;
            text-decoration: underline;
        }
    </style>
</head>
<body>

    <!-- Navigation Header -->
    <nav>
        <div class="nav-container">
            <div class="nav-links">
                <a href="#home">Home</a>
                <a href="#about">About</a>
                <a href="#expertise">Expertise</a>
                <a href="#impact">Areas of Impact</a>
                <a href="#partnerships">Partnerships</a>
                <a href="#research">Research</a>
                <a href="#projects">Projects</a>
                <a href="#contact">Contacts</a>
            </div>
        </div>
    </nav>

    <!-- Hero Header -->
    <header class="hero" id="home">
        <div class="hero-container">
            <img src="photo_2025-11-24_14-14-04.jpg" alt="Hailu Tilahun Kebede" class="profile-img">
            <h1>Hailu Tilahun Kebede</h1>
            <h2>Animal Scientist | Researcher | Climate & Sustainable Development Specialist</h2>
            <p>Connecting Science, Nature, Finance & Markets for Sustainable Development</p>
            <div class="btn-group">
                <a href="#contact" class="btn btn-primary">Let's Connect</a>
                <a href="#impact" class="btn btn-outline">Explore Areas of Impact</a>
            </div>
        </div>
    </header>

    <div class="container">

        <!-- About Section -->
        <section id="about">
            <h2 class="section-title">About</h2>
            <div class="text-block">
                <p style="margin-bottom: 1.2rem;">
                    <strong>Hailu Tilahun Kebede</strong> is an Animal Scientist and Researcher with an MSc in Animal Breeding and Genetics and over eight years of experience in livestock research, academic instruction, and community-based development. His work bridges science, sustainable agriculture, climate action, biodiversity, climate finance, and international markets to develop practical, inclusive, and sustainable solutions. He combines technical expertise with community-focused approaches to improve agricultural productivity, resilience, sustainable livelihoods, and opportunities for farmers, women, and youth.
                </p>
                <p style="margin-bottom: 1.5rem;">
                    I work at the intersection of science, agricultural innovation, climate action, biodiversity conservation, carbon finance, sustainable development, and international markets. My work connects scientific research and practical implementation to help develop climate-resilient livelihoods, sustainable agricultural systems, nature-positive solutions, and international partnerships.
                </p>
                
                <h3 style="color: var(--primary); margin-bottom: 1rem; font-size: 1.2rem;">At a Glance</h3>
                <div class="grid">
                    <div style="background: var(--light-bg); padding: 1rem; border-radius: 6px; border-left: 3px solid var(--accent);">
                        <strong>Animal Science & Genetics:</strong> Animal breeding, livestock genetics, genomics, GWAS, genetic-resource conservation, and sustainable livestock systems.
                    </div>
                    <div style="background: var(--light-bg); padding: 1rem; border-radius: 6px; border-left: 3px solid var(--accent);">
                        <strong>Climate & Carbon:</strong> Carbon-credit development, climate finance, mitigation, adaptation, climate-smart agriculture, and climate-resilient development.
                    </div>
                    <div style="background: var(--light-bg); padding: 1rem; border-radius: 6px; border-left: 3px solid var(--accent);">
                        <strong>Nature & Agriculture:</strong> Biodiversity conservation, agroforestry, ecosystem restoration, regenerative agriculture, and sustainable land management.
                    </div>
                    <div style="background: var(--light-bg); padding: 1rem; border-radius: 6px; border-left: 3px solid var(--accent);">
                        <strong>Coffee & International Markets:</strong> Sustainable coffee production, value-chain development, export, international market linkage, and agricultural trade partnerships.
                    </div>
                </div>
            </div>
        </section>

        <!-- Expertise Section -->
        <section id="expertise">
            <h2 class="section-title">Expertise</h2>
            <div class="grid">
                <div class="card">
                    <h3>01 — Animal Science & Livestock</h3>
                    <ul>
                        <li>Animal Breeding & Genetics</li>
                        <li>Livestock Genomics & GWAS</li>
                        <li>Genetic Resource Conservation</li>
                        <li>Sustainable Livestock Production</li>
                        <li>Climate-Resilient Livestock Systems</li>
                        <li>Agricultural Research & Innovation</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>02 — Climate, Carbon & Sustainable Finance</h3>
                    <ul>
                        <li>Carbon Credit Development</li>
                        <li>Climate Finance</li>
                        <li>Climate Mitigation & Adaptation</li>
                        <li>Climate-Smart Agriculture</li>
                        <li>Climate-Resilient Development</li>
                        <li>Sustainable Investment</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>03 — Biodiversity, Nature & Restoration</h3>
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
                    <h3>04 — Agriculture & Food Systems</h3>
                    <ul>
                        <li>Sustainable Agriculture</li>
                        <li>Agroecology</li>
                        <li>Climate-Smart Production</li>
                        <li>Sustainable Food Systems</li>
                        <li>Community-Based Agriculture</li>
                        <li>Sustainable Development Goals</li>
                        <li>Agricultural Value Chains</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>05 — Coffee & Global Trade</h3>
                    <ul>
                        <li>Sustainable Coffee Production</li>
                        <li>Coffee Export</li>
                        <li>International Market Linkage</li>
                        <li>Agricultural Investment & Trade Partnerships</li>
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
                    <p>Developing approaches that connect climate action with sustainable finance, including carbon markets, climate mitigation, adaptation, and climate-resilient development.</p>
                </div>

                <div class="card">
                    <h3>Nature & Biodiversity</h3>
                    <p>Supporting biodiversity conservation, agroforestry, ecosystem restoration, and nature-based solutions that strengthen ecosystems while creating benefits for communities.</p>
                </div>

                <div class="card">
                    <h3>Sustainable Agriculture</h3>
                    <p>Promoting agricultural systems that improve productivity, resilience, environmental sustainability, and long-term livelihoods.</p>
                </div>

                <div class="card">
                    <h3>Livestock & Genetic Resources</h3>
                    <p>Applying animal science, genetics, genomics, and research to strengthen livestock productivity, resilience, and genetic-resource conservation.</p>
                </div>

                <div class="card">
                    <h3>Coffee & Global Markets</h3>
                    <p>Connecting Ethiopia's agricultural production with international markets, investment opportunities, value-chain development, and sustainable trade.</p>
                </div>

                <div class="card">
                    <h3>Inclusive Community Development</h3>
                    <p>Supporting approaches that create opportunities for youth, women, farmers, communities, researchers, institutions, and private-sector partners.</p>
                </div>
            </div>
        </section>

        <!-- Partnerships Section -->
        <section id="partnerships">
            <h2 class="section-title">Partnerships</h2>
            <div class="text-block">
                <h3 style="text-align: center; color: var(--primary); margin-bottom: 1rem;">Building International Partnerships for Practical Impact</h3>
                <p style="text-align: center; margin-bottom: 1.5rem;">I collaborate with organizations and institutions across research, government, development, agriculture, climate, finance, investment, trade, and civil society.</p>
                
                <p style="margin-bottom: 0.5rem;"><strong>Potential Collaboration Partners:</strong></p>
                <div class="tag-cloud" style="margin-bottom: 2rem; justify-content: flex-start;">
                    <span class="tag">Universities & Research Institutions</span>
                    <span class="tag">Governments & Public Institutions</span>
                    <span class="tag">International Organizations</span>
                    <span class="tag">Development Partners</span>
                    <span class="tag">NGOs & Civil Society Organizations</span>
                    <span class="tag">Private-Sector Companies</span>
                    <span class="tag">Investors & Financial Institutions</span>
                    <span class="tag">Agricultural Producers & Cooperatives</span>
                    <span class="tag">Climate & Carbon-Market Organizations</span>
                    <span class="tag">International Buyers & Trading Partners</span>
                </div>

                <p style="margin-bottom: 0.5rem;"><strong>Partnership Areas:</strong></p>
                <p style="color: var(--accent); font-weight: 600;">
                    Research | Climate Action | Carbon Finance | Agriculture | Biodiversity | Investment | Trade | Innovation | Sustainable Development
                </p>
            </div>
        </section>

        <!-- Research Section -->
        <section id="research">
            <h2 class="section-title">Research</h2>
            <div class="text-block">
                <h3 style="color: var(--primary); margin-bottom: 0.8rem;">Research for Resilient Food Systems and Communities</h3>
                <p style="margin-bottom: 1.2rem;">My research interests focus on the relationship between: <strong>Animal Science | Genetics | Agriculture | Climate Resilience | Biodiversity | Sustainable Land Use | Community Development</strong></p>
                <p style="margin-bottom: 1.5rem;">The objective is to translate research and evidence into practical solutions that can benefit farmers, communities, institutions, businesses, and development partners.</p>
                
                <h4 style="color: var(--primary); margin-bottom: 0.8rem;">Research Interests</h4>
                <div class="tag-cloud" style="justify-content: flex-start;">
                    <span class="tag">Animal Breeding & Genetics</span>
                    <span class="tag">Livestock Genomics</span>
                    <span class="tag">Agricultural Innovation</span>
                    <span class="tag">Climate-Smart Agriculture</span>
                    <span class="tag">Sustainable Livestock Systems</span>
                    <span class="tag">Biodiversity & Genetic Resources</span>
                    <span class="tag">Agroecology</span>
                    <span class="tag">Climate Resilience</span>
                    <span class="tag">Sustainable Development</span>
                </div>
            </div>
        </section>

        <!-- Strategic Projects & Initiatives Section -->
        <section id="projects">
            <h2 class="section-title">Projects & Initiatives</h2>
            <div class="text-block">
                <p style="margin-bottom: 1.5rem;">My current project interests and initiatives focus on translating ideas into practical, scalable solutions.</p>
                <div class="grid">
                    <div class="card" style="border-top-color: var(--accent-light);">
                        <h3>Climate & Carbon</h3>
                        <p>Carbon-credit development, climate finance, mitigation, adaptation, and climate-resilient development.</p>
                    </div>
                    <div class="card" style="border-top-color: var(--accent-light);">
                        <h3>Agriculture & Livestock</h3>
                        <p>Sustainable livestock systems, animal genetic improvement, climate-smart agriculture, and resilient food systems.</p>
                    </div>
                    <div class="card" style="border-top-color: var(--accent-light);">
                        <h3>Nature & Biodiversity</h3>
                        <p>Biodiversity conservation, agroforestry, ecosystem restoration, and nature-based solutions.</p>
                    </div>
                    <div class="card" style="border-top-color: var(--accent-light);">
                        <h3>Coffee & International Trade</h3>
                        <p>Sustainable coffee production, value-chain development, export, international market linkage, and agricultural investment.</p>
                    </div>
                    <div class="card" style="border-top-color: var(--accent-light); grid-column: 1 / -1;">
                        <h3>Inclusive Community & Youth Development</h3>
                        <p>Inclusive development, youth empowerment, women's economic participation, capacity building, and community-based initiatives. Supporting approaches that create opportunities for youth, women, farmers, communities, researchers, institutions, and private-sector partners.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Collaboration Section -->
        <section>
            <h2 class="section-title">Collaboration</h2>
            <div class="text-block" style="text-align: center;">
                <h3 style="color: var(--primary); font-size: 1.4rem; margin-bottom: 1rem;">Let's Turn Ideas Into Impact</h3>
                <p style="margin-bottom: 1.5rem;">I am open to strategic collaboration with organizations and individuals seeking to develop credible, practical, scalable, and sustainable solutions.</p>
                
                <p style="margin-bottom: 0.8rem;"><strong>Potential areas of collaboration:</strong></p>
                <div class="tag-cloud">
                    <span class="tag">Research Collaboration</span>
                    <span class="tag">Strategic Partnerships</span>
                    <span class="tag">Climate & Carbon Finance</span>
                    <span class="tag">Agricultural Investment</span>
                    <span class="tag">Nature & Biodiversity Projects</span>
                    <span class="tag">Sustainable Development Initiatives</span>
                    <span class="tag">International Trade</span>
                </div>
            </div>
        </section>

    </div>

    <!-- Contacts & Footer -->
    <footer id="contact">
        <h2 style="font-size: 1.6rem; margin-bottom: 1rem; color: #ffffff;">Let's Connect</h2>
        <p style="margin-bottom: 0.5rem; font-size: 1rem;">
            <strong>Email:</strong> <a href="mailto:hailshtilahun@gmail.com">hailshtilahun@gmail.com</a>
        </p>
        <p style="margin-bottom: 1.5rem; font-size: 1rem;">
            <strong>WhatsApp / Mobile:</strong> <a href="tel:+251910204390">+251 910 204 390</a>
        </p>

        <!-- Social Media Links -->
        <p class="footer-social-title">Follow Me</p>
        <div class="social-grid">
            <a href="https://linkedin.com/in/YOUR-LINKEDIN-USERNAME" target="_blank" class="social-btn linkedin">LinkedIn</a>
            <a href="https://wa.me/251910204390" target="_blank" class="social-btn whatsapp">WhatsApp</a>
            <a href="https://instagram.com/YOUR-INSTAGRAM-USERNAME" target="_blank" class="social-btn instagram">Instagram</a>
            <a href="https://t.me/YOUR-TELEGRAM-USERNAME" target="_blank" class="social-btn telegram">Telegram</a>
            <a href="https://facebook.com/YOUR-FACEBOOK-USERNAME" target="_blank" class="social-btn facebook">Facebook</a>
            <a href="https://twitter.com/YOUR-TWITTER-USERNAME" target="_blank" class="social-btn twitter">X</a>
        </div>

        <p style="margin-top: 1.5rem; font-size: 0.85rem; opacity: 0.8;">&copy; 2026 Hailu Tilahun Kebede. All Rights Reserved.</p>
    </footer>

</body>
</html>
