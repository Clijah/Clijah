<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Zeus Motors</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #333;
            color: white;
            padding: 1rem 0;
            text-align: center;
        }
        nav {
            background-color: #444;
            color: white;
            display: flex;
            justify-content: center;
            padding: 1rem 0;
        }
        nav a {
            color: white;
            margin: 0 1rem;
            text-decoration: none;
        }
        nav a:hover {
            text-decoration: underline;
        }
        .container {
            padding: 2rem;
            display: none;
        }
        .container.active {
            display: block;
        }
        .product, .cart-item {
            border: 1px solid #ccc;
            margin: 1rem;
            padding: 1rem;
            text-align: center;
        }
        .product img, .cart-item img {
            max-width: 100%;
            height: auto;
        }
        .product h2, .cart-item h2 {
            font-size: 1.5rem;
        }
        .product p, .cart-item p {
            margin: 1rem 0;
        }
        .add-to-cart, .remove-from-cart, .checkout {
            background-color: #28a745;
            border: none;
            color: white;
            cursor: pointer;
            padding: 0.5rem 1rem;
        }
        .add-to-cart:hover, .remove-from-cart:hover, .checkout:hover {
            background-color: #218838;
        }
        footer {
            background-color: #333;
            color: white;
            padding: 1rem 0;
            text-align: center;
            margin-top: 2rem;
        }
        .homepage-image {
            display: block;
            margin: 2rem auto;
            max-width: 100%;
            height: auto;
        }
        .billing-form {
            display: none;
            margin-top: 2rem;
        }
        .billing-form.active {
            display: block;
        }
        .billing-form input, .billing-form textarea {
            display: block;
            width: 100%;
            margin: 0.5rem 0;
            padding: 0.5rem;
			.product {
        border: 1px solid #ccc;
        margin: 1rem;
        padding: 1rem;
        text-align: center;
        width: 300px; /* Set a fixed width for uniform size */
        display: inline-block; /* Display products inline */
        vertical-align: top; /* Align products to the top */
    }

    .product img {
        max-width: 100%;
        height: auto;
        max-height: 200px; /* Limit image height for uniformity */
    }
        }
    </style>
