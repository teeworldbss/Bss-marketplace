<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BSS Market Place | Official</title>
    <style>
        :root {
            --wa-teal: #075e54;
            --wa-light-teal: #128c7e;
            --wa-bg: #e5ddd5;
            --wa-white: #ffffff;
            --wa-smoke: #f0f2f5;
            --admin-red: #ff3b30;
            --seller-green: #25d366;
            --buyer-blue: #34b7f1;
        }

        body { font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; background-color: var(--wa-bg); margin: 0; padding: 0; }
        
        /* Fixed Header - Dev Contact */
        .header { background-color: var(--wa-teal); color: white; padding: 12px; position: sticky; top: 0; z-index: 1000; box-shadow: 0 2px 4px rgba(0,0,0,0.2); }
        .header-main { display: flex; justify-content: space-between; align-items: center; max-width: 800px; margin: 0 auto; }
        .dev-tag { font-size: 11px; color: #dcf8c6; letter-spacing: 0.5px; }

        .container { max-width: 800px; margin: 0 auto; height: 100vh; display: flex; flex-direction: column; }
        
        /* Chat Display Area */
        #display { flex: 1; overflow-y: auto; padding: 15px; display: flex; flex-direction: column; gap: 10px; }
        
        /* Message Bubbles */
        .msg { padding: 10px 15px; border-radius: 10px; max-width: 85%; font-size: 14.5px; position: relative; line-height: 1.4; box-shadow: 0 1px 0.5px rgba(0,0,0,0.13); }
        .system-bubble { align-self: center; background: #fff3cd; color: #856404; font-size: 12px; padding: 5px 15px; border-radius: 5px; }
        
        /* Hierarchy UI Bubbles */
        .admin-msg { align-self: flex-start; background: #fff; border-left: 5px solid var(--admin-red); }
        .seller-msg { align-self: flex-start; background: #fff; border-left: 5px solid var(--seller-green); }
        .buyer-msg { align-self: flex-start; background: #fff; border-left: 5px solid var(--buyer-blue); }
        .guest-msg { align-self: flex-start; background: #fff; border-left: 5px solid #999; }

        /* Dashboard & Number Menu */
        .footer-menu { background: var(--wa-smoke); padding: 15px; border-top: 1px solid #ddd; }
        .menu-title { font-size: 12px; color: #667781; margin-bottom: 10px; font-weight: bold; }
        .grid-menu { display: grid; grid-template-columns: 1fr 1fr; gap: 10px; }
        
        button { padding: 12px; border: none; border-radius: 8px; background: var(--wa-light-teal); color: white; cursor: pointer; font-size: 14px; text-align: left; }
        button:hover { background: var(--wa-teal); }
        .badge { font-weight: bold; text-decoration: underline; }
    </style>
</head>
<body>

<div class="header">
    <div class="header-main">
        <div><strong>🛡️ BSS MARKET PLACE</strong></div>
        <div class="dev-tag">DEV: 08118428191</div>
    </div>
</div>

<div class="container">
    <div id="display">
        <div class="system-bubble">Today, 2026-04-06</div>
        <div class="system-bubble">Connected to bss_bizgroup (Gemini Cloud)</div>
        
        <div class="msg guest-msg">
            <b>⚪ <u>Guest Mode</u></b><br>
            Welcome to the Marketplace. You have 5 free interactions before mandatory registration.
        </div>
    </div>

    <div class="footer-menu" id="nav-panel">
        <div class="menu-title">MAIN NAVIGATION (Select a Number)</div>
        <div class="grid-menu">
            <button onclick="loadDashboard('admin')">1. 🔴 Admin Login</button>
            <button onclick="loadDashboard('seller')">2. 🟢 Seller Dashboard</button>
            <button onclick="loadDashboard('buyer')">3. 🔵 Buyer Dashboard</button>
            <button onclick="window.location.href='/register'">4. 📝 Register Account</button>
        </div>
    </div>
</div>

<script>
    // System Prompt v1.0.1 Logic
    const display = document.getElementById('display');
    const nav = document.getElementById('nav-panel');

    function loadDashboard(role) {
        display.innerHTML = ''; // Clear for Dashboard view
        
        if(role === 'admin') {
            display.innerHTML += `<div class="msg admin-msg"><b>🔴 <u>ADMIN MASTER NODE</u></b><br>
                1. Verify Sellers (ID/Passport)<br>
                2. Subscription Toggle (ON/OFF)<br>
                3. Global Transaction View<br>
                4. Download System Prompt</div>`;
        } else if(role === 'seller') {
            display.innerHTML += `<div class="msg seller-msg"><b>🟢 <u>SELLER HUB</u></b><br>
                1. Post Advert (<b>BOLD ID</b>)<br>
                2. Stock Management<br>
                3. Transaction Monitor<br>
                4. Integrity Score: 5.0 ⭐</div>`;
        } else if(role === 'buyer') {
            display.innerHTML += `<div class="msg buyer-msg"><b>🔵 <u>BUYER PORTAL</u></b><br>
                1. View Group Adverts<br>
                2. Request Product<br>
                3. Tracking & Receipts<br>
                4. Confirm Delivery</div>`;
        }
        
        display.innerHTML += `<div class="system-bubble">Select an action above or type '0' to return.</div>`;
    }
</script>

</body>
</html>
