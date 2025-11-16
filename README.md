<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minecraft Server Store</title>
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #333;
            min-height: 100vh;
        }
        header {
            background-color: rgba(44, 62, 80, 0.9);
            color: white;
            text-align: center;
            padding: 40px 20px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.3);
        }
        header h1 {
            font-size: 2.5em;
            margin: 0;
        }
        header p {
            font-size: 1.2em;
            margin: 10px 0 0;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        .section {
            background-color: rgba(255, 255, 255, 0.95);
            margin: 20px 0;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 8px 16px rgba(0,0,0,0.2);
            transition: transform 0.3s ease;
        }
        .section:hover {
            transform: translateY(-5px);
        }
        .section h2 {
            color: #2c3e50;
            border-bottom: 3px solid #3498db;
            padding-bottom: 10px;
            font-size: 2em;
        }
        .item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin: 20px 0;
            padding: 20px;
            border: 2px solid #ddd;
            border-radius: 10px;
            background-color: #f9f9f9;
            transition: box-shadow 0.3s ease;
        }
        .item:hover {
            box-shadow: 0 4px 12px rgba(0,0,0,0.15);
        }
        .item img {
            width: 100px;
            height: 100px;
            border-radius: 10px;
            margin-right: 20px;
            object-fit: cover;
        }
        .item-content {
            flex: 1;
        }
        .item h3 {
            margin: 0 0 10px;
            color: #2c3e50;
        }
        .price {
            font-weight: bold;
            color: #e74c3c;
            font-size: 1.2em;
        }
        .buy-btn {
            background: linear-gradient(45deg, #3498db, #2980b9);
            color: white;
            border: none;
            padding: 12px 25px;
            border-radius: 25px;
            cursor: pointer;
            text-decoration: none;
            font-size: 1em;
            transition: background 0.3s ease;
        }
        .buy-btn:hover {
            background: linear-gradient(45deg, #2980b9, #21618c);
        }
        .payment-options {
            display: flex;
            gap: 10px;
            margin-top: 10px;
        }
        .payment-btn {
            background-color: #27ae60;
            color: white;
            border: none;
            padding: 8px 15px;
            border-radius: 20px;
            cursor: pointer;
            font-size: 0.9em;
            transition: background 0.3s ease;
        }
        .payment-btn:hover {
            background-color: #229954;
        }
        footer {
            background-color: rgba(44, 62, 80, 0.9);
            color: white;
            text-align: center;
            padding: 30px;
            box-shadow: 0 -4px 8px rgba(0,0,0,0.3);
        }
        .server-link {
            background: linear-gradient(45deg, #e67e22, #d35400);
            color: white;
            padding: 15px 30px;
            border-radius: 25px;
            text-decoration: none;
            font-size: 18px;
            display: inline-block;
            margin: 10px 0;
            transition: background 0.3s ease;
        }
        .server-link:hover {
            background: linear-gradient(45deg, #d35400, #a04000);
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to Our Minecraft Server Store</h1>
        <p>Enhance your gameplay with exclusive ranks and crate keys!</p>
    </header>

    <div class="container">
        <section class="section">
            <h2>Available Ranks</h2>
            <div class="item">
                <img src="https://cdn.pixabay.com/photo/2017/09/04/09/06/golden-2713973_1280.jpg" alt="VIP Rank Icon"> <!-- VIP Rank Image -->
                <div class="item-content">
                    <h3>VIP RANK</h3>
                    <p>Enjoy priority access, exclusive perks, and more!</p>
                </div>
                <div>
                    <span class="price">₹30</span>
                    <button class="buy-btn">Buy Now</button>
                    <div class="payment-options">
                        <button class="payment-btn" onclick="payUPI('upi://pay?pa=ishant-shadow-empir@fam&pn=MinecraftStore&am=30&cu=INR&tn=VIPRank')">UPI</button>
                        <button class="payment-btn" onclick="window.open('https://phon.pe/pay?amount=30&note=VIPRank', '_blank')">PhonePe</button>
                        <button class="payment-btn" onclick="window.open('tez://upi/pay?pa=ishant-shadow-empir@fam&pn=MinecraftStore&am=30&cu=INR&tn=VIPRank', '_blank')">GPay</button>
                    </div>
                </div>
            </div>
            <div class="item">
                <img src="https://cdn.pixabay.com/photo/2016/11/29/05/45/astronomy-1867616_1280.jpg" alt="Shadow Rank Icon"> <!-- Shadow Rank Image -->
                <div class="item-content">
                    <h3>SHADOW RANK</h3>
                    <p>Unlock shadow abilities and hidden features!</p>
                </div>
                <div>
                    <span class="price">₹35</span>
                    <button class="buy-btn">Buy Now</button>
                    <div class="payment-options">
                        <button class="payment-btn" onclick="payUPI('upi://pay?pa=ishant-shadow-empir@fam&pn=MinecraftStore&am=35&cu=INR&tn=ShadowRank')">UPI</button>
                        <button class="payment-btn" onclick="window.open('https://phon.pe/pay?amount=35&note=ShadowRank', '_blank')">PhonePe</button>
                        <button class="payment-btn" onclick="window.open('tez://upi/pay?pa=ishant-shadow-empir@fam&pn=MinecraftStore&am=35&cu=INR&tn=ShadowRank', '_blank')">GPay</button>
                    </div>
                </div>
            </div>
            <div class="item">
                <img src="https://cdn.pixabay.com/photo/2017/08/30/01/05/milky-way-2695569_1280.jpg" alt="Elite Rank Icon"> <!-- Elite Rank Image -->
                <div class="item-content">
                    <h3>ELITE RANK</h3>
                    <p>Become an elite player with top-tier benefits!</p>
                </div>
                <div>
                    <span class="price">₹30</span>
                    <button class="buy-btn">Buy Now</button>
                    <div class="payment-options">
                        <button class="payment-btn" onclick="payUPI('upi://pay?pa=ishant-shadow-empir@fam&pn=MinecraftStore&am=30&cu=INR&tn=EliteRank')">UPI</button>
                        <button class="payment-btn" onclick="window.open('https://phon.pe/pay?amount=30&note=EliteRank', '_blank')">PhonePe</button>
                        <button class="payment-btn" onclick="window.open('tez://upi/pay?pa=ishant-shadow-empir@fam&pn=MinecraftStore&am=30&cu=INR&tn=EliteRank', '_blank')">GPay</button>
                    </div>
                </div>
            </div>
        </section>

        <section class="section">
            <h2>Crate Keys</h2>
            <div class="item">
                <img src="https://cdn.pixabay.com/photo/2014/04/03/10/32/key-310745_1280.png" alt="Spawner Key Icon"> <!-- Spawner Key Image -->
                <div class="item-content">
                    <h3>SPAWNER KEY</h3>
                    <p>Open spawner crates for rare mobs and items!</p>
                </div>
                <div>
                    <span class="price">₹10</span>
                    <button class="buy-btn">Buy Now</button>
                    <div class="payment-options">
                        <button class="payment-btn" onclick="payUPI('upi://pay?pa=ishant-shadow-empir@fam&pn=MinecraftStore&am=10&cu=INR&tn=SpawnerKey')">UPI</button>
                        <button class="payment-btn" onclick="window.open('https://phon.pe/pay?amount=10&note=SpawnerKey', '_blank')">PhonePe</button>
                        <button class="payment-btn" onclick="window.open('tez://upi/pay?pa=ishant-shadow-empir@fam&pn=MinecraftStore&am=10&cu=INR&tn=SpawnerKey', '_blank')">GPay</button>
                    </div>
                </div>
            </div>
            <div class="item">
                <img src="https://cdn.pixabay.com/photo/2016/03/31/19/51/key-1294564_1280.png" alt="Shadow Key Icon"> <!-- Shadow Key Image -->
                <div class="item-content">
                    <h3>SHADOW KEY</h3>
                    <p>Unlock shadow-themed loot and surprises!</p>
                </div>
                <div>
                    <span class="price">₹20</span>
                    <button class="buy-btn">Buy Now</button>
                    <div class="payment-options">
                        <button class="payment-btn" onclick="payUPI('upi://pay?pa=ishant-shadow-empir@fam&pn=MinecraftStore&am=20&cu=INR&tn=ShadowKey')">UPI</button>
                        <button class="payment-btn" onclick="window.open('https://phon.pe/pay?amount=20&note=ShadowKey', '_blank')">PhonePe</button>
                        <button class="payment-btn" onclick="window.open('tez://upi/pay?pa=ishant-shadow-empir@fam&pn=MinecraftStore&am=20&cu=INR&tn=ShadowKey', '_blank')">GPay</button>
                    </div>
                </div>
            </div>
            <div class="item">
                <img src="https://cdn.pixabay.com/photo/2013/07/12/19/16/key-154565_1280.png" alt="Pro Key Icon"> <!-- Pro Key Image -->
                <div class="item-content">
                    <h3>PRO KEY</h3>
                    <p>Access pro-level crates with epic rewards!</p>
                </div>
                <div>
                    <span class="price">₹10</span>
                    <button class="buy-btn">Buy Now</button>
                    <div class="payment-options">
                        <button class="payment-btn" onclick="payUPI('upi://pay?pa=ishant-shadow-empir@fam&pn=MinecraftStore&am=10&cu=INR&tn=ProKey')">UPI</button>
                        <button class="payment-btn" onclick="window.open('https://phon.pe/pay?amount=10&note=ProKey', '_blank')">PhonePe</button>
                        <button class="payment-btn" onclick="window.open('tez://upi/pay?pa=ishant-shadow-empir@fam&pn=MinecraftStore&am=10&cu=INR&tn=ProKey', '_blank')">GPay</button>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <footer>
        <p>Ready to join the adventure?</p>
        <a href="mc://earth.spinex.cloud:19390" class="server-link">Join Server Now</a>
        <p>Server IP: earth.spinex.cloud:19390</p>
    </footer>

    <script>
        function payUPI(upiLink) {
            window.location.href = upiLink;
        }
    </script>
</body>
</html>
