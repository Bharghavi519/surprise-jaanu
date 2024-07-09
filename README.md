<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday!</title>
    <style>
        body {
            background-color: #ffecd2;
            text-align: center;
            font-family: 'Comic Sans MS', 'Comic Sans', cursive;
            color: #ff69b4;
            overflow: hidden;
        }
        .container {
            margin-top: 50px;
        }
        .message {
            font-size: 2.5em;
            margin-bottom: 20px;
            animation: fadeIn 2s ease-in-out;
        }
        .cake {
            font-size: 5em;
            animation: bounce 2s infinite;
        }
        .balloons {
            position: absolute;
            bottom: -100px;
            width: 100%;
            animation: rise 5s infinite;
        }
        .balloon {
            font-size: 2em;
            position: absolute;
            bottom: 0;
        }
        .balloon:nth-child(1) { left: 20%; animation-delay: 0s; }
        .balloon:nth-child(2) { left: 40%; animation-delay: 1s; }
        .balloon:nth-child(3) { left: 60%; animation-delay: 2s; }
        .balloon:nth-child(4) { left: 80%; animation-delay: 3s; }

        .hidden-content {
            display: none;
            margin-top: 20px;
            animation: fadeIn 2s ease-in-out;
        }
        .hidden-content img {
            width: 300px;
            height: auto;
            border: 5px solid #ff69b4;
            border-radius: 15px;
            margin: 10px;
        }
        .hidden-content .extra-message {
            font-size: 1.5em;
            margin-top: 20px;
            color: #ff69b4;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% { transform: translateY(0); }
            40% { transform: translateY(-30px); }
            60% { transform: translateY(-15px); }
        }

        @keyframes rise {
            0% { bottom: -100px; }
            100% { bottom: 110%; }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="message">Happy Birthday, [Friend's Name]!</div>
        <div class="cake">🎂</div>
        <p>Hope you have a fantastic day filled with joy and surprises!</p>
        <button onclick="showSurprise()">Click for a Surprise!</button>
    </div>
    <div class="balloons">
        <div class="balloon">🎈</div>
        <div class="balloon">🎈</div>
        <div class="balloon">🎈</div>
        <div class="balloon">🎈</div>
    </div>
    <div class="hidden-content" id="hiddenContent">
        <img src="C:\Users\91003108\OneDrive - bioMerieux\Pictures\Screenshots" alt="Picture 1">
        <img src="C:\Users\91003108\OneDrive - bioMerieux\Pictures\Screenshots" alt="Picture 2">
        <div class="extra-message">You're the best! Happy Birthday again!</div>
    </div>

    <script>
        function showSurprise() {
            document.getElementById('hiddenContent').style.display = 'block';
        }
    </script>
</body>
</html>
