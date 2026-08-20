<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Portfolio of Sureshkumar Kaneriya - Quality & Technical Inspection Professional">
    <title>Sureshkumar Kaneriya | Portfolio</title>
    
    <!-- Google Fonts & Font Awesome Icons -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Inter', sans-serif;
        }

        /* Full Screen Dark Background */
        body {
            background-color: #0b0f19;
            color: #cbd5e1;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 40px 20px;
        }

        /* Main Container - Side by Side Grid Layout */
        .portfolio-container {
            max-width: 1050px;
            width: 100%;
            display: grid;
            grid-template-columns: 320px 1fr; /* Left Sidebar: 320px, Right Content: Remaining space */
            gap: 30px;
            align-items: start;
        }

        /* Left Side Profile Card */
        .sidebar-card {
            background: linear-gradient(145deg, #111827, #0f172a);
            text-align: center;
            padding: 35px 25px;
            border-radius: 16px;
            border: 1px solid #1e293b;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
            position: sticky;
            top: 40px;
        }

        /* Photo Styling with Glow */
        .photo-wrapper {
            margin-bottom: 20px;
            display: inline-block;
        }

        .photo-wrapper img {
            width: 160px;
            height: 160px;
            border-radius: 50%;
            border: 4px solid #38bdf8;
            box-shadow: 0 0 25px rgba(56, 189, 248, 0.35);
            object-fit: cover;
        }

        .sidebar-card h1 {
            color: #38bdf8;
            font-size: 1.5rem;
            font-weight: 700;
            margin-bottom: 8px;
            letter-spacing: 0.5px;
            line-height: 1.2;
        }

        .sidebar-card .subtitle {
            color: #94a3b8;
            font-size: 0.95rem;
            font-weight: 500;
            margin-bottom: 15px;
            line-height: 1.4;
        }

        .sidebar-card .location {
            color: #cbd5e1;
            font-size: 0.9rem;
            background-color: #1e293b;
            padding: 6px 12px;
            border-radius: 20px;
            display: inline-block;
            margin-bottom: 20px;
        }

        /* Social Link Buttons */
        .sidebar-actions {
            display: flex;
            flex-direction: column;
            gap: 10px;
        }

        .btn {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
            padding: 10px 16px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 600;
            font-size: 0.9rem;
            transition: all 0.2s ease;
        }

        .btn-primary {
            background-color: #0284c7;
            color: #ffffff;
        }

        .btn-primary:hover {
            background-color: #0369a1;
        }

        .btn-secondary {
            background-color: #1e293b;
            color: #38bdf8;
            border: 1px solid #334155;
        }

        .btn-secondary:hover {
            background-color: #334155;
        }

        /* Right Side Content Section */
        .content-area {
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        .card-section {
            background-color: #0f172a;
            padding: 25px;
            border-radius: 14px;
            border: 1px solid #1e293b;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
        }

        .about-card { border-left: 5px solid #38bdf8; }
        .projects-card { border-left: 5px solid #a855f7; }
        .contact-card { border-left: 5px solid #10b981; }

        .card-section h2 {
            font-size: 1.25rem;
            margin-bottom: 12px;
            font-weight: 600;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .about-card h2 { color: #38bdf8; }
        .projects-card h2 { color: #a855f7; }
        .contact-card h2 { color: #10b981; }

        .card-section p {
            line-height: 1.7;
            font-size: 0.98rem;
        }

        /* Contact Details List */
        .contact-list {
            list-style: none;
            line-height: 2.2;
            font-size: 0.98rem;
        }

        .contact-list li {
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .contact-list i {
            width: 20px;
            color: #10b981;
        }

        .contact-list a {
            color: #38bdf8;
            text-decoration: none;
            font-weight: 500;
        }

        .contact-list a:hover {
            text-decoration: underline;
        }

        /* Responsive Layout for Mobile Devices */
        @media (max-width: 850px) {
            .portfolio-container {
                grid-template-columns: 1fr; /* Switch to single column on small screens */
            }

            .sidebar-card {
                position: static;
            }
        }
    </style>
</head>
<body>

    <main class="portfolio-container">

        <!-- LEFT SIDE: Profile Sidebar -->
        <aside class="sidebar-card">
            <div class="photo-wrapper">
                <img src="my.jpg" alt="Sureshkumar Kaneriya" onerror="this.src='https://placehold.co/160x160/0f172a/38bdf8?text=SK'">
            </div>
            
            <h1>SURESHKUMAR KANERIYA</h1>
            <p class="subtitle">Quality & Technical Inspection Professional | Solar PV Manufacturing</p>
            <p class="location"><i class="fa-solid fa-location-dot" style="color: #ef4444;"></i> Surat, Gujarat, India</p>

            <div class="sidebar-actions">
                <a href="mailto:ksuresh0261@gmail.com" class="btn btn-primary"><i class="fa-solid fa-envelope"></i> Contact Me</a>
                <a href="https://www.linkedin.com/in/sureshkumar-k-34267719a" target="_blank" rel="noopener noreferrer" class="btn btn-secondary"><i class="fa-brands fa-linkedin"></i> LinkedIn Profile ↗</a>
            </div>
        </aside>

        <!-- RIGHT SIDE: Main Content -->
        <div class="content-area">

            <!-- About Me Section -->
            <section class="card-section about-card">
                <h2><i class="fa-solid fa-user-check"></i> About Me</h2>
                <p>
                    Quality & Technical Inspection Professional with <b style="color: #f8fafc;">5+ years of experience</b> in Solar PV module manufacturing, IPQC, PDI, and third-party inspection. Skilled in quality assurance, IEC standards compliance, and vendor evaluation.
                </p>
            </section>

            <!-- Projects / Experience Section -->
            <section class="card-section projects-card" id="projects">
                <h2><i class="fa-solid fa-briefcase"></i> Experience & Key Projects</h2>
                <p>
                    Specialized in Solar PV Module Quality Assurance, IPQC, Factory Acceptance Testing (FAT), Pre-Dispatch Inspection (PDI), and Compliance Testing as per IEC 61215 / IEC 61730 standards.
                </p>
            </section>

            <!-- Contact Details Section -->
            <section class="card-section contact-card">
                <h2><i class="fa-solid fa-address-book"></i> Contact Details</h2>
                <ul class="contact-list">
                    <li>
                        <i class="fa-solid fa-phone"></i>
                        <b style="color: #f8fafc;">Phone:</b>
                        <a href="tel:+918320256171">+91 83202 56171</a>
                    </li>
                    <li>
                        <i class="fa-solid fa-envelope"></i>
                        <b style="color: #f8fafc;">Email:</b>
                        <a href="mailto:ksuresh0261@gmail.com">ksuresh0261@gmail.com</a>
                    </li>
                    <li>
                        <i class="fa-brands fa-linkedin"></i>
                        <b style="color: #f8fafc;">LinkedIn:</b>
                        <a href="https://www.linkedin.com/in/sureshkumar-k-34267719a" target="_blank" rel="noopener noreferrer">Sureshkumar Kaneriya Profile ↗</a>
                    </li>
                </ul>
            </section>

        </div>

    </main>

</body>
</html>
