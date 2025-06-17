<!-- HTML5 doctype declaration -->
<!DOCTYPE html>
<!-- Modernized and commented for clarity -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body {
            font-family: 'Segoe UI', Arial, sans-serif;
            background: #f4f6fb;
            margin: 0;
            padding: 0;
            color: #222;
        }
        h1 {
            text-align: center;
            margin-top: 30px;
            font-size: 2.5rem;
            color: #2d3a4b;
            letter-spacing: 0.05em;
            opacity: 0;
            transform: translateY(-30px);
            animation: fadeDown 1s ease-out forwards;
        }
        @keyframes fadeDown {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        nav {
            background-color: #2d3a4b;
            color: white;
            padding: 16px 0;
            text-align: center;
            letter-spacing: 0.15em;
            font-size: 1.1rem;
            margin-bottom: 30px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.04);
            opacity: 0;
            animation: fadeIn 1s 0.5s forwards;
        }
        nav::after {
            content: "";
            display: block;
            margin: 10px auto 0;
            width: 80%;
            height: 1px;
            background: #e0e6ed;
        }
        @keyframes fadeIn {
            to {
                opacity: 1;
            }
        }
        h2 {
            text-align: center;
            color: #4a5a6a;
            margin-bottom: 18px;
            font-size: 1.6rem;
            opacity: 0;
            transform: translateY(30px);
            animation: fadeUp 1s 1s forwards;
        }
        @keyframes fadeUp {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        p {
            max-width: 800px;
            margin: 0 auto 24px auto;
            line-height: 1.7;
            font-size: 1.05rem;
        }
        .Home, .Product {
            background: #fff;
            border-radius: 10px;
            box-shadow: 0 2px 12px rgba(44,62,80,0.07);
            max-width: 800px;
            margin: 30px auto;
            padding: 28px 32px;
            opacity: 0;
            transform: scale(0.97);
            animation: cardAppear 0.8s 1.5s forwards;
        }
        .Product {
            animation-delay: 1.8s;
        }
        @keyframes cardAppear {
            to {
                opacity: 1;
                transform: scale(1);
            }
        }
        .Home h3, .Product h3 {
            color: #2d3a4b;
            margin-top: 0;
            font-size: 1.3rem;
        }
        .product-list, .product-trial, .product-contact {
            margin-top: 18px;
            padding-left: 10px;
        }
        .product-list h4, .product-trial h4, .product-contact h4 {
            color: #3b4b5b;
            margin-bottom: 8px;
            font-size: 1.1rem;
        }
        ul {
            padding-left: 22px;
        }
        li {
            margin-bottom: 6px;
            opacity: 0;
            animation: listFadeIn 0.5s forwards;
        }
        .product-list li:nth-child(1) { animation-delay: 2.2s; }
        .product-list li:nth-child(2) { animation-delay: 2.4s; }
        .product-list li:nth-child(3) { animation-delay: 2.6s; }
        @keyframes listFadeIn {
            to {
                opacity: 1;
            }
        }
        a {
            color: #1a73e8;
            text-decoration: none;
            transition: color 0.2s;
        }
        a:hover {
            color: #0c47a1;
            text-decoration: underline;
        }
        @media (max-width: 600px) {
            .Home, .Product, p {
                padding: 16px 8px;
                max-width: 98vw;
            }
            h1 {
                font-size: 2rem;
            }
            h2 {
                font-size: 1.2rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to Gohel Developers</h1>
        <nav>
            <a href="#home">Home</a> |
            <a href="#products">Products</a> |
            <a href="#trial">Trial</a> |
            <a href="#contact">Contact</a> |
            <a href="#team">Team</a> |
            <a href="#blog">Blog</a> |
            <a href="#faq">FAQ</a>
        </nav>
    </header>
    <main>
        <section id="intro">
            <h2>Build, Learn, and Grow Together</h2>
            <p>
                Discover a world of web development resources, tutorials, and community support. Whether you're a beginner or a pro, Gohel Developers is your launchpad to success. Join us and start your journey today!
            </p>
        </section>
        <section class="Home" id="home">
            <h3>About Us</h3>
            <p>
                Gohel Developers is dedicated to empowering developers with the latest tools, guides, and best practices. Stay tuned for updates and exclusive content!
            </p>
            <p>
                Our mission is to make web development accessible and enjoyable for everyone. We believe in open knowledge, collaboration, and continuous learning.
            </p>
            <p>
                From HTML and CSS to advanced JavaScript frameworks, our platform covers a wide range of topics to help you stay ahead in the tech world.
            </p>
        </section>
        <section class="Product" id="products">
            <h3>Featured Products</h3>
            <div class="product-list">
                <h4>What We Offer</h4>
                <ul>
                    <li>Web Starter Kit – Everything you need to begin</li>
                    <li>Responsive UI Templates – Modern and mobile-ready</li>
                    <li>Interactive Learning Modules – Practice as you learn</li>
                    <li>API Playground – Test and learn with real APIs</li>
                    <li>Code Snippet Library – Ready-to-use solutions</li>
                    <li>Project Showcases – Inspiration from real projects</li>
                </ul>
            </div>
            <div class="product-trial" id="trial">
                <h4>Try for Free</h4>
                <p>
                    Sign up for a free 14-day trial and unlock premium features. No credit card required!
                </p>
                <ul>
                    <li>Access to all tutorials</li>
                    <li>Download premium templates</li>
                    <li>Join exclusive webinars</li>
                </ul>
            </div>
            <div class="product-contact" id="contact">
                <h4>Get in Touch</h4>
                <p>
                    Questions or feedback? Email us at <a href="mailto:support@goheldevelopers.com">support@goheldevelopers.com</a> or call <a href="tel:8866410100">8866410100</a>.
                </p>
                <p>
                    Follow us on 
                    <a href="#">Twitter</a>, 
                    <a href="#">Facebook</a>, 
                    <a href="#">LinkedIn</a>
                </p>
            </div>
        </section>
        <section class="Home" id="team">
            <h3>Meet Our Team</h3>
            <ul>
                <li><strong>Kashyap Gohel</strong> – Founder & Lead Developer</li>
                <li><strong>Priya Shah</strong> – UI/UX Designer</li>
                <li><strong>Arjun Patel</strong> – Backend Engineer</li>
                <li><strong>Sneha Mehta</strong> – Content Strategist</li>
                <li><strong>Rahul Singh</strong> – Community Manager</li>
            </ul>
            <p>
                Our diverse team brings together years of experience in web development, design, and education.
            </p>
        </section>
        <section class="Product" id="blog">
            <h3>Latest Blog Posts</h3>
            <div class="product-list">
                <ul>
                    <li><a href="#">10 Tips for Responsive Web Design</a> – June 2024</li>
                    <li><a href="#">Understanding Flexbox and Grid</a> – May 2024</li>
                    <li><a href="#">How to Build Accessible Websites</a> – April 2024</li>
                    <li><a href="#">JavaScript ES2024 Features</a> – March 2024</li>
                </ul>
            </div>
        </section>
        <section class="Home" id="faq">
            <h3>Frequently Asked Questions</h3>
            <div class="product-list">
                <h4>General</h4>
                <ul>
                    <li><strong>Is Gohel Developers free?</strong> – Yes, most resources are free. Premium features are available via subscription.</li>
                    <li><strong>Can I contribute?</strong> – Absolutely! Contact us to join our contributor program.</li>
                </ul>
                <h4>Technical</h4>
                <ul>
                    <li><strong>What technologies do you cover?</strong> – HTML, CSS, JavaScript, React, Node.js, and more.</li>
                    <li><strong>Do you offer certificates?</strong> – Yes, for select courses and challenges.</li>
                </ul>
            </div>
        </section>
        <section class="Product" id="testimonials">
            <h3>What Our Users Say</h3>
            <div class="product-list">
                <ul>
                    <li>"Gohel Developers helped me land my first developer job!" – <em>Anjali K.</em></li>
                    <li>"The tutorials are clear and easy to follow." – <em>Mohit S.</em></li>
                    <li>"Great community and support." – <em>Fatima R.</em></li>
                </ul>
            </div>
        </section>
        <section class="Home" id="newsletter">
            <h3>Subscribe to Our Newsletter</h3>
            <form>
                <input type="email" placeholder="Your email address" required style="padding:8px; border-radius:4px; border:1px solid #ccc;">
                <button type="submit" style="padding:8px 16px; border:none; border-radius:4px; background:#2d3a4b; color:#fff;">Subscribe</button>
            </form>
        </section>
    </main>
    <footer style="text-align:center; margin: 32px 0 12px 0; color: #7a8a99; font-size: 0.95rem;">
        &copy; 2013-2024 Gohel Developers. All rights reserved.
    </footer>
</body>
</html>
