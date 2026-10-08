<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Golden Crust | Premium Fast Food & Ice Cream Lahore</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        amberGold: '#D97706',
                        darkCharcoal: '#18181B'
                    }
                }
            }
        }
    </script>
    <!-- FontAwesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600;700&family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Poppins', sans-serif;
        }
        h1, h2, h3, .brand-font {
            font-family: 'Playfair Display', serif;
        }
    </style>
</head>
<body class="bg-darkCharcoal text-gray-100 antialiased selection:bg-amberGold selection:text-white">

    <!-- Navbar -->
    <header class="sticky top-0 z-50 bg-darkCharcoal/95 backdrop-blur-md border-b border-gray-800 shadow-lg">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
            <!-- Brand Logo -->
            <a href="#" class="flex items-center space-x-3 group">
                <div class="w-11 h-11 rounded-full bg-gradient-to-tr from-amber-600 to-amber-400 flex items-center justify-center shadow-md group-hover:scale-105 transition duration-300">
                    <i class="fa-solid fa-burger text-white text-xl"></i>
                </div>
                <div>
                    <span class="text-2xl font-bold tracking-wider brand-font text-white">The Golden Crust</span>
                    <span class="block text-xs text-amber-500 tracking-widest uppercase font-medium">Lahore, Pakistan</span>
                </div>
            </a>

            <!-- Navigation Links & Cart -->
            <div class="flex items-center space-x-6">
                <nav class="hidden md:flex items-center space-x-8 font-medium text-sm">
                    <a href="#menu" class="hover:text-amber-500 transition">Menu</a>
                    <a href="#delivery-info" class="hover:text-amber-500 transition">Delivery Info</a>
                    <a href="#about" class="hover:text-amber-500 transition">About Us</a>
                    <a href="#contact" class="hover:text-amber-500 transition">Contact</a>
                </nav>

                <!-- Cart Button -->
                <button onclick="toggleCart()" class="relative bg-amber-600 hover:bg-amber-500 text-white px-5 py-2.5 rounded-full font-medium shadow-md transition duration-300 flex items-center space-x-2">
                    <i class="fa-solid fa-cart-shopping"></i>
                    <span>Cart</span>
                    <span id="cart-count" class="absolute -top-1.5 -right-1.5 bg-red-600 text-white text-xs w-5 h-5 rounded-full flex items-center justify-center font-bold border-2 border-darkCharcoal shadow">0</span>
                </button>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="relative bg-gradient-to-r from-gray-900 via-zinc-900 to-black py-24 lg:py-32 overflow-hidden border-b border-gray-800">
        <div class="absolute inset-0 opacity-20 bg-[radial-gradient(#d97706_1px,transparent_1px)] [background-size:16px_16px]"></div>
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10 text-center">
            <span class="inline-block bg-amber-500/10 text-amber-400 text-sm font-semibold px-4 py-1.5 rounded-full mb-6 border border-amber-500/20">
                ✨ Same-Day Delivery in Lahore | 2-3 Working Days Nationwide
            </span>
            <h1 class="text-4xl sm:text-6xl lg:text-7xl font-extrabold tracking-tight text-white mb-6 leading-tight">
                Crafted with Passion, <br><span class="text-transparent bg-clip-text bg-gradient-to-r from-amber-500 to-amber-200">Served with Perfection.</span>
            </h1>
            <p class="max-w-2xl mx-auto text-lg text-gray-400 mb-10">
                Order gourmet smash burgers, simple everyday burgers, crispy fast food, and artisan ice creams directly via WhatsApp with easy JazzCash & EasyPaisa payment.
            </p>
            <div class="flex justify-center gap-4 flex-wrap">
                <a href="#menu" class="bg-amber-600 hover:bg-amber-500 text-white font-semibold px-8 py-3.5 rounded-full shadow-lg transition duration-300">
                    Explore Full Menu
                </a>
                <a href="https://wa.me/923034812714?text=Hello%20The%20Golden%20Crust,%20I%20want%20to%20place%20an%20order." target="_blank" class="bg-green-600 hover:bg-green-500 text-white font-semibold px-8 py-3.5 rounded-full shadow-lg transition duration-300 flex items-center">
                    <i class="fa-brands fa-whatsapp mr-2 text-xl"></i> Direct WhatsApp Order
                </a>
            </div>
        </div>
    </section>

    <!-- Delivery Notice Section -->
    <section id="delivery-info" class="bg-zinc-900 py-10 border-b border-gray-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 grid grid-cols-1 md:grid-cols-2 gap-6 text-center md:text-left items-center">
            <div class="flex items-center space-x-4 justify-center md:justify-start">
                <div class="w-12 h-12 bg-amber-500/10 rounded-2xl flex items-center justify-center text-amber-500 text-2xl">
                    <i class="fa-solid fa-truck-fast"></i>
                </div>
                <div>
                    <h3 class="font-bold text-white text-lg">Lahore: Same-Day Delivery</h3>
                    <p class="text-gray-400 text-sm">Get fresh hot meals delivered at your doorstep on the same day within Lahore.</p>
                </div>
            </div>
            <div class="flex items-center space-x-4 justify-center md:justify-start">
                <div class="w-12 h-12 bg-amber-500/10 rounded-2xl flex items-center justify-center text-amber-500 text-2xl">
                    <i class="fa-solid fa-box-open"></i>
                </div>
                <div>
                    <h3 class="font-bold text-white text-lg">Other Cities: 2-3 Working Days</h3>
                    <p class="text-gray-400 text-sm">Secure and fast delivery across Pakistan within 2 to 3 working days.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Menu Section -->
    <section id="menu" class="py-20 bg-zinc-950">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-12">
                <h2 class="text-3xl sm:text-4xl font-bold text-white mb-4">Our Signature Menu</h2>
                <div class="w-24 h-1 bg-amber-600 mx-auto rounded-full mb-4"></div>
                <p class="text-gray-400 max-w-xl mx-auto">Choose from our delicious items below. Filter by category or search instantly.</p>
            </div>

            <!-- Controls: Category Filters & Sorting -->
            <div class="flex flex-col md:flex-row items-center justify-between gap-4 mb-10 bg-zinc-900 p-4 rounded-2xl border border-gray-800">
                <!-- Category Buttons -->
                <div class="flex flex-wrap justify-center gap-2">
                    <button onclick="filterMenu('all')" class="filter-btn active-filter px-5 py-2 rounded-xl bg-amber-600 text-white font-medium text-sm transition shadow">All Items</button>
                    <button onclick="filterMenu('burgers')" class="filter-btn px-5 py-2 rounded-xl bg-zinc-800 text-gray-300 hover:bg-zinc-700 font-medium text-sm transition">Burgers</button>
                    <button onclick="filterMenu('fastfood')" class="filter-btn px-5 py-2 rounded-xl bg-zinc-800 text-gray-300 hover:bg-zinc-700 font-medium text-sm transition">Fast Food & Sides</button>
                    <button onclick="filterMenu('icecream')" class="filter-btn px-5 py-2 rounded-xl bg-zinc-800 text-gray-300 hover:bg-zinc-700 font-medium text-sm transition">Ice Cream</button>
                </div>

                <!-- Sorting Dropdown -->
                <div class="flex items-center space-x-2 w-full md:w-auto">
                    <span class="text-gray-400 text-sm whitespace-nowrap"><i class="fa-solid fa-sort mr-1"></i> Sort:</span>
                    <select id="sort-select" onchange="sortProducts()" class="bg-zinc-950 text-white text-sm border border-gray-700 rounded-xl px-4 py-2 focus:outline-none focus:border-amber-500 w-full md:w-auto">
                        <option value="default">Default</option>
                        <option value="low-high">Price: Low to High</option>
                        <option value="high-low">Price: High to Low</option>
                        <option value="name">Name (A-Z)</option>
                    </select>
                </div>
            </div>

            <!-- Product Grid -->
            <div id="product-grid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Items injected dynamically -->
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 bg-darkCharcoal border-t border-gray-900">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
            <div>
                <span class="text-amber-500 font-semibold tracking-wider text-sm uppercase">About The Golden Crust</span>
                <h2 class="text-3xl sm:text-4xl font-bold text-white mt-2 mb-6">Serving Great Taste Across Lahore</h2>
                <p class="text-gray-400 mb-4 leading-relaxed">
                    The Golden Crust started with a simple mission: to serve premium quality fast food and refreshing artisan ice creams made fresh every day with high-grade local ingredients.
                </p>
                <p class="text-gray-400 mb-6 leading-relaxed">
                    Whether you are craving our heavy gourmet smash burgers or our comforting simple burgers and fries, we ensure top-notch taste and speedy service.
                </p>
                <div class="grid grid-cols-2 gap-6 pt-4 border-t border-gray-800">
                    <div>
                        <h4 class="text-2xl font-bold text-amber-500">Same-Day</h4>
                        <p class="text-sm text-gray-400 mt-1">Delivery in Lahore</p>
                    </div>
                    <div>
                        <h4 class="text-2xl font-bold text-amber-500">Easy Payment</h4>
                        <p class="text-sm text-gray-400 mt-1">JazzCash & EasyPaisa</p>
                    </div>
                </div>
            </div>
            <div class="bg-zinc-900 p-8 rounded-2xl border border-gray-800 shadow-2xl relative overflow-hidden">
                <div class="absolute -right-10 -bottom-10 w-40 h-40 bg-amber-600/10 rounded-full blur-2xl"></div>
                <h3 class="text-2xl font-bold text-white mb-6">Payment & Contact Info</h3>
                <ul class="space-y-4 text-gray-300">
                    <li class="flex items-start space-x-3">
                        <i class="fa-solid fa-location-dot text-amber-500 mt-1.5"></i>
                        <span>Main Boulevard, Gulberg III, Lahore, Pakistan</span>
                    </li>
                    <li class="flex items-center space-x-3">
                        <i class="fa-solid fa-phone text-amber-500"></i>
                        <span class="font-semibold text-white">0303-4812714 (WhatsApp / Mobile)</span>
                    </li>
                    <li class="flex items-center space-x-3 bg-zinc-950 p-3 rounded-xl border border-gray-800">
                        <i class="fa-solid fa-wallet text-amber-500 text-xl"></i>
                        <div>
                            <p class="text-xs text-gray-400">JazzCash & EasyPaisa Account:</p>
                            <p class="font-bold text-white">03034812714</p>
                        </div>
                    </li>
                </ul>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer id="contact" class="bg-black py-12 border-t border-gray-900 text-center text-gray-500 text-sm">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <p class="text-white font-medium text-lg mb-2 brand-font">The Golden Crust - Lahore</p>
            <p class="mb-2">WhatsApp Orders & Payments: <span class="text-amber-500 font-bold">03034812714</span> (JazzCash / EasyPaisa)</p>
            <p>&copy; 2026 The Golden Crust. All rights reserved.</p>
        </div>
    </footer>

    <!-- Slide-over Cart Drawer -->
    <div id="cart-drawer" class="fixed inset-0 z-50 overflow-hidden hidden">
        <div class="absolute inset-0 bg-black/70 backdrop-blur-sm transition-opacity" onclick="toggleCart()"></div>
        <div class="absolute inset-y-0 right-0 max-w-full flex pl-10">
            <div class="w-screen max-w-md bg-zinc-900 border-l border-gray-800 flex flex-col shadow-2xl">
                <!-- Cart Header -->
                <div class="flex items-center justify-between px-6 py-5 border-b border-gray-800">
                    <h3 class="text-xl font-bold text-white flex items-center space-x-2">
                        <i class="fa-solid fa-cart-shopping text-amber-500"></i>
                        <span>Your Order Cart</span>
                    </h3>
                    <button onclick="toggleCart()" class="text-gray-400 hover:text-white p-2">
                        <i class="fa-solid fa-xmark text-xl"></i>
                    </button>
                </div>
                <!-- Cart Items Container -->
                <div id="cart-items" class="flex-1 overflow-y-auto p-6 space-y-4">
                    <!-- Dynamic cart items list -->
                </div>
                <!-- Cart Footer -->
                <div class="border-t border-gray-800 p-6 bg-zinc-950 space-y-4">
                    <div class="flex justify-between text-base font-medium text-white">
                        <span>Subtotal</span>
                        <span id="cart-total" class="text-amber-500 font-bold">PKR 0</span>
                    </div>
                    <button onclick="openCheckoutModal()" class="w-full bg-amber-600 hover:bg-amber-500 text-white font-semibold py-3.5 rounded-xl shadow-lg transition duration-300 flex items-center justify-center space-x-2">
                        <i class="fa-brands fa-whatsapp text-xl"></i>
                        <span>Order via WhatsApp</span>
                    </button>
                </div>
            </div>
        </div>
    </div>

    <!-- Checkout Modal for Delivery Details & Receipt -->
    <div id="checkout-modal" class="fixed inset-0 z-50 overflow-y-auto hidden flex items-center justify-center p-4">
        <div class="fixed inset-0 bg-black/75 backdrop-blur-sm" onclick="closeCheckoutModal()"></div>
        <div class="relative bg-zinc-900 border border-gray-800 rounded-2xl max-w-lg w-full p-6 shadow-2xl z-10">
            <div class="flex justify-between items-center mb-6 border-b border-gray-800 pb-4">
                <h3 class="text-xl font-bold text-white flex items-center space-x-2">
                    <i class="fa-solid fa-file-invoice-dollar text-amber-500"></i>
                    <span>Enter Delivery Details</span>
                </h3>
                <button onclick="closeCheckoutModal()" class="text-gray-400 hover:text-white"><i class="fa-solid fa-xmark text-xl"></i></button>
            </div>
            <div class="space-y-4">
                <div>
                    <label class="block text-xs text-gray-400 mb-1">Your Full Name</label>
                    <input type="text" id="customer-name" placeholder="e.g. Ali Khan" class="w-full bg-zinc-950 border border-gray-800 rounded-xl px-4 py-3 text-white text-sm focus:outline-none focus:border-amber-500">
                </div>
                <div>
                    <label class="block text-xs text-gray-400 mb-1">Phone Number</label>
                    <input type="text" id="customer-phone" placeholder="e.g. 03001234567" class="w-full bg-zinc-950 border border-gray-800 rounded-xl px-4 py-3 text-white text-sm focus:outline-none focus:border-amber-500">
                </div>
                <div>
                    <label class="block text-xs text-gray-400 mb-1">Delivery Address (Lahore Same-Day / Other Cities 2-3 Days)</label>
                    <textarea id="customer-address" rows="3" placeholder="Enter complete address..." class="w-full bg-zinc-950 border border-gray-800 rounded-xl px-4 py-3 text-white text-sm focus:outline-none focus:border-amber-500"></textarea>
                </div>
                <div class="bg-zinc-950 p-4 rounded-xl border border-gray-800 text-xs text-gray-300 space-y-1">
                    <p class="font-bold text-amber-500 mb-1"><i class="fa-solid fa-circle-info mr-1"></i> Payment Info:</p>
                    <p>Send payment via JazzCash or EasyPaisa to: <strong class="text-white">03034812714</strong></p>
                    <p class="text-gray-400">You can also pay Cash on Delivery (COD).</p>
                </div>
                <button onclick="finalizeOrder()" class="w-full bg-green-600 hover:bg-green-500 text-white font-semibold py-3.5 rounded-xl shadow-lg transition duration-300 flex items-center justify-center space-x-2">
                    <i class="fa-brands fa-whatsapp text-lg"></i>
                    <span>Send Order to WhatsApp & Get Receipt</span>
                </button>
            </div>
        </div>
    </div>

    <!-- Receipt / Success Modal -->
    <div id="receipt-modal" class="fixed inset-0 z-50 overflow-y-auto hidden flex items-center justify-center p-4">
        <div class="fixed inset-0 bg-black/80 backdrop-blur-sm"></div>
        <div class="relative bg-zinc-900 border border-amber-500/50 rounded-2xl max-w-md w-full p-6 shadow-2xl z-10 text-center">
            <div class="w-16 h-16 bg-green-500/10 text-green-500 rounded-full flex items-center justify-center text-3xl mx-auto mb-4 border border-green-500/30">
                <i class="fa-solid fa-check"></i>
            </div>
            <h3 class="text-2xl font-bold text-white mb-2 brand-font">Thank You!</h3>
            <p class="text-amber-500 text-sm font-medium mb-6">Your order has been sent via WhatsApp successfully!</p>
            
            <div id="receipt-details" class="bg-zinc-950 text-left p-4 rounded-xl border border-gray-800 text-xs text-gray-300 space-y-2 mb-6 font-mono">
                <!-- Receipt content populated dynamically -->
            </div>
            
            <button onclick="closeReceiptModal()" class="w-full bg-amber-600 hover:bg-amber-500 text-white font-semibold py-3 rounded-xl transition">
                Done / Back to Store
            </button>
        </div>
    </div>

    <!-- JavaScript Application Logic -->
    <script>
        const products = [
            { id: 1, name: "The Royal Truffle Burger", category: "burgers", price: 1250, desc: "Double Angus beef patty, truffle mayo, aged cheddar, caramelized onions.", icon: "fa-burger" },
            { id: 2, name: "Crispy Zinger Supreme", category: "burgers", price: 950, desc: "Extra crispy fried chicken breast, spicy honey glaze, crisp iceberg lettuce.", icon: "fa-drumstick-bite" },
            { id: 3, name: "Simple Burger", category: "burgers", price: 450, desc: "Classic beef patty with fresh lettuce, tomato, and house special sauce.", icon: "fa-burger" },
            { id: 4, name: "Simple Chicken Burger", category: "burgers", price: 480, desc: "Crispy chicken fillet with mayo, lettuce, and soft sesame bun.", icon: "fa-burger" },
            { id: 5, name: "Smokey BBQ Master Burger", category: "burgers", price: 1100, desc: "Charcoal grilled beef patty, hickory smoked BBQ sauce, beef bacon strips.", icon: "fa-burger" },
            { id: 6, name: "Loaded Cheese Fries", category: "fastfood", price: 650, desc: "Golden French fries drenched in warm liquid cheddar, jalapenos & beef bits.", icon: "fa-utensils" },
            { id: 7, name: "Crispy Buffalo Wings (8pcs)", category: "fastfood", price: 750, desc: "Tender wings tossed in fiery buffalo sauce served with ranch dip.", icon: "fa-fire" },
            { id: 8, name: "Crunchy Jalapeno Poppers", category: "fastfood", price: 550, desc: "Stuffed cheesy jalapeno bites fried to golden crisp perfection.", icon: "fa-pepper-hot" },
            { id: 9, name: "Belgium Chocolate Fudge Sundae", category: "icecream", price: 600, desc: "Rich dark chocolate ice cream scoops topped with hot fudge & brownie chunks.", icon: "fa-ice-cream" },
            { id: 10, name: "Mango Paradise Ice Cream Cup", category: "icecream", price: 450, desc: "Premium Alphonso mango artisan gelato served in a crunchy waffle cup.", icon: "fa-ice-cream" },
            { id: 11, name: "Salted Caramel Nut Crunch", category: "icecream", price: 520, desc: "Vanilla bean ice cream loaded with salted caramel swirls and roasted almonds.", icon: "fa-ice-cream" }
        ];

        let cart = [];
        let currentFilter = 'all';

        function renderProducts(filter = 'all', sortType = 'default') {
            currentFilter = filter;
            const grid = document.getElementById('product-grid');
            grid.innerHTML = '';
            
            let filtered = filter === 'all' ? [...products] : products.filter(p => p.category === filter);

            if (sortType === 'low-high') {
                filtered.sort((a, b) => a.price - b.price);
            } else if (sortType === 'high-low') {
                filtered.sort((a, b) => b.price - a.price);
            } else if (sortType === 'name') {
                filtered.sort((a, b) => a.name.localeCompare(b.name));
            }

            filtered.forEach(p => {
                const card = document.createElement('div');
                card.className = "bg-zinc-900 rounded-2xl p-6 border border-gray-800/80 shadow-lg hover:border-amber-500/50 transition duration-300 flex flex-col justify-between group";
                card.innerHTML = `
                    <div>
                        <div class="flex items-center justify-between mb-4">
                            <div class="w-12 h-12 rounded-xl bg-amber-500/10 text-amber-500 flex items-center justify-center text-xl group-hover:bg-amber-600 group-hover:text-white transition">
                                <i class="fa-solid ${p.icon}"></i>
                            </div>
                            <span class="text-lg font-bold text-amber-400">PKR ${p.price.toLocaleString()}</span>
                        </div>
                        <h3 class="text-xl font-bold text-white mb-2">${p.name}</h3>
                        <p class="text-gray-400 text-sm mb-6">${p.desc}</p>
                    </div>
                    <button onclick="addToCart(${p.id})" class="w-full bg-zinc-800 hover:bg-amber-600 text-white font-semibold py-2.5 rounded-xl transition duration-300 flex items-center justify-center space-x-2 border border-gray-700/50 group-hover:border-amber-600">
                        <i class="fa-solid fa-plus text-xs"></i>
                        <span>Add to Cart</span>
                    </button>
                `;
                grid.appendChild(card);
            });
        }

        function filterMenu(category) {
            document.querySelectorAll('.filter-btn').forEach(btn => {
                btn.classList.remove('bg-amber-600', 'text-white', 'active-filter');
                btn.classList.add('bg-zinc-800', 'text-gray-300');
            });
            event.target.classList.remove('bg-zinc-800', 'text-gray-300');
            event.target.classList.add('bg-amber-600', 'text-white', 'active-filter');
            
            const sortVal = document.getElementById('sort-select').value;
            renderProducts(category, sortVal);
        }

        function sortProducts() {
            const sortVal = document.getElementById('sort-select').value;
            renderProducts(currentFilter, sortVal);
        }

        function toggleCart() {
            const drawer = document.getElementById('cart-drawer');
            drawer.classList.toggle('hidden');
        }

        function addToCart(productId) {
            const product = products.find(p => p.id === productId);
            const existing = cart.find(item => item.id === productId);
            if (existing) {
                existing.qty++;
            } else {
                cart.push({ ...product, qty: 1 });
            }
            updateCartUI();
            toggleCart();
        }

        function updateCartUI() {
            const countEl = document.getElementById('cart-count');
            const itemsEl = document.getElementById('cart-items');
            const totalEl = document.getElementById('cart-total');

            const totalCount = cart.reduce((sum, item) => sum + item.qty, 0);
            countEl.textContent = totalCount;

            if (cart.length === 0) {
                itemsEl.innerHTML = `<p class="text-center text-gray-500 py-12">Your cart is empty.</p>`;
                totalEl.textContent = "PKR 0";
                return;
            }

            itemsEl.innerHTML = '';
            let subtotal = 0;

            cart.forEach(item => {
                subtotal += item.price * item.qty;
                const div = document.createElement('div');
                div.className = "flex items-center justify-between bg-zinc-950 p-4 rounded-xl border border-gray-800";
                div.innerHTML = `
                    <div>
                        <h4 class="font-semibold text-white text-sm">${item.name}</h4>
                        <p class="text-xs text-amber-500">PKR ${item.price.toLocaleString()} x ${item.qty}</p>
                    </div>
                    <div class="flex items-center space-x-2">
                        <button onclick="changeQty(${item.id}, -1)" class="w-7 h-7 bg-zinc-800 rounded-lg text-white hover:bg-zinc-700">-</button>
                        <span class="text-sm font-bold text-white">${item.qty}</span>
                        <button onclick="changeQty(${item.id}, 1)" class="w-7 h-7 bg-zinc-800 rounded-lg text-white hover:bg-zinc-700">+</button>
                    </div>
                `;
                itemsEl.appendChild(div);
            });

            totalEl.textContent = `PKR ${subtotal.toLocaleString()}`;
        }

        function changeQty(productId, delta) {
            const item = cart.find(i => i.id === productId);
            if (item) {
                item.qty += delta;
                if (item.qty <= 0) {
                    cart = cart.filter(i => i.id !== productId);
                }
                updateCartUI();
            }
        }

        function openCheckoutModal() {
            if (cart.length === 0) {
                alert('Please add items to your cart first!');
                return;
            }
            toggleCart();
            document.getElementById('checkout-modal').classList.remove('hidden');
        }

        function closeCheckoutModal() {
            document.getElementById('checkout-modal').classList.add('hidden');
        }

        function finalizeOrder() {
            const name = document.getElementById('customer-name').value.trim();
            const phone = document.getElementById('customer-phone').value.trim();
            const address = document.getElementById('customer-address').value.trim();

            if (!name || !phone || !address) {
                alert('Please fill in all delivery details.');
                return;
            }

            let total = 0;
            let itemsText = "";
            cart.forEach(item => {
                itemsText += `- ${item.name} (x${item.qty}): PKR ${item.price * item.qty}%0A`;
                total += item.price * item.qty;
            });

            let waMessage = `*New Order - The Golden Crust*%0A` +
                            `--------------------------------%0A` +
                            `*Customer Name:* ${name}%0A` +
                            `*Phone:* ${phone}%0A` +
                            `*Address:* ${address}%0A` +
                            `*Delivery Note:* Lahore Same-Day / Other Cities 2-3 Working Days%0A` +
                            `--------------------------------%0A` +
                            `*Order Items:*%0A${itemsText}` +
                            `--------------------------------%0A` +
                            `*Total Amount:* PKR ${total}%0A` +
                            `*Payment Info:* JazzCash / EasyPaisa (03034812714)%0A`;

            // Open WhatsApp
            window.open(`https://wa.me/923034812714?text=${waMessage}`, '_blank');

            // Show Receipt Modal
            showReceipt(name, phone, address, total);
            closeCheckoutModal();
        }

        function showReceipt(name, phone, address, total) {
            const receiptDiv = document.getElementById('receipt-details');
            let itemsListHtml = "";
            cart.forEach(item => {
                itemsListHtml += `<div>• ${item.name} (x${item.qty}) - PKR ${item.price * item.qty}</div>`;
            });

            receiptDiv.innerHTML = `
                <div class="border-b border-gray-800 pb-2 mb-2 text-white font-bold">THE GOLDEN CRUST - RECEIPT</div>
                <div><strong>Name:</strong> ${name}</div>
                <div><strong>Phone:</strong> ${phone}</div>
                <div><strong>Address:</strong> ${address}</div>
                <div class="border-t border-gray-800 pt-2 mt-2"><strong>Items:</strong></div>
                ${itemsListHtml}
                <div class="border-t border-gray-800 pt-2 mt-2 font-bold text-amber-500">Total: PKR ${total}</div>
                <div class="text-gray-400 text-[10px] mt-2">JazzCash/EasyPaisa: 03034812714</div>
            `;

            document.getElementById('receipt-modal').classList.remove('hidden');
            cart = [];
            updateCartUI();
        }

        function closeReceiptModal() {
            document.getElementById('receipt-modal').classList.add('hidden');
        }

        // Initial Load
        renderProducts();
    </script>
</body>
</html>
