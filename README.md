# nike-shoes  <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shoe Store</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Welcome to Our Shoe Store</h1>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#products">Products</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>
    
    <section id="home" class="hero">
        <h2>Find Your Perfect Shoes</h2>
        <a href="#products" class="cta-button">Shop Now</a>
    </section>
    
    <section id="products" class="product-grid">
        <div class="product">
            <img src="shoe1.jpg" alt="Shoe 1">
            <h2>Classic Sneakers</h2>
            <p>$49.99</p>
            <button>Add to Cart</button>
        </div>
        <div class="product">
            <img src="shoe2.jpg" alt="Shoe 2">
            <h2>Sporty Runners</h2>
            <p>$59.99</p>
            <button>Add to Cart</button>
        </div>
    </section>
    
    <footer>
        <p>&copy; 2025 Shoe Store. All Rights Reserved.</p>
    </footer>
</body>
</html>

// now  i will add css code//

/* General Styles */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    text-align: center;
    background: linear-gradient(to right, #ffafbd, #ffc3a0);
}

/* Header */
header {
    background: #333;
    color: white;
    padding: 15px 0;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

nav a {
    color: white;
    text-decoration: none;
    font-weight: bold;
}

/* Hero Section */
.hero {
    background: url('hero-bg.jpg') no-repeat center center/cover;
    color: white;
    padding: 100px 20px;
}

.hero h2 {
    font-size: 2.5em;
}

.cta-button {
    background: #ff6600;
    color: white;
    padding: 15px 25px;
    text-decoration: none;
    font-weight: bold;
    border-radius: 5px;
    display: inline-block;
    margin-top: 15px;
}

/* Product Grid */
.product-grid {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 20px;
    padding: 20px;
}

.product {
    background: white;
    padding: 15px;
    width: 220px;
    border-radius: 8px;
    box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
    transition: transform 0.2s;
}

.product:hover {
    transform: scale(1.05);
}

.product img {
    width: 100%;
    border-radius: 5px;
    transition: transform 0.3s ease-in-out;
}

.scrolling-image:hover {
    transform: rotate(5deg) scale(1.1);
}

button {
    background: #ff6600;
    color: white;
    border: none;
    padding: 10px;
    cursor: pointer;
    border-radius: 5px;
    margin-top: 10px;
    transition: background 0.3s;
}

button:hover {
    background: #cc5500;
}

/* About & Contact Section */
#about, #contact {
    padding: 50px;
    background: #fff;
}

/* Footer */
footer {
    background: #222;
    color: white;
    padding: 15px 0;
}


// now i will add javascript code//
document.addEventListener("DOMContentLoaded", function () {
    let images = document.querySelectorAll(".scrolling-image");

    images.forEach(img => {
        img.addEventListener("mouseover", () => {
            img.style.transform = "scale(1.2)";
        });
        img.addEventListener("mouseout", () => {
            img.style.transform = "scale(1)";
        });
    });
})
// the end you only put some pictures and all right//
