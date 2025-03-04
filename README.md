<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fresh Grocery</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f8f8f8;
            display: flex;
            flex-direction: column;
            min-height: 100vh;
        }

        header {
            background-color: #4CAF50;
            color: white;
            padding: 15px;
            text-align: center;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        header h1 {
            margin: 0;
        }

        nav ul {
            list-style-type: none;
            padding: 0;
            margin: 0;
        }

        nav ul li {
            display: inline;
            margin: 0 15px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            cursor: pointer;
        }

        .search-bar {
            display: flex;
        }

        .search-bar input[type="text"] {
            padding: 5px;
            font-size: 16px;
            border: none;
            border-radius: 5px 0 0 5px;
        }

        .search-bar button {
            padding: 5px 10px;
            background-color: white;
            border: none;
            color: #4CAF50;
            cursor: pointer;
            border-radius: 0 5px 5px 0;
        }

        .search-bar button:hover {
            background-color: #ddd;
        }

        .banner {
            background: url('grocery-banner.jpg') no-repeat center center/cover;
            text-align: center;
            color: rgb(16, 4, 4);
            padding: 50px;
            font-size: 24px;
            font-weight: bold;
        }

        .products, .about, .contact {
            text-align: center;
            padding: 20px;
            flex-grow: 1;
        }

        .product-list {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }

        .product {
            background-color: white;
            padding: 15px;
            border-radius: 5px;
            box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.1);
            width: 200px;
            text-align: center;
        }

        .product img {
            width: 100%;
            height: 150px;
            object-fit: cover;
            border-radius: 5px;
        }

        footer {
            text-align: center;
            padding: 10px;
            background-color: #4CAF50;
            color: white;
            width: 100%;
            position: relative;
            bottom: 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>Fresh Grocery</h1>
        <nav>
            <ul>
                <li><a href="#banner">Home</a></li>
                <li><a href="#products">Products</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
        <div class="search-bar">
            <input type="text" placeholder="Search for products...">
            <button type="submit">Search</button>
        </div>
    </header>

    <section class="banner" id="banner">
        <h2>All your essentials,<br>find them here!</h2>
    </section>

    <!-- About Section -->
    <section class="about" id="about">
        <h2>About Us</h2>
        <p>We are a locally sourced grocery store providing <br><strong>fresh fruits </strong> <br> <strong>vegetables</strong><br> <strong>dairy products</strong><br> Our mission is to offer healthy and organic products straight from farms to your table.</p>
    </section>

    <!-- Products Section -->
    <section class="products" id="products">
        <h2>Our Products</h2>
        <div class="product-list">
            <div class="product">
                <img src="" alt="Fruits">
                <h3>Fresh Fruits</h3>
                <p>Organic and farm-fresh fruits</p>
            </div>
            <div class="product">
                <img src="" alt="Vegetables">
                <h3>Green Vegetables</h3>
                <p>Locally sourced fresh vegetables</p>
            </div>
            <div class="product">
                <img src="" alt="Dairy Products">
                <h3>Dairy Products</h3>
                <p>Milk, cheese, butter, and more</p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact" id="contact">
        <h2>Contact Us</h2>
        <form>
            <label for="name">Name:</label><br>
            <input type="text" id="name" name="name"><br><br>
            <label for="email">Email:</label><br>
            <input type="email" id="email" name="email"><br><br>
            <label for="order">Order Details:</label><br>
            <textarea id="order" name="order"></textarea><br><br>
            <label for ="payment screenshot">payment screenshot</label><br>
            <textarea id="screenshot" name="screenshot"></textarea><br><br>
            <button type="submit">Submit</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2025 Fresh Grocery. All rights reserved.</p>
    </footer>

    <script>
        // Smooth scroll for navigation links
        document.querySelectorAll('nav ul li a').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                target.scrollIntoView({ behavior: 'smooth' });
            });
        });
    </script>
</body>
</html>
