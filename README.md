<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <title>Site Web 2.0</title>
    <style>
        body {
            background-color: #64CDE8;
            font-family: 'Courier New', Courier, monospace;
            text-align: center;
            padding: 20px;
        }
        button {
            font-size: 20px;
            margin: 10px;
            padding: 10px 20px;
            background-color: white;
            border: none;
            cursor: pointer;
            border-radius: 8px;
            transition: background-color 0.3s;
        }
        button:hover {
            background-color: #e0e0e0;
        }
        #imageContainer img {
            max-width: 1000px;
            max-height: 600px;
            margin-top: 20px;
            border-radius: 10px;
        }
    </style>
</head>
<body>
    <h1>Site Web 2.0</h1>
    <button onclick="openLink('https://www.youtube.com/@FuzeIII')">Ouvrir YouTube Fuze</button>
    <button onclick="openLink('https://www.youtube.com/results?search_query=ksp+fr')">KSP FR</button>
    <button onclick="openLink('https://www.youtube.com/')">Accueil YouTube</button>
    <button onclick="openLink('https://meteofrance.com/')">Météo France</button>
    <button onclick="openLink('https://www.youtube.com/@theo_ksp5546')">YouTube Theo KSP</button>
    <br><br>
    <button onclick="showImage()">Afficher l'image</button>
    <button onclick="hideImage()">Cacher l'image</button>
    <div id="imageContainer"></div>
    <script>
        function openLink(url) {
            window.open(url, '_blank');
        }
        function showImage() {
            const container = document.getElementById("imageContainer");
            if (!document.getElementById("mainImage")) {
                const img = document.createElement("img");
                img.src = "101_1296_edited.jpg"; // Assure-toi que l'image est dans le même dossier
                img.id = "mainImage";
                container.appendChild(img);
            }
        }
        function hideImage() {
            const img = document.getElementById("mainImage");
            if (img) {
                img.remove();
            }
        }
    </script>

</body>
</html>
