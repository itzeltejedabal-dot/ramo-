# ramo-
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ramo Hot Wheels</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background: #fdf6f9;
    }
    h1 {
      margin-top: 20px;
      color: #d63384;
    }
    .ramo {
      display: flex;
      flex-direction: column;
      align-items: center;
      margin-top: 30px;
      gap: 15px;
    }
    .fila {
      display: flex;
      justify-content: center;
      gap: 15px;
    }
    .carrito {
      width: 150px;
      cursor: pointer;
      border-radius: 12px;
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .carrito:hover {
      transform: scale(1.1);
      box-shadow: 0px 8px 15px rgba(0,0,0,0.2);
    }
    #frase {
      margin-top: 30px;
      font-size: 1.3em;
      font-weight: bold;
      color: #444;
      padding: 15px;
      border-radius: 10px;
      background: #fff;
      display: inline-block;
      box-shadow: 0px 4px 10px rgba(0,0,0,0.1);
    }
  </style>
</head>
<body>
  <h1>🚗🌸 Ramo de Hot Wheels</h1>
  <p>Haz clic en un carrito para ver su mensaje especial.</p>

  <div class="ramo">
    <div class="fila">
      <img src="https://m.media-amazon.com/images/I/81sYJh8e5nL._AC_SL1500_.jpg" 
           class="carrito" onclick="mostrarFrase(0)">
    </div>
    <div class="fila">
      <img src="https://m.media-amazon.com/images/I/91ibqBPdQIL._AC_SL1500_.jpg" 
           class="carrito" onclick="mostrarFrase(1)">
      <img src="https://m.media-amazon.com/images/I/81OmvCUEC6L._AC_SL1500_.jpg" 
           class="carrito" onclick="mostrarFrase(2)">
    </div>
    <div class="fila">
      <img src="https://m.media-amazon.com/images/I/91bTft3wlgL._AC_SL1500_.jpg" 
           class="carrito" onclick="mostrarFrase(3)">
      <img src="https://m.media-amazon.com/images/I/91fxa4oaTRL._AC_SL1500_.jpg" 
           class="carrito" onclick="mostrarFrase(4)">
      <img src="https://m.media-amazon.com/images/I/81SK8z4y7oL._AC_SL1500_.jpg" 
           class="carrito" onclick="mostrarFrase(5)">
    </div>
  </div>

  <div id="frase"></div>

  <script>
    const frases = [
      "Gracias por enseñarme el amor verdadero ❤️",
      "Eres la luz de mis ojos ✨",
      "Quiero estar contigo por el resto de mi vida ❤️‍🩹",
      "Mi pensamiento favorito eres tú día a día 💭",
      "Te amo a pasitos de hurón 🐹🤍",
      "Eres lo mejor que me ha pasado y no lo cambiaría por nada 💖"
    ];

    function mostrarFrase(indice) {
      document.getElementById("frase").innerText = frases[indice];
    }
  </script>
</body>
</html>
