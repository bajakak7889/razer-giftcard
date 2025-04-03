<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Razer Gold Gift Card Generator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 50px;
            background-color: #222;
            color: white;
        }
        #loader {
            display: none;
            font-size: 20px;
            margin-top: 20px;
        }
        #result {
            display: none;
            font-size: 24px;
            margin-top: 20px;
            color: red;
            font-weight: bold;
        }
        .button {
            background-color: #00ff00;
            color: black;
            padding: 10px 20px;
            font-size: 18px;
            border: none;
            cursor: pointer;
        }
        .button:hover {
            background-color: #00cc00;
        }
    </style>
</head>
<body>
    <h1>Razer Gold Gift Card Generator</h1>
    <p>Klicke auf den Button, um deine kostenlose $25 Razer Gold Karte zu generieren!</p>
    <button class="button" onclick="startGeneration()">Jetzt Generieren</button>
    <p id="loader">Generiere Code... Bitte warten...</p>
    <p id="result"></p>
    
    <script>
        function startGeneration() {
            document.getElementById('loader').style.display = 'block';
            setTimeout(() => {
                document.getElementById('loader').style.display = 'none';
                document.getElementById('result').style.display = 'block';
                document.getElementById('result').innerText = 'Leider ist ein Fehler aufgetreten. Bitte versuche es später noch einmal.';
            }, 3000);
        }
    </script>
</body>
</html>
