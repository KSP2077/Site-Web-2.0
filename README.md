<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <title>Site Web 2.0</title>

    <!-- ===== CSS ===== -->
    <style>
        body {
            background-color: #64CDE8;
            font-family: Courier, monospace;
            text-align: center;
            margin: 0;
            padding: 20px;
        }

        h1 {
            margin-bottom: 5px;
        }

        .bonne-annee {
            font-size: 28px;
            font-weight: bold;
            color: white;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px #00000055;
        }

        .buttons {
            margin: 15px 0;
        }

        button {
            font-size: 16px;
            padding: 10px 15px;
            margin: 5px;
            background-color: white;
            border: none;
            border-radius: 6px;
            cursor: pointer;
        }

        button:hover {
            background-color: #e0e0e0;
        }

        .images {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }

        .images img {
            max-width: 500px;
            max-height: 500px;
            display: none;
            border-radius: 8px;
        }
    </style>
</head>

<body>

<h1>Site Web 2.0</h1>
<div class="bonne-annee">🎆 Bonne année 2026 🎆</div>

<!-- ===== Boutons Web ===== -->
<div class="buttons">
    <button onclick="openUrl('https://www.youtube.com/@FuzeIII')">Fuze III</button>
    <button onclick="openUrl('https://www.youtube.com/results?search_query=ksp+fr')">KSP FR</button>
    <button onclick="openUrl('https://www.youtube.com/')">YouTube</button>
    <button onclick="openUrl('https://meteofrance.com/')">Météo France</button>
    <button onclick="openUrl('https://discord.com/')">Discord</button>
    <button onclick="openUrl('https://steamcommunity.com/')">Steam</button>
</div>

<!-- ===== Boutons Images ===== -->
<div class="buttons">
    <button onclick="changerImages()">Changer les images</button>
    <button onclick="cacherImages()">Cacher les images</button>
</div>

<!-- ===== Zone Images ===== -->
<div class="images">
    <img id="img1">
    <img id="img2">
</div>

<!-- ===== JavaScript ===== -->
<script>
    const images1 = ["101_1295_edited.jpg", "101_1296_edited.jpg"];
    const images2 = ["101_1349_edited.jpg", "101_1350_edited.jpg"];
    let index = 0;

    function openUrl(url) {
        window.open(url, "_blank");
    }

    function changerImages() {
        const img1 = document.getElementById("img1");
        const img2 = document.getElementById("img2");

        img1.src = images1[index % images1.length];
        img2.src = images2[index % images2.length];

        img1.style.display = "block";
        img2.style.display = "block";

        index++;
    }

    function cacherImages() {
        document.getElementById("img1").style.display = "none";
        document.getElementById("img2").style.display = "none";
    }
</script>

</body>
</html>


