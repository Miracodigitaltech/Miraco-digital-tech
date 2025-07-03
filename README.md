<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Miraco Digital Tech - Empowering Digital Growth in Nigeria</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* Global Styles */
        :root {
            --primary: #2563eb;
            --primary-dark: #1d4ed8;
            --secondary: #f59e0b;
            --dark: #1e293b;
            --light: #f8fafc;
            --gray: #64748b;
            --success: #10b981;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #ffffff;
            color: var(--dark);
            line-height: 1.6;
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        section {
            padding: 80px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 50px;
        }
        
        .section-title h2 {
            font-size: 2.5rem;
            color: var(--dark);
            margin-bottom: 15px;
        }
        
        .section-title p {
            color: var(--gray);
            font-size: 1.1rem;
            max-width: 700px;
            margin: 0 auto;
        }
        
        .btn {
            display: inline-block;
            padding: 12px 24px;
            background-color: var(--primary);
            color: white;
            border-radius: 4px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
        }
        
        .btn:hover {
            background-color: var(--primary-dark);
            transform: translateY(-2px);
        }
        
        .btn-secondary {
            background-color: var(--secondary);
        }
        
        .btn-secondary:hover {
            background-color: #e67e22;
        }
        
        /* Header Styles */
        header {
            background-color: white;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }
        
        .logo {
            display: flex;
            align-items: center;
        }
        
        .logo img {
            height: 50px;
            width: 50px;
            border-radius: 50px;
            margin-right: 10px;
        }
        
        .logo h1 {
            font-size: 1.5rem;
            color: var(--primary);
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 30px;
        }
        
        nav ul li a {
            text-decoration: none;
            color: var(--dark);
            font-weight: 600;
            transition: color 0.3s ease;
        }
        
        nav ul li a:hover {
            color: var(--primary);
        }
        
        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            font-size: 1.5rem;
            color: var(--dark);
            cursor: pointer;
        }
        
        .whatsapp-float {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background-color: #25D366;
            color: white;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 2rem;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
            z-index: 999;
            transition: all 0.3s ease;
        }
        
        .whatsapp-float:hover {
            transform: scale(1.1);
            box-shadow: 0 6px 16px rgba(0, 0, 0, 0.2);
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #2563eb 0%, #1d4ed8 100%);
            color: white;
            padding: 180px 0 100px;
            text-align: center;
        }
        
        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }
        
        .hero h1 {
            font-size: 3rem;
            margin-bottom: 20px;
            line-height: 1.2;
        }
        
        .hero p {
            font-size: 1.2rem;
            margin-bottom: 30px;
            opacity: 0.9;
        }
        
        .hero-btns {
            display: flex;
            justify-content: center;
            gap: 20px;
        }
        
        /* Services Section */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 50px;
        }
        
        .service-card {
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }
        
        .service-icon {
            background-color: var(--primary);
            color: white;
            height: 80px;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 2.5rem;
        }
        
        .service-content {
            padding: 30px;
        }
        
        .service-content h3 {
            font-size: 1.5rem;
            margin-bottom: 15px;
            color: var(--dark);
        }
        
        .service-content p {
            color: var(--gray);
            margin-bottom: 20px;
        }
        
        /* About Section */
        .about {
            background-color: #f8fafc;
        }
        
        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: center;
        }
        
        .about-text h2 {
            font-size: 2rem;
            margin-bottom: 20px;
            color: var(--dark);
        }
        
        .about-text p {
            margin-bottom: 15px;
            color: var(--gray);
        }
        
        .about-values {
            margin-top: 30px;
        }
        
        .value-item {
            display: flex;
            margin-bottom: 20px;
        }
        
        .value-icon {
            background-color: var(--primary);
            color: white;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            margin-right: 15px;
            flex-shrink: 0;
        }
        
        .value-text h4 {
            font-size: 1.1rem;
            margin-bottom: 5px;
            color: var(--dark);
        }
        
        .value-text p {
            font-size: 0.9rem;
        }
        
        .about-image img {
            width: 100%;
            border-radius: 8px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }
        
        /* Contact Section */
        .contact {
            background-color: var(--primary);
            color: white;
        }
        
        .contact .section-title h2,
        .contact .section-title p {
            color: white;
        }
        
        .contact-container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
        }
        
        .contact-info h3 {
            font-size: 1.5rem;
            margin-bottom: 20px;
        }
        
        .contact-details {
            margin-bottom: 30px;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            margin-bottom: 15px;
        }
        
        .contact-icon {
            margin-right: 15px;
            font-size: 1.2rem;
        }
        
        .social-links {
            display: flex;
            gap: 15px;
        }
        
        .social-links a {
            color: white;
            font-size: 1.5rem;
            transition: transform 0.3s ease;
        }
        
        .social-links a:hover {
            transform: translateY(-3px);
        }
        
        .contact-form input,
        .contact-form textarea {
            width: 100%;
            padding: 12px 15px;
            margin-bottom: 20px;
            border: none;
            border-radius: 4px;
            background-color: rgba(255, 255, 255, 0.9);
        }
        
        .contact-form textarea {
            height: 150px;
            resize: vertical;
        }
        
        /* Footer */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 50px 0 20px;
        }
        
        .footer-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 30px;
            margin-bottom: 40px;
        }
        
        .footer-col h3 {
            font-size: 1.2rem;
            margin-bottom: 20px;
            position: relative;
            padding-bottom: 10px;
        }
        
        .footer-col h3::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: 0;
            width: 40px;
            height: 2px;
            background-color: var(--primary);
        }
        
        .footer-col ul {
            list-style: none;
        }
        
        .footer-col ul li {
            margin-bottom: 10px;
        }
        
        .footer-col ul li a {
            color: #cbd5e1;
            text-decoration: none;
            transition: color 0.3s ease;
        }
        
        .footer-col ul li a:hover {
            color: white;
        }
        
        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #cbd5e1;
            font-size: 0.9rem;
        }
        
        /* Responsive Styles */
        @media (max-width: 992px) {
            .about-content,
            .contact-container {
                grid-template-columns: 1fr;
            }
            
            .about-image {
                order: -1;
            }
        }
        
        @media (max-width: 768px) {
            nav {
                position: fixed;
                top: 80px;
                left: -100%;
                width: 100%;
                height: calc(100vh - 80px);
                background-color: white;
                transition: all 0.3s ease;
                padding: 30px;
            }
            
            nav.active {
                left: 0;
            }
            
            nav ul {
                flex-direction: column;
            }
            
            nav ul li {
                margin: 15px 0;
            }
            
            .mobile-menu-btn {
                display: block;
            }
            
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .hero-btns {
                flex-direction: column;
                gap: 10px;
            }
            
            .btn {
                width: 100%;
            }
        }
        
        @media (max-width: 576px) {
            .section-title h2 {
                font-size: 2rem;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
            
            .hero p {
                font-size: 1rem;
            }
        }
    </style>
</head>
<body>
    <!-- WhatsApp Float Button -->
    <a href="https://wa.me/2349161112862" class="whatsapp-float" target="_blank">
        <i class="fab fa-whatsapp"></i>
    </a>

    <!-- Header -->
    <header>
        <div class="container header-container">
            <div class="logo">
                <img src="Black and Orange Neon Futuristic Simple Technology Logo_20240906_234021_0000.png" alt="Miraco Digital Tech Logo">
                <h1>Miraco Digital Tech</h1>
            </div>
            
            <button class="mobile-menu-btn" id="mobileMenuBtn">
                <i class="fas fa-bars"></i>
            </button>
            
            <nav id="mainNav">
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <div class="hero-content">
                <h1>Empowering Digital Growth in Nigeria</h1>
                <p>Comprehensive digital solutions for SMEs - Website Development, Graphics Design, Social Media Management & More</p>
                <div class="hero-btns">
                    <a href="#contact" class="btn">Get Free Consultation</a>
                    <a href="#services" class="btn btn-secondary">View Our Services</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="services" id="services">
        <div class="container">
            <div class="section-title">
                <h2>Our Digital Services</h2>
                <p>We offer a comprehensive suite of digital services designed to empower your business growth in Nigeria's dynamic digital landscape.</p>
            </div>
            
            <div class="services-grid">
                <!-- Service 1 -->
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-laptop-code"></i>
                    </div>
                    <div class="service-content">
                        <h3>Website Development</h3>
                        <p>Professional, responsive websites that are SEO-friendly and optimized for all devices. From simple brochure sites to complex e-commerce platforms.</p>
                        <a href="#contact" class="btn">Learn More</a>
                    </div>
                </div>
                
                <!-- Service 2 -->
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-paint-brush"></i>
                    </div>
                    <div class="service-content">
                        <h3>Graphic Design</h3>
                        <p>Stunning visual assets including logos, branding materials, social media graphics, and marketing collateral that make your brand stand out.</p>
                        <a href="#contact" class="btn">Learn More</a>
                    </div>
                </div>
                
                <!-- Service 3 -->
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-qrcode"></i>
                    </div>
                    <div class="service-content">
                        <h3>QR Code Generation</h3>
                        <p>Professional QR codes for your marketing materials, business cards, and products to bridge your offline and online presence seamlessly.</p>
                        <a href="#contact" class="btn">Learn More</a>
                    </div>
                </div>
                
                <!-- Service 4 -->
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-hashtag"></i>
                    </div>
                    <div class="service-content">
                        <h3>Social Media Management</h3>
                        <p>Complete management of your social media presence including strategy, content creation, posting, and performance analytics.</p>
                        <a href="#contact" class="btn">Learn More</a>
                    </div>
                </div>
                
                <!-- Service 5 -->
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-users"></i>
                    </div>
                    <div class="service-content">
                        <h3>CRM Implementation</h3>
                        <p>End-to-end CRM solutions to help you manage customer relationships, streamline processes, and improve customer satisfaction.</p>
                        <a href="#contact" class="btn">Learn More</a>
                    </div>
                </div>
                
                <!-- Service 6 -->
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-video"></i>
                    </div>
                    <div class="service-content">
                        <h3>Video Editing</h3>
                        <p>Professional video editing services for marketing videos, social media content, product demos, and more to engage your audience.</p>
                        <a href="#contact" class="btn">Learn More</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section class="about" id="about">
        <div class="container">
            <div class="about-content">
                <div class="about-text">
                    <h2>About Miraco Digital Tech</h2>
                    <p>We are a Nigerian digital technology company dedicated to empowering SMEs with innovative, integrated digital solutions that foster sustainable growth.</p>
                    <p>Our mission is to help Nigerian businesses establish a strong digital presence, enhance customer engagement, and drive measurable results through strategic digital solutions.</p>
                    
                    <div class="about-values">
                        <h3>Our Core Values</h3>
                        
                        <div class="value-item">
                            <div class="value-icon">
                                <i class="fas fa-user"></i>
                            </div>
                            <div class="value-text">
                                <h4>Client-Centricity</h4>
                                <p>We prioritize your unique business goals and tailor solutions to your specific needs.</p>
                            </div>
                        </div>
                        
                        <div class="value-item">
                            <div class="value-icon">
                                <i class="fas fa-lightbulb"></i>
                            </div>
                            <div class="value-text">
                                <h4>Innovation</h4>
                                <p>We continuously integrate emerging technologies to keep you ahead of the competition.</p>
                            </div>
                        </div>
                        
                        <div class="value-item">
                            <div class="value-icon">
                                <i class="fas fa-handshake"></i>
                            </div>
                            <div class="value-text">
                                <h4>Integrity & Transparency</h4>
                                <p>We build trust through honest communication and deliver on our promises.</p>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="about-image">
                    <img src="IMG_8137.jpg" alt="Miraco Digital Tech Team">
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact" id="contact">
        <div class="container">
            <div class="section-title">
                <h2>Get In Touch</h2>
                <p>Ready to empower your digital growth? Contact us today for a free consultation.</p>
            </div>
            
            <div class="contact-container">
                <div class="contact-info">
                    <h3>Contact Information</h3>
                    
                    <div class="contact-details">
                        <div class="contact-item">
                            <div class="contact-icon">
                                <i class="fas fa-map-marker-alt"></i>
                            </div>
                            <div>
                                <p>Kano, Nigeria</p>
                            </div>
                        </div>
                        
                        <div class="contact-item">
                            <div class="contact-icon">
                                <i class="fas fa-phone-alt"></i>
                            </div>
                            <div>
                                <p><a href="tel:+2349161112862">+234 916 111 2862</a></p>
                            </div>
                        </div>
                        
                        <div class="contact-item">
                            <div class="contact-icon">
                                <i class="fas fa-envelope"></i>
                            </div>
                            <div>
                                <p><a href="mailto:ammaaribrahimabubabakar@gmail.com">ammaaribrahimabubabakar@gmail.com</a></p>
                            </div>
                        </div>
                    </div>
                    
                    <h3>Follow Us</h3>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-linkedin-in"></i></a>
                    </div>
                </div>
                
                <div class="contact-form">
                    <form id="contactForm">
                        <input type="text" placeholder="Your Name" required>
                        <input type="email" placeholder="Your Email" required>
                        <input type="text" placeholder="Subject">
                        <textarea placeholder="Your Message" required></textarea>
                        <button type="submit" class="btn btn-secondary">Send Message</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-container">
                <div class="footer-col">
                    <h3>Miraco Digital</h3>
                    <p>Empowering Nigerian businesses with comprehensive digital solutions for sustainable growth and success.</p>
                </div>
                
                <div class="footer-col">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="#home">Home</a></li>
                        <li><a href="#services">Services</a></li>
                        <li><a href="#about">About Us</a></li>
                        <li><a href="#contact">Contact</a></li>
                    </ul>
                </div>
                
                <div class="footer-col">
                    <h3>Services</h3>
                    <ul>
                        <li><a href="#services">Website Development</a></li>
                        <li><a href="#services">Graphic Design</a></li>
                        <li><a href="#services">Social Media Management</a></li>
                        <li><a href="#services">CRM Implementation</a></li>
                    </ul>
                </div>
                
                <div class="footer-col">
                    <h3>Contact</h3>
                    <ul>
                        <li><i class="fas fa-phone-alt"></i> +234 916 111 2862</li>
                        <li><i class="fas fa-envelope"></i> ammaaribrahimabubabakar@gmail.com</li>
                        <li><i class="fas fa-map-marker-alt"></i> Kano, Nigeria</li>
                    </ul>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2023 Miraco Digital Tech Company. All Rights Reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Mobile Menu Toggle
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');
        const mainNav = document.getElementById('mainNav');
        
        mobileMenuBtn.addEventListener('click', () => {
            mainNav.classList.toggle('active');
            mobileMenuBtn.innerHTML = mainNav.classList.contains('active') ? 
                '<i class="fas fa-times"></i>' : '<i class="fas fa-bars"></i>';
        });
        
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                if(this.getAttribute('href') === '#') return;
                
                const target = document.querySelector(this.getAttribute('href'));
                if(target) {
                    window.scrollTo({
                        top: target.offsetTop - 80,
                        behavior: 'smooth'
                    });
                    
                    // Close mobile menu if open
                    if(mainNav.classList.contains('active')) {
                        mainNav.classList.remove('active');
                        mobileMenuBtn.innerHTML = '<i class="fas fa-bars"></i>';
                    }
                }
            });
        });
        
        // Form submission
        const contactForm = document.getElementById('contactForm');
        if(contactForm) {
            contactForm.addEventListener('submit', function(e) {
                e.preventDefault();
                alert('Thank you for your message! We will contact you soon.');
                this.reset();
            });
        }
    </script>
</body>
</html>
