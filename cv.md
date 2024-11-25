<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.2/css/bootstrap.min.css" rel="stylesheet">
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css" rel="stylesheet">
    <style>
        :root {
            --primary: #2563eb;
            --secondary: #1e40af;
            --accent: #ef4444;
            --text-primary: #1f2937;
            --text-secondary: #4b5563;
        }

        body {
            font-family: 'Inter', system-ui, -apple-system, sans-serif;
            background: linear-gradient(135deg, #f8fafc 0%, #f1f5f9 100%);
            color: var(--text-primary);
            line-height: 1.7;
        }

        /* Header Animations */
        header {
            opacity: 0;
            animation: fadeInDown 1s ease forwards;
        }

        /* Section Animations */
        section {
            opacity: 0;
            animation: fadeInUp 1s ease forwards;
            animation-delay: 0.3s;
        }

        /* Header Styles */
        header h1 {
            font-size: 3.5rem;
            font-weight: 800;
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 1.5rem;
        }

        .contact-info {
            background: rgba(255, 255, 255, 0.9);
            border-radius: 50px;
            padding: 1rem 2rem;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
            display: inline-flex;
            gap: 2rem;
        }

        .contact-info i {
            color: var(--primary);
        }

        /* Section Styles */
        .section-title {
            font-size: 2.25rem;
            font-weight: 700;
            color: var(--primary);
            position: relative;
            display: inline-block;
            margin-bottom: 2rem;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 100%;
            height: 4px;
            background: linear-gradient(90deg, var(--primary), transparent);
            border-radius: 2px;
        }

        /* Experience Cards */
        .experience-card {
            background: white;
            border-radius: 16px;
            padding: 2rem;
            margin-bottom: 2rem;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
            transform: translateY(0);
            transition: all 0.3s ease;
        }

        .experience-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
        }

        /* Certificate Cards */
        .certificate-frame {
            background: white;
            border-radius: 16px;
            padding: 1.5rem;
            height: 100%;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
            transform: translateY(0);
            transition: all 0.3s ease;
            border: none;
        }

        .certificate-frame:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
        }

        .certificate-title {
            font-size: 1.1rem;
            color: var(--primary);
            margin-bottom: 0.5rem;
        }

        /* Skills Pills */
        .skill-pill {
            background: white;
            color: var(--primary);
            border: 2px solid var(--primary);
            padding: 0.75rem 1.5rem;
            border-radius: 50px;
            display: inline-block;
            font-weight: 500;
            transition: all 0.3s ease;
            margin: 0.5rem;
        }

        .skill-pill:hover {
            background: var(--primary);
            color: white;
            transform: translateY(-3px);
            box-shadow: 0 4px 6px -1px rgba(37, 99, 235, 0.3);
        }

        /* Hobby & Language Cards */
        .hobby-card, .language-card {
            background: white;
            border-radius: 16px;
            padding: 1rem;
            height: 100%;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
        }

        .hobby-card:hover, .language-card:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
        }

        /* Badges */
        .badge-custom {
            background: rgba(37, 99, 235, 0.1);
            color: var(--primary);
            font-weight: 500;
            padding: 0.5rem 1rem;
            border-radius: 50px;
            margin: 0.25rem;
        }

        /* Animations */
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

        /* Responsive adjustments */
        @media (max-width: 768px) {
            header h1 {
                font-size: 2.5rem;
            }
            
            .contact-info {
                flex-direction: column;
                gap: 1rem;
                padding: 1rem;
            }

            .section-title {
                font-size: 1.75rem;
            }
        }
    </style>
