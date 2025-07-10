<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>E-commerce Store</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            line-height: 1.6;
        }

        /* Navigation Styles */
        nav {
            background: #333;
            color: white;
            padding: 1rem;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            margin-left: 1.5rem;
            font-size: 1rem;
        }

        .nav-links a:hover {
            color: #ddd;
        }

        .cart-icon {
            position: relative;
        }

        .cart-count {
            position: absolute;
            top: -10px;
            right: -10px;
            background: red;
            color: white;
            border-radius: 50%;
            padding: 2px 6px;
            font-size: 0.8rem;
        }

        /* Main Content Styles */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
        }

        /* Home Page */
        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .product-card {
            border: 1px solid #ddd;
            padding: 1rem;
            text-align: center;
            border-radius: 8px;
            transition: transform 0.3s;
        }

        .product-card:hover {
            transform: translateY(-5px);
        }

        .product-card img {
            max-width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 4px;
        }

        .product-card h3 {
            margin: 0.5rem 0;
        }

        .product-card p {
            color: #555;
        }

        .add-to-cart {
            background: #28a745;
            color: white;
            border: none;
            padding: 0.5rem 1rem;
            border-radius: 4px;
            cursor: pointer;
            margin-top: 1rem;
        }

        .add-to-cart:hover {
            background: #218838;
        }

        /* Product Details Page */
        .product-details {
            display: flex;
            gap: 2rem;
            margin-top: 2rem;
        }

        .product-details img {
            max-width: 400px;
            border-radius: 8px;
        }

        .product-info {
            flex: 1;
        }

        /* Cart Page */
        .cart-items {
            margin-top: 2rem;
        }

        .cart-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 1px solid #ddd;
            padding: 1rem 0;
        }

        .cart-item img {
            width: 80px;
            height: 80px;
            object-fit: cover;
        }

        .remove-item {
            color: red;
            cursor: pointer;
        }

        /* Checkout Page */
        .checkout-form {
            max-width: 600px;
            margin: 2rem auto;
        }

        .form-group {
            margin-bottom: 1rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
        }

        .form-group input {
            width: 100%;
            padding: 0.5rem;
            border: 1px solid #ddd;
            border-radius: 4px;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .nav-container {
                flex-direction: column;
                gap: 1rem;
            }

            .nav-links a {
                margin: 0 0.5rem;
            }

            .product-details {
                flex-direction: column;
            }

            .product-details img {
                max-width: 100%;
            }
        }g
    </style>
