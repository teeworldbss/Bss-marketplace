<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BSS Market Place | Full Logic v2.0.8</title>
    <script src="https://www.gstatic.com/firebasejs/10.7.1/firebase-app-compat.js"></script>
    <script src="https://www.gstatic.com/firebasejs/10.7.1/firebase-firestore-compat.js"></script>

    <style>
        :root { --wa-teal: #075e54; --wa-light-teal: #128c7e; --wa-bg: #e5ddd5; --wa-smoke: #f0f2f5; --admin-red: #d32f2f; --mod-gold: #ffc107; --seller-green: #25d366; --buyer-blue: #34b7f1; }
        body { font-family: 'Segoe UI', Helvetica, Arial, sans-serif; background-color: var(--wa-bg); margin: 0; padding: 0; }
        .header { background-color: var(--wa-teal); color: white; padding: 12px; position: sticky; top: 0; z-index: 1000; box-shadow: 0 2px 5px rgba(0,0,0,0.2); }
        .header-content { display: flex; justify-content: space-between; align-items: center; max-width: 600px; margin: 0 auto; }
        .dev-info { font-size: 10px; color: #dcf8c6; font-weight: bold; }
        
        .container { max-width: 600px; margin: 0 auto; min-height: 100vh; display: flex; flex-direction: column; padding-bottom: 180px; }
        #chat-area { flex: 1; padding: 15px; display: flex; flex-direction: column; gap: 10px; }
        
        .bubble { padding: 12px; border-radius: 10px; max-width: 92%; font-size: 13.5px; box-shadow: 0 1px 1px rgba(0,0,0,0.1); background: white; line-height: 1.6; }
        .system-note { align-self: center; background: #fff3cd; color: #856404; font-size: 11px; padding: 4px 12px; border-radius: 4px; border: 1px solid #ffeeba; margin: 5px 0; }
        
        .admin-b { border-left: 6px solid var(--admin-red); }
        .mod-b { border-left: 6px solid var(--mod-gold); }
        .seller-b { border-left: 6px solid var(--seller-green); }
        .buyer-b { border-left: 6px solid var(--buyer-blue); }

        .footer-nav { background: var(--wa-smoke); padding: 10px; border-top: 1px solid #ccc; position: fixed; bottom: 0; width: 100%; max-width: 600px; box-sizing: border-box; }
        .grid { display: grid; grid-template-columns: 1fr 1fr; gap: 6px; margin-bottom: 8px; }
        button { padding: 10px; border: none; border-radius: 6px; background: var(--wa-light-teal); color: white; cursor: pointer; font-size: 10px; font-weight: 700; text-transform: uppercase; }
        
        .input-bar { display: flex; gap: 5px; background: white; padding: 5px; border-radius: 25px; border: 1px solid #bbb; align-items: center; }
        input { flex: 1; border: none; padding: 10px 15px; outline: none; font-size: 14px; background: transparent; }
        .send-btn { background: var(--wa-teal); color: white; border: none; width: 40px; height: 40px; border-radius: 50%; font-weight: bold; cursor: pointer; display: flex; align-items: center; justify-content: center; }
    </style>
</head>
<body>

<div class="header">
    <div class="header-content">
        <div>🛡️ BSS MARKET PLACE</div>
        <div class="dev-info">TAIWO FASHOLA: 08118428191</div>
    </div>
</div>

<div class="container">
    <div id="chat-area">
        <div class="system-note">bss_bizgroup Engine v2.0.8 | Fully Loaded</div>
        <div class="bubble buyer-b"><b>System Online.</b><br>Select your tier to view the full command menu and unified messaging inbox.</div>
    </div>

    <div class="footer-nav">
        <div class="grid">
            <button onclick="loadTier('admin')">🔴 ADMIN</button>
            <button onclick="loadTier('mod')">🟡 MODERATOR</button>
            <button onclick="loadTier('seller')">🟢 SELLER</button>
            <button onclick="loadTier('buyer')">🔵 BUYER</button>
        </div>
        <div class="input-bar">
            <input type="text" id="userMsg" placeholder="Type message or command...">
            <button class="send-btn" onclick="sendMessage()">➤</button>
        </div>
    </div>
</div>

<script>
    // Configuration Placeholder
    const firebaseConfig = { apiKey: "YOUR_KEY", authDomain: "YOUR_ID.firebaseapp.com", projectId: "YOUR_ID", storageBucket: "YOUR_ID.appspot.com", messagingSenderId: "ID", appId: "APP_ID" };
    firebase.initializeApp(firebaseConfig);
    const db = firebase.firestore();

    function loadTier(role) {
        const chat = document.getElementById('chat-area');
        let m = "";

        if(role === 'admin') {
            m = `<b>🔴 ADMIN MASTER (FULL MENU)</b><hr>
                1. <b>Verify Sellers:</b> Passport/NIN Document Approval<br>
                2. <b>System Toggle:</b> Seller Subscription Fee (ON/OFF)<br>
                3. <b>User Management:</b> Block, Unblock, or Terminate Users<br>
                4. <b>Global Monitoring:</b> View All Transactions & Group Logs<br>
                5. <b>Finance Center:</b> View Total Revenue & Payout Requests<br>
                6. <b>Core Engine:</b> Edit/Update System Prompt v2.0.8<br>
                7. <b>Permissions:</b> Assign or Revoke Moderator Roles<br>
                8. <b>Admin Messaging:</b> Private Inbox / Broadcast Alerts`;
        } else if(role === 'mod') {
            m = `<b>🟡 MODERATOR TOOLS (FULL MENU)</b><hr>
                1. <b>Group Oversight:</b> Real-time Chat Policy Monitoring<br>
                2. <b>Content Enforcement:</b> Delete Fake/Illegal Adverts<br>
                3. <b>Dispute Mediation:</b> Settle Buyer/Seller Conflict Tickets<br>
                4. <b>Private Inbox:</b> Receive Support Reports & Direct Inquiries<br>
                5. <b>Messaging:</b> Send Warnings / Report to Admin Hub<br>
                6. <b>Verification Check:</b> Review Seller Integrity Scores`;
        } else if(role === 'seller') {
            m = `<b>🟢 SELLER HUB (FULL MENU)</b><hr>
                1. <b>Post Advert:</b> Product Listing (Mandatory Bold ID)<br>
                2. <b>Inventory Logic:</b> Update Availability & Stock Quantities<br>
                3. <b>Order Tracking:</b> Pending -> Dispatched -> Delivered<br>
                4. <b>Private Inbox:</b> Direct Buyer Negotiations & Questions<br>
                5. <b>Messaging:</b> Send Bulk Stock Updates to Interested Buyers<br>
                6. <b>Secure Link:</b> Generate Direct WhatsApp/In-App Chat Invite<br>
                7. <b>Integrity Score:</b> Monitor Feedback (Target: 5.0 ⭐)`;
        } else if(role === 'buyer') {
            m = `<b>🔵 BUYER PORTAL (FULL MENU)</b><hr>
                1. <b>Market Search:</b> View Verified Active Advert Listings<br>
                2. <b>Product Request:</b> Post Inquiries for Needed Items<br>
                3. <b>Payment Portal:</b> Upload Proof of Payment (Receipts)<br>
                4. <b>Private Inbox:</b> Direct Messaging with Verified Sellers<br>
                5. <b>Messaging:</b> Send Delivery Location & Contact Details<br>
                6. <b>Tracking:</b> Monitor Arrival Time & Date Calculations<br>
                7. <b>Confirmation:</b> Confirm Delivery & Finalize Integrity Score`;
        }

        chat.innerHTML += `<div class="bubble ${role}-b">${m}</div>`;
        window.scrollTo(0, document.body.scrollHeight);
    }

    function sendMessage() {
        const input = document.getElementById('userMsg');
        const chat = document.getElementById('chat-area');
        if(input.value.trim() === "") return;

        chat.innerHTML += `<div class="bubble" style="align-self: flex-end; background: #dcf8c6; border-bottom-right-radius: 2px;">${input.value}</div>`;
        
        db.collection("messages").add({
            content: input.value,
            timestamp: firebase.firestore.FieldValue.serverTimestamp()
        });

        input.value = "";
        window.scrollTo(0, document.body.scrollHeight);
    }
</script>

</body>
</html>
