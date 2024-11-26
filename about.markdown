<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chernet</title>
    <!-- Bootstrap CSS -->
    <link href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.0/css/bootstrap.min.css" rel="stylesheet">
    <!-- Font Awesome -->
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap');

        body {
            background-color: #f8f9fa;
            font-family: 'Inter', sans-serif;
            color: #333;
            line-height: 1.7;
        }

        .main-content {
            min-height: 72vh;
            display: flex;
            align-items: center;
            padding: 4rem 0;
        }

        .profile-container {
            background-color: white;
            border-radius: 15px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.1);
            padding: 2.5rem;
            transition: transform 0.3s ease;
        }

        .profile-container:hover {
            transform: translateY(-10px);
        }

        .profile-image {
            width: 250px;
            height: 250px;
            object-fit: cover;
            border-radius: 50%;
            border: 5px solid #e9ecef;
            box-shadow: 0 10px 25px rgba(0,0,0,0.15);
            transition: all 0.3s ease;
        }

        .profile-image:hover {
            transform: scale(1.05);
        }

        .profile-info h2 {
            color: #2c3e50;
            font-weight: 700;
            margin-bottom: 0.5rem;
        }

        .profile-subtitle {
            color: #6c757d;
            margin-bottom: 0.75rem;
        }

        .about-section h1 {
            color: #10477d;
            font-weight: 700;
            border-bottom: 3px solid #3498db;
            padding-bottom: 0.5rem;
            margin-bottom: 1.5rem;
        }

        .about-section {
            padding: 1rem;
        }

        .about-section p {
            margin-bottom: 1rem;
            text-align: start;
            font-family: San-sarif;
            padding-right: 0.7rem;
        }

        .btn-custom {
            margin: 0.5rem;
            border-radius: 50px;
            padding: 10px 20px;
            font-weight: 600;
            transition: all 0.3s ease;
        }

        .btn-custom:hover {
            transform: translateY(-5px);
            box-shadow: 0 7px 14px rgba(0,0,0,0.1);
        }

        @media (max-width: 768px) {
            .profile-container {
                text-align: center;
                padding: 1.5rem;
            }
            .profile-image {
                width: 200px;
                height: 200px;
            }
        }
    </style>
</head>
<body>
    <main id="content" class="main-content">
        <div class="container">
            <div class="profile-container">
                <div class="row align-items-center">
                    <div class="col-md-4 text-center">
                        <img src="/assets/images/me.webp" alt="Chernet Asmamaw" class="profile-image mb-4">
                        <div class="profile-info">
                            <h2>Chernet Asmamaw</h2>
                            <p class="profile-subtitle">
                                <i class="fas fa-graduation-cap me-2"></i>Software Engineering Student
                            </p>
                            <p class="profile-subtitle">
                                <i class="fas fa-map-marker-alt me-2"></i>Kigali, Rwanda
                            </p>
                        </div>
                    </div>
                    <div class="col-md-8">
                        <div class="about-section">
                            <h1>About Me</h1>
                            <i class="my-2">
                                <p class="lead">
                                    I am a passionate software engineer specializing in creating innovative, impactful solutions to address real-world challenges. With expertise in full-stack development, artificial intelligence, and low-level programming, I continuously strive to push the boundaries of technology.
                                </p>
                            </i>
                            <p>
                                Currently completing my final year at African Leadership University, I have developed comprehensive skills in mobile application development, data analysis, and research methodologies. My academic journey has strengthened my technical expertise and instilled a profound drive for innovation.
                            </p>
                            <p>
                                I am actively involved in tech communities, collaborating on open-source projects and mentoring aspiring developers. I believe in the transformative power of teamwork and continuous learning to advance technological progress.
                            </p>
                            <div class="mt-4 text-left">
                                <a href="/contact" class="btn btn-primary btn-lg btn-custom">
                                    <i class="fas fa-envelope me-2"></i>Get in Touch
                                </a>
                                <a href="https://www.linkedin.com/in/chernet-asmamaw/" target="_blank" class="btn btn-outline-primary btn-lg btn-custom">
                                    <i class="fab fa-linkedin me-2"></i>Connect on LinkedIn
                                </a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </main>

    <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.0/js/bootstrap.bundle.min.js"></script>
</body>
</html>