</head>
<body>
    <nav>
        <div class="nav-container">
            <h1>E-Shop</h1>
            <div class="nav-links">
                <a href="#home" onclick="showPage('home')">Home</a>
                <a href="#cart" onclick="showPage('cart')">Cart <span class="cart-count" id="cart-count">0</span></a>
                <a href="#checkout" onclick="showPage('checkout')">Checkout</a>
            </div>
        </div>
    </nav>

    <div class="container">
        <!-- Home Page -->
        <div id="home" class="page">
            <h2>Our Products</h2>
            <div class="products-grid" id="products-grid"></div>
        </div>

        <!-- Product Details Page -->
        <div id="product-details" class="page" style="display: none;">
            <div class="product-details" id="product-details-content"></div>
        </div>

        <!-- Cart Page -->
        <div id="cart" class="page" style="display: none;">
            <h2>Your Cart</h2>
            <div class="cart-items" id="cart-items"></div>
            <div id="cart-total" style="margin-top: 1rem; font-weight: bold;"></div>
        </div>

        <!-- Checkout Page -->
        <div id="checkout" class="page" style="display: none;">
            <h2>Checkout</h2>
            <div class="checkout-form">
                <div class="form-group">
                    <label for="name">Full Name</label>
                    <input type="text" id="name" required>
                </div>
                <div class="form-group">
                    <label for="email">Email</label>
                    <input type="email" id="email" required>
                </div>
                <div class="form-group">
                    <label for="address">Shipping Address</label>
                    <input type="text" id="address" required>
                </div>
                <button class="add-to-cart" onclick="completeCheckout()">Complete Purchase</button>
            </div>
        </div>
    </div>

    <script>
        // Sample products
        const products = [
            { id: 1, name: "Laptop", price: 99.99, image: "Laptop image.jpeg", description: "High-performance laptop with 16GB RAM and 512GB SSD." },
            { id: 2, name: "Smartphone", price: 69.99, image: "Smartphone image.jpeg", description: "Latest smartphone with 5G support and 128GB storage." },
            { id: 3, name: "Headphones", price: 19.99, image: "Headphones image.jpeg", description: "Wireless noise-canceling headphones with 20-hour battery life." },
            { id: 4, name: "Smartwatch", price: 24.99, image: "Smartwatch image.jpeg", description: "Fitness tracking smartwatch with heart rate monitor." }
        ];

        let cart = JSON.parse(localStorage.getItem('cart')) || [];

        // Display products
        function displayProducts() {
            const grid = document.getElementById('products-grid');
            grid.innerHTML = '';
            products.forEach(product => {
                const card = document.createElement('div');
                card.className = 'product-card';
                card.innerHTML = `
                    <img src="${product.image}" alt="${product.name}">
                    <h3>${product.name}</h3>
                    <p>$${product.price.toFixed(2)}</p>
                    <button class="add-to-cart" onclick="viewProduct(${product.id})">View Details</button>
                `;
                grid.appendChild(card);
            });
        }

        // Show product details
        function viewProduct(productId) {
            const product = products.find(p => p.id === productId);
            const details = document.getElementById('product-details-content');
            details.innerHTML = `
                <img src="${product.image}" alt="${product.name}">
                <div class="product-info">
                    <h2>${product.name}</h2>
                    <p>$${product.price.toFixed(2)}</p>
                    <p>${product.description}</p>
                    <button class="add-to-cart" onclick="addToCart(${product.id})">Add to Cart</button>
                </div>
            `;
            showPage('product-details');
        }

        // Add to cart
        function addToCart(productId) {
            const product = products.find(p => p.id === productId);
            const cartItem = cart.find(item => item.id === productId);
            if (cartItem) {
                cartItem.quantity += 1;
            } else {
                cart.push({ ...product, quantity: 1 });
            }
            localStorage.setItem('cart', JSON.stringify(cart));
            updateCart();
            alert(`${product.name} added to cart!`);
        }

        // Update cart display
        function updateCart() {
            const cartItems = document.getElementById('cart-items');
            const cartCount = document.getElementById('cart-count');
            const cartTotal = document.getElementById('cart-total');
            cartItems.innerHTML = '';
            let total = 0;
            let itemCount = 0;

            cart.forEach(item => {
                total += item.price * item.quantity;
                itemCount += item.quantity;
                const div = document.createElement('div');
                div.className = 'cart-item';
                div.innerHTML = `
                    <img src="${item.image}" alt="${item.name}">
                    <div>${item.name}</div>
                    <div>$${item.price.toFixed(2)} x ${item.quantity}</div>
                    <div class="remove-item" onclick="removeFromCart(${item.id})">Remove</div>
                `;
                cartItems.appendChild(div);
            });

            cartCount.textContent = itemCount;
            cartTotal.textContent = `Total: $${total.toFixed(2)}`;
        }

        // Remove from cart
        function removeFromCart(productId) {
            cart = cart.filter(item => item.id !== productId);
            localStorage.setItem('cart', JSON.stringify(cart));
            updateCart();
        }

        // Show specific page
        function showPage(pageId) {
            document.querySelectorAll('.page').forEach(page => {
                page.style.display = page.id === pageId ? 'block' : 'none';
            });
            if (pageId === 'cart') updateCart();
        }

        // Complete checkout
        function completeCheckout() {
            const name = document.getElementById('name').value;
            const email = document.getElementById('email').value;
            const address = document.getElementById('address').value;

            if (name && email && address && cart.length > 0) {
                alert('Purchase completed! Thank you for your order.');
                cart = [];
                localStorage.setItem('cart', JSON.stringify(cart));
                updateCart();
                showPage('home');
            } else {
                alert('Please fill all fields and ensure your cart is not empty.');
            }
        }

        // Initialize
        displayProducts();
        updateCart();
        showPage('home');
    </script>
</body>
</html>
