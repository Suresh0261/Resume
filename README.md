<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Suresh Kaneriya | Solar PV Quality Expert</title>
    <!-- Font Awesome Icons के लिए -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        /* CSS कोड - जैसा फोटो में दिखाया गया था */
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; }
        
        /* डार्क बैकग्राउंड और टेक्स्ट कलर */
        body { background-color: #0d1117; color: #c9d1d9; line-height: 1.6; }

        /* हेडर और नेविगेशन (जैसा फोटो में ऊपर था) */
        header { position: fixed; top: 0; width: 100%; background: rgba(13, 17, 23, 0.9); backdrop-filter: blur(10px); display: flex; justify-content: space-between; align-items: center; padding: 15px 10%; z-index: 1000; border-bottom: 1px solid #21262d; }
        header .logo { font-size: 1.5rem; font-weight: 700; color: #38bdf8; }
        header nav ul { display: flex; list-style: none; gap: 20px; }
        header nav ul a { color: #8b949e; text-decoration: none; font-weight: 500; font-size: 0.9rem; transition: 0.3s; }
        header nav ul a:hover { color: #38bdf8; }

        /* मुख्य कंटेनर (Side-by-Side डिज़ाइन) */
        .main-container { max-width: 1300px; margin: 100px auto 0; padding: 80px 10%; display: flex; align-items: center; gap: 60px; flex-wrap: wrap; min-height: 85vh; }
        
        /* बायीं तरफ बड़ी फोटो का सेक्शन */
        .photo-section { flex: 1; min-width: 350px; display: flex; justify-content: center; position: relative; }
        .photo-section img { width: 100%; max-width: 450px; /* बड़ी फोटो */ height: auto; border-radius: 20px; border: 3px solid #38bdf8; box-shadow: 0 0 40px rgba(56, 189, 248, 0.2); object-fit: cover; }
        
        /* सोलर पैनल और ड्रोन के छोटे आइकन */
        .icon-overlay { position: absolute; color: #38bdf8; opacity: 0.3; font-size: 1.5rem; }
        .icon-overlay.solar1 { top: -20px; left: -20px; }
        .icon-overlay.drone1 { top: 30%; right: -30px; font-size: 2rem; }
        .icon-overlay.solar2 { bottom: -20px; right: 50px; font-size: 1rem; }

        /* दायीं तरफ प्रोफाइल समरी का सेक्शन */
        .content-section { flex: 1.3; min-width: 350px; }
        .greeting { font-size: 1.6rem; color: #38bdf8; font-weight: 600; }
        h1 { font-size: 3.5rem; color: #ffffff; margin: 5px 0 10px 0; }
        .role { font-size: 1.1rem; color: #8b949e; margin-bottom: 25px; }
        
        /* प्रोफाइल समरी हेडिंग और टेक्स्ट */
        h2.summary-heading { font-size: 2rem; color: #38bdf8; margin-bottom: 15px; border-bottom: 1px solid #21262d; padding-bottom: 10px; }
        .summary-text { color: #c9d1d9; font-size: 1.05rem; line-height: 1.9; margin-bottom: 15px; }
        
        /* नीचे कांटेक्ट बार (जैसा फोटो में था) */
        .contact-bar { background-color: #161b22; width: 100%; padding: 25px 10%; display: flex; justify-content: center; align-items: center; gap: 40px; flex-wrap: wrap; border-top: 1px solid #21262d; }
        .contact-item { display: flex; align-items: center; gap: 10px; color: #8b949e; font-size: 1rem; }
        .contact-item i { color: #38bdf8; font-size: 1.2rem; }
        .linkedin-btn { background-color: #0077b5; color: white; padding: 10px 20px; border-radius: 5px; text-decoration: none; font-weight: 600; transition: 0.3s; display: flex; align-items: center; gap: 8px; }
        .linkedin-btn:hover { background-color: #005582; }

        /* फुटर */
        footer { text-align: center; padding: 15px; background: #0d1117; color: #484f58; font-size: 0.8rem; border-top: 1px solid #21262d; }
    </style>
</head>
<body>

    <!-- नेविगेशन हेडर -->
    <header>
        <div class="logo">Suresh.PV</div>
        <nav>
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#experience">Experience</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- मेन सेक्शन - साइड-बाय-साइड -->
    <div class="main-container" id="about">
        
        <!-- बड़ी फोटो (बाईं तरफ) -->
        <div class="photo-section">
            <i class="fas fa-solar-panel icon-overlay solar1"></i>
            <i class="fas fa-helicopter icon-overlay drone1"></i>
            <img src="profile.jpg" alt="Suresh Kaneriya">
            <i class="fas fa-satellite-dish icon-overlay solar2"></i>
        </div>

        <!-- प्रोफाइल समरी (दायीं तरफ) -->
        <div class="content-section">
            <div class="greeting">Hello, I'm</div>
            <h1>Suresh Kaneriya</h1>
            <p class="role">Assistant Manager – Technical Inspection & Quality Assurance (Solar PV)</p>
            
            <h2 class="summary-heading">Profile Summary</h2>
            <p class="summary-text">
                Results-driven Quality and Technical Inspection professional with <strong>7+ years of experience</strong> across Solar PV module manufacturing, quality assurance, and third-party inspection consultancy. Skilled in IPQC/PDI inspection management, IEC 61215/61730 compliance, vendor evaluation, SOP development, and technical team leadership.
            </p>
            <p class="summary-text">
                Proven track record managing inspection programs for <strong>500+ MW</strong> of solar projects, coordinating with OEMs and clients, and supporting ISO/IEC 17020 and NABCB accreditation initiatives.
            </p>
            <p class="summary-text">
                Adept at drone-based thermography and inspection data analysis using <strong>Agisoft Metashape</strong> and <strong>QGIS</strong>.
            </p>
        </div>

    </div>

    <!-- नीचे कांटेक्ट बार -->
    <div class="contact-bar" id="contact">
        <div class="contact-item">
            <i class="fas fa-map-marker-alt"></i>
            <span>Surat, Gujarat, India</span>
        </div>
        <div class="contact-item">
            <i class="fas fa-envelope"></i>
            <a href="mailto:suresh.pvv@gmail.com" style="color: #c9d1d9; text-decoration: none;">suresh.pvv@gmail.com</a>
        </div>
        <a href="https://linkedin.com" target="_blank" class="linkedin-btn">
            <i class="fab fa-linkedin"></i> LinkedIn
        </a>
    </div>

    <!-- फुटर -->
    <footer>
        © Suresh Kaneriya. All Rights Reserved.
    </div>

</body>
</html>
