<div class="container">
    <style>
        :root {
            --primary: #2563eb;
            --primary-light: #60a5fa;
            --secondary: #64748b;
            --bg-light: #f8fafc;
            --text-primary: #0f172a;
            --text-secondary: #475569;
            --linkedin-color: #0077b5;
            --github-color: #333333;
            --twitter-color: #1da1f2;
            --ocean-blue: #0066cc;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: var(--bg-light);
        }

        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 1rem;
        }

        section {
            min-height: 90vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            padding: 4rem 0;
            position: relative;
        }

        .section-header {
            text-align: center;
            margin-bottom: 2rem;
        }

        .section-header h1 {
            font-size: 3rem;
            background: linear-gradient(135deg, #8b4513, #2563eb);
            -webkit-background-clip: text;
            color: transparent;
            font-weight: 700;
            margin-bottom: 1rem;
            line-height: 1.2;
            margin-top: 5rem;
        }

        .section-header p {
            font-size: 1.2rem;
            color: var(--text-secondary);
            max-width: 600px;
            margin: 0 auto;
            line-height: 1.6;
        }

        .contact-details {
            background-color: white;
            border-radius: 2rem;
            padding: 3rem 2rem;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
            margin: auto;
            width: 100%;
            max-width: 1100px;
        }

        .contact-cards {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 2rem;
            margin-bottom: 3rem;
        }

        .contact-card {
            text-align: center;
            padding: 2rem;
            border: 1px solid rgba(0, 0, 0, 0.08);
            background: white;
            border-radius: 1rem;
            transition: all 0.3s ease;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.04);
        }

        .contact-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
        }

        .contact-card i {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 1.5rem;
        }

        .contact-card h5 {
            font-size: 1.25rem;
            font-weight: 600;
            margin-bottom: 0.75rem;
            color: var(--text-primary);
        }

        .contact-card p {
            color: var(--text-secondary);
            font-size: 1rem;
            line-height: 1.6;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin-top: 3rem;
        }

        .social-btn {
            display: flex;
            align-items: center;
            gap: 0.75rem;
            padding: 0.875rem 2rem;
            border-radius: 50px;
            font-weight: 500;
            color: white;
            text-decoration: none;
            transition: all 0.3s ease;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        .social-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
            filter: brightness(1.1);
        }

        .social-btn.linkedin {
            background-color: var(--linkedin-color);
        }

        .social-btn.github {
            background-color: var(--github-color);
        }

        .social-btn.twitter {
            background-color: var(--twitter-color);
        }

        .social-btn img {
            width: 24px;
            height: 24px;
            filter: brightness(0) invert(1);
        }

        .contact-form-section {
            background-color: ;
            min-height: 80vh;
        }

        .form-container {
            max-width: 800px;
            margin: 0 auto;
        }

        .form-group {
            margin-bottom: 1rem;
        }

        .form-group label {
            display: block;
            font-weight: 500;
            color: var(--text-primary);
            margin-bottom: 0.75rem;
            font-size: 1.1rem;
        }

        .form-control {
            width: 100%;
            padding: 1rem;
            border: 2px solid #e2e8f0;
            border-radius: 0.75rem;
            font-size: 1rem;
            transition: all 0.3s ease;
            background-color: var(--bg-light);
        }

        .form-control:focus {
            outline: none;
            border-color: var(--ocean-blue);
            box-shadow: 0 0 0 3px rgba(0, 102, 204, 0.1);
        }

        textarea.form-control {
            min-height: 130px;
            resize: vertical;
        }

        .submit-btn {
            background: var(--ocean-blue);
            color: white;
            border: none;
            margin-top: 1rem;
            padding: 1rem 3rem;
            font-size: 1.1rem;
            font-weight: 500;
            border-radius: 0.75rem;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        .submit-btn:hover {
            background: #0077ee;
            transform: translateY(-2px);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
        }

        .scroll-indicator {
            position: absolute;
            bottom: 2rem;
            left: 50%;
            transform: translateX(-50%);
            animation: bounce 2s infinite;
            color: var(--text-secondary);
            font-size: 2rem;
            cursor: pointer;
        }

        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% {
                transform: translateY(0) translateX(-50%);
            }
            40% {
                transform: translateY(-20px) translateX(-50%);
            }
            60% {
                transform: translateY(-10px) translateX(-50%);
            }
        }

        @media (max-width: 968px) {
            .contact-cards {
                grid-template-columns: 1fr;
                gap: 1.5rem;
            }
            
            .social-links {
                flex-direction: column;
                align-items: stretch;
                gap: 1rem;
            }
            
            .social-btn {
                justify-content: center;
            }

            .section-header h1 {
                font-size: 2.5rem;
            }
        }
    </style>

    <!-- Section 1: Contact Details -->
    <section>
        <div class="section-header">
            <h1>Contact Me</h1>
            <p>Feel free to reach out anytime. I'm always open to collaborating!</p>
        </div>
        
        <div class="contact-details">
            <div class="contact-cards">
                <div class="contact-card">
                    <i class="fas fa-envelope"></i>
                    <h5>Email</h5>
                    <p>c.asmamaw@alustudent.com</p>
                </div>
                <div class="contact-card">
                    <i class="fas fa-map-marker-alt"></i>
                    <h5>Location</h5>
                    <p>Kigali, Rwanda</p>
                </div>
                <div class="contact-card">
                    <i class="fas fa-clock"></i>
                    <h5>Available Hours</h5>
                    <p>Tuesday - Friday: 9:00 AM - 6:00 PM CAT</p>
                </div>
            </div>

            <div class="social-links">
                <a href="https://www.linkedin.com/in/chernet-asmamaw/" class="social-btn linkedin">
                    <img src="https://cdn-icons-png.flaticon.com/512/174/174857.png" alt="LinkedIn"> LinkedIn
                </a>
                <a href="https://github.com/chernetasmamaw" class="social-btn github">
                    <img src="https://cdn-icons-png.flaticon.com/512/25/25231.png" alt="GitHub"> GitHub
                </a>
                <a href="https://twitter.com/" target="_blank" class="social-btn twitter">
                    <img src="https://cdn-icons-png.flaticon.com/512/733/733579.png" alt="Twitter"> Twitter
                </a>
            </div>
        </div>
        
        <div class="scroll-indicator">
            <i class="fas fa-chevron-down"></i>
        </div>
    </section>

    <!-- Section 2: Contact Form -->
    <section class="contact-form-section">
        <div class="form-container">
            <div class="section-header">
                <h1>Send Me a Message</h1>
                <p>Got a question or proposal? Go ahead!</p>
            </div>
            
            <form id="contactForm" action="/submit-form" method="POST">
                <div class="form-group">
                    <label for="name">Full Name</label>
                    <input type="text" class="form-control" id="name" name="name" required>
                </div>
                <div class="form-group">
                    <label for="email">Email Address</label>
                    <input type="email" class="form-control" id="email" name="email" required>
                </div>
                <div class="form-group">
                    <label for="subject">Subject</label>
                    <input type="text" class="form-control" id="subject" name="subject" required>
                </div>
                <div class="form-group">
                    <label for="message">Message</label>
                    <textarea class="form-control" id="message" name="message" required></textarea>
                </div>
                <div style="text-align: center;">
                    <button type="submit" class="submit-btn">Send Message</button>
                </div>
            </form>
        </div>
    </section>
</div>