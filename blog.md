<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tech Journey & Insights</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body {
            background-color: #f4f6f9;
            font-family: 'Inter', sans-serif;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
        }

        .header-gradient {
            <!-- background: #d8e9f3; -->
            color: #003f5c;
            padding: 2rem 0;
            margin-bottom: 2rem;
            clip-path: polygon(0 0, 100% 0, 100% 85%, 0 100%);
        }

        .header-gradient h1 {
            font-weight: 700;
        }

        .btn-filter {
            transition: all 0.3s ease;
            border: none;
        }

        .btn-filter:hover {
            transform: scale(1.05);
            background-color: #004b6f;
            color: white;
        }

        .card {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            border: none;
            background-color: #ffffff;
            padding: 2rem;
            text-align: center;
            border-radius: 12px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.1);
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 12px 24px rgba(0, 0, 0, 0.15);
        }

        .card-title {
            font-size: 1.5rem;
            font-weight: 600;
            color: #3a3a3a;
        }

        .filter-container {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            justify-content: center;
            margin-bottom: 2rem;
        }

        @media (max-width: 576px) {
            .filter-container .btn-filter {
                flex: 1 0 100%;
                margin-bottom: 0.5rem;
            }
        }

        .coming-soon-card {
            display: flex;
            align-items: flex-start;
            margin: 10rem auto;
            max-width: 400px;
            animation: fadeIn 0.6s ease forwards;
            opacity: 0;
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

        footer {
            background-color: #d8e9f3;
            color: #003f5c;
            padding: 1rem 0;
            text-align: center;
            margin-top: auto;
        }
    </style>
</head>
<body>
    <header class="header-gradient text-center">
        <div class="container">
            <h1 style="background: linear-gradient(to right, #8b4513, #2563eb); -webkit-background-clip: text; color: transparent; font-weight: 700;">My Tech Journey & Insights</h1>

            <p class="lead">Sharing knowledge, experiences, and discoveries in software development</p>
        </div>
    </header>

    <main class="container">
        <!-- <div class="filter-container">
            <button class="btn btn-filter" style="background-color: #004b6f; color: white;">All Posts</button>
            <button class="btn  btn-filter" style="color: #004b6f">Web Development</button>
            <button class="btn  btn-filter" style="color: #004b6f;">Mobile Development</button>
            <button class="btn  btn-filter" style="color: #004b6f;">DevOps</button>
            <button class="btn  btn-filter" style="color: #004b6f;">Tutorial</button>
        </div> -->

        <div class="coming-soon-card">
            <div class="card">
                <div class="card-body">
                    <h4 class="card-title">Coming Soon...</h4>
                    <p class="text-muted">Exciting content is on the way. Stay tuned for updates!</p>
                </div>
            </div>
        </div>
    </main>


    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
