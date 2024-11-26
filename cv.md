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
            <h1 style="background: linear-gradient(135deg, #4a90e2, #6c757d); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">Chernet Asmamaw</h1>
            <div class="contact-info" style="background: linear-gradient(135deg, rgba(74, 144, 226, 0.1), rgba(108, 117, 125, 0.1));">
                <span><i class="fas fa-envelope me-2"></i> c.asmamaw@alustudent.com</span>
                <span><i class="fas fa-phone me-2"></i> +251-98-8257-788</span>
                <span><i class="fas fa-map-marker-alt me-2"></i> Kigali, Rwanda</span>
            </div>
            <div class="mt-4">
                <a href="/assets/pdf/RESUME.pdf" class="btn btn-primary btn-lg" download style="background: linear-gradient(135deg, #4a90e2, #6c757d); border: none;">
                    <i class="fas fa-download me-2"></i>Download CV
                </a>
            </div>
        </header>

    <style>
        :root {
            --primary: #4a90e2;
            --secondary: #6c757d;
        }

        .timeline {
            position: relative;
            padding: 0;
            list-style: none;
        }

        .timeline::before {
            content: '';
            position: absolute;
            top: 0;
            bottom: 0;
            width: 4px;
            background: var(--primary);
            left: 20px;
            margin-left: -2px;
        }

        .timeline-item {
            position: relative;
            margin-bottom: 2rem;
        }

        .timeline-icon {
            position: absolute;
            left: 12px;
            top: 0;
            width: 16px;
            height: 16px;
            border-radius: 50%;
            background: var(--primary);
            border: 4px solid white;
            box-shadow: 0 0 0 2px var(--primary);
        }

        .timeline-content {
            margin-left: 40px;
            background: white;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
        }

        .experience-card {
            padding: 1.5rem;
        }

        .experience-card:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .text-primary {
            color: var(--primary) !important;
            font-size: 0.9rem;
            font-weight: 500;
        }

        .text-secondary {
            color: var(--secondary) !important;
        }

        .badge-custom {
            display: inline-block;
            padding: 0.4rem 0.8rem;
            margin: 0.2rem;
            border-radius: 20px;
            background: rgba(74, 144, 226, 0.1);
            color: var(--primary);
            font-size: 0.85rem;
            transition: all 0.2s ease;
        }

        .badge-custom:hover {
            background: var(--primary);
            color: white;
        }

        .timeline-list {
            max-height: none;
            overflow: hidden;
            transition: max-height 0.3s ease;
            padding-left: 1.2rem;
        }

        .timeline-list.collapsed {
            max-height: 80px;
        }

        .timeline-list li {
            margin-bottom: 0.8rem;
            line-height: 1.5;
        }

        .read-more-btn {
            display: none;
            background: none;
            border: none;
            color: var(--primary);
            padding: 0.5rem 0;
            margin-top: 0.5rem;
            cursor: pointer;
            font-weight: 500;
            text-decoration: underline;
        }

        /* Responsive Styles */
        @media (max-width: 768px) {
            .experience-card {
                padding: 1rem;
            }

            .timeline-content {
                margin-left: 35px;
            }

            .badge-custom {
                padding: 0.3rem 0.6rem;
                font-size: 0.75rem;
                margin: 0.15rem;
            }

            .read-more-btn {
                display: block;
            }

            /* Adjust heading sizes for mobile */
            .h4 {
                font-size: 1.1rem;
            }

            .h5 {
                font-size: 0.95rem;
            }

            /* Make badges wrap better on mobile */
            .badge-container {
                display: flex;
                flex-wrap: wrap;
                gap: 0.25rem;
                margin-top: 0.75rem;
            }
        }

        /* Animation for collapse/expand */
        .timeline-list {
            transition: max-height 0.3s ease-out;
        }
    </style>

    <script>
        // Initialize read more functionality
        document.addEventListener('DOMContentLoaded', function() {
            // Function to handle the read more toggle
            function initializeReadMore() {
                document.querySelectorAll('.timeline-list').forEach(list => {
                    const readMoreBtn = list.nextElementSibling;
                    
                    if (window.innerWidth <= 768) {
                        list.classList.add('collapsed');
                        readMoreBtn.style.display = 'block';
                        
                        readMoreBtn.addEventListener('click', function() {
                            const isCollapsed = list.classList.contains('collapsed');
                            list.classList.toggle('collapsed');
                            this.textContent = isCollapsed ? 'Read Less' : 'Read More';
                            
                            if (isCollapsed) {
                                list.style.maxHeight = list.scrollHeight + 'px';
                            } else {
                                list.style.maxHeight = '80px';
                            }
                        });
                    } else {
                        list.classList.remove('collapsed');
                        readMoreBtn.style.display = 'none';
                        list.style.maxHeight = 'none';
                    }
                });
            }

            // Initialize on load
            initializeReadMore();

            // Re-initialize on window resize
            let resizeTimer;
            window.addEventListener('resize', function() {
                clearTimeout(resizeTimer);
                resizeTimer = setTimeout(initializeReadMore, 250);
            });
        });
    </script>

    <!-- Professional Summary -->
    <section class="mb-5">
        <h2 class="section-title">Professional Summary</h2>
        <div class="experience-card">
            <p class="lead" style="font-family: sans-serif; font-size: 1.2rem;">
                Final-year Software Engineering student at the African Leadership University with a First Class Honors. Skilled in full-stack development, AI tools, and low-level programming. Passionate about solving real-world challenges, I have led projects in education technology, conservation, and community development. Experienced in operations, stakeholder engagement, and building scalable tech solutions.
            </p>      
        </div>
    </section>


    <!-- Professional Experience -->
    <section class="mb-5">
        <h2 class="section-title">Professional Experience</h2>
        <div class="timeline">
            <div class="timeline-item">
                <div class="timeline-icon"></div>
                <div class="timeline-content">
                    <div class="experience-card">
                        <div class="d-flex justify-content-between align-items-center mb-3">
                            <h3 class="h4 mb-0">Operations Intern</h3>
                            <span class="text-primary">August 2024 - Present</span>
                        </div>
                        <h4 class="h5 text-secondary mb-3">School of Wildlife Conservation (SOWC)</h4>
                        <ul class="timeline-list">
                            <li>Worked on data management and analysis for the Business of Conservation Conference (BCC).</li>
                            <li>Assisted in event management using the Swoogo platform to streamline operations.</li>
                            <li>Generated data for insights, enhancing my data science skills.</li>
                            <li>Collaborated closely with SOWC management on 7 initiatives, including masterclasses and hackathons.</li>
                            <li>Increased conservation efforts and student engagement on the ALU campus.</li>
                            <li>Improved my research and presentation skills.</li>                 
                        </ul>
                        <button class="read-more-btn">Read More</button>
                        <div class="badge-container">
                            <span class="badge-custom">Event Management</span>
                            <span class="badge-custom">Data Analysis</span>
                            <span class="badge-custom">Collaboration</span>
                        </div>
                    </div>
                </div>
            </div>

            <div class="timeline-item">
                <div class="timeline-icon"></div>
                <div class="timeline-content">
                    <div class="experience-card">
                        <div class="d-flex justify-content-between align-items-center mb-3">
                            <h3 class="h4 mb-0">Coding Intern</h3>
                            <span class="text-primary">January 2024 - May 2024</span>
                        </div>
                        <h4 class="h5 text-secondary mb-3">The SOZO Foundation</h4>
                        <ul class="timeline-list">
                            <li>Developed a voting and survey collection app that is now live within SOZO.</li>
                            <li>Assessed the need for and proposed a comprehensive development plan for a student engagement platform, and built it using programming skills.</li>
                            <li>Organized tech workshops teaching business owners how to utilize tech to scale their businesses.</li>
                            <li>Collaborated with entrepreneurs to develop their venture ideas and business plans, and assisted in developing business websites.</li>
                            <li>Volunteered in baking, barista training, nail tech, and hair-cutting programs, acquiring diverse practical skills.</li>
                        </ul>
                        <button class="read-more-btn">Read More</button>
                        <div class="badge-container">
                            <span class="badge-custom">App Development</span>
                            <span class="badge-custom">Tech Workshops</span>
                            <span class="badge-custom">Entrepreneurship</span>
                        </div>
                    </div>
                </div>
            </div>

            <div class="timeline-item">
                <div class="timeline-icon"></div>
                <div class="timeline-content">
                    <div class="experience-card">
                        <div class="d-flex justify-content-between align-items-center mb-3">
                            <h3 class="h4 mb-0">Freshwater and Community Conservation Extern</h3>
                            <span class="text-primary">Feb 2024 - Apr 2024</span>
                        </div>
                        <h4 class="h5 text-secondary mb-3">NGS & TNC | Remote | Part-time</h4>
                        <ul class="timeline-list">
                            <li>Conducted a landscape and gap analysis to identify freshwater challenges in Ethiopia.</li>
                            <li>Collaborated with community leaders and experts to gather insights.</li>
                            <li>Utilized primary and secondary research methods to investigate ongoing efforts and underlying issues.</li>
                            <li>Created a story map using ArcGIS StoryMaps to communicate findings effectively and raise awareness.</li>
                            <li>Contributed actionable recommendations for local freshwater conservation initiatives.</li>
                        </ul>
                        <button class="read-more-btn">Read More</button>
                        <div class="badge-container">
                            <span class="badge-custom">Research</span>
                            <span class="badge-custom">Data Analysis</span>
                            <span class="badge-custom">Storytelling</span>
                        </div>
                    </div>
                </div>
            </div>

            <div class="timeline-item">
                <div class="timeline-icon"></div>
                <div class="timeline-content">
                    <div class="experience-card">
                        <div class="d-flex justify-content-between align-items-center mb-3">
                            <h3 class="h4 mb-0">Technical Intern</h3>
                            <span class="text-primary">Sept 2023 - Dec 2023</span>
                        </div>
                        <h4 class="h5 text-secondary mb-3">Caribou Digital | UK/Remote | Full-time</h4>
                        <ul class="timeline-list">
                            <li>Contributed to developing an internal tool to enhance Caribu's operational processes, reducing manual tasks and improving efficiency through AI.</li>
                            <li>Assisted with the project brief and documentation, showcasing my writing and organizational skills.</li>
                            <li>Developed a prototype for the final app using the Retrieval Augmented Generation (RAG) process.</li>
                            <li>Learned multiple new technologies, enhancing my technical skills and expanding my knowledge of AI and machine learning.</li>
                            <li>Collaborated with team members to ensure the successful implementation of the tool.</li>                 
                        </ul>
                        <button class="read-more-btn">Read More</button>
                        <div class="badge-container">
                            <span class="badge-custom">AI</span>
                            <span class="badge-custom">Machine Learning</span>
                            <span class="badge-custom">Prototyping</span>
                        </div>
                    </div>
                </div>
            </div>

            <div class="timeline-item">
                <div class="timeline-icon"></div>
                <div class="timeline-content">
                    <div class="experience-card">
                        <div class="d-flex justify-content-between align-items-center mb-3">
                            <h3 class="h4 mb-0">Gaming Market Research & Analytics Externship</h3>
                            <span class="text-primary">Nov 2023 - Dec 2023</span>
                        </div>
                        <h4 class="h5 text-secondary mb-3">Mobalytics | Paragon One | Remote | Part-time</h4>
                        <ul class="timeline-list">
                            <li>Conducted competitive analysis of FPS and MOBA mobile games to understand the mobile gaming industry.</li>
                            <li>Enhanced research and analytical skills through detailed market analysis.</li>
                            <li>Identified key player personas and their gaming experiences.</li>
                            <li>Explored player psychology and its impact on game engagement.</li>
                            <li>Presented insights on game revenue models and market expansion opportunities to the Mobalytics team.</li>                 
                        </ul>
                        <button class="read-more-btn">Read More</button>
                        <div class="badge-container">
                            <span class="badge-custom">Market Research</span>
                            <span class="badge-custom">Analytics</span>
                            <span class="badge-custom">Presentation</span>
                        </div>
                    </div>
                </div>
            </div>
            <!-- Add more timeline items as needed -->
        </div>
    </section>

      

        <!-- Certifications -->
        <section class="mb-5">
            <h2 class="section-title">Certifications</h2>
            <div class="row g-4">
                
                <div class="col-md-3 col-sm-6">
                    <a href="https://coursera.org/share/7bed351acf34e1a4db3f631e92e6c09e" target="_blank" style="text-decoration: none;">
                        <div class="certificate-frame">
                            <h5 class="certificate-title">Python For Everybody Specialization</h5>
                            <p class="text-secondary mb-1">Coursera | 5 Certificates</p>
                            <p class="text-secondary mb-2">University of Michigan</p>
                            <p class="text-success mb-0">December 2023</p>
                        </div>
                    </a>
                </div>

                <div class="col-md-3 col-sm-6">
                    <div class="certificate-frame">
                        <h5 class="certificate-title">Meta Back-End Developer Professional Certificates</h5>
                        <p class="text-secondary mb-1">Coursera | 7 Certificates</p>
                        <p class="text-secondary mb-2">Meta</p>
                        <p class="text-success mb-0">May 2024</p>
                    </div>
                </div>

                <div class="col-md-3 col-sm-6">
                    <div class="certificate-frame">
                        <h5 class="certificate-title">Meta Front-End Developer Professional Certificates</h5>
                        <p class="text-secondary mb-1">Coursera | 7 Certificates</p>
                        <p class="text-secondary mb-2">Meta</p>
                        <p class="text-success mb-0">July 2024</p>
                    </div>
                </div>

                <div class="col-md-3 col-sm-6">
                    <div class="certificate-frame">
                        <h5 class="certificate-title">Algorithmic Toolbox: Data Structures and Algorithms Specialization</h5>
                        <p class="text-secondary mb-2">Coursera</p>
                        <p class="text-secondary mb-2">University of California San Diego</p>
                        <p class="text-success mb-0">January 2023</p>
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
                        <h5 class="certificate-title">Internet History, Technology, and Security</h5>
                        <p class="text-secondary mb-1">Coursera</p>
                        <p class="text-secondary mb-2">University of Michigan</p>
                        <p class="text-success mb-0">January 2023</p>
                    </div>
                </div>

                <div class="col-md-3 col-sm-6">
                    <div class="certificate-frame">
                        <h5 class="certificate-title">Google IT Automation with Python Professional Certificate</h5>
                        <p class="text-secondary mb-2">Coursera</p>
                        <p class="text-secondary mb-2">Google</p>
                        <p class="text-success mb-0">January 2023</p>
                    </div>
                </div>

                <div class="col-md-3 col-sm-6">
                    <div class="certificate-frame">
                        <h5 class="certificate-title">Configuration Management and the Cloud</h5>
                        <p class="text-secondary mb-2">Coursera</p>
                        <p class="text-secondary mb-2">Google</p>
                        <p class="text-success mb-0">January 2023</p>
                    </div>
                </div>

                <div class="col-md-3 col-sm-6">
                    <div class="certificate-frame">
                        <h5 class="certificate-title">DevOps Culture and Mindset Course</h5>
                        <p class="text-secondary mb-2">Coursera</p>
                        <p class="text-secondary mb-1">University of California, Davis</p>
                        <p class="text-success mb-0">January 2023</p>
                    </div>
                </div>


                <div class="col-md-3 col-sm-6">
                    <div class="certificate-frame">
                        <h5 class="certificate-title">IBM DevOps and Software Engineering Professional Certificate</h5>
                        <p class="text-secondary mb-2">Coursera</p>
                        <p class="text-secondary mb-1">Introduction to DevOps</p>
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
            <h2 class="section-title">Hobbies</h2>
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