Overview of the website 

I designed this website for a small bakery shop. It’s simple and interactive, featuring warm colours and standout text.
The design was inspired by a small vintage bakery that I used to frequent when I was younger. 
To attract customers, I included graphics as well as a separate offers page. The target audience ranges from 13 to 50 years old. 
In addition, the website includes a contact page to promote quick communication.

The website includes six primary pages: Home, Menu, Gallery, About us, offers and Contact. 
In this website I have used HTML for structure, CSS for styling, and JavaScript for interactivity. 

#index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bakery Shop Home</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

    <header>
        <img src="bakery_logo.png" alt="Bakery Logo" class="logo">
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="menu.html">Menu</a></li>
                <li><a href="Gallery.html">Gallery</a></li>
                <li><a href="offers.html">Offers</a></li>
                <li><a href="about.html">About us</a></li>
                <li><a href="contact.html">Contact</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section class="hero">
            <h1>Welcome to Our Bakery</h1>
            <p>Enjoy our handmade breads, pastries, and more.</p>
        </section>
        <section class="features">
            <h2>Why Choose Us?</h2>
            <div class="cards">
                <div>
                    <h3>Fresh Ingredients</h3>
                    <p>All our products are made with the highest quality, fresh ingredients.</p>
                </div>
                <div>
                    <h3>Family Recipe</h3>
                    <p>Our recipes have been passed down through generations with love.</p>
                </div>
                <div>
                    <h3>Community Focused</h3>
                    <p>We pride ourselves on enriching the local community through our baked goods.</p>
                </div>
            </div>
        </section>
    </main>
    <footer>
        <p>© 2024 Bakery Shop. All rights reserved.</p>
    </footer>
    <script src="script.js"></script>

</body>
</html>


...........................................................................................................................

#style.css



...................................................................................................................

#script.js

const contactForm = document.getElementById('contactForm');
    if (contactForm) {
        contactForm.addEventListener('submit', (event) => {
            const name = document.getElementById('name').value.trim();
            const email = document.getElementById('email').value.trim();
            const message = document.getElementById('message').value.trim();

            if (!name || !email || !message) {
                event.preventDefault();
                alert('Please fill out all fields.');
            } else {
                alert('Form submitted successfully!');
            }
        });
    }
    

