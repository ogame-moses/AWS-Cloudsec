unsecure static website 

<img width="1698" height="963" alt="image" src="https://github.com/user-attachments/assets/a9ae606f-450b-44c7-b736-94958d87795c" />

secure static website

<img width="1608" height="843" alt="image" src="https://github.com/user-attachments/assets/8b557e1f-7e82-42df-8b3d-5c0b6d5fcf8d" />

Below html code is used to build the above static website which introduces the designer

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Simple Website</title>
    <style>
        /* --- CSS for styling the website --- */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
            line-height: 1.6;
        }

        .container {
            max-width: 960px;
            margin: 0 auto;
            padding: 20px;
        }

        header {
            background-color: #333;
            color: #fff;
            padding: 1rem 0;
            text-align: center;
        }

        header h1 {
            margin: 0;
            font-size: 2.5rem;
        }

        nav ul {
            list-style-type: none;
            padding: 0;
            display: flex;
            justify-content: center;
        }

        nav li {
            margin: 0 15px;
        }

        nav a {
            color: #fff;
            text-decoration: none;
            font-weight: bold;
        }
        
        main {
            padding: 20px 0;
        }

        .content-section {
            background-color: #fff;
            padding: 20px;
            margin-bottom: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        footer {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 1rem 0;
            position: relative;
            bottom: 0;
            width: 100%;
        }

        /* --- Simple responsive design --- */
        @media (max-width: 600px) {
            nav ul {
                flex-direction: column;
                align-items: center;
            }

            nav li {
                margin: 5px 0;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="container">
            <h1>My Awesome Website</h1>
            <nav>
                <ul>
                    <li><a href="#about">About</a></li>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main class="container">
        
        <section id="about" class="content-section">
            <h2>About Us</h2>
            <p>Welcome to our simple website! This page is built using basic HTML, CSS, and a touch of JavaScript to show you how a website is structured. We are dedicated to providing excellent content and a great user experience.</p>
        </section>

        <section id="services" class="content-section">
            <h2>Our Services</h2>
            <p>We offer a range of services designed to meet your needs. Whether you're looking for web development, design, or content creation, we've got you covered.</p>
            <ul>
                <li>Web Design</li>
                <li>Frontend Development</li>
                <li>Content Writing</li>
                <li>SEO Optimization</li>
            </ul>
        </section>
        
        <section id="contact" class="content-section">
            <h2>Contact Us</h2>
            <p>Have a question? Feel free to get in touch with us!</p>
            <form id="contact-form">
                <label for="name">Name:</label><br>
                <input type="text" id="name" name="name"><br><br>
                <label for="email">Email:</label><br>
                <input type="email" id="email" name="email"><br><br>
                <label for="message">Message:</label><br>
                <textarea id="message" name="message" rows="4"></textarea><br><br>
                <button type="submit">Send Message</button>
            </form>
        </section>

    </main>

    <footer>
        <div class="container">
            <p>&copy; 2025 My Simple Website. All Rights Reserved.</p>
        </div>
    </footer>
    
    <script>
        const contactForm = document.getElementById('contact-form');
        contactForm.addEventListener('submit', function(event) {
            event.preventDefault(); // Prevents the form from actually submitting
            alert('Thank you for your message! This is a simple alert from JavaScript.');
        });
    </script>

</body>
</html>
