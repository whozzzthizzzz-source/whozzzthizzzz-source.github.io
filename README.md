# personal-branding-website
Official personal branding website of Danish Malik – Young Entrepreneur | Business Mindset | Digital Growth Vision.”
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Whozzzthizzzz</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #f0f4ff, #e6fff9);
            color: #333;
        }
        header {
            background: #0077cc;
            color: white;
            padding: 50px 20px;
            text-align: center;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }
        header h1 {
            font-size: 3em;
            margin: 0 0 10px;
        }
        header p {
            font-size: 1.2em;
            opacity: 0.85;
        }
        main {
            max-width: 900px;
            margin: -40px auto 40px auto;
            padding: 30px;
            background: white;
            border-radius: 12px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
        }
        h2 {
            color: #0077cc;
            margin-top: 30px;
        }
        a {
            color: #0077cc;
            text-decoration: none;
        }
        a:hover {
            text-decoration: underline;
        }
        pre {
            background: #f4f4f4;
            padding: 15px;
            border-radius: 8px;
            overflow-x: auto;
            white-space: pre-wrap;
            word-wrap: break-word;
            font-size: 0.95em;
        }
        footer {
            text-align: center;
            padding: 20px;
            font-size: 0.9em;
            color: #555;
        }
        /* Smooth fade-in animation */
        main, header {
            opacity: 0;
            transform: translateY(20px);
            animation: fadeIn 1s forwards;
        }
        main {
            animation-delay: 0.3s;
        }
        @keyframes fadeIn {
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to Whozzzthizzzz!</h1>
        <p>Your modern GitHub Pages website is live 🚀</p>
    </header>
    <main>
        <h2>About This Project</h2>
        <p>This website automatically displays the contents of the README.md file from your repository, and updates dynamically whenever you edit it.</p>

        <h2>README Content</h2>
        <pre id="readme">Loading README...</pre>

        <h2>Repository</h2>
        <p>Visit the GitHub repo: <a href="https://github.com/your-username/whozzzthizzzz-source" target="_blank">whozzzthizzzz-source</a></p>
    </main>
    <footer>
        &copy; 2025 Whozzzthizzzz | Built with ❤️ & GitHub Pages
    </footer>

    <script>
        // Auto-load README.md
        fetch('https://raw.githubusercontent.com/your-username/whozzzthizzzz-source/main/README.md')
        .then(response => response.text())
        .then(data => {
            document.getElementById('readme').textContent = data;
        })
        .catch(err => {
            document.getElementById('readme').textContent = "Could not load README.md";
            console.error(err);
        });
    </script>
</body>
</html>