</head>
<body>
    <div class="container my-5">
        <!-- Header -->
        <header class="text-center mb-5">
            <h1>Chernet Asmamaw</h1>
            <div class="contact-info">
                <span><i class="fas fa-envelope me-2"></i> c.asmamaw@alustudent.com</span>
                <span><i class="fas fa-phone me-2"></i> +250 79 1500 661</span>
                <span><i class="fas fa-map-marker-alt me-2"></i> Kigali, Rwanda</span>
            </div>
        </header>

        <!-- Professional Summary -->
        <section class="mb-5">
            <h2 class="section-title">Professional Summary</h2>
            <div class="experience-card">
                <p class="lead">
                    Final-year Software Engineering student at the African Leadership University with a predicted First Class Honors. Skilled in full-stack development, AI tools, and low-level programming. Passionate about solving real-world challenges, I have led projects in education technology, conservation, and community development. Experienced in operations, stakeholder engagement, and building scalable tech solutions.
                </p>
            </div>
        </section>

        <!-- Professional Experience -->
        <section class="mb-5">
            <h2 class="section-title">Professional Experience</h2>
            
            <!-- SOWC -->
            <div class="experience-card">
                <div class="d-flex justify-content-between align-items-center mb-3">
                    <h3 class="h4 mb-0">Operations Intern</h3>
                    <span class="text-primary">August 2024 - Present</span>
                </div>
                <h4 class="h5 text-secondary mb-3">School of Wildlife Conservation (SOWC)</h4>
                <ul class="mb-3">
                    <li>Coordinated events, masterclasses, and field trips, enhancing student and faculty engagement.</li>
                    <li>Streamlined operational processes, including data management and reporting.</li>
                    <li>Collaborated on initiatives to expand the impact of conservation-focused programs.</li>
                </ul>
                <div>
                    <span class="badge-custom">Event Management</span>
                    <span class="badge-custom">Data Analysis</span>
                    <span class="badge-custom">Collaboration</span>
                </div>
            </div>

            <!-- Coding Intern -->
            <div class="experience-card">
                <div class="d-flex justify-content-between align-items-center mb-3">
                    <h3 class="h4 mb-0">Coding Intern</h3>
                    <span class="text-primary">Jan 2024 - May 2024</span>
                </div>
                <h4 class="h5 text-secondary mb-3">The SOZO Foundation | Cape Town, South Africa | Full-time</h4>
                <ul class="mb-3">
                    <li>Developed a voting and survey collection app that is now live within SOZO. Assessed the need for and proposed a comprehensive development plan for a student engagement platform, and I’m currently building it using my programming skills.</li>
                    <li>Organized tech workshops teaching business owners how to utilize tech to scale their businesses. Collaborated with entrepreneurs to develop their venture ideas and business plans, and assisted in developing business websites.</li>
                    <li>Volunteered in baking, barista training, nail tech, and hair-cutting programs, acquiring diverse practical skills.</li>
                </ul>
                <div>
                    <span class="badge-custom">App Development</span>
                    <span class="badge-custom">Tech Workshops</span>
                    <span class="badge-custom">Entrepreneurship</span>
                </div>
            </div>
            <!-- Freshwater and Community Conservation Extern -->
            <div class="experience-card">
                <div class="d-flex justify-content-between align-items-center mb-3">
                    <h3 class="h4 mb-0">Freshwater and Community Conservation Extern</h3>
                    <span class="text-primary">Feb 2024 - Apr 2024</span>
                </div>
                <h4 class="h5 text-secondary mb-3">NGS & TNC | Remote | Part-time</h4>
                <ul class="mb-3">
                    <li>Conducted a landscape and gap analysis to identify freshwater challenges in Ethiopia. Collaborated with community leaders and experts to gather insights. Utilized primary and secondary research methods to investigate ongoing efforts and underlying issues.</li>
                    <li>Created a story map using ArcGIS StoryMaps to communicate findings effectively and raise awareness, enhancing my research, data analysis, and storytelling skills, while also contributing actionable recommendations for local freshwater conservation initiatives.</li>
                </ul>
                <div>
                    <span class="badge-custom">Research</span>
                    <span class="badge-custom">Data Analysis</span>
                    <span class="badge-custom">Storytelling</span>
                </div>
            </div>

            <!-- Technical Intern -->
            <div class="experience-card">
                <div class="d-flex justify-content-between align-items-center mb-3">
                    <h3 class="h4 mb-0">Technical Intern</h3>
                    <span class="text-primary">Sept 2023 - Dec 2023</span>
                </div>
                <h4 class="h5 text-secondary mb-3">Caribou Digital | UK/Remote | Full-time</h4>
                <ul class="mb-3">
                    <li>Contributed to the development of an internal tool aimed at enhancing Caribu's operational processes, reducing manual tasks, and improving efficiency through AI. Helped with the project brief and documentation, showcasing my writing and organizational skills.</li>
                    <li>Developed a prototype for the final app using the Retrieval Augmented Generation (RAG) process, which required learning multiple new technologies, enhancing my technical skills, and expanding my knowledge of AI and machine learning.</li>
                </ul>
                <div>
                    <span class="badge-custom">AI Development</span>
                    <span class="badge-custom">Project Documentation</span>
                    <span class="badge-custom">Machine Learning</span>
                </div>
            </div>

            <!-- Gaming Market Research & Analytics Externship -->
            <div class="experience-card">
                <div class="d-flex justify-content-between align-items-center mb-3">
                    <h3 class="h4 mb-0">Gaming Market Research & Analytics Externship</h3>
                    <span class="text-primary">Nov 2023 - Dec 2023</span>
                </div>
                <h4 class="h5 text-secondary mb-3">Mobalytics | Paragon One | Remote | Part-time</h4>
                <ul class="mb-3">
                    <li>Analyzed the competitive landscape of FPS and MOBA gaming genres, focusing on specific mobile games to enhance my understanding of the mobile gaming industry and improve my research and analytical skills.</li>
                    <li>Organized a presentation at the end of my internship, offering the Mobalytics team insights into key topics such as player personas, experience, psychology, and game revenue models, as Mobalytics evaluates opportunities for market expansion.</li>
                </ul>
                <div>
                    <span class="badge-custom">Market Research</span>
                    <span class="badge-custom">Analytical Skills</span>
                    <span class="badge-custom">Presentation</span>
                </div>
            </div>


            <!-- Add other experience cards similarly -->
        </section>

        <!-- Certifications -->
        <section class="mb-5">
            <h2 class="section-title">Certifications</h2>
            <div class="row g-4">
                <!-- Certificate cards with the same structure but enhanced styling -->
                <div class="col-md-3 col-sm-6">
                    <div class="certificate-frame">
                        <h5 class="certificate-title">Meta Backend Specialization</h5>
                        <p class="text-secondary mb-1">Coursera | 7 Certificates</p>
                        <p class="text-secondary mb-2">Meta</p>
                        <p class="text-success mb-0">May 2024</p>
                    </div>
                </div>

                <div class="col-md-3 col-sm-6">
                    <div class="certificate-frame">
                        <h5 class="certificate-title">Meta Front Specialization</h5>
                        <p class="text-secondary mb-1">Coursera | 7 Certificates</p>
                        <p class="text-secondary mb-2">Meta</p>
                        <p class="text-success mb-0">July 2024</p>
                    </div>
                </div>

                <div class="col-md-3 col-sm-6">
                    <div class="certificate-frame">
                        <h5 class="certificate-title">Meta Front Specialization</h5>
                        <p class="text-secondary mb-1">Coursera | 7 Certificates</p>
                        <p class="text-secondary mb-2">Meta</p>
                        <p class="text-success mb-0">July 2024</p>
                    </div>
                </div>

                <div class="col-md-3 col-sm-6">
                    <div class="certificate-frame">
                        <h5 class="certificate-title">Django For Everyone Specialization</h5>
                        <p class="text-secondary mb-1">Coursera | 5 Certificates</p>
                        <p class="text-secondary mb-2">University of Michigan</p>
                        <p class="text-success mb-0">December 2024</p>
                    </div>
                </div>

                <div class="col-md-3 col-sm-6">
                    <div class="certificate-frame">
                        <h5 class="certificate-title">Python For Everybody Specialization</h5>
                        <p class="text-secondary mb-1">Coursera | 5 Certificates</p>
                        <p class="text-secondary mb-2">University of Michigan</p>
                        <p class="text-success mb-0">December 2023</p>
                    </div>
                </div>

                <div class="col-md-3 col-sm-6">
                    <div class="certificate-frame">
                        <h5 class="certificate-title">Internet History, Technology, and Security</h5>
                        <p class="text-secondary mb-1">Coursera</p>
                        <p class="text-secondary mb-2">University of Michigan</p>
                        <p class="text-success mb-0">January 2023</p>
                    </div>
                </div>

                <div class="col-md-3 col-sm-6">
                    <div class="certificate-frame">
                        <h5 class="certificate-title">Data Structures and Algorithms Specialization</h5>
                        <p class="text-secondary mb-1">Algorithmic Toolbox</p>
                        <p class="text-secondary mb-2">University of California San Diego</p>
                        <p class="text-success mb-0">January 2023</p>
                    </div>
                </div>

                <div class="col-md-3 col-sm-6">
                    <div class="certificate-frame">
                        <h5 class="certificate-title">Google IT Automation with Python Professional Certificate</h5>
                        <p class="text-secondary mb-1">Google</p>
                        <p class="text-secondary mb-2">Google</p>
                        <p class="text-success mb-0">January 2023</p>
                    </div>
                </div>

                <div class="col-md-3 col-sm-6">
                    <div class="certificate-frame">
                        <h5 class="certificate-title">Configuration Management and the Cloud</h5>
                        <p class="text-secondary mb-1">Google</p>
                        <p class="text-secondary mb-2">Google</p>
                        <p class="text-success mb-0">January 2023</p>
                    </div>
                </div>

                <div class="col-md-3 col-sm-6">
                    <div class="certificate-frame">
                        <h5 class="certificate-title">DevOps Culture and Mindset</h5>
                        <p class="text-secondary mb-1">University of California, Davis</p>
                        <p class="text-success mb-0">January 2023</p>
                    </div>
                </div>

                <div class="col-md-3 col-sm-6">
                    <div class="certificate-frame">
                        <h5 class="certificate-title">Introduction to GitHub Actions</h5>
                        <p class="text-secondary mb-1">Duke University</p>
                        <p class="text-success mb-0">January 2023</p>
                    </div>
                </div>

                <div class="col-md-3 col-sm-6">
                    <div class="certificate-frame">
                        <h5 class="certificate-title">IBM DevOps and Software Engineering Professional Certificate</h5>
                        <p class="text-secondary mb-1">Introduction to DevOps</p>
                        <p class="text-secondary mb-2">IBM</p>
                        <p class="text-success mb-0">January 2023</p>
                    </div>
                </div>

                <!-- Add other certificate cards similarly -->
            </div>
        </section>

        <!-- Skills -->
        <section class="mb-5">
            <h2 class="section-title">Skills</h2>
            <div class="mb-4">
                <h3 class="h4 text-secondary mb-3">Core Skills</h3>
                <div class="d-flex flex-wrap justify-content-center">
                    <span class="skill-pill">Leadership</span>
                    <span class="skill-pill">Problem-Solving</span>
                    <span class="skill-pill">Communication</span>
                    <span class="skill-pill">Presentation</span>
                    <span class="skill-pill">Organization</span>
                    <span class="skill-pill">Teamwork</span>
                    <span class="skill-pill">Decision-making</span>
                    <span class="skill-pill">Critical Thinking</span>
                    <!-- Add other core skills -->
                </div>
            </div>
            <div>
                <h3 class="h4 text-secondary mb-3">Technical Skills</h3>
                <div class="d-flex flex-wrap justify-content-center">
                    <span class="skill-pill">Python (Django, Flask)</span>
                    <span class="skill-pill">JavaScript (Next.js, React)</span>
                    <span class="skill-pill">GitHub</span>

                    <span class="skill-pill">Flutter</span>
                    <span class="skill-pill">TypeScript</span>
                    <span class="skill-pill">RegEx</span>
                    <span class="skill-pill">Shell</span>
                    <span class="skill-pill">NodeJs</span>
                    <span class="skill-pill">Figma</span>
                    <span class="skill-pill">Canva</span>
                    <span class="skill-pill">Dribble</span>
                    <span class="skill-pill">HTML</span>
                    <span class="skill-pill">CSS (Tailwind, Bootstrap, SASS, SCSS)</span>
                    <span class="skill-pill">Docker</span>
                    <span class="skill-pill">SQL</span>
                    <span class="skill-pill">MongoDB</span>
                    <span class="skill-pill">Firebase</span>
                    <span class="skill-pill">Redis</span>
                    <span class="skill-pill">Render</span>
                    <span class="skill-pill">Vercel</span>
                    <!-- Add other technical skills -->
                </div>
            </div>
        </section>

        <!-- Hobbies Section -->
        <section class="section-header mb-5">
            <h2 class="section-title text-center text-primary mb-4">Hobbies</h2>
            <div class="row text-center">
                <div class="col-md-6 mb-3">
                    <div class="p-3 shadow-sm rounded bg-light">🏃‍♂️ <strong>Running & Hiking</strong></div>
                </div>
                <div class="col-md-6 mb-3">
                    <div class="p-3 shadow-sm rounded bg-light">🍳 <strong>Cooking & Baking</strong></div>
                </div>
                <div class="col-md-6 mb-3">
                    <div class="p-3 shadow-sm rounded bg-light">📸 <strong>Photography</strong></div>
                </div>
                <div class="col-md-6 mb-3">
                    <div class="p-3 shadow-sm rounded bg-light">✈️ <strong>Traveling</strong></div>
                </div>
                <div class="col-md-6 mb-3">
                    <div class="p-3 shadow-sm rounded bg-light">📚 <strong>Poetry & Literature</strong></div>
                </div>
                <div class="col-md-6 mb-3">
                    <div class="p-3 shadow-sm rounded bg-light">🥋 <strong>Martial Arts</strong></div>
                </div>
                <div class="col-md-6 mb-3">
                    <div class="p-3 shadow-sm rounded bg-light">📺 <strong>Watching History Shows</strong></div>
                </div>
                <div class="col-md-6 mb-3">
                    <div class="p-3 shadow-sm rounded bg-light">🎨 <strong>Graphic Design</strong></div>
                </div>
                <div class="col-md-6 mb-3">
                    <div class="p-3 shadow-sm rounded bg-light">⛸️ <strong>Skating</strong></div>
                </div>
                <div class="col-md-6 mb-3">
                    <div class="p-3 shadow-sm rounded bg-light">🏊‍♂️ <strong>Swimming</strong></div>
                </div>
                <div class="col-md-6 mb-3">
                    <div class="p-3 shadow-sm rounded bg-light">🏍️ <strong>Motor Biking</strong></div>
                </div>
                <div class="col-md-6 mb-3">
                    <div class="p-3 shadow-sm rounded bg-light">✏️ <strong>Drawing</strong></div>
                </div>
                <div class="col-md-6 mb-3">
                    <div class="p-3 shadow-sm rounded bg-light">🎨 <strong>Painting</strong></div>
                </div>
                <div class="col-md-6 mb-3">
                    <div class="p-3 shadow-sm rounded bg-light">🎵 <strong>Music</strong></div>
                </div>
            </div>
        </section>

        <!-- Languages -->
        <section class="mb-5">
            <h2 class="section-title">Languages</h2>
            <div class="row g-4">
                <div class="col-md-4">
                    <div class="language-card">
                        <p class="mb-0">🇪🇹 <strong>Amharic</strong> (Native)</p>
                    </div>
                </div>

                <div class="col-md-4">
                    <div class="language-card">
                        <p class="mb-0">🇪🇹 <strong>Guragina</strong> (Native)</p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="language-card">
                        <p class="mb-0">🇬🇧 <strong>English</strong> (Professional)</p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="language-card">
                        <p class="mb-0">🇷🇺 <strong>Russian</strong> (Conversational)</p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="language-card">
                        <p class="mb-0">🇪🇸 <strong>Spanish</strong> (Beginner)</p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="language-card">
                        <p class="mb-0">🇷🇼 <strong>Kinyarwanda</strong> (Basic)</p>
                    </div>
                </div>
                <!-- Add other language cards -->
            </div>
        </section>
    </div>

    <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.2/js/bootstrap.bundle.min.js"></script>
</body>
</html>