<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Portfolio of Sureshkumar Kaneriya - Quality & Technical Inspection Professional">
    <title>Sureshkumar Kaneriya | Professional Portfolio</title>
    
    <!-- Google Fonts & Icons -->
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Plus Jakarta Sans', sans-serif;
        }

        /* Premium Dark Theme with subtle gradient */
        body {
            background: radial-gradient(circle at top left, #0f172a, #0b0f19, #05070e);
            color: #cbd5e1;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: flex-start;
            padding: 40px 20px;
        }

        /* Grid Layout */
        .portfolio-container {
            max-width: 1150px;
            width: 100%;
            display: grid;
            grid-template-columns: 340px 1fr;
            gap: 30px;
            align-items: start;
        }

        /* Left Glass Sidebar */
        .sidebar-card {
            background: rgba(15, 23, 42, 0.75);
            backdrop-filter: blur(12px);
            text-align: center;
            padding: 40px 24px;
            border-radius: 20px;
            border: 1px solid rgba(56, 189, 248, 0.15);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.6);
            position: sticky;
            top: 40px;
        }

        /* Larger Photo Frame */
        .photo-wrapper {
            margin-bottom: 22px;
            display: inline-block;
            position: relative;
        }

        .photo-wrapper img {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            border: 4px solid #38bdf8;
            box-shadow: 0 0 35px rgba(56, 189, 248, 0.4);
            object-fit: cover;
        }

        .sidebar-card h1 {
            color: #f8fafc;
            font-size: 1.4rem;
            font-weight: 700;
            margin-bottom: 6px;
            letter-spacing: 0.5px;
            line-height: 1.2;
        }

        .sidebar-card .subtitle {
            color: #38bdf8;
            font-size: 0.88rem;
            font-weight: 600;
            margin-bottom: 14px;
            line-height: 1.4;
        }

        .sidebar-card .location {
            color: #94a3b8;
            font-size: 0.85rem;
            background-color: rgba(30, 41, 59, 0.8);
            padding: 6px 14px;
            border-radius: 20px;
            display: inline-block;
            margin-bottom: 22px;
            border: 1px solid rgba(255,255,255,0.05);
        }

        /* Action Buttons */
        .sidebar-actions {
            display: flex;
            flex-direction: column;
            gap: 12px;
        }

        .btn {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            padding: 12px 18px;
            border-radius: 10px;
            text-decoration: none;
            font-weight: 600;
            font-size: 0.9rem;
            transition: all 0.3s ease;
        }

        .btn-primary {
            background: linear-gradient(135deg, #0284c7, #0369a1);
            color: #ffffff;
            box-shadow: 0 4px 15px rgba(2, 132, 199, 0.3);
        }

        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(2, 132, 199, 0.5);
        }

        .btn-secondary {
            background: rgba(30, 41, 59, 0.8);
            color: #38bdf8;
            border: 1px solid rgba(56, 189, 248, 0.2);
        }

        .btn-secondary:hover {
            background: rgba(51, 65, 85, 0.8);
            transform: translateY(-2px);
        }

        /* Right Content Area */
        .content-area {
            display: flex;
            flex-direction: column;
            gap: 22px;
        }

        .card-section {
            background: rgba(15, 23, 42, 0.7);
            backdrop-filter: blur(10px);
            padding: 26px;
            border-radius: 18px;
            border: 1px solid rgba(255, 255, 255, 0.05);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
        }

        .about-card { border-left: 4px solid #38bdf8; }
        .skills-card { border-left: 4px solid #eab308; }
        .exp-card { border-left: 4px solid #a855f7; }
        .edu-card { border-left: 4px solid #ec4899; }
        .cert-card { border-left: 4px solid #10b981; }

        .card-section h2 {
            font-size: 1.2rem;
            margin-bottom: 16px;
            font-weight: 700;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .about-card h2 { color: #38bdf8; }
        .skills-card h2 { color: #eab308; }
        .exp-card h2 { color: #a855f7; }
        .edu-card h2 { color: #ec4899; }
        .cert-card h2 { color: #10b981; }

        .card-section p {
            line-height: 1.6;
            font-size: 0.95rem;
            color: #cbd5e1;
        }

        /* Skill Chips */
        .skills-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }

        .skill-badge {
            background: rgba(30, 41, 59, 0.9);
            color: #e2e8f0;
            padding: 6px 14px;
            border-radius: 20px;
            border: 1px solid rgba(255, 255, 255, 0.08);
            font-size: 0.85rem;
            font-weight: 500;
        }

        /* Work Experience Items */
        .exp-item {
            position: relative;
            padding-left: 20px;
            border-left: 2px solid #1e293b;
            margin-bottom: 20px;
        }

        .exp-item:last-child {
            margin-bottom: 0;
        }

        .exp-item::before {
            content: '';
            position: absolute;
            left: -6px;
            top: 4px;
            width: 10px;
            height: 10px;
            border-radius: 50%;
            background: #a855f7;
        }

        .exp-title {
            color: #f8fafc;
            font-size: 1rem;
            font-weight: 600;
        }

        .exp-company {
            color: #38bdf8;
            font-size: 0.88rem;
            margin: 2px 0;
            font-weight: 500;
        }

        .exp-duration {
            color: #64748b;
            font-size: 0.8rem;
            margin-bottom: 8px;
        }

        .exp-bullets {
            padding-left: 16px;
            color: #94a3b8;
            font-size: 0.88rem;
            line-height: 1.6;
        }

        /* Compact Grid for Education & Certs */
        .compact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 14px;
        }

        .compact-box {
            background: rgba(30, 41, 59, 0.5);
            padding: 14px;
            border-radius: 10px;
            border: 1px solid rgba(255, 255, 255, 0.05);
        }

        .compact-box h4 {
            color: #f8fafc;
            font-size: 0.92rem;
            font-weight: 600;
            margin-bottom: 4px;
        }

        .compact-box p {
            font-size: 0.84rem;
            color: #94a3b8;
            margin: 0;
        }

        /* Responsive Layout */
        @media (max-width: 850px) {
            .portfolio-container {
                grid-template-columns: 1fr;
            }

            .sidebar-card {
                position: static;
            }
        }
    </style>
</head>
<body>

    <main class="portfolio-container">

        <!-- LEFT SIDE: Profile Card -->
        <aside class="sidebar-card">
            <div class="photo-wrapper">
                <img src="my.jpg" alt="Sureshkumar Kaneriya" onerror="this.src='https://placehold.co/180x180/0f172a/38bdf8?text=SK'">
            </div>
            
            <h1>SURESHKUMAR KANERIYA</h1>
            <p class="subtitle">Quality & Technical Inspection Professional<br>Solar PV Manufacturing</p>
            <p class="location"><i class="fa-solid fa-location-dot" style="color: #ef4444;"></i> Surat, Gujarat, India</p>

            <div class="sidebar-actions">
                <a href="mailto:ksuresh0261@gmail.com" class="btn btn-primary"><i class="fa-solid fa-paper-plane"></i> Contact Me</a>
                <a href="tel:+918320256171" class="btn btn-secondary"><i class="fa-solid fa-phone"></i> +91 83202 56171</a>
                <a href="https://www.linkedin.com/in/sureshkumar-k-34267719a" target="_blank" rel="noopener noreferrer" class="btn btn-secondary"><i class="fa-brands fa-linkedin"></i> LinkedIn Profile ↗</a>
            </div>
        </aside>

        <!-- RIGHT SIDE: Resume Information -->
        <div class="content-area">

            <!-- Profile Summary -->
            <section class="card-section about-card">
                <h2><i class="fa-solid fa-user-check"></i> Profile Summary</h2>
                <p>
                    Results-driven Quality & Technical Inspection professional with <b>7+ years of experience</b> in Solar PV module manufacturing, IPQC/PDI management, and third-party inspections. Managed quality inspection programs for <b>500+ MW</b> of solar projects. Experienced in IEC 61215/61730 standards, ISO/IEC 17020 compliance, and drone thermography using Agisoft Metashape & QGIS.
                </p>
            </section>

            <!-- Core Competencies -->
            <section class="card-section skills-card">
                <h2><i class="fa-solid fa-gears"></i> Core Competencies</h2>
                <div class="skills-grid">
                    <span class="skill-badge">IPQC & PDI Inspection</span>
                    <span class="skill-badge">IEC 61215 / IEC 61730</span>
                    <span class="skill-badge">ISO/IEC 17020 & NABCB</span>
                    <span class="skill-badge">Vendor Evaluation</span>
                    <span class="skill-badge">Inline & FQC Inspection</span>
                    <span class="skill-badge">BOM Verification</span>
                    <span class="skill-badge">Drone Thermography</span>
                    <span class="skill-badge">Agisoft Metashape & QGIS</span>
                    <span class="skill-badge">Defect Analysis</span>
                    <span class="skill-badge">SOP Development</span>
                </div>
            </section>

            <!-- Experience -->
            <section class="card-section exp-card">
                <h2><i class="fa-solid fa-briefcase"></i> Work Experience</h2>
                
                <div class="exp-item">
                    <div class="exp-title">Assistant Manager – Technical Inspection</div>
                    <div class="exp-company">JSR Photonics LLP, Surat</div>
                    <div class="exp-duration">Oct 2024 – Present</div>
                    <ul class="exp-bullets">
                        <li>Managed Solar PV module IPQC, inline inspection, and PDI for 500+ MW projects.</li>
                        <li>Lead customer/OEM coordination, vendor evaluations, and SOP development.</li>
                        <li>Executed drone thermography plant inspections using Agisoft Metashape & QGIS.</li>
                    </ul>
                </div>

                <div class="exp-item">
                    <div class="exp-title">Jr. Engineer – Quality Department</div>
                    <div class="exp-company">Goldi Solar Pvt. Ltd., Surat</div>
                    <div class="exp-duration">Feb 2022 – Oct 2024</div>
                    <ul class="exp-bullets">
                        <li>Conducted process audits, defect analysis, and module reliability testing.</li>
                        <li>Managed ISO documentation, DQRs, and Final Quality Control (FQC).</li>
                    </ul>
                </div>

                <div class="exp-item">
                    <div class="exp-title">Quality Engineer – Merlin Dept.</div>
                    <div class="exp-company">Waaree Energies Ltd., Surat</div>
                    <div class="exp-duration">Feb 2019 – Feb 2022</div>
                    <ul class="exp-bullets">
                        <li>Inspected flexible & foldable Solar PV modules manufactured using Merlin technology.</li>
                    </ul>
                </div>

                <div class="exp-item">
                    <div class="exp-title">Trainee Engineer – Quality Dept.</div>
                    <div class="exp-company">Sonali Solar Pvt. Ltd., Surat</div>
                    <div class="exp-duration">Jul 2018 – Dec 2018</div>
                    <ul class="exp-bullets">
                        <li>Handled Line QC, EL testing, visual inspection, and daily quality records.</li>
                    </ul>
                </div>
            </section>

            <!-- Licenses & Education -->
            <section class="card-section edu-card">
                <h2><i class="fa-solid fa-graduation-cap"></i> Education & Licenses</h2>
                <div class="compact-grid">
                    <div class="compact-box">
                        <h4>B.E. in Electrical Engineering</h4>
                        <p>CKPCET, Surat (GTU) | CGPA: 7.81 (2016)</p>
                    </div>
                    <div class="compact-box">
                        <h4>Electrical Supervisor Permit</h4>
                        <p>Approved by Govt. of Gujarat (Feb 2020)</p>
                    </div>
                    <div class="compact-box">
                        <h4>ISO/IEC 17020 Certification</h4>
                        <p>Inspection Body Requirements & Audits</p>
                    </div>
                    <div class="compact-box">
                        <h4>HSC (12th) & SSC (10th)</h4>
                        <p>GSEB | 12th: 63% | 10th: 73%</p>
                    </div>
                </div>
            </section>

            <!-- Projects & Industrial Training -->
            <section class="card-section cert-card">
                <h2><i class="fa-solid fa-diagram-project"></i> Key Projects & Training</h2>
                <div class="compact-grid">
                    <div class="compact-box">
                        <h4>B.E. Final Year Project</h4>
                        <p>Microcontroller-Based Prototype of Underground Fault Detector</p>
                    </div>
                    <div class="compact-box">
                        <h4>Industrial Internships</h4>
                        <p>Utran Power Plant & Surat District Milk Producers Union</p>
                    </div>
                </div>
            </section>

        </div>

    </main>

</body>
</html>
