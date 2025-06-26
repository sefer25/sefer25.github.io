<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Weincose - Plataforma Educativa</title>
  <style>
    body { font-family: 'Segoe UI', sans-serif; margin: 0; padding: 0; background: #eef2f7; color: #333; }
    header, nav, footer { background: #1a3551; color: white; padding: 1em; }
    header { display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; }
    header h1, header p { margin: 0; }
    nav { display: flex; justify-content: center; align-items: center; flex-wrap: wrap; background-color: #294766; }
    nav .links { display: flex; gap: 15px; }
    nav .icons { display: flex; gap: 15px; align-items: center; }
    nav a { color: white; text-decoration: none; font-weight: bold; }
    .icon-img { width: 24px; height: 24px; filter: brightness(0) invert(1); transition: transform 0.3s ease; }
    .icon-img:hover { transform: scale(1.1); }
    .page { display: none; padding: 2em; max-width: 1000px; margin: auto; }
    .active { display: block; }
    .card { background: white; padding: 2em; border-radius: 15px; margin-bottom: 2em; box-shadow: 0 5px 15px rgba(0,0,0,0.1); }
    h2 { color: #102542; }
    ul { list-style-type: disc; margin-left: 20px; }
    .button { background: #1f7a8c; color: white; padding: 0.7em 1.2em; border: none; border-radius: 8px; cursor: pointer; margin-top: 1em; }
    .button:hover { background: #16697a; }
    .flex { display: flex; justify-content: space-between; align-items: center; gap: 2em; flex-wrap: wrap; }
    .flex .text { flex: 1 1 60%; }
    .flex .image { flex: 1 1 30%; text-align: center; }
    .flex .image img { max-width: 150px; height: auto; }
    .social-icons {
      position: absolute;
      right: 1em;
      bottom: 1em;
      display: flex;
      gap: 1em;
    }
    .social-icons img { width: 30px; height: 30px; filter: brightness(0) invert(1); transition: transform 0.3s ease; }
    .social-icons img:hover { transform: scale(1.1); }
    .image-row { display: flex; gap: 2em; flex-wrap: wrap; justify-content: center; margin-top: 2em; }
    .image-row img { border-radius: 10px; box-shadow: 0 4px 10px rgba(0,0,0,0.1); }
    .image-small { width: 200px; height: auto; }
    .image-large { width: 100%; max-width: 600px; height: auto; }
    .nav-buttons { display: flex; justify-content: space-around; margin-top: 2em; flex-wrap: wrap; gap: 1em; }
    .nav-buttons a { background: #1f7a8c; color: white; padding: 1em 2em; text-decoration: none; border-radius: 10px; font-weight: bold; box-shadow: 0 4px 10px rgba(0,0,0,0.1); transition: background 0.3s ease; }
    .nav-buttons a:hover { background: #16697a; }
    footer { position: relative; }
  </style>
</head>
<body>
  <header>
    <div>
      <h1>Weincose</h1>
      <p>Educación y Seguridad en Línea</p>
    </div>
    <div class="icons">
      <a href="#"><img src="https://cdn-icons-png.flaticon.com/512/3524/3524659.png" class="icon-img" alt="Carrito"></a>
      <a href="#"><img src="https://cdn-icons-png.flaticon.com/512/1077/1077114.png" class="icon-img" alt="Inicio de sesión"></a>
      <a href="#"><img src="logos/informacion.png" class="icon-img" alt="Ayuda"></a>
    </div>
  </header>
  <nav>
    <div class="links">
      <a href="#" onclick="showPage('pagina1')">Inicio</a>
      <a href="#" onclick="showPage('pagina2')">Paquetes</a>
      <a href="#" onclick="showPage('pagina3')">Blogs</a>
      <a href="#" onclick="showPage('pagina4')">Promociones</a>
      <a href="#" onclick="showPage('pagina5')">Programa</a>
    </div>
  </nav>

  <main>
    <div id="pagina1" class="page active">
      <div class="card">
        <div class="flex">
          <div class="text">
            <h2>Plataforma Weincose</h2>
            <p>Diseñada para ofrecer una experiencia de compra segura y educativa, con prevención de estafas y consejos útiles.</p>
            <ul>
              <li>Interfaz clara y accesible</li>
              <li>Catálogo de productos</li>
              <li>Foros y blogs informativos</li>
              <li>Gestión de compras y pagos desde dispositivos móviles y de escritorio</li>
            </ul>
          </div>
          <div class="image">
            <img src="weincose.png" alt="Logo Weincose">
          </div>
        </div>

        <div class="image-row">
          <img src="pequeño2.png" class="image-small" alt="Imagen pequeña">
          <img src="grande.png" class="image-large" alt="Imagen grande">
        </div>

        <div class="nav-buttons">
          <a href="#">Paquetes</P></a>
          <a href="#">Blogs</a>
          <a href="#">Información</a>
        </div>
      </div>
    </div>

    <div id="pagina2" class="page">
      <div class="card">
        <h2>Paquetes de Seguridad</h2>
        <ul>
          <li>Paquete Básico de Seguridad en Internet</li>
          <li>Paquete Avanzado de Ciberseguridad</li>
          <li>Paquete Especial para Padres y Educadores</li>
          <li>Paquete Completo de Comercio Electrónico Seguro</li>
          <li>Paquete Personalizado de Consultoría</li>
        </ul>
      </div>
    </div>

    <div id="pagina3" class="page">
      <div class="card">
        <h2>Consejos de Seguridad</h2>
        <ul>
          <li>Verifica la URL y busca el candado de seguridad</li>
          <li>Usa métodos de pago seguros (tarjeta, PayPal)</li>
          <li>Lee reseñas de otros compradores</li>
          <li>Usa contraseñas fuertes y únicas</li>
        </ul>
      </div>
    </div>

    <div id="pagina4" class="page">
      <div class="card">
        <h2>Promociones Disponibles</h2>
        <ul>
          <li>Clases de Introducción Gratuitas</li>
          <li>Webinars Educativos Gratuitos</li>
          <li>Acceso Gratuito a Módulos Educativos</li>
          <li>Descuento por Inscripción Temprana</li>
          <li>Oferta "Trae a un Amigo"</li>
        </ul>
      </div>
    </div>

    <div id="pagina5" class="page">
      <div class="card">
        <h2>Programa Educativo</h2>
        <p>Cursos y tutorías personalizadas en seguridad cibernética y comercio electrónico seguro.</p>
        <ul>
          <li>Desde conceptos básicos hasta avanzados</li>
          <li>Protección de datos personales y detección de malware</li>
          <li>Sesiones con expertos</li>
          <li>Tutoriales interactivos y módulos estructurados</li>
        </ul>
      </div>
    </div>
  </main>

  <footer>
    <p>&copy; 2025 Weincose - Protege tu mundo digital</p>
    <div class="social-icons">
      <a href="#"><img src="logos/facebook.png" alt="Facebook"></a>
      <a href="#"><img src="logos/x.png" alt="Twitter"></a>
      <a href="#"><img src="https://cdn-icons-png.flaticon.com/512/733/733614.png" alt="Instagram"></a>
    </div>
  </footer>

  <script>
    function showPage(id) {
      document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
      document.getElementById(id).classList.add('active');
    }
  </script>
</body>
</html>
