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
        }
        .header-gradient {
            background: linear-gradient(135deg, #6a11cb 0%, #2575fc 100%);
            color: white;
            padding: 2rem 0;
            margin-bottom: 2rem;
            clip-path: polygon(0 0, 100% 0, 100% 85%, 0 100%);
        }
        .card {
            transition: all 0.3s ease;
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
            border: none;
            overflow: hidden;
        }
        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.15);
        }
        .card-img-top {
            transition: transform 0.3s ease;
        }
        .card:hover .card-img-top {
            transform: scale(1.1);
        }
        .btn-filter {
            transition: all 0.3s ease;
        }
        .btn-filter:hover {
            transform: scale(1.05);
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .post-card {
            animation: fadeIn 0.6s ease forwards;
            opacity: 0;
        }
        .post-card:nth-child(1) { animation-delay: 0.2s; }
        .post-card:nth-child(2) { animation-delay: 0.4s; }
        .post-card:nth-child(3) { animation-delay: 0.6s; }
    </style>
</head>
<body>
    <div class="header-gradient text-center py-5">
        <div class="container">
            <h1 class="display-4 fw-bold mb-3">My Tech Journey & Insights</h1>
            <p class="lead text-white-50">Sharing knowledge, experiences, and discoveries in software development</p>
        </div>
    </div>

    <div class="container">
        <div class="d-flex justify-content-center mb-5">
            <div class="btn-group" role="group">
                <button class="btn btn-primary btn-filter mx-2">All Posts</button>
                <button class="btn btn-outline-primary btn-filter mx-2">Web Development</button>
                <button class="btn btn-outline-primary btn-filter mx-2">Software Architecture</button>
                <button class="btn btn-outline-primary btn-filter mx-2">DevOps</button>
                <button class="btn btn-outline-primary btn-filter mx-2">Tutorial</button>
            </div>
        </div>

        <section class="row g-4">
            <div class="col-md-4 post-card">
                <div class="card h-100 w-100">
                    <img src="/assets/images/post2.jpeg" class="card-img-top" alt="Post image">
                    <div class="card-body">
                        <h5 class="card-title">Getting Started with Next.js</h5>
                        <p class="card-text text-muted">A comprehensive guide to building your first application with Next.js...</p>
                        <div class="d-flex justify-content-between align-items-center">
                            <small class="text-muted">Web Development</small>
                            <small class="text-muted">6 min read</small>
                        </div>
                    </div>
                </div>
            </div>
            <div class="col-md-4 post-card">
                <div class="card h-100 w-100 text-center d-flex align-items-center justify-content-center">
                    <div class="card-body">
                        <h4 class="card-title text-muted">More coming soon...</h4>
                        <p>Stay tuned for new content!</p>
                    </div>
                </div>
            </div>
        </section>
            
    </div>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>