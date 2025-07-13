# taller-formativo3
pagina web con html ,boostrap y css
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Informe Lighthouse - Bancos de Chile</title>

  <!-- Bootstrap -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" />
  <!-- Animate.css -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css"/>
  <!-- AOS -->
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/aos@2.3.4/dist/aos.css" />
  <!-- Custom CSS -->
  <link rel="stylesheet" href="styles.css" />
</head>
<body>

<!-- Navbar -->
<nav class="navbar navbar-expand-lg navbar-dark bg-dark sticky-top shadow">
  <div class="container">
    <a class="navbar-brand" href="#">Análisis Web</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#nav">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="nav">
      <ul class="navbar-nav ms-auto">
        <li class="nav-item"><a class="nav-link" href="#inicio">Inicio</a></li>
        <li class="nav-item"><a class="nav-link" href="#falabella">Banco Falabella</a></li>
        <li class="nav-item"><a class="nav-link" href="#estado">BancoEstado</a></li>
        <li class="nav-item"><a class="nav-link" href="#comparacion">Comparación</a></li>
      </ul>
    </div>
  </div>
</nav>

<!-- Hero -->
<header class="hero d-flex align-items-center text-white text-center" id="inicio">
  <div class="container">
    <h1 class="display-4 animate__animated animate__fadeInDown">Informe de Métricas Web</h1>
    <p class="lead animate__animated animate__fadeInUp">Evaluación con Google Lighthouse: Banco Falabella vs BancoEstado</p>
  </div>
</header>

<!-- Sección Banco Falabella -->
<section class="py-5" id="falabella">
  <div class="container" data-aos="fade-up">
    <h2 class="text-center mb-4">Banco Falabella</h2>
    <p><strong>URL evaluada:</strong> www.bancofalabella.cl</p>
    <div class="row">
      <div class="col-md-6">
        <ul>
          <li><strong>Performance:</strong> 41</li>
          <li><strong>Accesibilidad:</strong> 89</li>
          <li><strong>Buenas Prácticas:</strong> 80</li>
          <li><strong>SEO:</strong> 91</li>
        </ul>
      </div>
      <div class="col-md-6">
        <p>El sitio posee un diseño visual moderno pero tiene bajo rendimiento en velocidad, probablemente por el uso de imágenes grandes y scripts sin optimizar.</p>
      </div>
    </div>
  </div>
</section>

<!-- Sección BancoEstado -->
<section class="py-5 bg-light" id="estado">
  <div class="container" data-aos="fade-up">
    <h2 class="text-center mb-4">BancoEstado</h2>
    <p><strong>URL evaluada:</strong> www.bancoestado.cl</p>
    <div class="row">
      <div class="col-md-6">
        <ul>
          <li><strong>Performance:</strong> 60</li>
          <li><strong>Accesibilidad:</strong> 92</li>
          <li><strong>Buenas Prácticas:</strong> 94</li>
          <li><strong>SEO:</strong> 90</li>
        </ul>
      </div>
      <div class="col-md-6">
        <p>BancoEstado tiene mejor puntuación técnica general, con buena estructura semántica y optimización para SEO y accesibilidad.</p>
      </div>
    </div>
  </div>
</section>

<!-- Sección Comparación -->
<section class="py-5" id="comparacion">
  <div class="container" data-aos="fade-up">
    <h2 class="text-center mb-4">Comparación General</h2>
    <div class="table-responsive">
      <table class="table table-bordered text-center">
        <thead class="table-dark">
          <tr>
            <th>Métrica</th>
            <th>Banco Falabella</th>
            <th>BancoEstado</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td><strong>Performance</strong></td>
            <td>41</td>
            <td>60</td>
          </tr>
          <tr>
            <td><strong>Accesibilidad</strong></td>
            <td>89</td>
            <td>92</td>
          </tr>
          <tr>
            <td><strong>Buenas Prácticas</strong></td>
            <td>80</td>
            <td>94</td>
          </tr>
          <tr>
            <td><strong>SEO</strong></td>
            <td>91</td>
            <td>90</td>
          </tr>
        </tbody>
      </table>
    </div>
    <p class="text-center">Ambos sitios son funcionales, pero BancoEstado está mejor optimizado técnicamente, mientras que Banco Falabella destaca por el diseño visual.</p>
  </div>
</section>

<!-- Footer -->
<footer class="bg-dark text-white text-center py-3">
</footer>

<!-- Scripts -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/aos@2.3.4/dist/aos.js"></script>
<script>
  AOS.init();
</script>
</body>
</html>
body {
  scroll-behavior: smooth;
  font-family: 'Segoe UI', sans-serif;
}

.hero {
  background: linear-gradient(to bottom, rgba(0, 0, 0, 0.7), rgba(60, 60, 60, 0.7)),
              url('https://images.unsplash.com/photo-1542744095-fcf48d80b0fd') center/cover no-repeat;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

.nav-link:hover {
  color: #ffc107 !important;
  transition: 0.3s;
}

h1, h2 {
  font-weight: bold;
}

ul {
  list-style: none;
  padding-left: 0;
}

ul li::before {
  content: "✔️ ";
  color: green;
}
