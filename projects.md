<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Featured Projects</title>
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
            margin: 0 auto;
            padding: 0 2rem;
        }

        .section-header {
            text-align: center;
            margin-bottom: 4rem;
        }

        .section-header p {
            color: var(--text-secondary);
            font-size: 1.125rem;
        }

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 2rem;
        }

        .project-card {
            background: white;
            border-radius: 24px;
            box-shadow: 
                0 20px 40px rgba(0, 0, 0, 0.05),
                0 0 0 1px rgba(0, 0, 0, 0.05);
            overflow: hidden;
            transition: all 0.3s ease;
            position: relative;
        }

        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 
                0 30px 60px rgba(0, 0, 0, 0.1),
                0 0 0 1px rgba(0, 0, 0, 0.05);
        }

        .project-image {
            width: 100%;
            height: 250px;
            object-fit: cover;
            transition: transform 0.3s ease;
        }

        .project-card:hover .project-image {
            transform: scale(1.05);
        }

        .project-content {
            padding: 2rem;
        }

        .project-title {
            font-size: 1.75rem;
            font-weight: 700;
            margin-bottom: 1rem;
            color: var(--text-primary);
        }

        .project-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-bottom: 1rem;
        }

        .project-tag {
            padding: 0.25rem 0.75rem;
            border-radius: 100px;
            font-size: 0.75rem;
            font-weight: 600;
            background: var(--bg-light);
            color: var(--text-secondary);
            transition: all 0.3s ease;
        }

        .project-tag:hover {
            background: rgba(37, 99, 235, 0.1);
            color: var(--primary);
        }

        .project-description {
            color: var(--text-secondary);
            margin-bottom: 1rem;
            line-height: 1.6;
        }

        .project-features {
            margin-bottom: 1rem;
        }

        .project-features h3 {
            font-size: 1rem;
            font-weight: bold;
            margin-bottom: 0.5rem;
        }

        .project-features ul {
            list-style-type: none;
            padding-left: 0;
        }

        .project-features li {
            position: relative;
            padding-left: 1.5rem;
            margin-bottom: 0.5rem;
            color: var(--text-secondary);
            font-size: 14px;
        }

        .project-features li::before {
            content: '•';
            position: absolute;
            left: 0;
            color: var(--primary);
            font-weight: bold;
        }

        .project-stats {
            display: flex;
            justify-content: space-between;
            margin-bottom: 1.5rem;
        }

        .project-stat {
            text-align: center;
        }

        .project-stat-value {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--primary);
        }

        .project-stat-label {
            font-size: 0.875rem;
            color: var(--text-secondary);
        }

        .project-actions {
            display: flex;
            gap: 1rem;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            padding: 0.75rem 1.5rem;
            border-radius: 100px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
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
        }

        .btn-outline:hover {
            border-color: var(--primary);
            background: rgba(37, 99, 235, 0.05);
        }

        @media (max-width: 1024px) {
            .projects-grid {
                grid-template-columns: 1fr;
            }
        }

        @media (max-width: 768px) {
            .section-header h1 {
                font-size: 2.5rem;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header class="section-header">
            <h1 style="background: linear-gradient(to right, #8b4513, #2563eb); -webkit-background-clip: text; color: transparent; font-weight: 700;">Featured Projects</h1>
            <p style="color: #004b6f;">A showcase of my technical expertise and problem-solving abilities</p>
        </header>
         <div class="projects-grid">
             <div class="project-card">
              <img src="/assets/images/project1.png" alt="Community Connect" class="project-image">
              <div class="project-content">
                  <h2 class="project-title">Community Connect</h2>
                  <div class="project-tags">
                   <span class="project-tag">Next.js</span>
                   <span class="project-tag">React</span>
                   <span class="project-tag">MongoDB</span>
                  </div>
                  <p class="project-description">
                   Connect communities with local services and artisans.
                  </p>
                  <div class="project-features">
                   <h3>Key Features</h3>
                   <ul class="features-list">
                    <li><strong>Service and Artisan Directory:</strong> Discover local businesses and talented artisans in your area.</li>
                    <li><strong>Location-Based Search:</strong> Find businesses and services tailored to your proximity.</li>
                    <li><strong>User Reviews and Ratings:</strong> Make confident decisions with trusted feedback from your community.</li>
                   </ul>
                  </div>
                  <div class="project-actions">
                   <a href="https://community-connect-five.vercel.app/" target='_blank' class="btn btn-primary">Live Demo</a>
                   <a href="https://github.com/ChernetAsmamaw/Community-Connect.git" class="btn btn-outline">GitHub</a>
                  </div>
              </div>
             </div>
             <div class="project-card">
              <div class="project-content">
                  <h2 class="project-title"> Small React Projects</h2>
                  <div class="project-tags">
                   <span class="project-tag">React</span>
                   <span class="project-tag">JavaScript</span>
                   <span class="project-tag">CSS</span>
                  </div>
                  <div class="project-description">
                   <p>
                    Explore my simple projects built while learning React. Both the Budget as well as the weather app are simple yet sophisticated with graphs and pie charts.
                   </p>
                  </div>
                  <div class="project-features">
                   <h3>Budgeting App</h3>
                   <ul class="features-list">
                    <li><strong>Expense Tracking:</strong> Monitor your spending and manage your budget.</li>
                    <li><strong>Category Management:</strong> Organize expenses into categories.</li>
                   </ul>
                   <div class="project-actions">
                    <a href="https://chernetasmamaw.github.io/Budgeting-app/" target='_blank' class="btn btn-primary">Live Demo</a>
                    <a href="https://github.com/ChernetAsmamaw/Budgeting-App" class="btn btn-outline">GitHub</a>
                   </div>
                  </div>
                  <hr style="margin: 2rem 0;">
                  <div class="project-features">
                   <h3>Weather App</h3>
                   <ul class="features-list">
                    <li><strong>Weather:</strong> Get real-time weather updates for any location</li>
                    <li><strong>Forcast:</strong> View the wather for the next 24h.</li>
                    <li><strong>Search by City:</strong> Find weather information by city or country.</li>
                   </ul>
                   <div class="project-actions">
                    <a href="https://chernetasmamaw.github.io/Weather_APP_TS-REACT/" target='_blank' class="btn btn-primary">Live Demo</a>
                    <a href="https://github.com/ChernetAsmamaw/Weather_APP_TS-REACT" class="btn btn-outline">GitHub</a>
                   </div>
                  </div>
                  <style>
                    .card {
                        border-radius: 15px;
                        background-color: #ffffff;
                    }

                    .logo-placeholder {
                        display: flex;
                        justify-content: center;
                        align-items: center;
                        font-size: 1.2rem;
                        color: white;
                        font-weight: bold;
                    }

                    .project-actions .btn {
                        margin-top: 10px;
                    }

                    .card .row > div {
                        text-align: center;
                    }

                    .card .row .border-end {
                        border-color: #d1d5db;
                    }

                  </style>
              </div>
             </div>
         </div>
        
    </div>
    
</body>
</html>