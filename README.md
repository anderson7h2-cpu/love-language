# love-language
codicia
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Para ti 💖</title>

  <style>
    body {
      margin: 0;
      padding: 0;
      background-color: #8b0000;
      color: white;
      font-family: Arial, sans-serif;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      position: relative;
      overflow: hidden;
    }

    #container {
      max-width: 500px;
      z-index: 2;
    }

    .button {
      margin-top: 25px;
      padding: 12px 25px;
      border: none;
      background-color: white;
      color: #8b0000;
      font-size: 18px;
      border-radius: 10px;
      cursor: pointer;
    }

    /* Imágenes laterales */
    .side {
      position: absolute;
      width: 120px;
      border-radius: 15px;
      opacity: 0.85;
    }

    /* Lado izquierdo */
    .left1 { left: 10px; top: 15%; }
    .left2 { left: 10px; top: 55%; }

    /* Lado derecho */
    .right1 { right: 10px; top: 10%; }
    .right2 { right: 10px; top: 40%; }
    .right3 { right: 10px; top: 70%; }
  </style>
</head>

<body>

  <!-- Izquierda -->
  <img src="UNO.jpeg" class="side left1">
  <img src="DOS.jpeg" class="side left2">

  <!-- Derecha -->
  <img src="TRES.jpeg" class="side right1">
  <img src="CUATRO.jpeg" class="side right2">
  <img src="MY LOVE.jpeg" class="side right3">

  <!-- Mensaje central -->
  <div id="container">
    <h1 id="message">Yo me casaré contigo 💍</h1>
    <button id="nextBtn" class="button">Siguiente</button>
  </div>

  <script>
    const messages = [
      "Yo me casaré contigo 💕",
      "En la iglesia del canton, porque yo te amo mucho ",
      "tu me tiene medio  loco con esos ojitos lendos" 
      "Eres lo más bonito que me ha pasado en la vida 💖"
    ];

    let index = 0;

    document.getElementById("nextBtn").addEventListener("click", function () {
      index++;
      if (index < messages.length) {
        document.getElementById("message").textContent = messages[index];
      } else {
        document.getElementById("message").textContent = "Te amo 💞";
        this.style.display = "none";
      }
    });
  </script>

</body>
</html>
