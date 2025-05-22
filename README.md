<style>
  /* Base para el contenedor principal */
  .profile-container {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    color: #333;
    background: linear-gradient(135deg, #e0f2f7 0%, #ffffff 100%);
    padding: 40px 20px;
    border-radius: 15px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
    text-align: center;
    max-width: 900px;
    margin: 30px auto;
    overflow: hidden; /* Para contener las animaciones si se salen */
  }

  /* Estilo del título principal */
  .profile-container h1 {
    font-size: 3em;
    color: #2c3e50;
    margin-bottom: 15px;
    text-shadow: 2px 2px 4px rgba(0,0,0,0.1);
    animation: fadeInDown 1s ease-out; /* Animación de entrada */
  }

  /* Estilo para el subtítulo/descripción */
  .profile-container p {
    font-size: 1.2em;
    color: #555;
    line-height: 1.6;
    margin-bottom: 30px;
    animation: fadeInUp 1s ease-out; /* Animación de entrada */
    animation-delay: 0.2s; /* Retraso para que aparezca después del título */
    animation-fill-mode: both; /* Mantiene el estado final de la animación */
  }

  /* Contenedor de habilidades/lenguajes */
  .skills-grid {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 25px; /* Espacio entre los iconos */
    margin-top: 40px;
  }

  /* Estilo individual de cada habilidad/lenguaje */
  .skill-item {
    background-color: #f7f7f7;
    border: 1px solid #ddd;
    border-radius: 12px;
    padding: 20px;
    width: 150px;
    text-align: center;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.08);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    animation: zoomIn 0.6s ease-out; /* Animación de entrada para cada skill */
    opacity: 0; /* Oculto inicialmente para la animación */
  }

  /* Animación de hover para cada habilidad */
  .skill-item:hover {
    transform: translateY(-10px) scale(1.05); /* Efecto de levitación y ligero aumento */
    box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
  }

  /* Estilo de los iconos SVG */
  .skill-item svg {
    width: 60px;
    height: 60px;
    margin-bottom: 10px;
    /* Colores base para que los iconos no se vean con borde */
    fill: currentColor;
    color: #3498db; /* Color por defecto para los iconos */
  }

  /* Colores específicos para los iconos si quieres distinguirlos */
  .php-icon { color: #777BB4; }
  .css-icon { color: #1572B6; }
  .java-icon { color: #E34A00; } /* Un tono más naranja/rojizo para Java */
  .mysql-icon { color: #00758F; }
  .ajax-icon { color: #4D4D4D; } /* AJAX no tiene un color oficial, elegimos un gris oscuro */


  .skill-item h3 {
    font-size: 1.1em;
    color: #333;
    margin: 0;
  }

  /* Animaciones CSS */
  @keyframes fadeInDown {
    from { opacity: 0; transform: translateY(-30px); }
    to { opacity: 1; transform: translateY(0); }
  }

  @keyframes fadeInUp {
    from { opacity: 0; transform: translateY(30px); }
    to { opacity: 1; transform: translateY(0); }
  }

  @keyframes zoomIn {
    from { opacity: 0; transform: scale(0.8); }
    to { opacity: 1; transform: scale(1); }
  }

  /* Retrasos para la animación de cada skill-item */
  .skill-item:nth-child(1) { animation-delay: 0.4s; }
  .skill-item:nth-child(2) { animation-delay: 0.6s; }
  .skill-item:nth-child(3) { animation-delay: 0.8s; }
  .skill-item:nth-child(4) { animation-delay: 1.0s; }
  .skill-item:nth-child(5) { animation-delay: 1.2s; }

  /* Estilos para el footer */
  .footer {
    margin-top: 50px;
    font-size: 0.9em;
    color: #777;
    border-top: 1px solid #eee;
    padding-top: 20px;
  }

  .social-links a {
    margin: 0 10px;
    text-decoration: none;
    color: #3498db;
    font-weight: bold;
    transition: color 0.3s ease;
  }

  .social-links a:hover {
    color: #2980b9;
  }

  .container {
            background-color: #fff;
            padding: 25px;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            max-width: 600px;
            margin: auto;
        }
        h1 {
            color: #0056b3;
            text-align: center;
            margin-bottom: 30px;
        }
        ul {
            list-style: none;
            padding: 0;
        }
        li {
            background-color: #e9f5ff;
            border: 1px solid #cce5ff;
            margin-bottom: 15px;
            padding: 15px 20px;
            border-radius: 5px;
            display: flex;
            align-items: center;
        }
        li:hover {
            background-color: #d7edff;
        }
        .ministry-info strong {
            display: block;
            font-size: 1.2em;
            color: #004085;
        }
        .ministry-info a {
            color: #0056b3;
            text-decoration: none;
            font-weight: bold;
        }
        .ministry-info a:hover {
            text-decoration: underline;
        }
</style>

<div class="profile-container">
  <h1>Hola! Soy Luis Barrera</h1>
  <p>Desarrollador web apasionado por la creaci&oacute;n de soluciones robustas y eficientes. Especializado en (Linux, Apache, MySQL, PHP) y con experiencia en interfaces din&aacute;micas usando CSS, Jacript y AJAX.</p>
  <h1>Experiencias laborales</h1>
  <div class="container">
        <ul>
            <li>
                <div class="ministry-info">
                    <strong>Ministerio de Salud de El Salvador</strong>
                    <br><a href="https://www.salud.gob.sv/" target="_blank">https://www.salud.gob.sv</a>
                </div>
            </li>
            <li>
                <div class="ministry-info">
                    <strong>Ministerio de Salud y Protecci&oacute;n Social de Colombia</strong>
                    <br>
                    <a href="https://www.minsalud.gov.co/" target="_blank">https://www.minsalud.gov.co</a>
                </div>
            </li>
            <li>
                <div class="ministry-info">
                    <strong>Instituto Salvadore&ntilde;o de Rehabilitaci&oacute;n Integral</strong>
                    <br>
                    <a href="https://isri.gob.sv/" target="_blank">https://isri.gob.sv</a>
                </div>
            </li>
        </ul>
    </div>
  <h2>Aportes</h2>
  <br>
  
[![Aditya's GitHub Activity Graph](https://activity-graph.herokuapp.com/graph?username=Aditya664&theme=tokyonight)](https://git.io/praveenscience)

| ![Aditya's github stats](https://github-readme-stats.vercel.app/api?username=Aditya664&show_icons=true&theme=tokyonight) | ![Aditya GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=Aditya664&theme=tokyonight) |
| --- | --- |
| ![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Aditya664&theme=tokyonight) | ![Github Stars](https://github-readme-stats.vercel.app/api?username=Aditya664&show_icons=true&locale=en&count_private=true&hide_rank=true&custom_title=My%20GitHub%20Stats&disable_animations=true&theme=tokyonight) |

![Jokes Card](https://readme-jokes.vercel.app/api?theme=tokyonight)


<br>


  <h2>Mis Habilidades Clave</h2>
  <div class="skills-grid">
    <div class="skill-item">
      <svg class="php-icon" viewBox="0 0 128 128" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
        <path d="M64 0C28.7 0 0 28.7 0 64s28.7 64 64 64 64-28.7 64-64S99.3 0 64 0zM72.2 110.8c-2.3 4.6-7.3 7.8-12.7 7.8s-10.4-3.2-12.7-7.8L19 64c-2.3-4.6-2.3-10.4 0-15s7.3-7.8 12.7-7.8c5.4 0 10.4 3.2 12.7 7.8L64 96.2l19.6-39.2c2.3-4.6 7.3-7.8 12.7-7.8s10.4 3.2 12.7 7.8l-27.8 55.6z"/>
      </svg>
      <h3>PHP</h3>
    </div>

    <div class="skill-item">
      <svg class="css-icon" viewBox="0 0 512 512" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
        <path d="M416 0H96C42.98 0 0 42.98 0 96v320c0 53.02 42.98 96 96 96h320c53.02 0 96-42.98 96-96V96c0-53.02-42.98-96-96-96zm-48 108.61h-240c-6.627 0-12-5.373-12-12v-24c0-6.627 5.373-12 12-12h240c6.627 0 12 5.373 12 12v24c0 6.627-5.373 12-12 12zM368 256H144c-6.627 0-12-5.373-12-12v-24c0-6.627 5.373-12 12-12h224c6.627 0 12 5.373 12 12v24c0 6.627-5.373 12-12 12zM368 400H144c-6.627 0-12-5.373-12-12v-24c0-6.627 5.373-12 12-12h224c6.627 0 12 5.373 12 12v24c0 6.627-5.373 12-12 12z"/>
      </svg>
      <h3>CSS3</h3>
    </div>

    <div class="skill-item">
      <svg class="java-icon" viewBox="0 0 448 512" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
        <path d="M224 0C100.2 0 0 100.2 0 224c0 110.2 81 201.2 186 219.7V448c0 17.67 14.33 32 32 32h64c17.67 0 32-14.33 32-32v-4.3c105-18.5 186-109.5 186-219.7C448 100.2 347.8 0 224 0zm0 416c-105.8 0-192-86.2-192-192S118.2 32 224 32s192 86.2 192 192-86.2 192-192 192zM224 64c-88.37 0-160 71.63-160 160s71.63 160 160 160 160-71.63 160-160-71.63-160-160-160zM176 192c-17.67 0-32 14.33-32 32s14.33 32 32 32 32-14.33 32-32-14.33-32-32-32zm96 0c-17.67 0-32 14.33-32 32s14.33 32 32 32 32-14.33 32-32-14.33-32-32-32z"/>
      </svg>
      <h3>Java</h3>
    </div>

    <div class="skill-item">
      <svg class="mysql-icon" viewBox="0 0 640 512" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
        <path d="M368.5 256.3c-1.3 46.9-42.5 83.3-89.8 83.3-46.9 0-85.1-36.4-89.8-83.3h179.6zm233.1 9.9c0 126.9-102.5 229.4-229.4 229.4S13.4 393.2 13.4 266.3c0-126.9 102.5-229.4 229.4-229.4 126.9 0 229.4 102.5 229.4 229.4zM320 64c-114.7 0-207.6 92.9-207.6 207.6S205.3 479.2 320 479.2c114.7 0 207.6-92.9 207.6-207.6S434.7 64 320 64zM240 160c-26.5 0-48 21.5-48 48s21.5 48 48 48 48-21.5 48-48-21.5-48-48-48zm160 0c-26.5 0-48 21.5-48 48s21.5 48 48 48 48-21.5 48-48-21.5-48-48-48z"/>
      </svg>
      <h3>MySQL</h3>
    </div>

    <div class="skill-item">
      <svg class="ajax-icon" viewBox="0 0 512 512" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
        <path d="M480 208H288L320 32C192 32 128 176 128 208H32L64 480C224 480 288 336 288 208z"/>
      </svg>
      <h3>AJAX</h3>
    </div>
  </div>
<h2>Aportes</h2>
  <div class="footer">
    <p>Conéctate conmigo:</p>
    <div class="social-links">
      <a href="mailto:lbarrerac@gmail.com">Email</a>
    </div>
  </div>
</div>
