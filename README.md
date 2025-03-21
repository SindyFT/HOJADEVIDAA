<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hoja de Vida CV - Sindy Fonte</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: #5acddf;
            color: white;
        }
        .container {
            display: flex;
            width: 90%;
            max-width: 1200px;
            height: 80vh; /* Ajuste para ser más horizontal */
            background: white;
            color: #333;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.2);
        }
        /* ... (resto del CSS sin cambios) ... */
    </style>
</head>
<body>
    <div class="container">
        <!-- Barra lateral -->
        <div class="sidebar">
            <img src="C:/Users/sindy/Downloads/FOOTO/1.jpg" alt="Foto de perfil">
            <h2>Sindy Fonte</h2>
            <div class="contact-info">
                <p><strong>Correo:</strong> <a href="mailto:luial2@correo.ugr.es">Sindy.melft05@correo.ugr.es</a></p>
                <p><strong>Teléfono:</strong> <a href="tel:+573176990561">+593 981135571</a></p>
            </div>
            <br>
            <div class="links">
                <h3>Links Externos</h3>
                <a href="#">Hoja de vida PDF</a>
                <a href="#">LinkedIn</a>
            </div>
        </div>

        <!-- Sección Principal -->
        <div class="main-content">
            <h1>Hoja de Vida</h1>

            <div class="bio">
                <h2>Biografía</h2>
                <p>Ingeniera en Logística y Transporte graduada de la Universidad Politécnica Estatal del Carchi, con sólida formación en gestión logística, análisis de datos, y manejo de KPIs. Experta en herramientas analíticas como Power BI y en la implementación de software ERP, como Odoo, entre otros, para optimizar procesos y mejorar la eficiencia operativa. Proactiva, con habilidades en trabajo en equipo y resolución de problemas.</p>
            </div>
            <div class="interests">
                <h2>Intereses Profesionales</h2>
                <ul>
                    <li>Logística y Cadena de Suministro</li>
                    <li>Transporte y Operaciones</li>
                    <li>Gestión de Compras y Abastecimiento</li>
                    <li>Consultoría en optimización de procesos logísticos y operativos</li>
                    <li>Logística para eventos y conciertos</li>
                    <li>Gestión de inventario y transporte en producciones Audiovisuales.</li>
                    <li>Automatización y Digitalización Logística</li>
                </ul>
            </div>

            <div class="portfolio">
                <h2>Portafolio de Proyectos</h2>
                <div class="tabs">
                    <div class="tab-btn" onclick="showTab('consultoria', this)">Proyectos Consultoría</div>
                    <div class="tab-btn" onclick="showTab('investigacion', this)">Proyectos Investigación</div>
                    <div class="tab-btn" onclick="showTab('cursos', this)">Cursos</div>
                    <div class="tab-btn" onclick="showTab('colaboraciones', this)">Colaboraciones</div>
                </div>

                <div id="consultoria" class="tab-content active">
                    <div class="year" onclick="toggleYear('y2023')">2023</div>
                    <div id="y2023" class="year-content">Contenido del año 2023...</div>
                </div>
                <div id="investigacion" class="tab-content">Contenido de investigación...</div>
                <div id="cursos" class="tab-content">Contenido de cursos...</div>
                <div id="colaboraciones" class="tab-content">Contenido de colaboraciones...</div>
            </div>
        </div>
    </div>

    <script>
        function showTab(tabName, element) {
            document.querySelectorAll('.tab-content').forEach(tab => tab.classList.remove('active'));
            document.getElementById(tabName).classList.add('active');

            document.querySelectorAll('.tab-btn').forEach(btn => btn.classList.remove('active'));
            element.classList.add('active');
        }

        function toggleYear(yearId) {
            let yearContent = document.getElementById(yearId);
            yearContent.style.display = yearContent.style.display === 'block' ? 'none' : 'block';
        }
    </script>
</body>
</html>
