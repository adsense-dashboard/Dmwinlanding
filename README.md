            border: 2px solid white;
        }

        .btn-login:hover {
            background: white;
            color: #ff6b35;
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
        }

        .btn-signup {
            background: linear-gradient(135deg, #00d4ff 0%, #0099ff 100%);
            color: white;
            box-shadow: 0 8px 20px rgba(0, 153, 255, 0.3);
        }

        .btn-signup:hover {
            transform: translateY(-3px);
            box-shadow: 0 12px 30px rgba(0, 153, 255, 0.5);
        }

        /* Floating Animation */
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }

        @keyframes pulse {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.8; }
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #0f2027 0%, #203a43 50%, #2c5364 100%);
            color: white;
            padding: 6rem 2rem;
            min-height: 700px;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 600"><defs><pattern id="grid" width="60" height="60" patternUnits="userSpaceOnUse"><circle cx="30" cy="30" r="2" fill="rgba(255,255,255,0.1)"/></pattern></defs><rect width="1200" height="600" fill="url(%23grid)" /></svg>');
            animation: float 6s ease-in-out infinite;
        }

        .hero-container {
            max-width: 1400px;
            width: 100%;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            align-items: center;
            position: relative;
            z-index: 1;
        }

        .hero-content {
            animation: slideInLeft 0.8s ease-out;
        }

        @keyframes slideInLeft {
            from {
                opacity: 0;
                transform: translateX(-50px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            font-weight: 900;
            line-height: 1.2;
        }

        .hero .highlight {
            background: linear-gradient(135deg, #00d4ff 0%, #0099ff 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .hero-subtitle {
            font-size: 1.3rem;
            margin-bottom: 1.5rem;
            opacity: 0.95;
            color: #a0d995;
        }

        .winning-stats {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 1rem;
            margin: 2rem 0;
        }

        .stat-card {
            background: rgba(255, 255, 255, 0.1);
            padding: 1.5rem;
            border-radius: 15px;
            border-left: 4px solid #00d4ff;
            backdrop-filter: blur(10px);
        }

        .stat-number {
            font-size: 2rem;
            font-weight: 900;
            color: #00d4ff;
        }

        .stat-text {
            font-size: 0.9rem;
            opacity: 0.8;
            margin-top: 0.5rem;
        }

        .hero-buttons {
            display: flex;
            gap: 1.5rem;
            flex-wrap: wrap;
            margin-top: 2rem;
        }

        .btn-primary, .btn-secondary {
            padding: 1.1rem 3rem;
            border: none;
            border-radius: 35px;
            font-size: 1.05rem;
            cursor: pointer;
            font-weight: 700;
            transition: all 0.3s;
            text-decoration: none;
            display: inline-block;
            text-align: center;
        }

        .btn-primary {
            background: linear-gradient(135deg, #00d4ff 0%, #0099ff 100%);
            color: white;
            box-shadow: 0 10px 30px rgba(0, 153, 255, 0.4);
        }

        .btn-primary:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 40px rgba(0, 153, 255, 0.6);
        }

        .btn-secondary {
            background: rgba(255, 255, 255, 0.15);
            color: white;
            border: 2px solid #00d4ff;
        }

        .btn-secondary:hover {
            background: #00d4ff;
            color: #0f2027;
            transform: translateY(-5px);
        }

        .hero-image {
            position: relative;
            animation: slideInRight 0.8s ease-out;
        }

        @keyframes slideInRight {
            from {
                opacity: 0;
                transform: translateX(50px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        .hero-card {
            background: linear-gradient(135deg, rgba(0, 212, 255, 0.1) 0%, rgba(0, 153, 255, 0.1) 100%);
            border: 2px solid rgba(0, 212, 255, 0.3);
            border-radius: 20px;
            padding: 2.5rem;
            backdrop-filter: blur(10px);
            animation: float 4s ease-in-out infinite;
        }

        .game-emoji {
            font-size: 5rem;
            text-align: center;
            margin-bottom: 1rem;
            animation: pulse 2s ease-in-out infinite;
        }

        /* Daily Gift Code Section */
        .gift-banner {
            background: linear-gradient(135deg, #ff6b35 0%, #f7931e 100%);
            padding: 2rem;
            border-radius: 20px;
            margin: 2rem 0;
            text-align: center;
            box-shadow: 0 10px 30px rgba(255, 107, 53, 0.3);
        }

        .gift-banner h3 {
            color: white;
            font-size: 1.5rem;
            margin-bottom: 1rem;
        }

        .gift-code {
            background: white;
            padding: 1rem 2rem;
            border-radius: 15px;
            font-size: 1.3rem;
            font-weight: 800;
            letter-spacing: 2px;
            color: #ff6b35;
            display: inline-block;
            margin: 0.5rem 0;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }

        .gift-text {
            color: white;
            font-size: 0.9rem;
            margin-top: 0.5rem;
        }

        /* Features Section */
        .features {
            padding: 5rem 2rem;
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
        }

        .features-container {
            max-width: 1400px;
            margin: 0 auto;
        }

        .section-title {
            text-align: center;
            font-size: 2.8rem;
            margin-bottom: 1rem;
            color: #0f2027;
            font-weight: 900;
        }

        .section-subtitle {
            text-align: center;
            color: #555;
            margin-bottom: 3rem;
            font-size: 1.15rem;
        }

        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2.5rem;
        }

        .feature-card {
            background: white;
            padding: 2.5rem;
            border-radius: 20px;
            text-align: center;
            transition: all 0.3s;
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.08);
            border-top: 5px solid transparent;
            position: relative;
        }

        .feature-card:nth-child(1) { border-top-color: #ff6b35; }
        .feature-card:nth-child(2) { border-top-color: #00d4ff; }
        .feature-card:nth-child(3) { border-top-color: #a0d995; }
        .feature-card:nth-child(4) { border-top-color: #ff6b35; }
        .feature-card:nth-child(5) { border-top-color: #00d4ff; }
        .feature-card:nth-child(6) { border-top-color: #a0d995; }

        .feature-card:hover {
            transform: translateY(-15px);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
        }

        .feature-icon {
            width: 90px;
            height: 90px;
            margin: 0 auto 1.5rem;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2.5rem;
            position: relative;
        }

        .feature-card:nth-child(1) .feature-icon { background: linear-gradient(135deg, #ff6b35 0%, #ff8c5a 100%); }
        .feature-card:nth-child(2) .feature-icon { background: linear-gradient(135deg, #00d4ff 0%, #0099ff 100%); }
        .feature-card:nth-child(3) .feature-icon { background: linear-gradient(135deg, #a0d995 0%, #7cb342 100%); }
        .feature-card:nth-child(4) .feature-icon { background: linear-gradient(135deg, #ff6b35 0%, #ff8c5a 100%); }
        .feature-card:nth-child(5) .feature-icon { background: linear-gradient(135deg, #00d4ff 0%, #0099ff 100%); }
        .feature-card:nth-child(6) .feature-icon { background: linear-gradient(135deg, #a0d995 0%, #7cb342 100%); }

        .feature-icon::after {
            content: '';
            position: absolute;
            top: -5px;
            right: -5px;
            width: 25px;
            height: 25px;
            background: #ffdd00;
            border-radius: 50%;
            opacity: 0;
            transition: opacity 0.3s;
            animation: pulse 2s ease-in-out infinite;
        }

        .feature-card:hover .feature-icon::after {
            opacity: 1;
        }

        .feature-card h3 {
            color: #0f2027;
            margin-bottom: 1rem;
            font-size: 1.4rem;
            font-weight: 800;
        }

        .feature-card p {
            color: #666;
            line-height: 1.8;
            font-size: 0.95rem;
        }

        /* Games Section */
        .games {
            padding: 5rem 2rem;
            background: linear-gradient(135deg, #0f2027 0%, #203a43 50%, #2c5364 100%);
            color: white;
        }

        .games-container {
            max-width: 1400px;
            margin: 0 auto;
        }

        .games h2 {
            color: white;
        }

        .games .section-subtitle {
            color: #a0d995;
        }

        .games-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 2.5rem;
            margin-top: 2rem;
        }

        .game-card {
            position: relative;
            border-radius: 20px;
            overflow: hidden;
            cursor: pointer;
            transition: transform 0.3s;
            group: one;
        }

        .game-card:hover {
            transform: scale(1.08);
        }

        .game-card-image {
            width: 100%;
            height: 230px;
            background: linear-gradient(135deg, #ff6b35 0%, #f7931e 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 4rem;
            position: relative;
        }

        .game-card:nth-child(2) .game-card-image { background: linear-gradient(135deg, #00d4ff 0%, #0099ff 100%); }
        .game-card:nth-child(3) .game-card-image { background: linear-gradient(135deg, #a0d995 0%, #7cb342 100%); }
        .game-card:nth-child(4) .game-card-image { background: linear-gradient(135deg, #ff6b35 0%, #f7931e 100%); }

        .game-card-overlay {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(0, 0, 0, 0.7);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            opacity: 0;
            transition: opacity 0.3s;
        }

        .game-card:hover .game-card-overlay {
            opacity: 1;
        }

        .game-play-btn {
            background: linear-gradient(135deg, #00d4ff 0%, #0099ff 100%);
            color: white;
            padding: 0.9rem 2rem;
            border: none;
            border-radius: 30px;
            cursor: pointer;
            font-weight: 700;
            margin-bottom: 0.5rem;
            transition: all 0.3s;
        }

        .game-play-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(0, 153, 255, 0.4);
        }

        .game-prize {
            color: #ffdd00;
            font-size: 0.9rem;
            font-weight: 700;
        }

        .game-name {
            padding: 1.2rem;
            background: rgba(0, 0, 0, 0.3);
            text-align: center;
            font-weight: 700;
            color: white;
            font-size: 1rem;
        }

        /* Promotions Section */
        .promotions {
            padding: 5rem 2rem;
            background: linear-gradient(135deg, #ffeaa7 0%, #fdcb6e 50%, #e17055 100%);
        }

        .promotions-container {
            max-width: 1400px;
            margin: 0 auto;
        }

        .promotions h2 {
            color: white;
            text-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }

        .promotions-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 2.5rem;
            margin-top: 3rem;
        }

        .promo-card {
            background: white;
            padding: 2.5rem;
            border-radius: 20px;
            transition: all 0.3s;
            position: relative;
            overflow: hidden;
        }

        .promo-card::before {
            content: '';
            position: absolute;
            top: -50%;
            right: -50%;
            width: 300px;
            height: 300px;
            background: linear-gradient(135deg, rgba(0, 212, 255, 0.1) 0%, rgba(0, 153, 255, 0.1) 100%);
            border-radius: 50%;
        }

        .promo-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
        }

        .promo-content {
            position: relative;
            z-index: 1;
        }

        .promo-card h3 {
            font-size: 1.4rem;
            margin-bottom: 1rem;
            color: #0f2027;
            font-weight: 800;
        }

        .promo-value {
            font-size: 2.5rem;
            font-weight: 900;
            margin: 1rem 0;
            background: linear-gradient(135deg, #ff6b35 0%, #f7931e 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .promo-card p {
            color: #666;
            line-height: 1.8;
        }

        .promo-badge {
            display: inline-block;
            background: #ffdd00;
            color: #0f2027;
            padding: 0.4rem 0.8rem;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 700;
            margin-top: 1rem;
        }

        /* Stats Section */
        .stats {
            padding: 4rem 2rem;
            background: linear-gradient(135deg, #0f2027 0%, #203a43 100%);
            color: white;
        }

        .stats-container {
            max-width: 1400px;
            margin: 0 auto;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .stats-card {
            text-align: center;
            padding: 2rem;
        }

        .stats-number {
            font-size: 3rem;
            font-weight: 900;
            background: linear-gradient(135deg, #00d4ff 0%, #0099ff 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 0.5rem;
        }

        .stats-label {
            font-size: 1.1rem;
            opacity: 0.9;
        }

        /* CTA Section */
        .cta {
            padding: 5rem 2rem;
            background: linear-gradient(135deg, #ff6b35 0%, #f7931e 100%);
            text-align: center;
            color: white;
        }

        .cta-content {
            max-width: 700px;
            margin: 0 auto;
        }

        .cta h2 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            font-weight: 900;
        }

        .cta p {
            font-size: 1.15rem;
            margin-bottom: 2rem;
  opacity: 0.95;
        }

        /* Footer */
        footer {
            background: #0a0a0a;
            color: white;
            padding: 4rem 2rem 1rem;
        }

        .footer-container {
            max-width: 1400px;
            margin: 0 auto;
        }

        .footer-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2.5rem;
            margin-bottom: 2rem;
        }

        .footer-section h4 {
            margin-bottom: 1.5rem;
            color: #00d4ff;
            font-size: 1.1rem;
            font-weight: 800;
        }

        .footer-section ul {
            list-style: none;
        }

        .footer-section li {
            margin-bottom: 0.7rem;
        }

        .footer-section a {
            color: #aaa;
            text-decoration: none;
            transition: color 0.3s;
            font-size: 0.95rem;
        }

        .footer-section a:hover {
            color: #00d4ff;
        }

        .footer-bottom {
            border-top: 1px solid #333;
            padding-top: 1.5rem;
            text-align: center;
            color: #666;
        }

        /* Trust Badges */
        .trust-badges {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin: 2rem 0;
            flex-wrap: wrap;
        }

        .badge {
            background: rgba(255, 255, 255, 0.1);
            padding: 0.8rem 1.5rem;
            border-radius: 50px;
            font-size: 0.9rem;
            font-weight: 700;
            border: 2px solid rgba(255, 255, 255, 0.2);
        }

        /* Responsive */
        @media (max-width: 968px) {
            .hero-container {
                grid-template-columns: 1fr;
                gap: 2rem;
            }

            .hero h1 {
                font-size: 2.5rem;
            }

            .nav-links {
                display: none;
            }

            .section-title {
                font-size: 2rem;
            }

            .hero-buttons {
                flex-direction: column;
            }

            .btn-primary, .btn-secondary {
                width: 100%;
            }
        }

        @media (max-width: 480px) {
            nav {
                padding: 0.8rem 1rem;
            }

            .logo {
                font-size: 1.3rem;
            }

            .nav-buttons {
                flex-direction: column;
                gap: 0.5rem;
                width: 100%;
            }

            .btn-login, .btn-signup {
                padding: 0.6rem 1.2rem;
                font-size: 0.85rem;
                width: 100%;
            }

            .hero {
                padding: 3rem 1rem;
                min-height: 500px;
            }

            .hero h1 {
                font-size: 1.8rem;
            }

            .section-title {
                font-size: 1.5rem;
            }
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav>
        <div class="nav-container">
            <div class="logo">
                <div class="logo-icon">🎮</div>
                DMWIN
            </div>
            <ul class="nav-links">
                <li><a href="#home">होम</a></li>
                <li><a href="#games">गेम्स</a></li>
                <li><a href="#features">विशेषताएं</a></li>
                <li><a href="#promotions">ऑफर्स</a></li>
                <li><a href="#contact">संपर्क</a></li>
            </ul>
            <div class="nav-buttons">
                <a href="http://dmwin.club" class="btn-login">लॉगिन करें</a>
                <a href="http://dmwin.club" class="btn-signup">रजिस्टर करें</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="hero-container">
            <div class="hero-content">
                <h1>भारत का <span class="highlight">#1 गेमिंग प्लेटफॉर्म</span></h1>
                <p class="hero-subtitle">🏆 रोज़ जीते ₹ लाखों | खेलो, जीतो, कमाओ</p>

                <div class="winning-stats">
                    <div class="stat-card">
                        <div class="stat-number">25 लाख+</div>
                        <div class="stat-text">सक्रिय खिलाड़ी</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-number">₹ 500+ Cr</div>
                        <div class="stat-text">जीते गए अवसर</div>
                    </div>
                </div>

                <div class="gift-banner">
                    <h3>🎁 आज का मुफ़्त उपहार कोड</h3>
                    <div class="gift-code" id="giftCode">DMWIN2026</div>
                    <p class="gift-text">₹500 बोनस पाने के लिए रजिस्टर करते समय यह कोड डालें</p>
                </div>

                <div class="hero-buttons">
                    <a href="http://dmwin.club" class="btn-primary">अभी खेलना शुरू करें</a>
                    <a href="#games" class="btn-secondary">गेम्स देखें</a>
                </div>

                <div class="trust-badges">
                    <div class="badge">✅ 100% सुरक्षित</div>
                    <div class="badge">⚡ तेज़ भुगतान</div>
                    <div class="badge">🎯 लाइसेंसप्राप्त</div>
                </div>
            </div>

            <div class="hero-image">
                <div class="hero-card">
                    <div class="game-emoji">🎰</div>
                    <p style="text-align: center; font-size: 1.5rem; font-weight: 800;">खेलो और जीतो</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section class="features" id="features">
        <div class="features-container">
            <h2 class="section-title">DMWIN को क्यों चुनें?</h2>
            <p class="section-subtitle">सर्वश्रेष्ठ गेमिंग अनुभव के लिए प्रीमियम विशेषताएं</p>
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">🎮</div>
                    <h3>100+ गेम्स</h3>
                    <p>सभी कौशल स्तरों के लिए सबसे लोकप्रिय और रोचक गेम्स का विशाल संग्रह।</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">🔒</div>
                    <h3>बिल्कुल सुरक्षित</h3>
                    <p>बैंक-स्तर की सुरक्षा से आपका पैसा और डेटा पूरी तरह सुरक्षित रहता है।</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">⚡</div>
                    <h3>तेज़ निकासी</h3>
                    <p>₹100 से अधिक जीते हुए पैसे को 5 मिनट में निकालें। कोई छिपी हुई फीस नहीं।</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">🎁</div>
                    <h3>रोज़ाना पुरस्कार</h3>
                    <p>हर दिन मुफ़्त उपहार कोड, बोनस और विशेष ऑफर पाएं।</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">📱</div>
                    <h3>आसान इंटरफेस</h3>
                    <p>सभी डिवाइसों पर मसलन-मुक्त गेमिंग अनुभव। नौसिखिए और विशेषज्ञ दोनों के लिए।</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">👥</div>
                    <h3>24/7 समर्थन</h3>
                    <p>हिंदी भाषी ग्राहक सेवा टीम सदैव आपकी मदद के लिए तैयार है।</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Games Section -->
    <section class="games" id="games">
        <div class="games-container">
            <h2 class="section-title">लोकप्रिय गेम्स</h2>
            <p class="section-subtitle">₹ लाखों जीतने का मौका पाएं</p>
            <div class="games-grid">
                <div class="game-card">
                    <div class="game-card-image">🃏</div>
                    <div class="game-card-overlay">
                        <button class="game-play-btn">अभी खेलें</button>
                        <div class="game-prize">जीतें ₹ 50,000</div>
                    </div>
                    <div class="game-name">टीन पत्ती प्रो</div>
                </div>
                <div class="game-card">
                    <div class="game-card-image">🎰</div>
                    <div class="game-card-overlay">
                        <button class="game-play-btn">अभी खेलें</button>
                        <div class="game-prize">जीतें ₹ 1,00,000</div>
                    </div>
                    <div class="game-name">स्लॉट मशीन</div>
                </div>
                <div class="game-card">
                    <div class="game-card-image">🎲</div>
                    <div class="game-card-overlay">
                        <button class="game-play-btn">अभी खेलें</button>
                        <div class="game-prize">जीतें ₹ 25,000</div>
                    </div>
                    <div class="game-name">डाइस गेम</div>
                </div>
                <div class="game-card">
                    <div class="game-card-image">🎯</div>
                    <div class="game-card-overlay">
                        <button class="game-play-btn">अभी खेलें</button>
                        <div class="game-prize">जीतें ₹ 75,000</div>
                    </div>
                    <div class="game-name">बिंगो प्लस</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Stats Section -->
    <section class="stats">
        <div class="stats-container">
            <div class="stats-grid">
                <div class="stats-card">
                    <div class="stats-number">25M+</div>
                    <div class="stats-label">खिलाड़ी विश्वास करते हैं</div>
                </div>
                <div class="stats-card">
                    <div class="stats-number">24/7</div>
                    <div class="stats-label">गेमिंग आनंद</div>
                </div>
                <div class="stats-card">
                    <div class="stats-number">₹ 500+Cr</div>
                    <div class="stats-label">वितरित पुरस्कार</div>
                </div>
                <div class="stats-card">
                    <div class="stats-number">1M+</div>
                    <div class="stats-label">रोज़ाना निकासी</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Promotions Section -->
    <section class="promotions" id="promotions">
        <div class="promotions-container">
            <h2 class="section-title">सीमित समय के ऑफर</h2>
            <div class="promotions-grid">
                <div class="promo-card">
                    <div class="promo-content">
                        <h3>🎉 स्वागत बोनस</h3>
                        <div class="promo-value">₹ 500</div>
                        <p>पहली जमा राशि पर 100% बोनस पाएं। रजिस्टर करते समय प्रमोशन कोड DMWIN2026 दर्ज करें।</p>
                        <span class="promo-badge">नए सदस्यों के लिए</span>
                    </div>
                </div>
                <div class="promo-card">
                    <div class="promo-content">
                        <h3>🏆 वफादारी पुरस्कार</h3>
                        <div class="promo-value">20%</div>
                        <p>हर खेल पर कैशबैक पाएं। जितना खेलेंगे, उतना ज़्यादा पुरस्कार जीतेंगे।</p>
                        <span class="promo-badge">हर दिन</span>
                    </div>
                </div>
                <div class="promo-card">
                    <div class="promo-content">
                        <h3>💰 दैनिक जैकपॉट</h3>
                        <div class="promo-value">₹ 25L+</div>
                        <p>हर दिन लाखों रुपये का जैकपॉट जीतने का मौका। आपकी किस्मत आज हो सकती है!</p>
                        <span class="promo-badge">हर दिन नई जीत</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section class="cta">
        <div class="cta-content">
            <h2>DMWIN में आज ही शामिल हों</h2>
            <p>₹500 का तुरंत बोनस पाएं। रजिस्टर करना बिल्कुल मुफ़्त है। कोई पहचान पत्र, कोई झंझट नहीं।</p>
            <a href="http://dmwin.club" class="btn-primary" style="padding: 1.2rem 3.5rem; font-size: 1.1rem;">अभी रजिस्टर करें</a>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="footer-container">
            <div class="footer-grid">
                <div class="footer-section">
                    <h4>🎮 DMWIN के बारे में</h4>
                    <ul>
                        <li><a href="#">हमारे बारे में</a></li>
                        <li><a href="#">हमारा मिशन</a></li>
                        <li><a href="#">कैरियर</a></li>
                        <li><a href="#">ब्लॉग</a></li>
                    </ul>
                </div>
                <div class="footer-section">
                    <h4>🎯 गेम्स</h4>
                    <ul>
                        <li><a href="#">सभी गेम्स</a></li>
                        <li><a href="#">नए गेम्स</a></li>
                        <li><a href="#">लोकप्रिय गेम्स</a></li>
                        <li><a href="#">टूर्नामेंट्स</a></li>
                    </ul>
                </div>
                <div class="footer-section">
                    <h4>💬 समर्थन</h4>
                    <ul>
                        <li><a href="#">सहायता केंद्र</a></li>
                        <li><a href="#">हमसे संपर्क करें</a></li>
                        <li><a href="#">अक्सर पूछे जाने वाले प्रश्न</a></li>
                        <li><a href="#">समस्या की रिपोर्ट करें</a></li>
                    </ul>
                </div>
                <div class="footer-section">
                    <h4>⚖️ कानूनी</h4>
                    <ul>
                        <li><a href="#">गोपनीयता नीति</a></li>
                        <li><a href="#">सेवा की शर्तें</a></li>
                        <li><a href="#">कुकी नीति</a></li>
                        <li><a href="#">जिम्मेदार गेमिंग</a></li>
                    </ul>
                </div>
            </div>
            <div class="footer-bottom">
                <p>&copy; 2026 DMWIN गेमिंग प्लेटफॉर्म। सर्वाधिकार सुरक्ष���त। | भारत में लाइसेंसप्राप्त और विनियमित।</p>
                <p style="margin-top: 1rem; font-size: 0.85rem;">⚠️ जिम्मेदारी से खेलें। 18+ के लिए। समस्या गेमिंग सहायता: 1-800-HELP</p>
            </div>
        </div>
    </footer>

    <script>
        // Dynamic Gift Code
        const giftCodes = ['DMWIN2026', 'WIN500INR', 'LUCKY2026', 'PLAY100FREE'];
        let codeIndex = 0;

        setInterval(() => {
            codeIndex = (codeIndex + 1) % giftCodes.length;
            document.getElementById('giftCode').textContent = giftCodes[codeIndex];
        }, 8000);

        // Smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                const href = this.getAttribute('href');
                if (href !== '#' && document.querySelector(href)) {
                    e.preventDefault();
                    document.querySelector(href).scrollIntoView({ behavior: 'smooth' });
                }
            });
        });

        // Button interactions
        document.querySelectorAll('.game-play-btn').forEach(btn => {
            btn.addEventListener('click', function(e) {
                e.preventDefault();
                alert('खेल शुरू हो रहा है... अपने गेमिंग सत्र को लोड किया जा रहा है! 🎮');
            });
        });

        // Copy gift code
        document.getElementById('giftCode').addEventListener('click', function() {
            const code = this.textContent;
            navigator.clipboard.writeText(code);
            alert('कोड कॉपी हो गया: ' + code);
        });

        // Counter animation
        function animateCounter(element, target, duration = 2000) {
            let start = 0;
            const increment = target / (duration / 16);
            const timer = setInterval(() => {
                start += increment;
                if (start >= target) {
                    element.textContent = target;
                    clearInterval(timer);
                } else {
                    element.textContent = Math.floor(start);
                }
            }, 16);
        }

        // Animate on scroll
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        });

        document.querySelectorAll('.feature-card, .game-card, .promo-card').forEach(el => {
            el.style.opacity = '0';
            el.style.transform = 'translateY(20px)';
            el.style.transition = 'all 0.6s ease-out';
            observer.observe(el);
        });
    </script>
</body>
</html>