</head>
<body>
    <header>
        <h1>Zeus Motors</h1>
    </header>
    <nav>
        <a href="#" onclick="showPage('home')">Home</a>
        <a href="#" onclick="showPage('products')">Products</a>
        <a href="#" onclick="showPage('cart')">Cart</a>
        <a href="#" onclick="showPage('checkout')">Checkout</a>
    </nav>
    <div id="home" class="container active">
        <h2>Welcome to Zeus Motors</h2>
        <p>Your one-stop shop for all things awesome.</p>
        <img src="C:\Users\User\Downloads\Homepage.jpg" alt="Homepage Image" class="homepage-image">
    </div>
    <div id="products" class="container">
        <h2>Products</h2>
        <div class="product">
            <img src="C:\Users\User\Downloads\Ninja400.jpg" alt="Product 1">
            <h2>Ninja 400 KRT</h2>
			<p>The Ninja 400 is a sleek and agile sport motorcycle designed for maximum performance on both city streets and winding roads. 
			With its compact design and powerful engine, it offers an exhilarating riding experience, perfect for riders seeking adrenaline-pumping thrills and precise handling.</p>
            <p>Price: ₱300000</p>
            <button class="add-to-cart" data-name="Ninja 400 KRT" data-price="300000">Add to Cart</button>
        </div>
        <div class="product">
            <img src="C:\Users\User\Downloads\Ninja650.jpg" alt="Product 2">
            <h2>Ninja 650</h2>
			<p>The Ninja 650 strikes a perfect balance between performance and practicality, offering sporty styling and nimble handling combined with everyday versatility. 
			Its smooth power delivery and comfortable ergonomics make it an ideal choice for both commuting and spirited rides.</p>
            <p>Price: ₱450000</p>
            <button class="add-to-cart" data-name="Ninja 650" data-price="450000">Add to Cart</button>
        </div>
        <div class="product">
            <img src="C:\Users\User\Downloads\Ninja1000.png" alt="Product 3">
            <h2>Ninja 1000</h2>
			<p>The Ninja 1000 combines exhilarating performance with long-distance comfort, making it the ultimate sport touring machine. 
			With a powerful inline-four engine, advanced electronics, and comfortable ergonomics, it offers thrilling acceleration and confidence-inspiring handling for riders who demand the best of both worlds.</p>
            <p>Price: ₱900000</p>
            <button class="add-to-cart" data-name="Ninja 1000" data-price="900000">Add to Cart</button>
        </div>
        <div class="product">
            <img src="C:\Users\User\Downloads\zx4r.jpg" alt="Product 4">
            <h2>Ninja ZX-4RR</h2>
			<p>The Ninja ZX-4RR is a track-focused supersport machine engineered for podium performance. With its lightweight chassis, race-tuned suspension, and high-revving inline-four engine, 
			it delivers razor-sharp handling and blistering acceleration, making it the weapon of choice for professional racers and track enthusiasts.</p>
            <p>Price: ₱470000</p>
            <button class="add-to-cart" data-name="Ninja ZX-4RR" data-price="470000">Add to Cart</button>
        </div>
        <div class="product">
            <img src="C:\Users\User\Downloads\ZX6R.jpg" alt="Product 5">
            <h2>Ninja ZX-6R</h2>
			<p>The Ninja ZX-6R is a high-performance middleweight sportbike designed to dominate both the street and the track. 
			With its race-derived technology, aggressive styling, and potent inline-four engine, it offers exceptional agility, precise handling, and adrenaline-pumping acceleration, setting the benchmark for supersport motorcycles.</p>
            <p>Price: ₱560000</p>
            <button class="add-to-cart" data-name="Ninja ZX-6R" data-price="₱560000">Add to Cart</button>
        </div>
        <div class="product">
            <img src="C:\Users\User\Downloads\ZX10R.jpg" alt="Product 6">
            <h2>Ninja ZX-10R</h2>
			<p>The Ninja ZX-10R is a championship-winning superbike engineered for absolute performance on the track. 
			With its potent inline-four engine, advanced electronics, and aerodynamic design, it delivers blistering acceleration, razor-sharp handling, and unmatched agility, making it the ultimate weapon for professional racers and adrenaline junkies alike.</p>
            <p>Price: ₱1200000</p>
            <button class="add-to-cart" data-name="Ninja ZX-10R" data-price="1200000">Add to Cart</button>
        </div>
        <div class="product">
            <img src="C:\Users\User\Downloads\H2.jpg" alt="Product 7">
            <h2>Ninja H2</h2>
			<p>The Ninja H2 is a hyperbike that pushes the boundaries of performance, engineering, and technology. With its supercharged inline-four engine delivering exhilarating power, 
			the Ninja H2 offers unmatched acceleration and top-end performance. Its aerodynamic design, advanced electronics, and race-inspired components make it a true powerhouse on both the street and the track. 
			Equipped with cutting-edge features such as Kawasaki's proprietary IMU-enhanced electronics suite, including traction control, launch control, and cornering ABS, the Ninja H2 provides ultimate control and confidence for riders seeking the pinnacle of sportbike performance.</p>
            <p>Price: ₱2800000</p>
            <button class="add-to-cart" data-name="Ninja H2" data-price="2,800,000">Add to Cart</button>
        </div>
    </div>
    <div id="cart" class="container">
        <h2>Shopping Cart</h2>
        <ul id="cart-items" style="list-style: none; padding: 0;">
        </ul>
        <p>Total: $<span id="cart-total">0</span></p>
        <button class="checkout" onclick="showPage('checkout')">Proceed to Checkout</button>
    </div>
    <div id="checkout" class="container">
        <h2>Checkout</h2>
        <form class="billing-form">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
            <label for="address">Address:</label>
            <textarea id="address" name="address" required></textarea>
            <p>Total: $<span id="checkout-total">0</span></p>
            <button type="submit">Submit</button>
        </form>
    </div>
    <footer>
        <p>&copy; 2024 Zeus Motors</p>
    </footer>
    <script>
        const pages = {
            home: document.getElementById('home'),
            products: document.getElementById('products'),
            cart: document.getElementById('cart'),
            checkout: document.getElementById('checkout')
        };

        function showPage(page) {
            for (let key in pages) {
                pages[key].classList.remove('active');
            }
            pages[page].classList.add('active');
        }

        document.addEventListener('DOMContentLoaded', () => {
            const cartItems = document.getElementById('cart-items');
            const cartTotal = document.getElementById('cart-total');
            const checkoutTotal = document.getElementById('checkout-total');
            let total = 0;

            document.querySelectorAll('.add-to-cart').forEach(button => {
                button.addEventListener('click', () => {
                    const name = button.getAttribute('data-name');
                    const price = parseFloat(button.getAttribute('data-price'));

                    const listItem = document.createElement('li');
                    listItem.className = 'cart-item';
                    listItem.innerHTML = `<h2>${name}</h2><p>Price: $${price}</p><button class="remove-from-cart" data-price="${price}">Remove</button>`;
                    cartItems.appendChild(listItem);

                    total += price;
                    cartTotal.textContent = total.toFixed(2);
                    checkoutTotal.textContent = total.toFixed(2);

                    listItem.querySelector('.remove-from-cart').addEventListener('click', () => {
                        cartItems.removeChild(listItem);
                        total -= price;
                        cartTotal.textContent = total.toFixed(2);
                        checkoutTotal.textContent = total.toFixed(2);
                    });
                });
            });

            document.querySelector('.billing-form').addEventListener('submit', (e) => {
                e.preventDefault();
                alert('Order placed successfully!');
                cartItems.innerHTML = '';
                cartTotal.textContent = '0';
                checkoutTotal.textContent = '0';
                showPage('home');
            });
        });
    </script>
</body>
</html>
## Hi there 👋

<!--
**Clijah/Clijah** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
