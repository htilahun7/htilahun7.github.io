<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hailu Tilahun Kebede - Personal Website</title>
    <style>
        :root {
            --primary: #1b4332;       /* Deep Forest Green */
            --accent: #2d6a4f;        /* Medium Forest Green */
            --light-green: #d8f3dc;    /* Light Green Accent */
            --bg-light: #f4f9f5;       /* Very Soft Green Tint Background */
            --text: #1d2a23;          /* Dark Slate/Greenish Text */
            --border: #b7e4c7;        /* Soft Green Border */
        }
        
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            color: var(--text);
            background-color: #ffffff;
            line-height: 1.6;
        }

        header {
            background-color: var(--primary);
            color: white;
            padding: 3rem 1.5rem;
            text-align: center;
        }

        header h1 {
            font-size: 2.2rem;
            margin-bottom: 0.5rem;
            color: #ffffff;
        }

        header p {
            font-size: 1.14rem;
            color: var(--light-green);
            font-weight: 500;
        }

        .contact-info {
            margin-top: 1rem;
            font-size: 0.95rem;
            color: #ffffff;
        }

        .contact-info a {
            color: var(--light-green);
            text-decoration: none;
            font-weight: bold;
        }

        .contact-info a:hover {
            text-decoration: underline;
        }

        nav {
            background: var(--accent);
            text-align: center;
            position: sticky;
            top: 0;
            z-index: 100;
        }

        nav a {
            color: white;
            padding: 0.8rem 1.2rem;
            text-decoration: none;
            display: inline-block;
            font-weight: 500;
            font-size: 0.95rem;
        }

        nav a:hover {
            background: #40916c;
        }

        .container {
            max-width: 900px;
            margin: 2rem auto;
            padding: 0 1.5rem;
        }

        section {
            margin-bottom: 2.5rem;
            background-color: var(--bg-light);
            padding: 1.5rem;
            border-radius: 8px;
            border-left: 5px solid var(--accent);
        }

        h2 {
            color: var(--primary);
            border-bottom: 2px solid var(--border);
            padding-bottom: 0.4rem;
            margin-bottom: 1rem;
            font-size: 1.4rem;
        }

        .item {
            margin-bottom: 1.5rem;
        }

        .item-title {
            font-weight: bold;
            font-size: 1.1rem;
            color: var(--primary);
        }

        .item-sub {
            color: #4a5d4e;
            font-style: italic;
            font-size: 0.95rem;
            margin-bottom: 0.4rem;
        }

        ul {
            list-style-type: square;
            margin-left: 1.5rem;
        }

        ul li {
            margin-bottom: 0.4rem;
        }

        .badge-list {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-top: 0.5rem;
        }

        .badge {
            background-color: #e8f5e9;
            border: 1px solid var(--border);
            color: var(--primary);
            padding: 0.4rem 0.8rem;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: bold;
        }

        footer {
            text-align: center;
            padding: 1.5rem;
            background-color: var(--primary);
            color: var(--light-green);
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

    <header>
        <h1>Hailu Tilahun Kebede</h1>
        <p>Animal Scientist (MSc) & Researcher</p>
        <div class="contact-info">
            📍 Addis Ababa, Ethiopia | 📱 (+251) 910204390 | ✉️ <a href="mailto:hailshtilahun@gmail.com">hailshtilahun@gmail.com</a>
        </div>
    </header>

    <nav>
        <a href="#about">About</a>
        <a href="#experience">Experience</a>
        <a href="#partnerships">Partnership Areas</a>
        <a href="#publications">Publications</a>
        <a href="#projects">Projects</a>
        <a href="#education">Education & Leadership</a>
    </nav>

    <div class="container">

        <!-- About Section -->
        <section id="about">
            <h2>About Me</h2>
            <p>
                I am a dedicated Animal Scientist with an MSc in Animal Breeding and Genetics and over 7 years of experience in research, academic instruction, and community development projects[cite: 1]. I specialize in bridging genomic and agricultural research with practical climate adaptation, regenerative agriculture, and inclusive community resilience[cite: 1].
            </p>
        </section>

        <!-- Experience Section -->
        <section id="experience">
            <h2>Work Experience</h2>
            
            <div class="item">
                <div class="item-title">Lecturer & Researcher</div>
                <div class="item-sub">08/07/2018 – Present</div>
                <ul>
                    <li>Academic instruction in Principles of Genetics, Animal Breeding, Research Methodology, Physiology, and Biotechnology[cite: 1].</li>
                    <li>Advanced statistical computing (SAS, SPSS) and biological data modeling using ANOVA, regression, and correlation analysis[cite: 1].</li>
                    <li>Genomic research focusing on livestock surveys and Genome-Wide Association Studies (GWAS)[cite: 1].</li>
                </ul>
            </div>

            <div class="item">
                <div class="item-title">Climate & Livestock Development Specialist</div>
                <div class="item-sub">01/01/2024 – Present</div>
                <ul>
                    <li>Lead project lifecycles, carbon credit initiatives, climate financing, and MER frameworks[cite: 1].</li>
                    <li>Design regenerative agriculture, agroecology, biodiversity restoration, and integrated organic farming initiatives[cite: 1].</li>
                    <li>Drive environmental safeguarding and gender-inclusive projects for women and youth[cite: 1].</li>
                    <li>Mobilize youth-led climate initiatives for global forums[cite: 1].</li>
                </ul>
            </div>
        </section>

        <!-- International Partnership Areas Section -->
        <section id="partnerships">
            <h2>International Partnership Areas</h2>
            <ul>
                <li><strong>Global Policy Dialogues:</strong> Official African Union (AU) Delegate at the G20 Social Summit on Climate Action & Global Inequity[cite: 1].</li>
                <li><strong>UN Sustainable Development:</strong> Official Delegate at the 12th United Nations Economic Commission for Africa (UNECA) Regional Forum[cite: 1].</li>
                <li><strong>International Climate Finance & MER:</strong> Designing frameworks for carbon credit systems, agroecology, and ecosystem restoration[cite: 1].</li>
                <li><strong>Capacity Building & Technical Transfer:</strong> Collaboration on agricultural technology transfer and community resilience strategies[cite: 1].</li>
            </ul>
        </section>

        <!-- Publications Section -->
        <section id="publications">
            <h2>Publications</h2>
            <ul>
                <li>
                    <strong>Hailu Tilahun</strong> (2023). Assessment on rearing and husbandry practices of indigenous goats in North Shewa Zone, Amhara Region, Ethiopia. <em>Journal of Applied Animal Research</em>, 51:1, 242-255[cite: 1].
                </li>
                <li>
                    Yaregal Derbie & <strong>Hailu Tilahun</strong> (2023). Phenotypic characterization of indigenous sheep breeds in the Jimma Zone, Oromia, Ethiopia. <em>Journal of Applied Animal Research</em>, 51:1, 644-652[cite: 1].
                </li>
                <li>
                    <strong>Hailu Tilahun</strong>, Aynalem Haile, Ahmed Seid (2019). Phenotypic Characterization of Indigenous Goats in North Shewa Zone, Amhara Region, Ethiopia. <em>International Journal of Research Studies in Agricultural Sciences (IJRSAS)</em>, 5(7), 44-55[cite: 1].
                </li>
            </ul>
        </section>

        <!-- Projects Section -->
        <section id="projects">
            <h2>Key Projects</h2>
            <ul>
                <li><strong>Establishment of Honeybee Farm:</strong> Principal project lead[cite: 1].</li>
                <li><strong>Model Cattle Crush Establishment:</strong> Principal lead across two districts in North Shewa Zone, Oromia[cite: 1].</li>
                <li><strong>Beekeeping & Hive Technology Assessment:</strong> Staff research project[cite: 1].</li>
                <li><strong>Estrus Synchronization & Dairy Management:</strong> Applied livestock development study[cite: 1].</li>
            </ul>
        </section>

        <!-- Education & Leadership -->
        <section id="education">
            <h2>Education & Global Delegations</h2>
            
            <div class="item">
                <div class="item-title">MSc in Animal Breeding and Genetics</div>
                <div class="item-sub">2015 – 2018</div>
            </div>

            <div class="item">
                <div class="item-title">BSc in Animal Science</div>
                <div class="item-sub">2012 – 2015</div>
            </div>

            <div class="item">
                <div class="item-title">Certifications & Leadership</div>
                <div class="badge-list">
                    <span class="badge">UNECA Delegate (2026)</span>
                    <span class="badge">AU G20 Social Summit Delegate (2025)</span>
                    <span class="badge">Udacity Data & AI Certifications</span>
                    <span class="badge">FARM to FARM Certification (USAID)</span>
                </div>
            </div>
        </section>

    </div>

    <footer>
        <p>&copy; 2026 Hailu Tilahun Kebede. All Rights Reserved.</p>
    </footer>

</body>
</html>
