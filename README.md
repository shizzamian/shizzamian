<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ramadan Date Request</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f8f9fa;
            margin: 50px;
        }
        h1 {
            color: #2c3e50;
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            font-size: 18px;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            cursor: pointer;
            border-radius: 8px;
        }
        #yes {
            background-color: #28a745;
            color: white;
        }
        #no {
            background-color: #dc3545;
            color: white;
            position: absolute;
        }
    </style>
</head>
<body>
    <h1>Will you be my date this Ramadan? 🌙</h1>
    <div class="buttons">
        <button id="yes">Yes ✅</button>
        <button id="no" onmouseover="moveNo()">No ❌</button>
    </div>
    <script>
        document.getElementById("yes").addEventListener("click", function() {
            alert("Yay, Habibi! Please retain this as a voucher for biscoff pudding 🌙✨");
        });
        
        function moveNo() {
            let button = document.getElementById('no');
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 100);
            button.style.left = `${x}px`;
            button.style.top = `${y}px`;
        }
    </script>
</body>
</html>
