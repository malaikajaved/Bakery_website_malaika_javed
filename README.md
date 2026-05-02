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

body {
    font-family: 'Arial', sans-serif;
    margin: 0;
    padding: 0;
    color: #333;
    background: #f9f9f9;
}


header {
    background-color: #793f2e;
    color: white;
    padding: 10px 20px;
    text-align: center;
}

header img.logo {
    height: 48%;
    vertical-align: middle;
}
    @media (mx-width: 768px) {
        img {
            width: 100%;

        }

    }


nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin-right: 20px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-weight: bold;
}

main {
    margin: 20px;
    text-align: center;
}

.hero {
    background-color: #e2d3c0;
    padding: 20px;
    margin-bottom: 20px;
}

.features .cards {
    display: flex;
    justify-content: space-around;
}

.features .cards div {
    width: 50%;
    padding: 20px;
    background-color: rgb(248, 238, 238);
   
}

#filter-buttons {
    text-align: center;
    margin: 20px 0;
}

#filter-buttons button {
    padding: 10px 20px;
    margin: 5px;
    background-color: #ca955d;
    border: none;
    cursor: pointer;
    color: white;
    font-size: 16px;
}

#filter-buttons button:hover {
    background-color: #d0a218;
}

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}


.logo {
    height: 50px;
}

nav ul {
    list-style-type: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

nav ul li a {
    color: rgb(233, 209, 209);
    text-decoration: none;
}




.offers {
    padding: 20px;
}

.offer-item {
    background-color: rgba(245, 203, 182, 0.618);
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(227, 25, 25, 0.918);
    margin-bottom: 20px;
    padding: 20px;
    text-align: center;
}

.offer-item img {
    max-width: 100%;
    height: auto;
    display: block;
    margin: 0 auto 10px;
}

/* Blinking effect */
@keyframes blink {
    0%, 50%, 100% {
        opacity: 1;
    }
    25%, 75% {
        opacity: 0;
    }
}

.blinking {
    animation: blink 1s infinite;
}

.contact-h2 

/* Blinking effect */
@keyframes blink {
    0%, 50%, 100% {
        opacity: 1;
    }
    25%, 75% {
        opacity: 0;
    }
}


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
    

