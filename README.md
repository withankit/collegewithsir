<!DOCTYPE html>
<html>
<head>
    <title>My First Website</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
        }
        header {
            background-color: #4CAF50;
            color: white;
            text-align: center;
            padding: 20px;
        }
        nav {
            background-color: #333;
            padding: 10px;
            text-align: center;
        }
        nav a {
            color: white;
            text-decoration: none;
            margin: 15px;
            font-weight: bold;
        }
        nav a:hover {
            color: yellow;
        }
        section {
            padding: 20px;
            text-align: center;
        }
        footer {
            background-color: #222;
            color: white;
            text-align: center;
            padding: 10px;
        }
    </style>
</head>
<body>

<header>
    <h1>Welcome to My Website</h1>
    <p>This is my simple HTML website</p>
</header>

<nav>
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Services</a>
    <a href="#">Contact</a>
</nav>

<section>
    <h2>About Us</h2>
    <p>This website is created using only HTML and CSS.</p>
    <button onclick="alert('Thank You for Visiting!')">Click Me</button>
</section>

<footer>
    <p>© 2026 My Website | All Rights Reserved</p>
</footer>

</body>
</html>
