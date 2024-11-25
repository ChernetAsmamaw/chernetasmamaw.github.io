<div class="container py-5">
    <style>
        :root {
            --primary: #2563eb;
            --primary-light: #60a5fa;
            --secondary: #64748b;
            --success: #10b981;
            --bg-light: #f8fafc;
            --text-primary: #0f172a;
            --text-secondary: #475569;
        }

        .contact-header {
            text-align: center;
            margin-bottom: 4rem;
            position: relative;
        }

        .contact-header h1 {
            font-size: 3.5rem;
            font-weight: 800;
            background: linear-gradient(135deg, var(--primary) 0%, var(--primary-light) 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 1rem;
            animation: fadeInDown 0.8s ease-out;
        }

        .contact-header p {
            font-size: 1.25rem;
            color: var(--text-secondary);
            max-width: 600px;
            margin: 0 auto;
            animation: fadeInUp 0.8s ease-out 0.2s backwards;
        }

        .contact-cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
            margin-bottom: 4rem;
        }

        .contact-card {
            background: white;
            border-radius: 1rem;
            padding: 2rem;
            text-align: center;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
            border: 1px solid rgba(0, 0, 0, 0.05);
            animation: fadeIn 0.8s ease-out 0.4s backwards;
        }

        .contact-card::before {
            content: '';
            position: absolute;
            inset: 0;
            background: linear-gradient(135deg, rgba(37, 99, 235, 0.1), transparent);
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .contact-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
        }

        .contact-card:hover::before {
            opacity: 1;
        }

        .contact-card i {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 1.5rem;
        }

        .contact-card h5 {
            font-size: 1.25rem;
            font-weight: 600;
            color: var(--text-primary);
            margin-bottom: 0.75rem;
        }

        .contact-card p {
            color: var(--text-secondary);
            margin: 0;
        }

        .contact-form-container {
            max-width: 800px;
            margin: 0 auto;
            background: white;
            padding: 3rem;
            border-radius: 1.5rem;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.05);
            animation: fadeIn 0.8s ease-out 0.6s backwards;
        }

        .form-title {
            text-align: center;
            font-size: 2rem;
            font-weight: 700;
            color: var(--text-primary);
            margin-bottom: 2rem;
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            font-weight: 500;
            color: var(--text-secondary);
            margin-bottom: 0.5rem;
        }

        .form-control {
            width: 100%;
            padding: 1rem;
            border: 2px solid #e2e8f0;
            border-radius: 0.75rem;
            transition: all 0.3s ease;
            font-size: 1rem;
        }

        .form-control:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 4px rgba(37, 99, 235, 0.1);
        }

        textarea.form-control {
            resize: vertical;
            min-height: 120px;
        }

        .submit-btn {
            background: var(--primary);
            color: white;
            font-weight: 600;
            font-size: 1.125rem;
            padding: 1rem 2rem;
            border: none;
            border-radius: 0.75rem;
            width: 100%;
            cursor: pointer;
            transition: all 0.3s ease;
            margin-top: 1rem;
        }

        .submit-btn:hover {
            background: var(--primary-light);
            transform: translateY(-2px);
            box-shadow: 0 10px 20px rgba(37, 99, 235, 0.2);
        }

        .social-section {
            text-align: center;
            margin-top: 4rem;
            animation: fadeIn 0.8s ease-out 0.8s backwards;
        }

        .social-section h2 {
            font-size: 2rem;
            font-weight: 700;
            color: var(--text-primary);
            margin-bottom: 2rem;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 1rem;
        }

        .social-btn {
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            padding: 0.75rem 1.5rem;
            border-radius: 0.75rem;
            font-weight: 600;
            text-decoration: none;
            transition: all 0.3s ease;
            border: 2px solid transparent;
        }

        .social-btn i {
            font-size: 1.25rem;
        }

        .social-btn.linkedin {
            background: #0077b5;
            color: white;
        }

        .social-btn.github {
            background: #24292e;
            color: white;
        }

        .social-btn.twitter {
            background: #1da1f2;
            color: white;
        }

        .social-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
            opacity: 0.9;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes fadeInDown {
            from {
                opacity: 0;
                transform: translateY(-20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }


        .social-section {
    margin-top: 2rem;
}

.social-links a {
    background: rgba(37, 99, 235, 0.1);
    color: dark;
    padding: 0.5rem 1rem;
    border-radius: 50px;
    display: inline-flex;
    align-items: center;
    transition: all 0.3s ease;
}

.social-links a:hover {
    background: var(--primary-color);
    color: white;
    transform: translateY(-3px);
}

.social-links img {
    border-radius: 50%;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease;
}

.social-links img:hover {
    transform: scale(1.1);
}


        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @media (max-width: 768px) {
            .contact-header h1 {
                font-size: 2.5rem;
            }
            
            .contact-form-container {
                padding: 2rem;
            }
            
            .social-links {
                flex-direction: column;
                align-items: stretch;
            }
            
            .social-btn {
                justify-content: center;
            }
        }
    </style>

    <div class="contact-header">
        <h1>Get in Touch</h1>
        <p>Have a project in mind or want to collaborate? I'd love to hear from you!</p>
    </div>

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

    <div class="contact-form-container">
        <h2 class="form-title">Send Me a Message</h2>
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
                <textarea class="form-control" id="message" name="message" rows="5" required></textarea>
            </div>

            <button type="submit" class="submit-btn">
                Send Message
                <i class="fas fa-paper-plane ml-2"></i>
            </button>
        </form>
    </div>

    <div class="social-section text-center">
    <h2 class="mb-4 fw-bold text-primary">Let's Connect</h2>
    <div class="social-links d-flex justify-content-center gap-3">

        <!-- LinkedIn -->
        <a href="https://linkedin.com/in/yourusername" class="social-btn linkedin d-flex align-items-center gap-2 text-decoration-none">
            <img src="https://cdn-icons-png.flaticon.com/512/174/174857.png" alt="LinkedIn Logo" width="30" height="30">
            LinkedIn
        </a>
        <!-- GitHub -->
        <a href="https://github.com/yourusername" class="social-btn github d-flex align-items-center gap-2 text-decoration-none">
            <img src="https://cdn-icons-png.flaticon.com/512/25/25231.png" alt="GitHub Logo" width="30" height="30">
            GitHub
        </a>
        <!-- Twitter -->
        <a href="https://twitter.com/yourusername" class="social-btn twitter d-flex align-items-center gap-2 text-decoration-none">
            <img src="https://cdn-icons-png.flaticon.com/512/733/733579.png" alt="Twitter Logo" width="30" height="30">
            Twitter
        </a>
    </div>
</div>

</div>