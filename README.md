# deforestacion

<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta http-equiv="X-UA-Compatible" content="ie=edge" />
  <title>La Deforestación</title>

  <style>
    :root {
      --bg-light: #2f302f;
      --text-color: #e7e3d8;
      --accent: #72ff26;
      --highlight: #b0926a;
      --blue-neon: #6b8c8e;
      --dark-accent: #3e3d36;
    }

    body {
      margin: 0;
      padding: 0;
      background-color: var(--bg-light);
      color: var(--text-color);
      font-family: 'Segoe UI', sans-serif;
      line-height: 1.6;
      transition: background 0.5s ease, color 0.5s ease;
      overflow-x: hidden;
    }

    header {
      background: linear-gradient(to right, var(--highlight), var(--blue-neon));
      padding: 60px 20px;
      text-align: center;
      color: var(--text-color);
      text-shadow: 0 1px 2px rgba(0, 0, 0, 0.6);
    }

    header h1 {
      font-size: 3rem;
      margin: 0;
    }

    header p {
      font-size: 1.2rem;
    }

    nav {
      background-color: var(--dark-accent);
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 15px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.3);
      flex-wrap: wrap;
    }

    nav a {
      color: var(--accent);
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s ease;
      font-size: 1.1rem;
    }

    nav a:hover {
      color: var(--highlight);
    }

    main {
      padding: 40px 20px;
      max-width: 100%;
      margin: auto;
      box-sizing: border-box;
    }

    section {
      background-color: rgba(255, 255, 255, 0.02);
      padding: 25px;
      margin-bottom: 30px;
      border-left: 6px solid var(--accent);
      border-radius: 12px;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.2);
      transition: transform 0.3s;
      box-sizing: border-box;
    }

    section:hover {
      transform: translateY(-5px);
    }

    section h2 {
      color: var(--accent);
      font-size: 1.8rem;
      margin-bottom: 15px;
    }

    section p {
      font-size: 1rem;
      line-height: 1.6;
      color: #d6d3c8;
    }

    section img {
      width: 100%;
      border-radius: 10px;
      margin-top: 20px;
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
      height: auto;
    }

    .video-wrapper {
      position: relative;
      padding-bottom: 56.25%; /* Aspect ratio 16:9 */
      height: 0;
      margin-top: 20px;
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.2);
    }

    .video-wrapper iframe {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      border: none;
    }

    blockquote {
      border-left: 5px solid var(--highlight);
      padding-left: 15px;
      margin-top: 20px;
      font-style: italic;
      color: #d6d3c8;
      background: rgba(255, 255, 255, 0.03);
    }

    #scrollToTop {
      position: fixed;
      bottom: 25px;
      right: 25px;
      background: var(--accent);
      color: white;
      border: none;
      border-radius: 50%;
      padding: 15px;
      font-size: 1.2rem;
      cursor: pointer;
      display: none;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.3);
      transition: background 0.3s ease;
    }

    #scrollToTop:hover {
      background-color: var(--highlight);
    }

    .toggle-mode {
      position: fixed;
      top: 20px;
      right: 20px;
      background: var(--highlight);
      color: black;
      padding: 10px 20px;
      border: none;
      border-radius: 30px;
      cursor: pointer;
      font-weight: bold;
      box-shadow: 0 2px 6px rgba(0, 0, 0, 0.3);
      transition: background 0.3s ease;
    }

    .toggle-mode:hover {
      background: var(--blue-neon);
    }

    footer {
      background-color: var(--dark-accent);
      color: #c0bdb4;
      text-align: center;
      padding: 20px;
      margin-top: 40px;
      border-top: 3px solid var(--accent);
    }

    /* Ajustes para pantallas pequeñas */
    @media (max-width: 768px) {
      header h1 {
        font-size: 2.5rem;
      }

      nav {
        flex-direction: column;
        align-items: center;
      }

      nav a {
        margin: 10px 0;
        font-size: 1rem;
        padding: 10px 0;
      }

      main {
        padding: 20px;
      }

      section h2 {
        font-size: 1.6rem;
      }

      section p {
        font-size: 1rem;
      }

      .video-wrapper {
        padding-bottom: 56.25%; /* Relación de aspecto 16:9 para dispositivos móviles */
      }

      #scrollToTop {
        bottom: 15px;
        right: 15px;
      }

      .toggle-mode {
        top: 10px;
        right: 10px;
        padding: 8px 15px;
        font-size: 1rem;
      }

      section img {
        width: 100%;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>La Deforestación: Un Problema Global</h1>
    <p>La deforestación es uno de los desafíos ambientales más grandes de nuestro tiempo. Cada año, grandes extensiones de bosques son destruidas, afectando nuestra biodiversidad, clima y recursos naturales.</p>
  </header>

  <nav>
    <a href="#section1">Causas</a>
    <a href="#section2">Consecuencias</a>
    <a href="#section3">Soluciones</a>
    <a href="#section4">Estadísticas</a>
    <a href="#section5">Impacto en las Especies</a>
    <a href="#section6">Ejemplos Globales</a>
    <a href="#videoSection">Video</a>
  </nav>

  <main>
    <section id="section1">
      <h2>Causas de la Deforestación</h2>
      <p>La deforestación es un fenómeno global impulsado por diversas causas, muchas de las cuales están relacionadas con actividades humanas que buscan recursos naturales a corto plazo, sin tomar en cuenta el impacto a largo plazo.</p>
      <p><strong>1. Agricultura comercial</strong>: La demanda global de productos agrícolas como la soja, el cacao, el café, y el aceite de palma lleva a la expansión de tierras agrícolas en zonas boscosas. Esta actividad es especialmente crítica en países como Brasil e Indonesia, donde los bosques tropicales se talan para plantar estos cultivos.</p>
      <p><strong>2. Ganadería</strong>: La necesidad de más tierras para pastoreo ha llevado a la deforestación masiva en muchas partes del mundo, especialmente en la Amazonía. La ganadería es una de las principales causas de pérdida de bosques en América Latina.</p>
      <p><strong>3. Tala ilegal de árboles</strong>: En muchos países, las leyes sobre la tala de árboles no se aplican correctamente o no existen en absoluto. Esto permite que se talen bosques sin ningún tipo de control, afectando la biodiversidad local y contribuyendo al cambio climático.</p>
      <p><strong>4. Urbanización y expansión de infraestructuras</strong>: A medida que las poblaciones crecen y las ciudades se expanden, se necesita más espacio para viviendas, comercios y carreteras. Este fenómeno afecta especialmente a los bosques urbanos y a las selvas tropicales.</p>
      <img src="https://www.example.com/imagen-causa-deforestacion.jpg" alt="Bosque destruido para agricultura" />
    </section>

    <section id="section2">
      <h2>Consecuencias de la Deforestación</h2>
      <p>La deforestación tiene repercusiones que van más allá de la simple pérdida de árboles. A continuación, se detallan algunas de las principales consecuencias que afectan al planeta y sus ecosistemas.</p>
      <p><strong>1. Pérdida de biodiversidad</strong>: Los bosques son hogar de una vasta cantidad de especies animales y vegetales. Al destruir estos hábitats, muchas especies se ven forzadas a desplazarse, algunas incluso pueden extinguirse debido a la falta de un entorno adecuado.</p>
      <p><strong>2. Cambio climático</strong>: Los árboles absorben grandes cantidades de dióxido de carbono, un gas de efecto invernadero. Al eliminar los bosques, liberamos grandes cantidades de CO2 a la atmósfera, lo que contribuye al calentamiento global.</p>
      <p><strong>3. Alteración del ciclo del agua</strong>: Los bosques desempeñan un papel crucial en la regulación del ciclo del agua. Sin árboles, las lluvias no se filtran correctamente en el suelo, lo que puede causar inundaciones o sequías extremas en diversas regiones.</p>
      <p><strong>4. Impactos en las comunidades locales</strong>: Muchas comunidades dependen de los bosques para su subsistencia, ya sea a través de la agricultura, la caza o la recolección de madera. La destrucción de los bosques afecta directamente a estos pueblos, llevándolos a la pobreza y la inseguridad alimentaria.</p>
      <img src="https://www.example.com/imagen-consecuencia-deforestacion.jpg" alt="Fauna afectada por la deforestación" />
    </section>

    <section id="section3">
      <h2>Soluciones para Combatir la Deforestación</h2>
      <p>A pesar de que la deforestación es un problema complejo, existen diversas soluciones y estrategias que pueden ayudar a mitigar su impacto y restaurar los ecosistemas perdidos.</p>
      <p><strong>1. Reforestación</strong>: La reforestación es un proceso mediante el cual se plantan árboles en áreas donde anteriormente existían bosques. Esta estrategia puede ayudar a restaurar los hábitats naturales, mejorar la calidad del aire y aumentar la biodiversidad.</p>
      <p><strong>2. Agricultura sostenible</strong>: Promover prácticas agrícolas que no destruyan los bosques, como la agroforestería, en la que se integran los árboles dentro de las parcelas agrícolas, puede contribuir a mantener la biodiversidad y mejorar la salud del suelo.</p>
      <p><strong>3. Leyes y regulaciones más estrictas</strong>: Es fundamental que los gobiernos implementen leyes más rigurosas para proteger los bosques y sancionar a las empresas que practican la tala ilegal. Además, los acuerdos internacionales como el Acuerdo de París pueden servir como marco para reducir la deforestación a nivel mundial.</p>
      <p><strong>4. Educación y concienciación</strong>: Informar a la población sobre los efectos de la deforestación y cómo sus hábitos de consumo pueden contribuir a la destrucción de los bosques es crucial para fomentar cambios positivos en la sociedad.</p>
      <img src="https://www.example.com/imagen-solucion-reforestacion.jpg" alt="Reforestación para recuperar bosques" />
    </section>

    <section id="section4">
      <h2>Estadísticas sobre la Deforestación</h2>
      <p>Las estadísticas sobre la deforestación muestran una realidad alarmante. A continuación, algunos datos clave que demuestran el impacto de la deforestación en el planeta:</p>
      <ul>
        <li><strong>Un 18%</strong> de las emisiones de gases de efecto invernadero provienen de la deforestación y la tala ilegal.</li>
        <li><strong>Más de 10 millones de hectáreas</strong> de bosques se pierden cada año debido a la deforestación.</li>
        <li>Las selvas tropicales han perdido alrededor de <strong>un 50%</strong> de su superficie en los últimos 40 años.</li>
        <li><strong>Brasil, Indonesia</strong> y <strong>Congo</strong> son algunos de los países con mayores tasas de deforestación.</li>
      </ul>
      <img src="https://www.example.com/imagen-estadisticas-deforestacion.jpg" alt="Gráfico sobre deforestación" />
    </section>

    <section id="section5">
      <h2>Impacto en las Especies</h2>
      <p>La deforestación afecta directamente a la fauna que depende de los bosques para su supervivencia. Algunas especies ya están en peligro debido a la pérdida de su hábitat natural:</p>
      <ul>
        <li><strong>Jaguar:</strong> Este majestuoso felino de América Latina está en peligro de extinción debido a la pérdida de su hábitat en las selvas tropicales.</li>
        <li><strong>Orangután:</strong> Los orangutanes de Borneo y Sumatra se encuentran en peligro crítico debido a la deforestación para la expansión de plantaciones de palma aceitera.</li>
        <li><strong>Elefante de Asia:</strong> Los elefantes están perdiendo sus hábitats debido a la expansión de la agricultura y la tala de bosques.</li>
      </ul>
      <img src="https://www.example.com/imagen-especies-deforestacion.jpg" alt="Especies afectadas por la deforestación" />
    </section>

    <section id="section6">
      <h2>Ejemplos Globales de Deforestación</h2>
      <p>En diferentes partes del mundo, la deforestación está ocurriendo a un ritmo alarmante. Algunos ejemplos destacados son:</p>
      <ul>
        <li><strong>Amazonía:</strong> La selva amazónica, conocida como el "pulmón del planeta", ha perdido grandes áreas de su cobertura boscosa debido a la tala ilegal y la expansión de la agricultura.</li>
        <li><strong>Indonesia:</strong> La deforestación en Indonesia ha sido impulsada por la expansión de las plantaciones de palma aceitera, que ha destruido vastas áreas de bosques tropicales.</li>
        <li><strong>África Central:</strong> En países como el Congo, la tala ilegal y la agricultura de subsistencia están destruyendo grandes partes de los bosques tropicales.</li>
      </ul>
      <img src="https://www.example.com/imagen-ejemplos-globales.jpg" alt="Deforestación en el mundo" />
    </section>

    <section id="videoSection">
      <h2>Video sobre la Deforestación</h2>
      <p>Este video es un documental educativo que explica las causas, consecuencias y posibles soluciones al problema de la deforestación. Es importante ver cómo afecta la vida en la Tierra y qué podemos hacer para reducir el impacto negativo.</p>
      <div class="video-wrapper">
        <iframe src="https://www.youtube.com/embed/IcBs3P6BKOY?si=SyUxoTugUs6aq9cm" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </div>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 PAGINA PARA LA INFORMACION SOBRE LA DEFORESTACION</p>
  </footer>

  <button id="scrollToTop" onclick="window.scrollTo(0, 0)">↑</button>

  <script>
    window.addEventListener('scroll', () => {
      const button = document.getElementById('scrollToTop');
      if (window.scrollY > 300) {
        button.style.display = 'block';
      } else {
        button.style.display = 'none';
      }
    });

    // Botón de cambio de modo oscuro/tema
    document.querySelector('.toggle-mode').addEventListener('click', () => {
      document.body.classList.toggle('dark-mode');
      if (document.body.classList.contains('dark-mode')) {
        document.querySelector('.toggle-mode').textContent = 'Modo Claro';
      } else {
        document.querySelector('.toggle-mode').textContent = 'Modo Oscuro';
      }
    });
  </script>

</body>
</html>
