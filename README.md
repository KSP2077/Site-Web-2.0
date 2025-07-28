<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Site Web 2.0 - Image GitHub</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #64CDE8;
      color: #fff;
      display: flex;
      flex-direction: column;
      align-items: center;
      min-height: 100vh;
    }
    h1 {
      margin: 30px 0 20px;
      font-size: 2.5em;
    }
    .button-container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 15px;
      margin-bottom: 30px;
    }
    button {
      background-color: #ffffff;
      color: #333;
      border: none;
      padding: 12px 20px;
      font-size: 16px;
      border-radius: 8px;
      cursor: pointer;
      transition: transform 0.2s, background-color 0.3s;
    }
    button:hover {
      background-color: #dff4ff;
      transform: scale(1.05);
    }
    #image-container {
      display: none;
      margin-bottom: 30px;
      max-width: 1000px;
      width: 90%;
      animation: fadeIn 0.6s ease-out forwards;
    }
    #image-container img {
      width: 100%;
      height: auto;
      border-radius: 10px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.2);
    }
    #footer {
      margin-top: auto;
      padding: 20px;
    }
    #footer button {
      color: blue;
      background-color: #fff;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
    @media (max-width: 600px) {
      h1 {
        font-size: 1.8em;
      }
      button {
        font-size: 14px;
        padding: 10px 15px;
      }
    }
  </style>
</head>
<body>

  <h1>Bienvenue sur site-wed-2.0</h1>

  <div class="button-container">
    <button onclick="openLink('https://www.youtube.com/@FuzeIII')">YouTube Fuze</button>
    <button onclick="openLink('https://www.youtube.com/results?search_query=ksp+fr')">KSP FR</button>
    <button onclick="openLink('https://www.youtube.com/')">Accueil YouTube</button>
    <button onclick="openLink('https://meteofrance.com/')">Météo France</button>
    <button onclick="showImage()">Afficher l'image</button>
    <button onclick="hideImage()">Cacher l'image</button>
  </div>

  <div id="image-container">
    <img src="https://github.com/user-attachments/assets/9d335bf0-79e5-462a-99c3-6334d2edebcb" alt="Image GitHub">
  </div>

  <div id="footer">
    <button onclick="openLink('https://www.youtube.com/@theo_ksp5546')">YouTube Theo KSP</button>
  </div>

  <script>
    function openLink(url) {
      window.open(url, '_blank');
    }

    function showImage() {
      document.getElementById("image-container").style.display = "block";
    }

    function hideImage() {
      document.getElementById("image-container").style.display = "none";
    }
  </script>

</body>
</html>
