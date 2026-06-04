<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
    <title>DILZ FLOWER STORE | Premium Social Media Services</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;500;600;700;800;900&family=Poppins:wght@300;400;500;600;700;800&family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: linear-gradient(135deg, #0a0a2a 0%, #0a0a1a 100%);
            font-family: 'Poppins', sans-serif;
            color: #fff;
            overflow-x: hidden;
            min-height: 100vh;
        }

        /* Custom Scrollbar */
        ::-webkit-scrollbar { width: 8px; }
        ::-webkit-scrollbar-track { background: #0a0a2a; }
        ::-webkit-scrollbar-thumb { background: #3b82f6; border-radius: 10px; }

        /* Animations */
        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(40px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }

        @keyframes pulse {
            0%, 100% { opacity: 1; text-shadow: 0 0 10px #3b82f6; }
            50% { opacity: 0.8; text-shadow: 0 0 30px #3b82f6; }
        }

        @keyframes shimmer {
            0% { background-position: -1000px 0; }
            100% { background-position: 1000px 0; }
        }

        @keyframes borderGlow {
            0%, 100% { border-color: #3b82f6; box-shadow: 0 0 5px #3b82f6; }
            50% { border-color: #60a5fa; box-shadow: 0 0 20px #3b82f6; }
        }

        .fade-up { animation: fadeInUp 0.8s ease-out forwards; }
        .float-animation { animation: float 3s ease-in-out infinite; }
        .glow-text { animation: pulse 2s infinite; }

        /* Glassmorphism */
        .glass-card {
            background: rgba(20, 30, 60, 0.4);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(59, 130, 246, 0.3);
            border-radius: 24px;
            transition: all 0.3s ease;
        }

        .glass-card:hover {
            border-color: #3b82f6;
            box-shadow: 0 10px 40px rgba(59, 130, 246, 0.2);
            transform: translateY(-5px);
        }

        /* Buttons */
        .btn-primary {
            background: linear-gradient(135deg, #1e3a8a, #3b82f6);
            border: none;
            padding: 12px 28px;
            border-radius: 40px;
            color: white;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s;
            font-family: 'Orbitron', monospace;
        }

        .btn-primary:hover {
            transform: scale(1.05);
            box-shadow: 0 5px 25px rgba(59, 130, 246, 0.5);
        }

        .btn-outline {
            background: transparent;
            border: 2px solid #3b82f6;
            padding: 10px 24px;
            border-radius: 40px;
            color: #3b82f6;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s;
        }

        .btn-outline:hover {
            background: #3b82f6;
            color: white;
            transform: scale(1.05);
        }

        /* Navbar */
        .navbar {
            background: rgba(10, 10, 30, 0.95);
            backdrop-filter: blur(20px);
            border-bottom: 1px solid rgba(59, 130, 246, 0.3);
            position: sticky;
            top: 0;
            z-index: 1000;
            padding: 15px 0;
        }

        .nav-container {
            max-width: 1280px;
            margin: 0 auto;
            padding: 0 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 15px;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .logo-icon {
            width: 45px;
            height: 45px;
            background: linear-gradient(135deg, #1e3a8a, #3b82f6);
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            animation: borderGlow 2s infinite;
        }

        .logo-text {
            font-size: 1.5rem;
            font-weight: 800;
            font-family: 'Orbitron', monospace;
        }

        .logo-text span { color: #3b82f6; }

        .nav-links {
            display: flex;
            gap: 20px;
            align-items: center;
            flex-wrap: wrap;
        }

        .nav-link {
            text-decoration: none;
            color: #ccc;
            font-weight: 500;
            transition: 0.3s;
            cursor: pointer;
        }

        .nav-link:hover, .nav-link.active { color: #3b82f6; }

        /* Hero Section */
        .hero {
            text-align: center;
            padding: 60px 20px;
            background: radial-gradient(ellipse at top, rgba(59,130,246,0.1), transparent);
        }

        .hero h1 {
            font-size: 3.5rem;
            font-family: 'Orbitron', monospace;
            margin-bottom: 20px;
        }

        .hero h1 span { color: #3b82f6; }
        .hero p { font-size: 1.2rem; opacity: 0.8; max-width: 600px; margin: 0 auto; }

        .stats-banner {
            display: flex;
            justify-content: center;
            gap: 40px;
            margin-top: 40px;
            flex-wrap: wrap;
        }

        .stat-item {
            text-align: center;
        }

        .stat-number {
            font-size: 2rem;
            font-weight: 800;
            color: #3b82f6;
            font-family: 'Orbitron', monospace;
        }

        /* Container */
        .container {
            max-width: 1280px;
            margin: 0 auto;
            padding: 40px 20px;
        }

        /* Section Title */
        .section-title {
            font-size: 2rem;
            font-family: 'Orbitron', monospace;
            margin-bottom: 30px;
            text-align: center;
        }

        .section-title span { color: #3b82f6; }

        /* Product Grid */
        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
            gap: 25px;
        }

        .product-card {
            background: rgba(15, 25, 50, 0.8);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(59, 130, 246, 0.3);
            border-radius: 20px;
            padding: 25px;
            transition: all 0.3s;
            cursor: pointer;
            position: relative;
            overflow: hidden;
        }

        .product-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(59,130,246,0.1), transparent);
            transition: left 0.5s;
        }

        .product-card:hover::before { left: 100%; }
        .product-card:hover { transform: translateY(-8px); border-color: #3b82f6; box-shadow: 0 20px 40px rgba(59,130,246,0.2); }

        .product-icon {
            font-size: 3rem;
            margin-bottom: 15px;
            color: #3b82f6;
        }

        .product-title {
            font-size: 1.3rem;
            font-weight: 700;
            margin-bottom: 10px;
        }

        .product-desc {
            font-size: 0.85rem;
            opacity: 0.7;
            margin-bottom: 15px;
        }

        .product-price {
            font-size: 1.8rem;
            font-weight: 800;
            color: #3b82f6;
            margin: 15px 0;
        }

        .product-features {
            display: flex;
            gap: 15px;
            margin-bottom: 20px;
            font-size: 0.75rem;
        }

        .product-features span {
            background: rgba(59,130,246,0.2);
            padding: 4px 10px;
            border-radius: 20px;
        }

        /* Payment Section */
        .payment-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
            gap: 20px;
            margin-bottom: 30px;
        }

        .payment-card {
            background: rgba(15, 25, 50, 0.8);
            border: 1px solid rgba(59, 130, 246, 0.3);
            border-radius: 16px;
            padding: 20px;
            text-align: center;
            cursor: pointer;
            transition: 0.3s;
        }

        .payment-card:hover { border-color: #3b82f6; transform: translateY(-3px); }
        .payment-card i { font-size: 40px; color: #3b82f6; margin-bottom: 10px; }
        .payment-card h4 { font-size: 1rem; margin-bottom: 5px; }

        /* QRIS */
        .qris-container {
            background: rgba(15, 25, 50, 0.8);
            border: 1px solid rgba(59, 130, 246, 0.3);
            border-radius: 24px;
            padding: 30px;
            text-align: center;
            max-width: 450px;
            margin: 0 auto;
        }

        .qris-img {
            width: 200px;
            height: 200px;
            margin: 20px auto;
            border-radius: 16px;
            overflow: hidden;
            border: 2px solid #3b82f6;
        }

        .qris-img img { width: 100%; height: 100%; object-fit: cover; }

        /* Chat Section */
        .chat-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
        }

        .chat-card {
            background: rgba(15, 25, 50, 0.8);
            border: 1px solid rgba(59, 130, 246, 0.3);
            border-radius: 20px;
            padding: 25px;
            text-align: center;
        }

        .chat-icon {
            width: 70px;
            height: 70px;
            background: rgba(59,130,246,0.2);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 15px;
            font-size: 2rem;
        }

        /* Transfer Form */
        .transfer-card {
            background: rgba(15, 25, 50, 0.8);
            border: 1px solid rgba(59, 130, 246, 0.3);
            border-radius: 24px;
            padding: 30px;
            max-width: 600px;
            margin: 0 auto;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group input, .form-group textarea {
            width: 100%;
            padding: 14px;
            background: rgba(0,0,0,0.5);
            border: 1px solid rgba(59,130,246,0.3);
            border-radius: 12px;
            color: white;
            font-family: 'Poppins', sans-serif;
        }

        .form-group input:focus, .form-group textarea:focus {
            outline: none;
            border-color: #3b82f6;
        }

        /* Cart Sidebar */
        .cart-sidebar {
            position: fixed;
            top: 0;
            right: -400px;
            width: 100%;
            max-width: 380px;
            height: 100%;
            background: #0a0a1a;
            border-left: 2px solid #3b82f6;
            z-index: 2000;
            transition: right 0.3s;
            display: flex;
            flex-direction: column;
        }

        .cart-sidebar.open { right: 0; }

        .cart-header {
            padding: 20px;
            border-bottom: 1px solid #3b82f6;
            display: flex;
            justify-content: space-between;
        }

        .cart-items { flex: 1; overflow-y: auto; padding: 15px; }
        .cart-item {
            display: flex;
            gap: 10px;
            padding: 12px;
            border-bottom: 1px solid #222;
        }
        .cart-item-info { flex: 1; }
        .cart-item-title { font-weight: 600; }
        .cart-item-price { color: #3b82f6; font-size: 12px; }
        .cart-item-remove { color: #ef4444; cursor: pointer; }

        .cart-footer {
            padding: 20px;
            border-top: 1px solid #3b82f6;
        }

        .cart-total {
            font-size: 1.2rem;
            font-weight: bold;
            margin-bottom: 15px;
        }

        .overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.7);
            z-index: 1999;
            display: none;
        }

        .overlay.active { display: block; }

        /* Toast Notification */
        .toast {
            position: fixed;
            bottom: 100px;
            right: 20px;
            background: #3b82f6;
            padding: 12px 24px;
            border-radius: 12px;
            color: white;
            z-index: 9999;
            animation: fadeInUp 0.3s ease;
        }

        /* Footer */
        .footer {
            background: rgba(10,10,30,0.95);
            border-top: 1px solid rgba(59,130,246,0.3);
            padding: 40px 20px;
            text-align: center;
            margin-top: 60px;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .hero h1 { font-size: 2rem; }
            .section-title { font-size: 1.5rem; }
            .products-grid { grid-template-columns: 1fr; }
            .nav-container { flex-direction: column; }
            .stats-banner { gap: 20px; }
        }
    </style>
</head>
<body>

<!-- Floating Particles Background -->
<div style="position: fixed; top: 0; left: 0; width: 100%; height: 100%; pointer-events: none; z-index: -1;">
    <canvas id="particlesCanvas"></canvas>
</div>

<!-- Navbar -->
<nav class="navbar">
    <div class="nav-container">
        <div class="logo">
            <div class="logo-icon"><i class="fas fa-crown"></i></div>
            <div class="logo-text">DILZ<span>FLOWER</span></div>
        </div>
        <div class="nav-links">
            <a class="nav-link active" data-page="home">🏠 Home</a>
            <a class="nav-link" data-page="products">📦 Products</a>
            <a class="nav-link" data-page="payment">💳 Payment</a>
            <a class="nav-link" data-page="transfer">📤 Bukti TF</a>
            <a class="nav-link" data-page="chat">💬 Chat</a>
            <div class="cart-icon" style="cursor: pointer;" onclick="toggleCart()">
                <i class="fas fa-shopping-cart" style="font-size: 1.2rem;"></i>
                <span id="cartCount" style="background:#3b82f6; padding:2px 6px; border-radius:50%; font-size:0.7rem; margin-left:5px;">0</span>
            </div>
        </div>
    </div>
</nav>

<!-- Main Content -->
<main>
    <!-- Page Home -->
    <div id="page-home" class="page-content active-page">
        <div class="hero">
            <h1 class="fade-up">Premium <span>Social Media</span><br>Growth Services</h1>
            <p class="fade-up">Dapatkan flower/followers berkualitas untuk TikTok & Instagram Anda</p>
            <div class="stats-banner fade-up">
                <div class="stat-item"><div class="stat-number">1000+</div><div>Happy Clients</div></div>
                <div class="stat-item"><div class="stat-number">24/7</div><div>Support</div></div>
                <div class="stat-item"><div class="stat-number">100%</div><div>Guaranteed</div></div>
                <div class="stat-item"><div class="stat-number">5★</div><div>Rating</div></div>
            </div>
        </div>

        <div class="container">
            <div class="glass-card" style="padding: 40px; text-align: center;">
                <i class="fas fa-quote-left" style="font-size: 2rem; color: #3b82f6;"></i>
                <p style="font-size: 1.2rem; margin: 20px 0;">"Kualitas flower terbaik, harga termurah, dan proses paling cepat!"</p>
                <div class="btn-outline" onclick="scrollToProducts()">Lihat Produk →</div>
            </div>
        </div>
    </div>

    <!-- Page Products -->
    <div id="page-products" class="page-content">
        <div class="container">
            <h2 class="section-title">Our <span>Products</span></h2>
            <div class="products-grid" id="productsGrid"></div>
        </div>
    </div>

    <!-- Page Payment -->
    <div id="page-payment" class="page-content">
        <div class="container">
            <h2 class="section-title">Payment <span>Methods</span></h2>
            <div class="payment-grid" id="paymentGrid"></div>
            <div class="qris-container">
                <h3><i class="fas fa-qrcode"></i> QRIS Payment</h3>
                <div class="qris-img">
                    <img src="https://files.catbox.moe/h7oeep.jpg" alt="QRIS">
                </div>
                <p>Scan QRIS di atas atau transfer ke rekening berikut:</p>
                <div style="background: rgba(0,0,0,0.3); padding: 15px; border-radius: 12px; margin-top: 15px;">
                    <p><strong>🏦 BCA</strong> : tidak ada a.n DILZ FLOWER</p>
                    <p><strong>📱 DANA/OVO</strong> : 083114960591</p>
                </div>
                <button class="btn-primary" style="margin-top: 15px;" onclick="copyText('088888888888')"><i class="fas fa-copy"></i> Copy Nomor</button>
            </div>
        </div>
    </div>

    <!-- Page Transfer -->
    <div id="page-transfer" class="page-content">
        <div class="container">
            <h2 class="section-title">Transfer <span>Confirmation</span></h2>
            <div class="transfer-card">
                <h3 style="margin-bottom: 20px; text-align: center;"><i class="fas fa-upload"></i> Kirim Bukti Transfer</h3>
                <div class="form-group">
                    <input type="text" id="buyerName" placeholder="Nama Lengkap">
                </div>
                <div class="form-group">
                    <input type="text" id="productOrdered" placeholder="Produk yang Dibeli">
                </div>
                <div class="form-group">
                    <input type="text" id="amountPaid" placeholder="Jumlah Transfer">
                </div>
                <div class="form-group">
                    <textarea id="proofLink" rows="3" placeholder="Link bukti transfer (imgur/google drive) atau deskripsi"></textarea>
                </div>
                <button class="btn-primary" style="width: 100%;" onclick="sendProof()">
                    <i class="fab fa-whatsapp"></i> Kirim ke Admin
                </button>
            </div>
        </div>
    </div>

    <!-- Page Chat -->
    <div id="page-chat" class="page-content">
        <div class="container">
            <h2 class="section-title">Contact <span>Admin</span></h2>
            <div class="chat-grid">
                <div class="chat-card">
                    <div class="chat-icon" style="color: #25D366;"><i class="fab fa-whatsapp"></i></div>
                    <h3>WhatsApp</h3>
                    <p style="margin: 10px 0;">+6283187714996</p>
                    <button class="btn-primary" onclick="window.open('https://wa.me/6283187714996', '_blank')">Chat Now</button>
                </div>
                <div class="chat-card">
                    <div class="chat-icon" style="color: #0088cc;"><i class="fab fa-telegram"></i></div>
                    <h3>Telegram</h3>
                    <p style="margin: 10px 0;">@DekingXilerr</p>
                    <button class="btn-primary" onclick="window.open('https://t.me/DekingXilerr', '_blank')">Chat Now</button>
                </div>
                <div class="chat-card">
                    <div class="chat-icon" style="color: #3b82f6;"><i class="fas fa-envelope"></i></div>
                    <h3>Email Support</h3>
                               <p style="margin: 10px 0;">support@dilzflower.com</p>
                    <button class="btn-primary" onclick="location.href='mailto:support@dilzflower.com'">Send Email</button>
                </div>
            </div>
            <div class="glass-card" style="margin-top: 30px; padding: 25px; text-align: center;">
                <i class="fas fa-clock" style="color: #3b82f6;"></i>
                <p style="margin-top: 10px;">Admin Online 24/7 | Response Time: <strong>&lt; 5 menit</strong></p>
            </div>
        </div>
    </div>
</main>

<footer class="footer">
    <p>© 2025 DILZ  STORE - Premium Social Media Services</p>
    <p style="margin-top: 10px; opacity: 0.6;">100% Guaranteed | Fast Delivery | 24/7 Support</p>
</footer>

<!-- Cart Sidebar -->
<div class="overlay" id="overlay" onclick="toggleCart()"></div>
<div class="cart-sidebar" id="cartSidebar">
    <div class="cart-header">
        <h3><i class="fas fa-shopping-bag"></i> Keranjang Saya</h3>
        <i class="fas fa-times" style="cursor: pointer; font-size: 1.2rem;" onclick="toggleCart()"></i>
    </div>
    <div class="cart-items" id="cartItems"><p style="text-align:center;color:#666;">Keranjang kosong</p></div>
    <div class="cart-footer">
        <div class="cart-total">Total: <span id="cartTotal">Rp 0</span></div>
        <button class="btn-primary" style="width: 100%;" onclick="checkout()">Checkout</button>
    </div>
</div>

<script>
    // PRODUCT DATA
    const products = [
        { id: 1, name: "Jasa Suntik 100 flower TikTok", variant: "100 Flower", price: 7000, icon: "fab fa-tiktok", features: ["Instan", "Quality", "Guarantee"] },
        { id: 2, name: "Jasa Suntik 200 Flower TikTok", variant: "200 Flower", price: 15000, icon: "fab fa-tiktok", features: ["Instan", "Quality", "Guarantee", "Bonus 10"] },
        { id: 3, name: "jasa suntik 300 Flower TikTok", variant: "300 Flower", price: 23000, icon: "fab fa-tiktok", features: ["instan", "berkualitas", ] },
        { id: 4, name: "jasa suntik 100 pengikut saluran whathap", variant: "100 pengikut", price: 7500, icon: "fab fa-whatsapp", features: ["Premium", "berkualitas", "Instan"] },
        { id: 5, name: "jasa Suntik 200 pengikut saluran WhatsApp",  variant: "200 Flower", price: 15000, icon: "fab fa-whatsapp", features: ["Instan", "Quality", "Guarantee", "Bonus 20"] },
        { id: 5, name: "jasa Suntik 300 pengikut saluran WhatsApp", variant: "300 pengikut", price: 22500, icon: "fab fa-whatsapp", features: ["intan", "cepat", "berkualitas"] },
        { id: 7, name: "Jasa Suntik Instagram", variant: "100 Flower", price: 4000, icon: "fab fa-instagram", features: ["Instan", "Quality", "Guarantee"] },
        { id: 8, name: "Jasa Suntik Instagram", variant: "200 Flower", price: 8000, icon: "fab fa-instagram", features: ["Instan", "Quality", "Guarantee", "Bonus 10"] },
        { id: 9, name: "jasa suntik 300 Flower Instagram", variant: "300 flower", price: 12000, icon: "fab fa-instagram", features: ["Instan", "cepat", "bonus 10"] },
        { id: 10, name: "apk bug vatonic 1h", variant: "work", price: 2500, icon: "fab fa-virus", features: ["di jamin work", "100%"] },
        { id: 11, name: "apk bug vatonic 7h", variant: "work", price: 6000, icon: "fab fa-virus", features: ["di jamin work", "100%"] },
        { id: 12, name: "apk bug vatonic 1bulan", variant: "work", price: 15000, icon: "fab fa-virus", features: ["di jamin work", "100%", "siap pakai"] },
        { id: 13, name: "apk bug vatonic permanen", variant: "work", price: 25000, icon: "fab fa-virus", features: ["di jamin work", "100%", "di masukin grup", "eror langsung di benarkan"] },
        { id: 14, name: "jasa suntik saluran Telegram", variant: "100 pengikut", price: 5000, icon: "fab fa-telegram", features: ["proses cepat", "100%"] },
        { id: 15, name: "jasa suntik saluran Telegram", variant: "200 pengikut", price: 10000, icon: "fab fa-telegram", features: ["proses cepat", "100%"] },
        { id: 16, name: "jasa suntik saluran Telegram", variant: "300 pengikut", price: 15000, icon: "fab fa-telegram", features: ["proses cepat", "100%"] },
        { id: 17, name: "murbug via Telegram", variant: "bebas spam", price: 6000, icon: "fab fa-telegram", features: ["work dan bebas spam", "100%", "bisa open jasa bug"] },
        { id: 18, name: "admin murbug via Telegram", variant: "bebas spam", price: 12000, icon: "fab fa-telegram", features: ["work dan bebas spam", "100%", "bisa open jasa bug", "bisa open member murbug"] },
        { id: 19, name: "murid suntik flower all sosmed", variant: "bisa open jasa suntik", price: 7000, icon: "fab fa-telegram", features: ["bisa untuk banyak", "100% berfungsi", "bisa balik modal"] },
    ];

    // PAYMENT DATA
    const payments = [
        { name: "DANA", number: "083114960591", icon: "fas fa-mobile-alt" },
        { name: "OVO", number: "083114960591", icon: "fas fa-wallet" },
        { name: "GOPAY", number: "-", icon: "fas fa-qrcode" },
        { name: "BCA", number: "-", icon: "fas fa-university" }
    ];

    let cart = [];

    function formatRupiah(amount) { return "Rp " + amount.toLocaleString("id-ID"); }

    function renderProducts() {
    const grid = document.getElementById("productsGrid");
        if(!grid) return;
        grid.innerHTML = products.map(p => `
            <div class="product-card">
                <div class="product-icon"><i class="${p.icon}"></i></div>
                <div class="product-title">${p.name}</div>
                <div class="product-desc">${p.variant} | Premium Quality</div>
        `).join("");
    }

    function addToCart(id) {
        const product = products.find(p => p.id === id);
        const existing = cart.find(item => item.id === id);
                <div class="product-features">${p.features.map(f => `<span>✓ ${f}</span>`).join('')}</div>
                <div class="product-price">${formatRupiah(p.price)}</div>
                <button class="btn-primary" style="width:100%;" onclick="addToCart(${p.id})"><i class="fas fa-cart-plus"></i> Tambah ke Keranjang</button>
            </div>
        `).join("");
    }

    function renderPayments() {
        const grid = document.getElementById("paymentGrid");
        if(!grid) return;
        grid.innerHTML = payments.map(p => `
            <div class="payment-card" onclick="copyText('${p.number}')">
                <i class="${p.icon}"></i>
                <h4>${p.name}</h4>
                <p>${p.number}</p>
                <small style="opacity:0.6;">Klik untuk copy</small>
            </div>
        if(existing) existing.quantity++;
        else cart.push({ ...product, quantity: 1 });
        updateCartUI();
        showToast(`✓ ${product.name} ${product.variant} ditambahkan!`);
    }

    function updateCartUI() {
        const count = cart.reduce((s, i) => s + i.quantity, 0);
        document.getElementById("cartCount").innerText = count;
        const cartItemsDiv = document.getElementById("cartItems");
        const cartTotalSpan = document.getElementById("cartTotal");
        if(cart.length === 0) {
            cartItemsDiv.innerHTML = '<p style="text-align:center;color:#666;">Keranjang kosong</p>';
            cartTotalSpan.innerText = formatRupiah(0);
            return;
        }
        cartItemsDiv.innerHTML = cart.map(item => `
            <div class="cart-item">
                <div class="cart-item-info">
                    <div class="cart-item-title">${item.name} (${item.variant})</div>
                    <div class="cart-item-price">${formatRupiah(item.price)} x ${item.quantity}</div>
                </div>
                <div class="cart-item-remove" onclick="removeFromCart(${item.id})"><i class="fas fa-trash-alt"></i></div>
            </div>
        `).join("");
        const total = cart.reduce((s, i) => s + (i.price * i.quantity), 0);
        cartTotalSpan.innerText = formatRupiah(total);
    }

    function removeFromCart(id) { cart = cart.filter(item => item.id !== id); updateCartUI(); }
    function toggleCart() {
        document.getElementById("cartSidebar").classList.toggle("open");
        document.getElementById("overlay").classList.toggle("active");
    }

    function checkout() {
        if(cart.length === 0) { showToast("Keranjang masih kosong!"); return; }
        const total = cart.reduce((s, i) => s + (i.price * i.quantity), 0);
        alert(`🛒 Total Pesanan: ${formatRupiah(total)}\n\nSilakan transfer ke:\n💰 DANA/OVO: 083114960591\n💰 BCA: -\n\nSetelah transfer, kirim bukti ke menu "Bukti TF"\nPesanan akan diproses dalam 5-30 menit.`);
        toggleCart();
    }

    function copyText(text) { navigator.clipboard.writeText(text); showToast(`✓ ${text} disalin!`); }
    
    function sendProof() {
        const name = document.getElementById("buyerName").value;
        const product = document.getElementById("productOrdered").value;
        const amount = document.getElementById("amountPaid").value;
        const proof = document.getElementById("proofLink").value;
        if(!name || !proof) { showToast("Isi nama dan bukti transfer!"); return; }
        const msg = `📝 *BUKTI TRANSFER DILZ FLOWER*\n\n👤 Nama: ${name}\n📦 Produk: ${product || '-'}\n💰 Jumlah: ${amount || '-'}\n📎 Bukti: ${proof}`;
        window.open(`https://wa.me/6283187714996?text=${encodeURIComponent(msg)}`, '_blank');
        showToast("✓ Bukti terkirim! Admin akan segera memproses.");
    }

    function showToast(msg) {
        const toast = document.createElement('div');
        toast.className = 'toast';
        toast.innerHTML = msg;
        document.body.appendChild(toast);
        setTimeout(() => toast.remove(), 3000);
    }

    // Particle Animation
    const canvas = document.getElementById('particlesCanvas');
    if(canvas) {
        canvas.width = window.innerWidth;
        canvas.height = window.innerHeight;
        const ctxPart = canvas.getContext('2d');
        const particles = [];
        for(let i = 0; i < 50; i++) {
            particles.push({ x: Math.random() * canvas.width, y: Math.random() * canvas.height, radius: Math.random() * 2 + 1, alpha: Math.random() });
        }
        function drawParticles() {
            ctxPart.clearRect(0, 0, canvas.width, canvas.height);
            particles.forEach(p => {
                ctxPart.beginPath();
                ctxPart.arc(p.x, p.y, p.radius, 0, Math.PI * 2);
                ctxPart.fillStyle = `rgba(59, 130, 246, ${p.alpha * 0.5})`;
                ctxPart.fill();
                p.y -= 0.5;
                if(p.y < 0) p.y = canvas.height;
            });
            requestAnimationFrame(drawParticles);
        }
        drawParticles();
        window.addEventListener('resize', () => { canvas.width = window.innerWidth; canvas.height = window.innerHeight; });
    }

    // Page Navigation
    function showPage(pageId) {
        document.querySelectorAll('.page-content').forEach(page => page.classList.remove('active-page'));
        document.getElementById(`page-${pageId}`).classList.add('active-page');
        document.querySelectorAll('.nav-link').forEach(link => link.classList.remove('active'));
        document.querySelector(`.nav-link[data-page="${pageId}"]`).classList.add('active');
        window.scrollTo({ top: 0, behavior: 'smooth' });
    }

    function scrollToProducts() { showPage('products'); }

    document.querySelectorAll('.nav-link').forEach(link => {
        link.addEventListener('click', () => showPage(link.getAttribute('data-page')));
    });

    // Initial Render
    renderProducts();
    renderPayments();
    document.querySelectorAll('.page-content').forEach(page => page.classList.remove('active-page'));
    document.getElementById('page-home').classList.add('active-page');

    // Style for active page
    const style = document.createElement('style');
    style.textContent = `.page-content { display: none; } .page-content.active-page { display: block; }`;
    document.head.appendChild(style);
</script>
</body>
</html>
