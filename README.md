<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<title>Site Web 2.0 – Bonne année 2026</title>

<style>
body {
    background-color: #64CDE8;
    font-family: Courier, monospace;
    text-align: center;
    margin: 0;
    padding: 20px;
}

h1 {
    color: white;
    font-size: 32px;
    text-shadow: 2px 2px 5px #00000055;
}

button {
    font-size: 16px;
    padding: 10px 15px;
    margin: 6px;
    background-color: white;
    border: none;
    border-radius: 6px;
    cursor: pointer;
}

button:hover {
    background-color: #e0e0e0;
}

#images {
    margin-top: 20px;
}

img {
    max-width: 900px;
    max-height: 500px;
    display: none;
    border-radius: 10px;
}
</style>
</head>

<body>

<h1>🎆 Bonne année 2026 🎆</h1>

<!-- Boutons liens -->
<div>
    <button onclick="openUrl('https://www.youtube.com/@FuzeIII')">YouTube Fuze</button>
    <button onclick="openUrl('https://www.youtube.com/results?search_query=ksp+fr')">KSP FR</button>
    <button onclick="openUrl('https://www.youtube.com')">Accueil YouTube</button>
    <button onclick="openUrl('https://meteofrance.com')">Météo France</button>
    <button onclick="openUrl('https://discord.com')">Discord</button>
    <button onclick="openUrl('https://steamcommunity.com')">Steam</button>
</div>

<!-- Boutons image -->
<div style="margin-top:15px;">
    <button onclick="showImage()">Afficher l'image</button>
    <button onclick="hideImage()">Cacher l'image</button>
</div>

<!-- Image -->
<div id="images">
    <img id="mainImage" src="101_1296_edited.jpg">
</div>

<script>
function openUrl(url) {
    window.open(url, "_blank");
}

function showImage() {
    document.getElementById("mainImage").style.display = "inline";
}

function hideImage() {
    document.getElementById("mainImage").style.display = "none";
}
</script>

</body>
</html>



