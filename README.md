<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flipkart Clone</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background-color: #2874f0;
            padding: 10px;
            color: white;
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
        }

        .search-bar {
            display: flex;
            flex-grow: 1;
            margin: 0 20px;
        }

        .search-bar input {
            flex-grow: 1;
            padding: 5px;
        }

        .search-bar button {
            padding: 5px 10px;
            background-color: #ff9f00;
            border: none;
            cursor: pointer;
        }

        .nav-links a {
            margin: 0 10px;
            color: white;
            text-decoration: none;
        }

        main {
            padding: 20px;
        }

        .product-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }

        .product-card {
            border: 1px solid #ddd;
            padding: 10px;
            width: calc(25% - 20px);
            box-sizing: border-box;
            text-align: center;
            opacity: 0;
            animation: fadeIn 1s forwards;
        }

        @keyframes fadeIn {
            to {
                opacity: 1;
            }
        }

        .product-card img {
            width: 200px;
            height: 200px;
            object-fit: cover;
            cursor: pointer;
        }

        .product-description {
            font-size: 14px;
            color: #555;
        }

        .rating {
            color: gold;
        }

        footer {
            text-align: center;
            padding: 10px;
            background-color: #f1f1f1;
        }

        .overlay {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }

        .overlay img {
            max-width: 90%;
            max-height: 90%;
        }

        .overlay .close {
            position: absolute;
            top: 20px;
            right: 20px;
            color: white;
            font-size: 30px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <header>
        <div class="navbar">
            <div class="logo">Flipkart</div>
            <div class="search-bar">
                <input type="text" placeholder="Search for products, brands and more">
                <button type="button">Search</button>
            </div>
            <div class="nav-links">
                <a href="#girl-shoes">Girl Shoes</a>
                <a href="#boy-shoes">Boy Shoes</a>
                <a href="#kids-shoes">Kids Shoes</a>
                <a href="#">Login</a>
                <a href="#">More</a>
                <a href="#">Cart</a>
            </div>
        </div>
    </header>

    <main>
        <section id="girl-shoes">
            <h2>Girl Shoes</h2>
            <div class="product-grid">
                <div class="product-card">
                    <img src="shoe.jpg" alt="Girl Shoe 1">
                    <h3>Girl Shoe 1</h3>
                    <p class="product-description">Stylish and comfortable for all-day wear.</p>
                    <p class="rating">★★★★☆</p>
                    <p>₹1000</p>
                    <button>Add to Cart</button>
                </div>
                <div class="product-card">
                    <img src="shoe1.webp" alt="Girl Shoe 2">
                    <h3>Girl Shoe 2</h3>
                    <p class="product-description">Perfect for both casual and formal occasions.</p>
                    <p class="rating">★★★★★</p>
                    <p>₹1500</p>
                    <button>Add to Cart</button>
                </div>
                <div class="product-card">
                    <img src="girlshoe.jpg" alt="Girl Shoe 3">
                    <h3>Girl Shoe 3</h3>
                    <p class="product-description">Affordable and durable, great for daily use.</p>
                    <p class="rating">★★★☆☆</p>
                    <p>₹500</p>
                    <button>Add to Cart</button>
                </div>
                <div class="product-card">
                    <img src="girlshoe1.webp" alt="Girl Shoe 4">
                    <h3>Girl Shoe 4</h3>
                    <p class="product-description">Trendy design with excellent grip.</p>
                    <p class="rating">★★★★☆</p>
                    <p>₹900</p>
                    <button>Add to Cart</button>
                </div>
                <!-- Add more girl shoes as needed -->
            </div>
        </section>

        <section id="boy-shoes">
            <h2>Boy Shoes</h2>
            <div class="product-grid">
                <div class="product-card">
                    <img src="shoeess.webp" alt="Boy Shoe 1">
                    <h3>Boy Shoe 1</h3>
                    <p class="product-description">Rugged and reliable, suitable for outdoor activities.</p>
                    <p class="rating">★★★★☆</p>
                    <p>₹1200</p>
                    <button>Add to Cart</button>
                </div>
                <div class="product-card">
                    <img src="shoee.jpg" alt="Boy Shoe 2">
                    <h3>Boy Shoe 2</h3>
                    <p class="product-description">Comfortable fit with a sleek look.</p>
                    <p class="rating">★★★★★</p>
                    <p>₹1300</p>
                    <button>Add to Cart</button>
                </div>
                <div class="product-card">
                    <img src="boysshoee1.webp" alt="Boy Shoe 3">
                    <h3>Boy Shoe 3</h3>
                    <p class="product-description">Lightweight and breathable for active kids.</p>
                    <p class="rating">★★★★☆</p>
                    <p>₹1100</p>
                    <button>Add to Cart</button>
                </div>
                <div class="product-card">
                    <img src="boyshoe2.webp" alt="Boy Shoe 4">
                    <h3>Boy Shoe 4</h3>
                    <p class="product-description">High-quality material with a modern design.</p>
                    <p class="rating">★★★★★</p>
                    <p>₹1600</p>
                    <button>Add to Cart</button>
                </div>
            </div>
        </section>

        <section id="kids-shoes">
            <h2>Kids Shoes</h2>
            <div class="product-grid">
                <div class="product-card">
                    <img src="shoee1.jpg" alt="Kids Shoe 1">
                    <h3>Kids Shoe 1</h3>
                    <p class="product-description">Fun design with easy-to-clean material.</p>
                    <p class="rating">★★★★☆</p>
                    <p>₹800</p>
                    <button>Add to Cart</button>
                </div>
                <div class="product-card">
                    <img src="kidds shoee.webp" alt="Kids Shoe 2">
                    <h3>Kids Shoe 2</h3>
                    <p class="product-description">Comfortable and supportive for growing feet.</p>
                    <p class="rating">★★★★☆</p>
                    <p>₹900</p>
                    <button>Add to Cart</button>
                </div>
                <div class="product-card">
                    <img src="kidsshoe1.webp" alt="Kids Shoe 3">
                    <h3>Kids Shoe 3</h3>
                    <p class="product-description">Bright colors and sturdy build.</p>
                    <p class="rating">★★★★★</p>
                    <p>₹1550</p>
                    <button>Add to Cart</button>
                </div>
                <div class="product-card">
                    <img src="kidsshoe2.jpg" alt="Kids Shoe 4">
                    <h3>Kids Shoe 4</h3>
                    <p class="product-description">Perfect for both playtime and school.</p>
                    <p class="rating">★★★★☆</p>
                    <p>₹1000</p>
                    <button>Add to Cart</button>
                </div>
                <!-- Add more kids shoes as needed -->
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2024 Flipkart Clone. All rights reserved.</p>
    </footer>

    <div class="overlay" id="overlay">
        <span class="close" id="close">&times;</span>
        <img id="overlay-img" src="" alt="Full Image">
    </div>

    <script>
        const overlay = document.getElementById('overlay');
        const overlayImg = document.getElementById('overlay-img');
        const close = document.getElementById('close');

        document.querySelectorAll('.product-card img').forEach(img => {
            img.addEventListener('click', () => {
                overlay.style.display = 'flex';
                overlayImg.src = img.src;
            });
        });

        close.addEventListener('click', () => {
            overlay.style.display = 'none';
        });

        overlay.addEventListener('click', (e) => {
            if (e.target === overlay) {
                overlay.style.display = 'none';
            }
        });
    </script>
</body>
</html>
