<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Bloom Bliss - Flower Shop</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}

body {
    background: linear-gradient(135deg, #ffe6f0, #fff5cc);
    color: #333;
}

/* Header */
header {
    background: linear-gradient(90deg, #ff66a3, #ffcc70);
    padding: 20px 60px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: white;
}

header h1 {
    font-size: 28px;
    font-weight: 700;
}

nav a {
    color: white;
    text-decoration: none;
    margin-left: 25px;
    font-weight: 500;
    transition: 0.3s;
}

nav a:hover {
    color: #fff5cc;
}

/* Hero Section */
.hero {
    height: 85vh;
    background: url('https://images.unsplash.com/photo-1490750967868-88aa4486c946') no-repeat center center/cover;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    color: white;
}

.hero h2 {
    font-size: 48px;
    background: rgba(0,0,0,0.5);
    padding: 20px 40px;
    border-radius: 15px;
}

/* Products Section */
.products {
    padding: 80px 60px;
    text-align: center;
}

.products h2 {
    font-size: 36px;
    margin-bottom: 40px;
    color: #ff4d94;
}

.product-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 30px;
}

.card {
    background: white;
    border-radius: 15px;
    overflow: hidden;
    box-shadow: 0 10px 25px rgba(0,0,0,0.1);
    transition: 0.3s;
}

.card:hover {
    transform: translateY(-10px);
}

.card img {
    width: 100%;
    height: 250px;
    object-fit: cover;
}

.card h3 {
    margin: 15px 0;
    color: #ff6699;
}

.card p {
    padding: 0 15px 20px;
}

.card button {
    margin-bottom: 20px;
    padding: 10px 20px;
    border: none;
    background: linear-gradient(90deg, #ff66a3, #ffcc70);
    color: white;
    border-radius: 25px;
    cursor: pointer;
    transition: 0.3s;
}

.card button:hover {
    opacity: 0.8;
}

/* About Section */
.about {
    background: #fff0f5;
    padding: 80px 60px;
    text-align: center;
}

.about h2 {
    color: #ff4d94;
    margin-bottom: 20px;
}

.about p {
    max-width: 700px;
    margin: auto;
    font-size: 18px;
}

/* Footer */
footer {
    background: linear-gradient(90deg, #ff66a3, #ffcc70);
    padding: 20px;
    text-align: center;
    color: white;
    margin-top: 50px;
}
</style>
</head>

<body>

<header>
    <h1>🌸 Bloom Bliss</h1>
    <nav>
        <a href="#">Home</a>
        <a href="#">Shop</a>
        <a href="#">About</a>
        <a href="#">Contact</a>
    </nav>
</header>

<section class="hero">
    <h2>Fresh Flowers for Every Occasion</h2>
</section>

<section class="products">
    <h2>Our Beautiful Collection</h2>
    <div class="product-grid">
        
        <div class="card">
            <img src="https://images.unsplash.com/photo-1509042239860-f550ce710b93" alt="Roses">
            <h3>Romantic Roses</h3>
            <p>Fresh red roses perfect for love and special moments.</p>
            <button>Order Now</button>
        </div>

        <div class="card">
            <img src="https://images.unsplash.com/photo-1463320726281-696a485928c7" alt="Tulips">
            <h3>Colorful Tulips</h3>
            <p>Bright and cheerful tulips to light up any day.</p>
            <button>Order Now</button>
        </div>

        <div class="card">
            <img src="https://images.unsplash.com/photo-1501004318641-b39e6451bec6" alt="Sunflowers">
            <h3>Sunny Sunflowers</h3>
            <p>Bring warmth and happiness with golden sunflowers.</p>
            <button>Order Now</button>
        </div>

    </div>
</section>

<section class="about">
    <h2>About Bloom Bliss</h2>
    <p>
        At Bloom Bliss, we believe flowers bring joy, love, and beauty into every life. 
        We carefully select fresh blooms daily to create stunning arrangements for weddings, birthdays, anniversaries, and all your special moments.
    </p>
</section>

<footer>
    © 2026 Bloom Bliss Flower Shop | Designed with ❤️
</footer>

</body>
</html>
