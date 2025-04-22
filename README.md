<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grothwave | Digital Marketing Agency</title>
    <meta name="description" content="Professional digital marketing services to grow your business online">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
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
            color: var(--dark);
            line-height: 1.6;
            overflow-x: hidden;
        }
        
        .container {
            width: 90%;
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
            padding: 12px 30px;
            background: var(--primary);
            color: white;
            border: none;
            border-radius: 5px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            text-decoration: none;
            transition: all 0.3s ease;
        }
        
        .btn:hover {
            background: var(--primary-dark);
            transform: translateY(-2px);
        }
        
        .btn-secondary {
            background: var(--secondary);
        }
        
        .btn-secondary:hover {
            background: #e67e22;
        }
        
        /* Header Styles */
        header {
            background: white;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            position: fixed;
            width: 100%;
            z-index: 1000;
            padding: 15px 0;
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: 800;
            color: var(--primary);
            text-decoration: none;
        }
        
        .logo span {
            color: var(--secondary);
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
            transition: color 0.3s;
        }
        
        nav ul li a:hover {
            color: var(--primary);
        }
        
        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            font-size: 1.5rem;
            cursor: pointer;
            color: var(--dark);
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #f0f9ff 0%, #e0f2fe 100%);
            padding: 180px 0 100px;
            text-align: center;
        }
        
        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
            color: var(--dark);
        }
        
        .hero p {
            font-size: 1.2rem;
            color: var(--gray);
            max-width: 700px;
            margin: 0 auto 40px;
        }
        
        .hero-btns {
            display: flex;
            justify-content: center;
            gap: 20px;
        }
        
        .hero-image {
            max-width: 800px;
            margin: 60px auto 0;
        }
        
        .hero-image img {
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1);
        }
        
        /* Clients Section */
        .clients {
            background: white;
            padding: 60px 0;
        }
        
        .clients h3 {
            text-align: center;
            margin-bottom: 30px;
            color: var(--gray);
            font-weight: 500;
        }
        
        .client-logos {
            display: flex;
            justify-content: space-around;
            align-items: center;
            flex-wrap: wrap;
            gap: 30px;
        }
        
        .client-logos img {
            height: 40px;
            opacity: 0.6;
            filter: grayscale(100%);
            transition: all 0.3s;
        }
        
        .client-logos img:hover {
            opacity: 1;
            filter: grayscale(0);
        }
        
        /* Services Section */
        .services {
            background: #f8fafc;
        }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .service-card {
            background: white;
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);
        }
        
        .service-icon {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 20px;
        }
        
        .service-card h3 {
            font-size: 1.5rem;
            margin-bottom: 15px;
        }
        
        .service-card p {
            color: var(--gray);
            margin-bottom: 20px;
        }
        
        /* About Section */
        .about {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: center;
        }
        
        .about-image img {
            width: 100%;
            border-radius: 10px;
        }
        
        .about-content h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }
        
        .about-content p {
            color: var(--gray);
            margin-bottom: 20px;
        }
        
        .about-stats {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
            margin-top: 30px;
        }
        
        .stat-item {
            text-align: center;
        }
        
        .stat-item h3 {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 5px;
        }
        
        .stat-item p {
            color: var(--gray);
            font-size: 0.9rem;
        }
        
        /* Testimonials */
        .testimonials {
            background: linear-gradient(135deg, #f0f9ff 0%, #e0f2fe 100%);
        }
        
        .testimonial-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .testimonial-card {
            background: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
        }
        
        .testimonial-text {
            font-style: italic;
            color: var(--gray);
            margin-bottom: 20px;
            position: relative;
        }
        
        .testimonial-text::before {
            content: '"';
            font-size: 4rem;
            color: var(--primary);
            opacity: 0.2;
            position: absolute;
            top: -20px;
            left: -15px;
        }
        
        .testimonial-author {
            display: flex;
            align-items: center;
        }
        
        .testimonial-author img {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            margin-right: 15px;
            object-fit: cover;
        }
        
        .author-info h4 {
            font-size: 1.1rem;
            margin-bottom: 5px;
        }
        
        .author-info p {
            color: var(--gray);
            font-size: 0.9rem;
        }
        
        /* CTA Section */
        .cta {
            background: var(--primary);
            color: white;
            text-align: center;
            padding: 100px 0;
        }
        
        .cta h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }
        
        .cta p {
            max-width: 700px;
            margin: 0 auto 40px;
            opacity: 0.9;
        }
        
        .cta .btn {
            background: white;
            color: var(--primary);
        }
        
        .cta .btn:hover {
            background: #e2e8f0;
        }
        
        /* Footer */
        footer {
            background: var(--dark);
            color: white;
            padding: 80px 0 30px;
        }
        
        .footer-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 40px;
            margin-bottom: 60px;
        }
        
        .footer-col h3 {
            font-size: 1.3rem;
            margin-bottom: 20px;
            position: relative;
            padding-bottom: 10px;
        }
        
        .footer-col h3::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: 0;
            width: 50px;
            height: 2px;
            background: var(--primary);
        }
        
        .footer-col p {
            color: #94a3b8;
            margin-bottom: 15px;
        }
        
        .footer-links {
            list-style: none;
        }
        
        .footer-links li {
            margin-bottom: 10px;
        }
        
        .footer-links a {
            color: #94a3b8;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-links a:hover {
            color: white;
        }
        
        .social-links {
            display: flex;
            gap: 15px;
        }
        
        .social-links a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            color: white;
            transition: all 0.3s;
        }
        
        .social-links a:hover {
            background: var(--primary);
            transform: translateY(-3px);
        }
        
        .footer-bottom {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #94a3b8;
            font-size: 0.9rem;
        }
        
        /* Responsive Styles */
        @media (max-width: 992px) {
            .hero h1 {
                font-size: 2.8rem;
            }
            
            .about {
                grid-template-columns: 1fr;
            }
            
            .about-image {
                order: -1;
            }
        }
        
        @media (max-width: 768px) {
            nav ul {
                position: fixed;
                top: 80px;
                left: -100%;
                background: white;
                width: 100%;
                height: calc(100vh - 80px);
                flex-direction: column;
                align-items: center;
                padding-top: 40px;
                transition: left 0.3s;
                box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);
            }
            
            nav ul.active {
                left: 0;
            }
            
            nav ul li {
                margin: 15px 0;
            }
            
            .mobile-menu-btn {
                display: block;
            }
            
            .hero-btns {
                flex-direction: column;
                align-items: center;
            }
            
            .hero h1 {
                font-size: 2.2rem;
            }
            
            section {
                padding: 60px 0;
            }
        }
        
        @media (max-width: 576px) {
            .section-title h2 {
                font-size: 2rem;
            }
            
            .about-stats {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-container">
            <a href="#" class="logo">Growth<span>Wave</span></a>
            <button class="mobile-menu-btn" id="mobileMenuBtn">
                <i class="fas fa-bars"></i>
            </button>
            <nav>
                <ul id="navMenu">
                    <li><a href="#services">Services</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#testimonials">Testimonials</a></li>
                    <li><a href="#contact">Contact</a></li>
                    <li><a href="#" class="btn btn-secondary">Get Started</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <h1>Grow Your Business With Our Digital Marketing Expertise</h1>
            <p>We help businesses increase their online visibility, generate more leads, and boost sales through data-driven marketing strategies tailored to your unique needs.</p>
            <div class="hero-btns">
                <a href="#" class="btn">Get Free Consultation</a>
                <a href="#" class="btn btn-secondary">Our Services</a>
            </div>
            <div class="hero-image">
                <img src="https://images.unsplash.com/photo-1551434678-e076c223a692?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Marketing team working">
            </div>
        </div>
    </section>

    <!-- Clients Section -->
    <section class="clients">
        <div class="container">
            <h3>Trusted by leading brands worldwide</h3>
            <div class="client-logos">
                <img src="https://via.placeholder.com/150x60?text=Client+1" alt="Client Logo">
                <img src="https://via.placeholder.com/150x60?text=Client+2" alt="Client Logo">
                <img src="https://via.placeholder.com/150x60?text=Client+3" alt="Client Logo">
                <img src="https://via.placeholder.com/150x60?text=Client+4" alt="Client Logo">
                <img src="https://via.placeholder.com/150x60?text=Client+5" alt="Client Logo">
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="services" id="services">
        <div class="container">
            <div class="section-title">
                <h2>Our Digital Marketing Services</h2>
                <p>We offer comprehensive digital marketing solutions to help your business thrive in the online landscape.</p>
            </div>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-search"></i>
                    </div>
                    <h3>SEO Services</h3>
                    <p>Improve your search engine rankings and drive organic traffic with our proven SEO strategies.</p>
                    <a href="#" class="btn">Learn More</a>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-ad"></i>
                    </div>
                    <h3>PPC Advertising</h3>
                    <p>Launch targeted ad campaigns that deliver measurable results and maximize your ROI.</p>
                    <a href="#" class="btn">Learn More</a>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-hashtag"></i>
                    </div>
                    <h3>Social Media Marketing</h3>
                    <p>Build brand awareness and engage with your audience across all major social platforms.</p>
                    <a href="#" class="btn">Learn More</a>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-pen-fancy"></i>
                    </div>
                    <h3>Content Marketing</h3>
                    <p>Create valuable content that attracts, engages, and converts your target audience.</p>
                    <a href="#" class="btn">Learn More</a>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-envelope"></i>
                    </div>
                    <h3>Email Marketing</h3>
                    <p>Nurture leads and build customer loyalty with personalized email campaigns.</p>
                    <a href="#" class="btn">Learn More</a>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-chart-line"></i>
                    </div>
                    <h3>Conversion Optimization</h3>
                    <p>Turn more visitors into customers by optimizing your website's conversion funnel.</p>
                    <a href="#" class="btn">Learn More</a>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section class="about-section" id="about">
        <div class="container">
            <div class="about">
                <div class="about-image">
                    <img src="https://images.unsplash.com/photo-1522071820081-009f0129c71c?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Our team">
                </div>
                <div class="about-content">
                    <h2>Why Choose GrowthWave?</h2>
                    <p>We're not just another digital marketing agency. Our team of experts combines creativity with data-driven strategies to deliver exceptional results for our clients.</p>
                    <p>With over 10 years of experience in the industry, we've helped businesses of all sizes achieve their marketing goals and grow their online presence.</p>
                    <div class="about-stats">
                        <div class="stat-item">
                            <h3>200+</h3>
                            <p>Happy Clients</p>
                        </div>
                        <div class="stat-item">
                            <h3>95%</h3>
                            <p>Client Retention</p>
                        </div>
                        <div class="stat-item">
                            <h3>5M+</h3>
                            <p>Revenue Generated</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section class="testimonials" id="testimonials">
        <div class="container">
            <div class="section-title">
                <h2>What Our Clients Say</h2>
                <p>Don't just take our word for it. Here's what our clients have to say about working with us.</p>
            </div>
            <div class="testimonial-grid">
                <div class="testimonial-card">
                    <div class="testimonial-text">
                        <p>GrowthWave transformed our online presence. Our website traffic increased by 300% in just 6 months, and we're now ranking for all our target keywords.</p>
                    </div>
                    <div class="testimonial-author">
                        <img src="https://randomuser.me/api/portraits/women/45.jpg" alt="Sarah Johnson">
                        <div class="author-info">
                            <h4>Sarah Johnson</h4>
                            <p>CEO, TechSolutions</p>
                        </div>
                    </div>
                </div>
                <div class="testimonial-card">
                    <div class="testimonial-text">
                        <p>The team at GrowthWave is simply amazing. They took the time to understand our business and developed a customized strategy that delivered real results.</p>
                    </div>
                    <div class="testimonial-author">
                        <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="Michael Chen">
                        <div class="author-info">
                            <h4>Michael Chen</h4>
                            <p>Marketing Director, UrbanEats</p>
                        </div>
                    </div>
                </div>
                <div class="testimonial-card">
                    <div class="testimonial-text">
                        <p>We've worked with several agencies before, but none have delivered the level of service and results that GrowthWave has. Highly recommended!</p>
                    </div>
                    <div class="testimonial-author">
                        <img src="https://randomuser.me/api/portraits/women/68.jpg" alt="Lisa Rodriguez">
                        <div class="author-info">
                            <h4>Lisa Rodriguez</h4>
                            <p>Founder, GreenLife</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section class="cta">
        <div class="container">
            <h2>Ready to Grow Your Business?</h2>
            <p>Let's discuss how we can help you achieve your marketing goals and take your business to the next level.</p>
            <a href="#" class="btn">Get Your Free Strategy Session</a>
        </div>
    </section>

    <!-- Footer -->
    <footer id="contact">
        <div class="container">
            <div class="footer-grid">
                <div class="footer-col">
                    <h3>GrowthWave</h3>
                    <p>Helping businesses grow through innovative digital marketing strategies since 2012.</p>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-linkedin-in"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                    </div>
                </div>
                <div class="footer-col">
                    <h3>Services</h3>
                    <ul class="footer-links">
                        <li><a href="#">SEO Services</a></li>
                        <li><a href="#">PPC Advertising</a></li>
                        <li><a href="#">Social Media Marketing</a></li>
                        <li><a href="#">Content Marketing</a></li>
                        <li><a href="#">Email Marketing</a></li>
                    </ul>
                </div>
                <div class="footer-col">
                    <h3>Company</h3>
                    <ul class="footer-links">
                        <li><a href="#">About Us</a></li>
                        <li><a href="#">Our Team</a></li>
                        <li><a href="#">Case Studies</a></li>
                        <li><a href="#">Blog</a></li>
                        <li><a href="#">Careers</a></li>
                    </ul>
                </div>
                <div class="footer-col">
                    <h3>Contact Us</h3>
                    <p><i class="fas fa-map-marker-alt"></i> 123 Marketing ,Moi avenue<br>Nairobi,kenya</p>
                    <p><i class="fas fa-phone"></i> +254116817308</p>
                    <p><i class="fas fa-envelope"></i> mary7anderson714@gmail.com</p>
                </div>
            </div>
            <div class="footer-bottom">
                <p> 2023 GrowthWave Digital Marketing. All Rights Reserved. | <a href="#">Privacy Policy</a> | <a href="#">Terms of Service</a></p>
            </div>
        </div>
    </footer>

    <script>
        // Mobile Menu Toggle
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');
        const navMenu = document.getElementById('navMenu');
        
        mobileMenuBtn.addEventListener('click', () => {
            navMenu.classList.toggle('active');
            mobileMenuBtn.innerHTML = navMenu.classList.contains('active') 
                ? '<i class="fas fa-times"></i>' 
                : '<i class="fas fa-bars"></i>';
        });
        
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                if(this.getAttribute('href') === '#') return;
                
                const target = document.querySelector(this.getAttribute('href'));
                if(target) {
                    window.scrollTo({
                        top: target.offsetTop - 80,
                        behavior: 'smooth'
                    });
                    
                    // Close mobile menu if open
                    if(navMenu.classList.contains('active')) {
                        navMenu.classList.remove('active');
                        mobileMenuBtn.innerHTML = '<i class="fas fa-bars"></i>';
                    }
                }
            });
        });
        
        // Add shadow to header on scroll
        window.addEventListener('scroll', () => {
            if(window.scrollY > 50) {
                document.querySelector('header').style.boxShadow = '0 4px 15px rgba(0, 0, 0, 0.1)';
            } else {
                document.querySelector('header').style.boxShadow = '0 2px 10px rgba(0, 0, 0, 0.1)';
            }
        });
    </script>
</body>
</html>
