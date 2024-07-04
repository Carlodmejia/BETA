<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mensajes lindos</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f3f3f3;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }

    .container {
      text-align: center;
      background-color: #fff;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
      max-width: 600px;
      margin: auto;
    }

    h1 {
      color: #ff69b4;
    }

    p {
      margin: 20px 0;
      font-size: 18px;
    }

    .heart {
      cursor: pointer;
      transition: transform 0.3s ease-in-out;
      display: inline-block;
      user-select: none;
    }

    .heart:hover {
      transform: scale(1.2);
    }

    .heart:active {
      transform: scale(1.4);
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Mensajes lindos 💖</h1>
    <p id="message">Haz clic en el corazón para ver mensajes lindos...</p>
    <div id="heartContainer">
      <span class="heart" onclick="showMessage()">❤️</span>
    </div>
  </div>

  <script>
    let clickCount = 0;

    function showMessage() {
      clickCount++;

      if (clickCount <= 10) {
        const messages = [
          "Eres mi luz en los días oscuros.",
          "Tu sonrisa ilumina mi día.",
          "Cada momento contigo es un tesoro.",
          "No puedo imaginar mi vida sin ti.",
          "Eres mi mejor amigo y mi amor verdadero.",
          "Siempre estaré a tu lado, pase lo que pase.",
          "Contigo, cada día es una aventura.",
          "Tu amor hace que todo sea posible.",
          "Eres mi inspiración diaria.",
          "Te amo más de lo que las palabras pueden expresar."
        ];

        const randomIndex = Math.floor(Math.random() * messages.length);
        const message = messages[randomIndex];
        document.getElementById('message').textContent = message;
      } else {
        document.getElementById('message').textContent = "¡Te amo!";
        const heart = document.querySelector('.heart');
        heart.textContent = "💖";
        heart.style.fontSize = "3em";
        heart.style.transform = "scale(2)";
        heart.style.transition = "transform 0.5s ease-in-out";
        heart.setAttribute('onclick', '');
      }
    }
  </script>
</body>
</html>
