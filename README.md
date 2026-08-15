<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Animal Scientist | Climate & Sustainable Development Specialist</title>
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
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 1rem 1.5rem;
        }

        .nav-links {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 1rem;
        }

        .nav-links a {
            color: #d8f3dc;
            text-decoration: none;
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
            padding: 4.5rem 1.5rem;
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
            font-size: 1.8rem;
            color: var(--accent-light);
            font-weight: 700;
            margin-bottom: 0.8rem;
        }

        .hero h2 {
            font-size: 1.3rem;
            color: #ffffff;
            font-weight: 600;
            margin-bottom: 1.2rem;
        }

        .hero p {
            font-size: 1.05rem;
            color: #e8f5e9;
            line-height: 1.7;
            margin-bottom: 1.5rem;
        }

        .btn-group {
            display: flex;
            gap: 1rem;
            justify-content: center;
            flex-wrap: wrap;
            margin-top: 2rem;
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

        /* Container Layout */
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

        .subtitle {
            text-align: center;
            color: var(--accent);
            font-size: 1.1rem;
            font-weight: 600;
            margin-top: -1.2rem;
            margin-bottom: 2rem;
        }

        /* Cards and Grids */
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

        /* Tables */
        .styled-table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 1rem;
            box-shadow: var(--shadow);
            border-radius: 8px;
            overflow: hidden;
            background: var(--card-bg);
        }

        .styled-table th, .styled-table td {
            padding: 1rem 1.2rem;
            text-align: left;
        }

        .styled-table th {
            background-color: var(--primary);
            color: #ffffff;
            font-weight: 600;
        }

        .styled-table tr:nth-child(even) {
            background-color: var(--light-bg);
        }

        .styled-table tr {
            border-bottom: 1px solid var(--border);
        }

        /* Flow Process */
        .process-flow {
            display: flex;
            justify-content: center;
            align-items: center;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin: 1.5rem 0;
            font-weight: 600;
            color: var(--primary);
        }

        .process-step {
            background: #e8f5e9;
            padding: 0.5rem 1rem;
            border-radius: 6px;
            border: 1px solid var(--border);
        }

        /* Footer & Social Media */
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
                <a href="#impact">Impact</a>
                <a href="#projects">Projects</a>
                <a href="#partnerships">Partnerships</a>
                <a href="#funding">Funding & Investment</a>
                <a href="#research">Research</a>
                <a href="#contact">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Hero Header -->
    <header class="hero" id="home">
        <div class="hero-container">
            <img src="photo_2025-11-24_14-14-04.jpg" alt="Profile Photo" class="profile-img">
            <h1>Animal Scientist | Researcher</h1>
            <h2>Climate & Sustainable Development Specialist</h2>
            <p><strong>Connecting Science, Nature, Finance & Markets for Sustainable Development</strong></p>
            <p style="max-width: 800px; margin: 0 auto;">
                I work at the intersection of animal science, sustainable agriculture, climate action, biodiversity conservation, carbon finance, sustainable development, and international markets. My work connects scientific research, local implementation, project development, finance, and international partnerships to advance practical and scalable solutions for climate resilience, sustainable livelihoods, ecosystem restoration, agricultural development, and inclusive economic opportunity.
            </p>
            <p style="max-width: 800px; margin: 1rem auto 0; font-size: 0.95rem; opacity: 0.9;">
                I collaborate with international foundations, donors, grant makers, NGOs, development agencies, investors, research institutions, governments, and private-sector partners seeking credible and sustainable pathways to measurable impact.
            </p>
            <div class="btn-group">
                <a href="#contact" class="btn btn-primary">Partnership Inquiries</a>
                <a href="#funding" class="btn btn-outline">Funding & Investment</a>
            </div>
        </div>
    </header>

    <div class="container">

        <!-- About Section -->
        <section id="about">
            <h2 class="section-title">About</h2>
            <div class="subtitle">From Science to Sustainable Impact</div>
            <div class="text-block">
                <p style="margin-bottom: 1.2rem;">
                    <strong>Hailu Tilahun Kebede</strong> is an Animal Scientist and Researcher with an MSc in Animal Breeding and Genetics and over eight years of experience in livestock research, academic instruction, and community-based development. His professional journey has expanded from animal science and livestock research into an integrated development approach connecting:
                </p>
                <div class="tag-cloud" style="margin-bottom: 1.5rem;">
                    <span class="tag">Science</span>
                    <span class="tag">Agriculture</span>
                    <span class="tag">Climate</span>
                    <span class="tag">Nature</span>
                    <span class="tag">Finance</span>
                    <span class="tag">Markets</span>
                    <span class="tag">Communities</span>
                </div>
                <p style="margin-bottom: 1.2rem;">
                    This multidisciplinary perspective supports solutions addressing interconnected challenges including climate change, food security, biodiversity loss, agricultural productivity, sustainable livelihoods, rural development, and access to international markets.
                </p>
                <p style="margin-bottom: 1.5rem;">
                    The focus is on connecting knowledge, resources, partnerships, and implementation to develop solutions that are practical, inclusive, scalable, and capable of generating measurable environmental, social, and economic value.
                </p>

                <div class="grid" style="margin-top: 2rem;">
                    <div style="background: var(--light-bg); padding: 1.5rem; border-radius: 6px; border-left: 4px solid var(--accent);">
                        <h3 style="color: var(--primary); margin-bottom: 0.5rem;">Mission</h3>
                        <p style="font-size: 0.95rem;">To connect science, innovation, finance, partnerships, and communities to advance sustainable solutions that strengthen resilience, protect nature, improve livelihoods, and create long-term economic and social value.</p>
                    </div>
                    <div style="background: var(--light-bg); padding: 1.5rem; border-radius: 6px; border-left: 4px solid var(--accent);">
                        <h3 style="color: var(--primary); margin-bottom: 0.5rem;">Vision</h3>
                        <p style="font-size: 0.95rem;">A future where science, responsible investment, sustainable finance, nature, agriculture, and international partnerships work together to create resilient communities, healthy ecosystems, and inclusive prosperity.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Why Partner Section -->
        <section>
            <h2 class="section-title">Why Partner</h2>
            <div class="subtitle">Connecting Local Potential With Global Opportunity</div>
            <p style="text-align: center; margin-bottom: 2rem;">
                High-impact development requires more than financial resources. It requires technical expertise, local knowledge, strong partnerships, project development capacity, implementation capability, and long-term commitment. My approach brings these elements together.
            </p>
            <div class="grid">
                <div class="card">
                    <h3>Scientific & Technical Expertise</h3>
                    <p>A professional foundation in animal science, breeding, genetics, genomics, agricultural research, and sustainable production systems.</p>
                </div>
                <div class="card">
                    <h3>Climate & Sustainability</h3>
                    <p>A multidisciplinary focus encompassing climate mitigation, adaptation, climate-smart agriculture, biodiversity, agroforestry, ecosystem restoration, carbon markets, and climate finance.</p>
                </div>
                <div class="card">
                    <h3>Community & Inclusion</h3>
                    <p>A strong commitment to smallholder farmers, communities, youth, women, sustainable livelihoods, and inclusive development.</p>
                </div>
                <div class="card">
                    <h3>Project Development</h3>
                    <p>Supporting the transformation of ideas into structured projects, partnerships, funding opportunities, investment concepts, and scalable initiatives.</p>
                </div>
                <div class="card">
                    <h3>International Collaboration</h3>
                    <p>Building connections among local institutions, communities, researchers, investors, donors, development organizations, businesses, and international partners.</p>
                </div>
                <div class="card">
                    <h3>Impact Orientation</h3>
                    <p>A commitment to solutions that generate measurable environmental, social, and economic outcomes.</p>
                </div>
            </div>
        </section>

        <!-- At a Glance Section -->
        <section>
            <h2 class="section-title">At a Glance</h2>
            <div class="grid">
                <div style="background: var(--card-bg); padding: 1.2rem; border-radius: 6px; border-left: 3px solid var(--accent); box-shadow: var(--shadow);">
                    <strong>Science & Genetics:</strong> Animal breeding, livestock genetics, genomics, GWAS, genetic-resource conservation, and sustainable livestock systems.
                </div>
                <div style="background: var(--card-bg); padding: 1.2rem; border-radius: 6px; border-left: 3px solid var(--accent); box-shadow: var(--shadow);">
                    <strong>Climate & Carbon:</strong> Carbon-credit development, climate finance, climate mitigation and adaptation, climate-smart agriculture, and climate resilience.
                </div>
                <div style="background: var(--card-bg); padding: 1.2rem; border-radius: 6px; border-left: 3px solid var(--accent); box-shadow: var(--shadow);">
                    <strong>Nature & Biodiversity:</strong> Biodiversity conservation, agroforestry, ecosystem restoration, regenerative agriculture, and nature-based solutions.
                </div>
                <div style="background: var(--card-bg); padding: 1.2rem; border-radius: 6px; border-left: 3px solid var(--accent); box-shadow: var(--shadow);">
                    <strong>Agriculture & Food Systems:</strong> Sustainable agriculture, agroecology, resilient food systems, agricultural value chains, and community-based production.
                </div>
                <div style="background: var(--card-bg); padding: 1.2rem; border-radius: 6px; border-left: 3px solid var(--accent); box-shadow: var(--shadow);">
                    <strong>Coffee & Global Markets:</strong> Sustainable coffee production, value-chain development, export, international market linkage, and agricultural investment.
                </div>
                <div style="background: var(--card-bg); padding: 1.2rem; border-radius: 6px; border-left: 3px solid var(--accent); box-shadow: var(--shadow);">
                    <strong>Inclusive Development:</strong> Youth empowerment, women's economic participation, community development, capacity building, and sustainable livelihoods.
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
                        <li>Agricultural Value Chains</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>05 — Coffee & International Trade</h3>
                    <ul>
                        <li>Sustainable Coffee Production</li>
                        <li>Coffee Value Chains</li>
                        <li>Coffee Export</li>
                        <li>International Market Linkage</li>
                        <li>Agricultural Investment</li>
                        <li>International Trade Partnerships</li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- Areas of Impact Section -->
        <section id="impact">
            <h2 class="section-title">Areas of Impact</h2>
            <div class="grid">
                <div class="card">
                    <h3>Climate Action & Resilience</h3>
                    <p>Developing approaches that connect climate action, adaptation, resilience, and sustainable finance to strengthen communities and productive systems facing climate-related challenges.</p>
                </div>

                <div class="card">
                    <h3>Carbon Markets & Climate Finance</h3>
                    <p>Supporting the development of opportunities that connect environmental outcomes with responsible climate finance and carbon-market mechanisms, with attention to community and ecosystem benefits.</p>
                </div>

                <div class="card">
                    <h3>Biodiversity & Nature</h3>
                    <p>Advancing biodiversity conservation, agroforestry, ecosystem restoration, sustainable land management, and nature-based solutions.</p>
                </div>

                <div class="card">
                    <h3>Sustainable Agriculture</h3>
                    <p>Promoting agricultural systems that improve productivity, resilience, food security, environmental sustainability, and long-term livelihoods.</p>
                </div>

                <div class="card">
                    <h3>Livestock & Genetic Resources</h3>
                    <p>Applying animal science, genetics, genomics, and innovation to strengthen livestock productivity, genetic-resource conservation, resilience, and sustainable production.</p>
                </div>

                <div class="card">
                    <h3>Coffee & Global Markets</h3>
                    <p>Connecting Ethiopia's agricultural potential with international buyers, investors, markets, value-chain development, export, and sustainable trade.</p>
                </div>

                <div class="card">
                    <h3>Youth & Women's Economic Empowerment</h3>
                    <p>Supporting opportunities for youth and women through skills, enterprise, agriculture, innovation, employment, and sustainable livelihoods.</p>
                </div>

                <div class="card">
                    <h3>Community-Led Development</h3>
                    <p>Promoting approaches that place communities at the center of planning, implementation, ownership, and long-term sustainability.</p>
                </div>
            </div>
        </section>

        <!-- Strategic Projects Section -->
        <section id="projects">
            <h2 class="section-title">Strategic Projects</h2>
            <div class="subtitle">From Ideas to Fundable and Scalable Initiatives</div>
            <p style="text-align: center; margin-bottom: 2rem;">
                My strategic project interests focus on developing practical initiatives that can attract grants, philanthropic support, climate finance, impact investment, technical partnerships, and private-sector participation.
            </p>

            <div class="grid">
                <div class="card">
                    <h3>01 — Climate & Carbon</h3>
                    <ul>
                        <li>Carbon-credit development</li>
                        <li>Climate mitigation & adaptation</li>
                        <li>Climate-resilient livelihoods</li>
                        <li>Climate-smart agriculture</li>
                        <li>Nature-based climate solutions</li>
                        <li>Climate finance</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>02 — Biodiversity & Ecosystem Restoration</h3>
                    <ul>
                        <li>Biodiversity conservation</li>
                        <li>Agroforestry & landscape restoration</li>
                        <li>Ecosystem rehabilitation</li>
                        <li>Sustainable land management</li>
                        <li>Nature-based solutions</li>
                        <li>Community conservation</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>03 — Sustainable Agriculture & Livestock</h3>
                    <ul>
                        <li>Sustainable livestock production</li>
                        <li>Animal breeding and genetic improvement</li>
                        <li>Climate-smart agriculture</li>
                        <li>Agricultural innovation & food-system resilience</li>
                        <li>Smallholder farmer development</li>
                        <li>Sustainable agricultural value chains</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>04 — Coffee & International Trade</h3>
                    <ul>
                        <li>Sustainable coffee production</li>
                        <li>Coffee value-chain development</li>
                        <li>Quality improvement & market linkage</li>
                        <li>International trade & export development</li>
                        <li>Agricultural investment</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>05 — Youth & Women's Empowerment</h3>
                    <ul>
                        <li>Youth entrepreneurship & green jobs</li>
                        <li>Women's economic participation</li>
                        <li>Skills development & climate innovation</li>
                        <li>Sustainable livelihoods</li>
                        <li>Community enterprise</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>06 — Research & Innovation</h3>
                    <ul>
                        <li>Agricultural research & evidence-based development</li>
                        <li>Animal genetics and genomics</li>
                        <li>Climate research & sustainable systems</li>
                        <li>Technology transfer & research partnerships</li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- Partnerships Section -->
        <section id="partnerships">
            <h2 class="section-title">Partnerships</h2>
            <div class="subtitle">Building International Partnerships for Practical Impact</div>
            <div class="text-block" style="margin-bottom: 2rem;">
                <p style="text-align: center; margin-bottom: 1rem;">
                    Strong development outcomes emerge when local knowledge, scientific expertise, financial resources, technology, institutional capacity, and international networks work together.
                </p>
                <p style="text-align: center; color: var(--primary); font-weight: 700;">
                    Partnerships Built On: Trust | Transparency | Evidence | Inclusion | Innovation | Accountability | Long-Term Impact
                </p>
            </div>

            <h3 style="color: var(--primary); text-align: center; margin-bottom: 1rem;">Partners & Stakeholders</h3>
            <div class="tag-cloud" style="margin-bottom: 3rem;">
                <span class="tag">International Foundations</span>
                <span class="tag">Donors & Grant Makers</span>
                <span class="tag">Development Agencies</span>
                <span class="tag">NGOs & Civil Society</span>
                <span class="tag">Impact Investors</span>
                <span class="tag">Climate Finance Institutions</span>
                <span class="tag">Research Institutions & Universities</span>
                <span class="tag">Governments & Public Institutions</span>
                <span class="tag">Private-Sector Companies</span>
                <span class="tag">Agricultural Producers & Cooperatives</span>
                <span class="tag">Climate & Carbon-Market Organizations</span>
                <span class="tag">International Buyers & Trading Partners</span>
            </div>

            <h3 style="color: var(--primary); text-align: center; margin-bottom: 1.5rem;">Partnership Models</h3>
            <div class="grid">
                <div class="card">
                    <h3>Grant Partnership</h3>
                    <p>Collaboration on the design and implementation of grant-funded programs addressing climate, agriculture, biodiversity, livelihoods, youth, women, and community development.</p>
                </div>
                <div class="card">
                    <h3>Strategic Partnership</h3>
                    <p>Long-term collaboration combining technical expertise, local implementation capacity, international networks, and shared resources.</p>
                </div>
                <div class="card">
                    <h3>Research Partnership</h3>
                    <p>Joint work on research, innovation, field studies, publications, data, capacity building, and knowledge exchange.</p>
                </div>
                <div class="card">
                    <h3>Investment Partnership</h3>
                    <p>Exploring responsible investment opportunities in sustainable agriculture, climate solutions, carbon projects, biodiversity, nature-based solutions, and agricultural value chains, subject to appropriate due diligence.</p>
                </div>
                <div class="card">
                    <h3>Technical Partnership</h3>
                    <p>Connecting initiatives with organizations providing technology, scientific expertise, capacity building, monitoring, finance, and implementation support.</p>
                </div>
                <div class="card">
                    <h3>Market Partnership</h3>
                    <p>Connecting sustainable agricultural products and projects with international buyers, investors, distributors, and market networks.</p>
                </div>
            </div>
        </section>

        <!-- Funding & Investment Section -->
        <section id="funding">
            <h2 class="section-title">Funding & Investment</h2>
            <div class="subtitle">Strategic Funding & Investment Opportunities</div>
            <p style="text-align: center; margin-bottom: 2rem;">
                I seek to connect high-potential initiatives with appropriate grant funding, philanthropic capital, climate finance, impact investment, technical assistance, and market partnerships.
            </p>

            <h3 style="color: var(--primary); margin-bottom: 1rem;">Priority Areas</h3>
            <table class="styled-table">
                <thead>
                    <tr>
                        <th>Opportunity</th>
                        <th>Focus</th>
                        <th>Partnership Type</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td><strong>Climate & Carbon</strong></td>
                        <td>Carbon, resilience, climate finance</td>
                        <td>Grant / Climate Finance / Investment</td>
                    </tr>
                    <tr>
                        <td><strong>Biodiversity & Nature</strong></td>
                        <td>Conservation, restoration, nature-based solutions</td>
                        <td>Grant / Climate Finance</td>
                    </tr>
                    <tr>
                        <td><strong>Sustainable Agriculture</strong></td>
                        <td>Farmers, livestock, food systems</td>
                        <td>Grant / Investment</td>
                    </tr>
                    <tr>
                        <td><strong>Coffee & Value Chains</strong></td>
                        <td>Production, value chain, export</td>
                        <td>Investment / Trade</td>
                    </tr>
                    <tr>
                        <td><strong>Youth & Women</strong></td>
                        <td>Enterprise, skills, livelihoods</td>
                        <td>Grant / NGO Partnership</td>
                    </tr>
                    <tr>
                        <td><strong>Research & Innovation</strong></td>
                        <td>Genetics, agriculture, climate</td>
                        <td>Research Grant / University Partnership</td>
                    </tr>
                </tbody>
            </table>

            <div class="grid" style="margin-top: 2.5rem;">
                <div class="card">
                    <h3>For Funders & Donors</h3>
                    <p style="margin-bottom: 1rem;">Potential collaboration flow:</p>
                    <div class="process-flow">
                        <span class="process-step">Project Development</span> &rarr;
                        <span class="process-step">Proposal Development</span> &rarr;
                        <span class="process-step">Funding Partnership</span> &rarr;
                        <span class="process-step">Implementation</span> &rarr;
                        <span class="process-step">Monitoring</span> &rarr;
                        <span class="process-step">Impact</span>
                    </div>
                </div>

                <div class="card">
                    <h3>For Investors</h3>
                    <p style="margin-bottom: 1rem;">Potential opportunities flow:</p>
                    <div class="process-flow">
                        <span class="process-step">Project ID</span> &rarr;
                        <span class="process-step">Feasibility & Due Diligence</span> &rarr;
                        <span class="process-step">Structuring</span> &rarr;
                        <span class="process-step">Partnership</span> &rarr;
                        <span class="process-step">Implementation</span> &rarr;
                        <span class="process-step">Impact</span>
                    </div>
                    <p style="font-size: 0.85rem; color: var(--text-sub); margin-top: 1rem;">
                        <em>Investment opportunities should be assessed individually based on project feasibility, legal structure, financial model, risks, environmental and social safeguards, and appropriate due diligence.</em>
                    </p>
                </div>
            </div>
        </section>

        <!-- Research Section -->
        <section id="research">
            <h2 class="section-title">Research</h2>
            <div class="subtitle">Research for Resilient Food Systems and Communities</div>
            <div class="text-block">
                <p style="margin-bottom: 1.2rem;">My research interests focus on the relationship between:</p>
                <div class="tag-cloud" style="margin-bottom: 1.5rem;">
                    <span class="tag">Animal Science</span>
                    <span class="tag">Genetics</span>
                    <span class="tag">Agriculture</span>
                    <span class="tag">Climate Resilience</span>
                    <span class="tag">Biodiversity</span>
                    <span class="tag">Sustainable Land Use</span>
                    <span class="tag">Community Development</span>
                </div>
                <p style="margin-bottom: 1.5rem;">
                    The objective is to translate research, evidence, and innovation into practical solutions that can benefit farmers, communities, institutions, businesses, and development partners.
                </p>

                <h3 style="color: var(--primary); margin-bottom: 1rem;">Research Interests</h3>
                <div class="tag-cloud" style="justify-content: flex-start; margin-bottom: 2rem;">
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

                <div style="background: var(--light-bg); padding: 1.2rem; border-radius: 6px; border-left: 4px solid var(--accent);">
                    <h4 style="color: var(--primary); margin-bottom: 0.5rem;">Research Collaboration</h4>
                    <p style="font-size: 0.95rem;">
                        I welcome collaboration with universities, research institutions, scientists, development organizations, and technical partners interested in joint research, field studies, publications, innovation, capacity building, and knowledge exchange.
                    </p>
                </div>
            </div>
        </section>

        <!-- Selected Experience & Impact Section -->
        <section>
            <h2 class="section-title">Selected Experience & Impact</h2>
            <div class="subtitle">Turning Knowledge Into Action</div>
            <div class="grid" style="margin-bottom: 2rem;">
                <div class="card">
                    <h3>Professional Foundation</h3>
                    <p><strong>8+ Years</strong></p>
                    <p>Experience in animal science, livestock research, academic instruction, and community-based development.</p>
                </div>
                <div class="card">
                    <h3>Scientific Expertise</h3>
                    <p><strong>Animal Breeding & Genetics</strong></p>
                    <p>Research and technical expertise in livestock breeding, genetics, genomics, and sustainable production.</p>
                </div>
                <div class="card">
                    <h3>Climate & Sustainable Development</h3>
                    <p><strong>Integrated Practice</strong></p>
                    <p>Connecting agriculture, climate resilience, biodiversity, carbon finance, sustainable livelihoods, and development.</p>
                </div>
                <div class="card">
                    <h3>Partnership Development</h3>
                    <p><strong>Local-to-Global Collaboration</strong></p>
                    <p>Connecting communities and local opportunities with researchers, institutions, donors, investors, businesses, and international partners.</p>
                </div>
            </div>

            <div class="text-block" style="margin-bottom: 2rem; background: var(--light-bg);">
                <h3 style="color: var(--primary); margin-bottom: 0.5rem;">Impact Evidence</h3>
                <p>Additional verified achievements, project results, beneficiaries, institutional partnerships, publications, and environmental outcomes can be presented here as the evidence base is documented.</p>
            </div>

            <h3 style="color: var(--primary); text-align: center; margin-bottom: 1rem;">What I Offer</h3>
            <div class="tag-cloud">
                <span class="tag">Project Development and Design</span>
                <span class="tag">Partnership Building</span>
                <span class="tag">Research and Technical Expertise</span>
                <span class="tag">Climate and Sustainability Solutions</span>
                <span class="tag">Community Engagement and Capacity Building</span>
                <span class="tag">Investment and Market Linkage Facilitation</span>
                <span class="tag">Monitoring, Learning and Impact-Oriented Approaches</span>
            </div>
        </section>

        <!-- Collaboration Section -->
        <section>
            <h2 class="section-title">Let's Turn Ideas Into Impact</h2>
            <div class="text-block" style="text-align: center;">
                <p style="margin-bottom: 1.5rem;">
                    I welcome discussions with international donors, foundations, grant makers, NGOs, development agencies, investors, research institutions, governments, companies, and strategic partners interested in developing or supporting high-impact initiatives.
                </p>

                <h3 style="color: var(--primary); margin-bottom: 1rem;">We Can Collaborate On</h3>
                <div class="tag-cloud" style="margin-bottom: 2rem;">
                    <span class="tag">Project Development</span>
                    <span class="tag">Grant & Funding Partnerships</span>
                    <span class="tag">Climate & Carbon Finance</span>
                    <span class="tag">Impact Investment</span>
                    <span class="tag">Research & Innovation</span>
                    <span class="tag">Agricultural Development</span>
                    <span class="tag">Biodiversity & Nature-Based Solutions</span>
                    <span class="tag">International Trade & Market Linkage</span>
                    <span class="tag">Youth & Women's Economic Empowerment</span>
                    <span class="tag">Community Development</span>
                </div>

                <h4 style="color: var(--primary); margin-bottom: 0.8rem;">From Concept to Impact</h4>
                <div class="process-flow">
                    <span class="process-step">Concept</span> &rarr;
                    <span class="process-step">Project Design</span> &rarr;
                    <span class="process-step">Partnership</span> &rarr;
                    <span class="process-step">Financing</span> &rarr;
                    <span class="process-step">Implementation</span> &rarr;
                    <span class="process-step">Monitoring</span> &rarr;
                    <span class="process-step">Impact</span>
                </div>
            </div>
        </section>

    </div>

    <!-- Contacts & Footer -->
    <footer id="contact">
        <h2 style="font-size: 1.6rem; margin-bottom: 0.5rem; color: #ffffff;">Let's Build Sustainable Solutions Together</h2>
        <p style="max-width: 700px; margin: 0 auto 1.5rem; opacity: 0.9; font-size: 0.95rem;">
            If you are a donor, foundation, grant maker, NGO, development organization, investor, researcher, government institution, or private-sector partner, I welcome the opportunity to explore a potential collaboration.
        </p>

        <h3 style="color: var(--accent-light); margin-bottom: 0.8rem; font-size: 1.1rem;">Partnership Inquiries</h3>
        <p style="margin-bottom: 1.5rem; font-size: 0.92rem; opacity: 0.9;">
            For partnership, investment, grant, research, project-development, climate-finance, agricultural, biodiversity, or international market opportunities, please get in touch.
        </p>

        <div style="margin-bottom: 2rem;">
            <p style="margin-bottom: 0.5rem; font-size: 1rem;">
                <strong>Email:</strong> <a href="mailto:hailshtilahun@gmail.com">hailshtilahun@gmail.com</a>
            </p>
            <p style="margin-bottom: 1.5rem; font-size: 1rem;">
                <strong>WhatsApp / Mobile:</strong> <a href="tel:+251910204390">+251 910 204 390</a>
            </p>
        </div>

        <!-- Social Media Links -->
        <p class="footer-social-title">Follow Me</p>
        <div class="social-grid">
            <a href="https://linkedin.com" target="_blank" class="social-btn linkedin">LinkedIn</a>
            <a href="https://wa.me/251910204390" target="_blank" class="social-btn whatsapp">WhatsApp</a>
            <a href="https://instagram.com" target="_blank" class="social-btn instagram">Instagram</a>
            <a href="https://t.me" target="_blank" class="social-btn telegram">Telegram</a>
            <a href="https://facebook.com" target="_blank" class="social-btn facebook">Facebook</a>
            <a href="https://twitter.com" target="_blank" class="social-btn twitter">X</a>
        </div>

        <p style="margin-top: 1.5rem; font-size: 0.85rem; opacity: 0.8;">&copy; 2026 Hailu Tilahun Kebede. All Rights Reserved.</p>
    </footer>

</body>
</html>
