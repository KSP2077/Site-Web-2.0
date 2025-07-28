# Site-Web-2.0
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>ksp1080p</title>
  <style>
    body {
      background-color: #64CDE8;
      font-family: Courier, monospace;
      text-align: center;
      padding-top: 50px;
    }
    h1 {
      color: #222;
    }
    .btn {
      font-size: 25px;
      font-family: Courier, monospace;
      padding: 15px 30px;
      margin: 20px;
      background-color: white;
      color: black;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }
    .btn:hover {
      background-color: #eaeaea;
    }
    .btn-blue {
      color: #0C19CF;
    }
  </style>
</head>
<body>

  <h1>Bonjour</h1>

  <button class="btn" id="btn-fuze">Ouvre Youtube Fuze</button><br>
  <button class="btn" id="btn-ksp">KSP FR</button><br>
  <button class="btn" id="btn-home">Ouvrir Youtube Accueil</button><br>
  <button class="btn btn-blue" id="btn-theo">Ouvrir Youtube KSP1080p</button>

  <script>
    document.getElementById("btn-fuze").onclick = function() {
      window.open("https://www.youtube.com/@FuzeIII", "_blank");
    };

    document.getElementById("btn-ksp").onclick = function() {
      window.open("https://www.youtube.com/results?search_query=ksp+fr", "_blank");
    };

    document.getElementById("btn-home").onclick = function() {
      window.open("https://www.youtube.com/", "_blank");
    };

    document.getElementById("btn-theo").onclick = function() {
      window.open("https://www.youtube.com/@theo_ksp5546", "_blank");
    };
  </script>

</body>
</html>
# Site-Web-2.0<button id="monBouton">Clique moi</button>

<script>
  document.getElementById("monBouton").onclick = function() {
    alert("Bouton cliqué !");
  };
</script>
