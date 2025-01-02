<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Online Course Platform</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
        }
        header {
            background-color: #4CAF50;
            color: white;
            padding: 1rem 2rem;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #333;
        }
        nav a {
            color: white;
            padding: 1rem;
            text-decoration: none;
        }
        nav a:hover {
            background-color: #575757;
        }
        .container {
            padding: 2rem;
        }
        .course {
            background: white;
            margin: 1rem 0;
            padding: 1rem;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        .footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 1rem;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>
    <header>
        <h1>Online Course Platform</h1>
        <p>Upload and sell your courses in Ethiopian Birr (ETB)</p>
    </header>
    <nav>
        <a href="#home">Home</a>
        <a href="#courses">Courses</a>
        <a href="#upload">Upload Course</a>
        <a href="#exam">Exam</a>
        <a href="#contact">Contact</a>
    </nav>

    <div class="container" id="home">
        <h2>Welcome!</h2>
        <p>Create, upload, and manage your courses easily.</p>
    </div>

    <div class="container" id="courses">
        <h2>Available Courses</h2>
        <div class="course">
            <h3>Course Title</h3>
            <p>Description of the course.</p>
            <button>Enroll - 500 ETB</button>
        </div>
        <!-- Additional courses can be added here -->
    </div>

    <div class="container" id="upload">
        <h2>Upload Your Course</h2>
        <form action="/upload" method="POST" enctype="multipart/form-data">
            <label for="title">Course Title:</label><br>
            <input type="text" id="title" name="title" required><br><br>

            <label for="description">Course Description:</label><br>
            <textarea id="description" name="description" required></textarea><br><br>

            <label for="price">Price (ETB):</label><br>
            <input type="number" id="price" name="price" required><br><br>

            <label for="video">Upload Video:</label><br>
            <input type="file" id="video" name="video" accept="video/*" required><br><br>

            <label for="notes">Attach Notes (PDF):</label><br>
            <input type="file" id="notes" name="notes" accept="application/pdf"><br><br>

            <button type="submit">Upload</button>
        </form>
    </div>

    <div class="container" id="exam">
        <h2>Schedule and Take Your Exam</h2>
        <p>Once you finish the course, you can schedule and take your exam to receive a certificate.</p>
        <button>Schedule Exam</button>
        <button>Take Exam</button>
    </div>

    <div class="container" id="contact">
        <h2>Contact Us</h2>
        <p>Email: support@onlineplatform.com</p>
        <p>Phone: +251-123-456-789</p>
    </div>

    <footer class="footer">
        <p>&copy; 2025 Online Course Platform. All rights reserved.</p>
    </footer>
</body>
</html>
