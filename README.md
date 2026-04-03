<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<title>Site web 2.0</title>

<style>
body {
    margin: 0;
    height: 100vh;
    background: linear-gradient(135deg, #64CDE8, #4facfe);
    font-family: Arial, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
}

.container {
    text-align: center;
}

h1 {
    color: white;
    margin-bottom: 40px;
    font-size: 40px;
}

button {
    display: block;
    margin: 15px auto;
    padding: 15px 40px;
    font-size: 18px;
    border: none;
    border-radius: 30px;
    background: white;
    cursor: pointer;
    transition: 0.3s;
    box-shadow: 0 5px 15px rgba(0,0,0,0.2);
}

button:hover {
    transform: translateY(-5px) scale(1.05);
    background: #f1f1f1;
    box-shadow: 0 10px 25px rgba(0,0,0,0.3);
}
</style>

</head>

<body>

<div class="container">
    <h1>🚀 Site web 2.0</h1>
    <button onclick="ouvrir('yt')">🎬 YT ksp1080p</button>
    <button onclick="ouvrir('meteo')">🌦️ Météo France</button>
    <button onclick="ouvrir('insta')">📸 Instagram</button>
</div>

<script>
function ouvrir(site) {
    if (site === "yt") {
        window.open("https://www.youtube.com/@theo_ksp5546");
    }
    else if (site === "meteo") {
        window.open("https://meteofrance.com");
    }
    else if (site === "insta") {
        window.open("https://www.instagram.com/ksp1080p/");
    }
}
</script>

</body>
</html>
