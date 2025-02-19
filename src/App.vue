<template>
  <head>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  </head>

  <div id="app">
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
      <div class="container">
        <a class="navbar-brand" href="#">My Portafolio</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
          <ul class="navbar-nav">
            <li class="nav-item">
              <a class="nav-link" href="#home">Home</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#about">About Me</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#gallery">Gallery</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#recommendations">Recommendations</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#contact">Contact</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
    <div class="container mt-4">
      <section id="home" class="text-center">
        <h1>Bienvenido a Mi Portafolio</h1>
        <p>Hola, Soy Leslie Baez, soy una amante de la animacion y aprendiz del diseño de paginas.</p>
      </section>
      <section id="about" class="text-center">
  <div class="row align-items-center">
    <div class="col-md-6">
      <h2>About Me</h2>
      <p>Estoy estudiando la carrera de Entornos Virtuales y Negocios Digitales en la Universidad Tecnológica de la Riviera Maya.</p>
    </div>
    <div class="col-md-6">
      <img src="../src/assets/yo.jpg" class="img-fluid rounded shadow" alt="Leslie Baez">
    </div>
  </div>
</section>
      <section id="gallery" class="text-center">
        <h2>Gallery</h2>
        <div class="gallery-container">
          <div class="row justify-content-center">
            <div class="col-md-4 d-flex flex-column align-items-center gallery-item">
              <img src="../src/assets/MI CV.png" class="img-fluid rounded shadow mb-2" alt="Project 1">
              <p>Project 1: Este es un Curriculum Vitae hecho con Html, CSS y un poco de Java Script.</p>
            </div>
            <div class="col-md-4 d-flex flex-column align-items-center gallery-item">
              <img src="../src/assets/TASK LIST.png" class="img-fluid rounded shadow mb-2" alt="Project 2">
              <p>Project 2: Es una Lista de Tareas donde te permite guardar todas tus actividades y ponerles fechas de entrega esta hecho de la misma manera con Html, CSS y Java Script, De igual manera puedes ver si se acompletaron las tareas o si se vencieron.</p>
            </div>
            <div class="col-md-4 d-flex flex-column align-items-center gallery-item">
              <img src="../src/assets/WK_MUSIC.png" class="img-fluid rounded shadow mb-2" alt="Project 3">
              <p>Project 3: Esta es una pagina de carga para un proyecto de la escuela compuesto con algunos compañeros, yo fui la que hizo la pagina de carga y aun se esta desarollando la pagina. </p>
            </div>
          </div>
        </div>
      </section>
      <section id="recommendations" class="text-center gallery-container mb-5">
        <h2>Recommendations</h2>
        <form class="mx-auto" style="max-width: 500px;">
          <div class="mb-3">
            <label for="rec-name" class="form-label">Your Name</label>
            <input type="text" class="form-control" id="rec-name" placeholder="Your Name">
          </div>
          <div class="mb-3">
            <label for="rec-message" class="form-label">Recommendation</label>
            <textarea class="form-control" id="rec-message" rows="3" placeholder="Your Recommendation"></textarea>
          </div>
          <button type="submit" class="btn btn-primary">Submit</button>
        </form>
      </section>
      <section id="contact" class="text-center contact-section">
        <h2>Contact</h2>
        <form class="mx-auto" style="max-width: 500px;">
          <div class="mb-3">
            <label for="name" class="form-label">Name</label>
            <input type="text" class="form-control" id="name" placeholder="Your Name">
          </div>
          <div class="mb-3">
            <label for="email" class="form-label">Email</label>
            <input type="email" class="form-control" id="email" placeholder="Your Email">
          </div>
          <div class="mb-3">
            <label for="message" class="form-label">Message</label>
            <textarea class="form-control" id="message" rows="3" placeholder="Your Message"></textarea>
          </div>
          <button type="submit" class="btn btn-primary">Send</button>
        </form>
      </section>
      <footer class="text-center mt-4">
  <p>Follow me on:</p>
  <a href="https://www.instagram.com/leslie._.bp/" class="btn btn-outline-primary mx-2">
    <i class="fab fa-instagram"></i>
  </a>
  <a href="lelo baez#5963" class="btn btn-outline-secondary mx-2">
    <i class="fab fa-discord"></i>
  </a>
</footer>

    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
};
</script>

<style>
body {
  font-family: Arial, sans-serif;
  background: linear-gradient(to bottom, #0a2a43, #1f3b4d, #3e4a4f, #704c42, #914e35);
  color: #fff;
}

section {
  padding: 50px 0;
}

.gallery-container, .contact-section, .recommendations-section {
  background-color: rgba(255, 255, 255, 0.1);
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
}

.gallery-item {
  text-align: center;
  padding: 10px;
}

img {
  max-width: 100%;
  height: auto;
  margin-bottom: 10px;
  border: 2px solid #ddd;
}

p {
  text-align: center;
  font-size: 1.1rem;
  color: #f8f9fa;
}

footer {
  padding: 20px;
  background: rgba(0, 0, 0, 0.5);
}

/* Ajuste de la barra de Follow Me */
footer {
  padding: 15px 0;
}

footer a {
  padding: 8px 15px;
  font-size: 16px;
}

/* Hacer que la barra se ajuste al ancho de la pantalla */
footer a {
  display: inline-block;
  width: auto;
}

@media (max-width: 768px) {
  .container {
    padding: 20px;
  }

  img {
    max-width: 90%;
  }

  form {
    max-width: 90%;
  }

  footer a {
    font-size: 14px;
    padding: 5px 10px;
  }
}
</style>
