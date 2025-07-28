<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>site-wed-2.0</title>
  <style>
    body {
      background-color: #64CDE8;
      font-family: Courier, monospace;
      text-align: center;
      padding: 50px 20px;
      margin: 0;
    }
    h1 {
      font-size: 32px;
      margin-bottom: 30px;
      color: #333;
    }
    .btn {
      display: block;
      width: 90%;
      max-width: 400px;
      margin: 10px auto;
      padding: 15px;
      font-size: 20px;
      background-color: white;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }
    .btn:hover {
      background-color: #e0e0e0;
    }
    .bottom {
      position: fixed;
      bottom: 20px;
      left: 50%;
      transform: translateX(-50%);
      width: 90%;
      max-width: 400px;
    }
    .theo-btn {
      color: #0C19CF;
      font-weight: bold;
    }
  </style>
</head>
<body>

  <h1>Bienvenue</h1>

  <button class="btn" onclick="openLink('https://www.youtube.com/@FuzeIII')">Chaîne Fuze</button>
  <button class="btn" onclick="openLink('https://www.youtube.com/results?search_query=ksp+fr')">Rechercher KSP FR</button>
  <button class="btn" onclick="openLink('https://www.youtube.com/')">Accueil YouTube</button>
  <button class="btn" onclick="openLink('https://meteofrance.com/')">Météo France</button>

  <div class="bottom">
    <button class="btn theo-btn" onclick="openLink('https://www.youtube.com/@theo_ksp5546')">
      Chaîne Theo KSP
    </button>
  </div>

  <script>
    function openLink(url) {
      window.open(url, '_blank');
    }
  </script>

</body>
</html>
