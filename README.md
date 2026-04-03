<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <title>Site web 2.0</title>
    <style>
        body {
            background-color: #64CDE8;
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 100px;
        }
        h1 {
            color: white;
            margin-bottom: 40px;
        }
        button {
            display: block;
            margin: 15px auto;
            padding: 15px 30px;
            font-size: 18px;
            border: none;
            border-radius: 10px;
            background-color: white;
            cursor: pointer;
            transition: 0.3s;
        }
        button:hover {
            background-color: #ddd;
            transform: scale(1.05);
        }
    </style>
</head>

<body>
    <h1>Site web 2.0</h1>
    <button onclick="ouvrirYT()">YT ksp1080p</button>
    <button onclick="ouvrirMeteo()">Météo France</button>
    <button onclick="ouvrirInsta()">Instagram</button>
    <script>
        function ouvrirYT() {
            window.open("https://www.youtube.com/@theo_ksp5546");
        }
        function ouvrirMeteo() {
            window.open("https://meteofrance.com");
        }
        function ouvrirInsta() {
            window.open("https://www.instagram.com/ksp1080p/");
        }
    </script>

</body>
</html>
