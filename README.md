<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sureshkumar Kaneriya | Portfolio</title>
    <!-- Google Font & Icons -->
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
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding: 40px 20px;
        }

        /* Main Container */
        .portfolio-container {
            max-width: 800px;
            width: 100%;
        }

        /* Header Card */
        .header-card {
            background: linear-gradient(145deg, #111827, #0f172a);
            text-align: center;
            padding: 40px 20px;
            border-radius: 16px;
            border: 1px solid #1e293b;
            margin-bottom: 25px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
        }

        .header-card h1 {
            color: #38bdf8;
            font-size: 2.2rem;
            font-weight: 700;
            margin-bottom: 8px;
            letter-spacing: 0.5px;
        }

        .header-card .subtitle {
            color: #94a3b8;
            font-size: 1.1rem;
            font-weight: 600;
            margin-bottom: 6px;
        }

        .header-card .location {
            color: #cbd5e1;
            font-size: 0.95rem;
        }

        /* Photo Styling with Glow Effect */
        .photo-wrapper {
            margin: 25px 0 15px 0;
            display: inline-block;
        }

        .photo-wrapper img {
            width: 210px;
            height: 210px;
            border-radius: 50%;
            border: 4px solid #38bdf8;
            box-shadow: 0 0 30px rgba(56, 189, 248, 0.35);
            object-fit: cover;
        }

        /* Content Sections */
        .card-section {
            background-color: #0f172a;
            padding: 25px;
            border-radius: 14px;
            border-top: 1px solid #1e293b;
            border-right: 1px solid #1e293b;
            border-bottom: 1px solid #1e293b;
            margin-bottom: 20px;
            box-shadow: 0 4px 20px rgba(0,0,0,0.3);
        }

        .about-card {
            border-left: 5px solid #38bdf8;
        }

        .contact-card {
            border-left: 5px solid #10b981;
        }

        .card-section h3 {
            font-size: 1.3rem;
            margin-bottom: 12px;
            font-weight: 600;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .about-card h3 { color: #38bdf8; }
        .contact-card h3 { color: #10b981; }

        .card-section p {
            line-height: 1.7;
            font-size: 1rem;
        }

        /* Contact Details List */
        .contact-list {
            list-style: none;
            line-height: 2.2;
            font-size: 1rem;
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
            transition: 0.2s;
        }

        .contact-list a:hover {
            text-decoration: underline;
        }

        /* Responsive Design */
        @media (max-width: 600px) {
            .header-card h1 { font-size: 1.8rem; }
            .header-card .subtitle { font-size: 0.95rem; }
            .photo-wrapper img { width: 170px; height: 170px; }
        }
    </style>
</head>
<body>

    <div class="portfolio-container">

        <!-- Header Section -->
        <div class="header-card">
            <h1>SURESHKUMAR KANERIYA</h1>
            <p class="subtitle">Quality & Technical Inspection Professional | Solar PV Manufacturing</p>
            <p class="location"><i class="fa-solid fa-location-dot" style="color: #ef4444;"></i> Surat, Gujarat, India</p>

            <div class="photo-wrapper">
                <img src="my.jpg" alt="Sureshkumar Kaneriya" onerror="this.src='https://via.placeholder.com/210'">
            </div>
        </div>

        <!-- About Me Section -->
        <div class="card-section about-card">
            <h3><i class="fa-solid fa-user-check"></i> About Me</h3>
            <p>
                Quality & Technical Inspection Professional with <b style="color: #f8fafc;">5+ years of experience</b> in Solar PV module manufacturing, IPQC, PDI, and third-party inspection. Skilled in quality assurance, IEC standards compliance, and vendor evaluation.
            </p>
        </div>

        <!-- Contact Section -->
        <div class="card-section contact-card">
            <h3><i class="fa-solid fa-address-book"></i> Contact Details</h3>
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
                    <a href="https://www.linkedin.com/in/sureshkumar-k-34267719a" target="_blank">Sureshkumar Kaneriya Profile ↗</a>
                </li>
            </ul>
        </div>

    </div>

</body>
</html>
