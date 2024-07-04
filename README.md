<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>10 IMAGENES QUE ME HACEN FELIZ</title>
<style>
body {
  font-family: Arial, sans-serif;
  background: linear-gradient(135deg, #8e24aa, #f06292);
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  margin: 0;
}

.carousel-container {
  width: 80%;
  overflow-x: hidden;
  background-color: rgba(255, 255, 255, 0.8);
  border-radius: 10px;
  box-shadow: 0 0 20px rgba(0, 0, 0, 0.2);
}

.carousel {
  display: flex;
  flex-wrap: nowrap;
  padding: 20px;
}

.box {
  width: 300px;
  height: 300px; /* Altura ajustada para mantener la proporción */
  background-color: #fff;
  border: 2px solid #ccc;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  margin-right: 20px;
  display: flex;
  flex-direction: column;
  position: relative;
  overflow: hidden; /* Para asegurar que las imágenes no sobresalgan */
}

.image-container {
  position: absolute;
  top: 10px;
  right: 10px;
  width: 50px;
  height: 50px;
}

.image-container img {
  width: 100%;
  height: 100%;
  object-fit: cover; /* Ajusta la imagen para cubrir todo el contenedor */
  border-radius: 50%;
}

.content {
  flex: 1;
  padding-top: 60px;
}

h2 {
  font-size: 20px;
  margin-bottom: 10px;
}

p {
  font-size: 14px;
  line-height: 1.6;
}
</style>
</head>
<body>

<div class="carousel-container">
  <div class="carousel">
    <!-- Primer recuadro -->
    <div class="box">
      <div class="image-container">
        <img src="1.jpeg" alt="Imagen 1">
      </div>
      <div class="content">
        <h2>1</h2>
        <p>Eres mi sol en días nublados.</p>
      </div>
    </div>

    <!-- Segundo recuadro -->
  <div class="box">
      <div class="image-container">
        <img src="2.jpeg" alt="Imagen 2">
      </div>
      <div class="content">
        <h2>2</h2>
        <p>Cada momento contigo es un tesoro.</p>
      </div>
   </div>

    <!-- Tercer recuadro -->
  <div class="box">
      <div class="image-container">
        <img src="3.jpeg" alt="Imagen 3">
      </div>
      <div class="content">
        <h2>3</h2>
        <p>Tu sonrisa ilumina todo a mi alrededor.</p>
      </div>
   </div>

    <!-- Cuarto recuadro -->
  <div class="box">
      <div class="image-container">
        <img src="4.jpeg" alt="Imagen 4">
      </div>
      <div class="content">
        <h2>4</h2>
        <p>Contigo, el mundo se vuelve un lugar más hermoso.</p>
      </div>
  </div>

    <!-- Quinto recuadro -->
  <div class="box">
      <div class="image-container">
        <img src="5.jpeg" alt="Imagen 5">
      </div>
      <div class="content">
        <h2>5</h2>
        <p>En tus ojos encuentro mi paz.</p>
      </div>
   </div>

    <!-- Sexto recuadro -->
   <div class="box">
      <div class="image-container">
        <img src="6.jpeg" alt="Imagen 6">
      </div>
      <div class="content">
        <h2>6</h2>
        <p>Eres mi mejor compañía, mi mejor historia.</p>
      </div>
  </div>

    <!-- Séptimo recuadro -->
  <div class="box">
      <div class="image-container">
        <img src="7.jpeg" alt="Imagen 7">
      </div>
      <div class="content">
        <h2>7</h2>
        <p>Contigo, cada día es una aventura que quiero vivir.</p>
      </div>
  </div>

    <!-- Octavo recuadro -->
   <div class="box">
      <div class="image-container">
        <img src="8.jpeg" alt="Imagen 8">
      </div>
      <div class="content">
        <h2>8</h2>
        <p>Tu risa es la melodía más bonita que he escuchado.</p>
      </div>
   </div>

    <!-- Noveno recuadro -->
  <div class="box">
      <div class="image-container">
        <img src="9.jpeg" alt="Imagen 9">
      </div>
      <div class="content">
        <h2>9</h2>
        <p>Amarte es la mejor decisión que he tomado.</p>
      </div>
  </div>

    <!-- Décimo recuadro -->
   <div class="box">
      <div class="image-container">
        <img src="10.jpeg" alt="Imagen 10">
      </div>
      <div class="content">
        <h2>10</h2>
        <p>Eres mi lugar favorito en este mundo.</p>
      </div>
    </div>
  </div>
</div>

<button class="prev-button">Anterior</button>
<button class="next-button">Siguiente</button>

<script>
const carousel = document.querySelector('.carousel-container');
const prevButton = document.createElement('button');
prevButton.textContent = 'Anterior';
prevButton.classList.add('prev-button');

const nextButton = document.createElement('button');
nextButton.textContent = 'Siguiente';
nextButton.classList.add('next-button');

carousel.insertAdjacentElement('beforebegin', prevButton);
carousel.insertAdjacentElement('afterend', nextButton);

function slideLeft() {
  carousel.scrollLeft -= carousel.offsetWidth;
}

function slideRight() {
  carousel.scrollLeft += carousel.offsetWidth;
}

prevButton.addEventListener('click', slideLeft);
nextButton.addEventListener('click', slideRight);
</script>

</body>
</html>


