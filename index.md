<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chernet</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
    <style>
        :root {
            --primary: #2563eb;
            --primary-dark: #1d4ed8;
            --secondary: #64748b;
            --bg-light: #f8fafc;
            --text-primary: #0f172a;
            --text-secondary: #475569;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
            color: var(--text-primary);
            background: white;
        }

        .container {
            max-width: 1200px;
            padding: 0 2rem;
        }

        .hero-section, .skills-section {
            background: white;
        }

        .hero-section {
            min-height: 90vh;
            display: flex;
            align-items: center;
            position: relative;
            overflow: hidden;
        }

        .hero-content {
            display: grid;
            grid-template-columns: 400px 1fr;
            gap: 6rem;
            align-items: center;
        }

        .hero-image {
            position: relative;
        }

        .profile-img {
            width: 100%;
            height: auto;
            border-radius: 16px;
            box-shadow: 
                0 20px 40px rgba(0, 0, 0, 0.1),
                0 0 0 1px rgba(255, 255, 255, 0.1);
            transition: transform 0.3s ease;
        }

        .profile-img:hover {
            transform: translateY(-5px);
        }
<!-- 
        .hero-title {
            font-size: 4.5rem;
            font-weight: 800;
            line-height: 1.1;
            margin-bottom: 1.5rem;
            background: linear-gradient(135deg, var(--primary) 0%, #6366f1 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        } -->

        .hero-subtitle {
            font-size: 1.5rem;
            color: var(--text-secondary);
            margin-bottom: 2rem;
            line-height: 1.6;
        }

        .hero-location {
            display: inline-flex;
            align-items: center;
            gap: 0.75rem;
            padding: 0.75rem 1.5rem;
            background: rgba(255, 255, 255, 0.8);
            backdrop-filter: blur(10px);
            border-radius: 100px;
            margin-bottom: 2.5rem;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        .hero-location i {
            color: var(--primary);
        }

        .hero-buttons {
            display: flex;
            gap: 1.5rem;
            align-items: center;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            padding: 1rem 2rem;
            border-radius: 100px;
            font-weight: 600;
            text-decoration: none;
            transition: all 0.3s ease;
            font-size: 1.125rem;
        }

        .btn-primary {
            background: var(--primary);
            color: white;
            box-shadow: 0 10px 20px rgba(37, 99, 235, 0.2);
        }

        .btn-primary:hover {
            background: var(--primary-dark);
            transform: translateY(-2px);
        }

        .btn-outline {
            border: 2px solid rgba(37, 99, 235, 0.2);
            color: var(--primary);
            background: rgba(255, 255, 255, 0.8);
            backdrop-filter: blur(10px);
        }

        .btn-outline:hover {
            border-color: var(--primary);
            background: rgba(37, 99, 235, 0.05);
        }

        .skills-section {
            padding: 1rem 0;
        }

        .section-title {
            text-align: center;
            font-size: 3rem;
            font-weight: 800;
            color: var(--text-primary);
            margin-bottom: 4rem;
            position: relative;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -1rem;
            left: 50%;
            transform: translateX(-50%);
            width: 60px;
            height: 4px;
            background: var(--primary);
            border-radius: 2px;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 2rem;
        }

        .skill-card {
            background: white;
            padding: 2.5rem;
            border-radius: 24px;
            box-shadow: 
                0 20px 40px rgba(0, 0, 0, 0.03),
                0 0 0 1px rgba(0, 0, 0, 0.05);
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .skill-card:hover {
            transform: translateY(-5px);
        }

        .skill-icon {
            font-size: 2rem;
            color: #3563eb;
            margin-bottom: 1rem;
        }

        .skill-card h3 {
            font-size: 1.5rem;
            font-weight: 700;
            margin-bottom: 1rem;
            color: var(--text-primary);
        }

        .skill-card p {
            color: var(--text-secondary);
            line-height: 1.6;
            margin-bottom: 1.5rem;
        }

        .tech-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 0.75rem;
        }

        .tech-tags span {
            background: var(--bg-light);
            padding: 0.5rem 1rem;
            border-radius: 100px;
            font-size: 0.875rem;
            color: var(--text-secondary);
            font-weight: 500;
            transition: all 0.3s ease;
        }

        .tech-tags span:hover {
            background: rgba(37, 99, 235, 0.1);
            color: var(--primary);
        }

        @media (max-width: 1024px) {
            .skills-grid {
                grid-template-columns: 1fr;
            }
        }

        @media (max-width: 768px) {
            .hero-content {
                grid-template-columns: 1fr;
                text-align: center;
                gap: 3rem;
            }

            .hero-image {
                max-width: 280px;
                margin: 0 auto;
            }

            .hero-text {
                align-items: center;
                text-align: center;
            }

            .hero-title {
                font-size: 3rem;
                white-space: normal;
            }

            .hero-buttons {
                justify-content: center;
                flex-direction: column;
                gap: 1rem;
            }

            .hero-location {
                justify-content: center;
            }
        }




    .hero-title {
          font-size: 4.5rem;
          font-weight: 800;
          line-height: 1.1;
          margin-bottom: 1.5rem;
          white-space: nowrap;
          overflow: hidden;
          position: relative;
          width: fit-content;
          background: linear-gradient(135deg, var(--primary) 0%, #6366f1 100%);
          -webkit-background-clip: text;
          -webkit-text-fill-color: transparent;
          clip-path: inset(0 100% 0 0); /* Initially hidden */
          animation: typing 4s steps(20, end) forwards; /* Typing effect */
     }

     .hero-title::after {
          content: '';
          position: absolute;
          right: -4px; /* Cursor position */
          top: 0;
          height: 100%;
          width: 3px;
          background: var(--primary);
          animation: blink 0.5s step-end infinite; /* Blinking effect */
     }

     @keyframes typing {
          from {
                clip-path: inset(0 100% 0 0); /* Text hidden */
          }
          to {
                clip-path: inset(0 0 0 0); /* Text revealed */
          }
     }

     @keyframes blink {
          50% {
                background: transparent; /* Blink effect */
          }
          100% {
                background: var(--primary);
          }
     }

     @media (max-width: 768px) {
          .hero-title {
                font-size: 3rem;
                white-space: normal; /* Allow text to wrap */
          }
     }

    </style>
</head>
<body>
    <div class="hero-section">
        <div class="container">
            <div class="hero-content">
                <div class="hero-image">
                    <img src="{{ '/assets/images/me.webp' | relative_url }}" alt="Chernet Asmamaw" class="profile-img">
                </div>
                <div class="hero-text">
                    <h1 class="hero-title" style="background: linear-gradient(to right, #74748b, #3563eb); -webkit-background-clip: text; color: transparent; font-weight: 700;">Hi, I'm Chernet 🫶</h1>
                    <p class="hero-subtitle" style="font-family: Verdana">Crafting innovative digital solutions through Full-Stack Development</p>
                    
                    <div class="hero-buttons">
                        <a href="/cv" class="btn btn-primary">
                            <i class="fas fa-code"></i>
                            Curriculum Vitea
                        </a>
                        <a href="/contact" class="btn btn-outline">
                            <i class="fas fa-paper-plane"></i>
                            Get in Touch
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <section class="skills-section">
        <div class="container">
            <h2 class="section-title" style="background: linear-gradient(to right, #74748b, #3563eb); -webkit-background-clip: text; color: transparent;">What I Do</h2>
            <div class="skills-grid">
                <div class="skill-card">
                    <div class="skill-icon">
                        <i class="fas fa-code"></i>
                    </div>
                    <h3>Full Stack Development</h3>
                    <p>Crafting scalable web applications with modern frameworks and clean architecture</p>
                    <div class="tech-tags">
                        <span>React</span>
                        <span>Node.js</span>
                        <span>Python</span>
                    </div>
                </div>

                <div class="skill-card">
                    <div class="skill-icon">
                        <i class="fas fa-mobile-alt"></i>
                    </div>
                    <h3>Mobile Development</h3>
                    <p>Building native and cross-platform mobile experiences that users love</p>
                    <div class="tech-tags">
                        <span>React Native</span>
                        <span>Flutter</span>
                        <span>Swift</span>
                    </div>
                </div>

                <div class="skill-card">
                    <div class="skill-icon">
                        <i class="fas fa-brain"></i>
                    </div>
                    <h3>AI & Research</h3>
                    <p>Implementing cutting-edge AI solutions to solve complex problems</p>
                    <div class="tech-tags">
                        <span>TensorFlow</span>
                        <span>PyTorch</span>
                        <span>ML</span>
                    </div>
                </div>

                <div class="skill-card">
                    <div class="skill-icon">
                        <i class="fas fa-database"></i>
                    </div>
                    <h3>Data Analysis</h3>
                    <p>Transforming raw data into actionable insights through advanced analytics</p>
                    <div class="tech-tags">
                        <span>Python</span>
                        <span>R</span>
                        <span>SQL</span>
                    </div>
                </div>
            </div>
        </div>
    </section>



</body>
</html>