<!DOCTYPE html>
<html>
<head>
    <title>Warzone Drop Spinner</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://telegram.org/js/telegram-web-app.js"></script>
    <style>
        body { background: #1a1a1a; color: white; text-align: center; font-family: sans-serif; padding: 20px; }
        #spinner-box { width: 300px; height: 300px; border: 5px solid #00ff00; border-radius: 50%; margin: 20px auto; position: relative; display: flex; align-items: center; justify-content: center; font-size: 24px; font-weight: bold; overflow: hidden; background: #333; }
        button { background: #00ff00; color: black; border: none; padding: 15px 30px; font-size: 20px; font-weight: bold; border-radius: 10px; cursor: pointer; }
        button:active { transform: scale(0.95); }
    </style>
</head>
<body>
    <h1>WARZONE DROP SPINNER</h1>
    <div id="spinner-box">?</div>
    <button onclick="spin()">SPIN THE WHEEL</button>

    <script>
        const spots = ["Superstore", "Military Base", "Storage Town", "Prison", "Hospital", "Airport", "Promenade"];
        function spin() {
            const box = document.getElementById('spinner-box');
            box.style.color = "#00ff00";
            box.innerText = "SPINNING...";
            setTimeout(() => {
                const randomSpot = spots[Math.floor(Math.random() * spots.length)];
                box.innerText = randomSpot;
                box.style.color = "white";
            }, 800);
        }
        // Tells Telegram the app is ready
        window.Telegram.WebApp.ready();
    </script>
</body>
</html>
