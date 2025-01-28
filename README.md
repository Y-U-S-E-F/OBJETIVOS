<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Objetivos del Proyecto</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
    <style>
        /* Estilos generales */
        body {
            font-family: 'Montserrat', sans-serif;
            line-height: 1.8;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
            color: #333;
        }

        /* Contenedor principal */
        .container {
            max-width: 900px;
            margin: 30px auto;
            padding: 20px;
            background: #ffffff;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        /* Encabezados */
        h1, h2 {
            color: #2c3e50;
            text-align: center;
        }

        h1 {
            font-size: 2.5em;
            margin-bottom: 20px;
        }

        h2 {
            font-size: 1.8em;
            margin-top: 30px;
            margin-bottom: 10px;
        }

        /* Párrafos */
        p {
            margin-bottom: 20px;
            text-align: justify;
        }

        /* Listas */
        ul {
            list-style-type: none;
            margin-left: 0;
            padding-left: 0;
        }

        ul li {
            margin-bottom: 10px;
            padding: 10px;
            background: #e8f0fe;
            border-radius: 5px;
        }

        ul li::before {
            content: '\25B6';
            color: #3498db;
            margin-right: 10px;
        }

        /* Botón interactivo */
        .toggle-btn {
            display: inline-block;
            margin: 20px auto;
            padding: 10px 20px;
            background-color: #3498db;
            color: #fff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1em;
            transition: background-color 0.3s ease;
        }

        .toggle-btn:hover {
            background-color: #2980b9;
        }

        /* Ocultar contenido dinámico */
        .hidden {
            display: none;
        }

        /* Modo oscuro */
        .dark-mode {
            background-color: #2c3e50;
            color: #ecf0f1;
        }

        .dark-mode .container {
            background-color: #34495e;
            color: #ecf0f1;
        }

        .dark-mode ul li {
            background: #3b4a5a;
        }

        .dark-mode .toggle-btn {
            background-color: #1abc9c;
        }

        .dark-mode .toggle-btn:hover {
            background-color: #16a085;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Objetivos del Proyecto</h1>
        <p>Llevar a cabo un proceso dinámico y participativo en el que se realiza una evaluación y posterior diagnóstico de la situación actual de cada una de las personas participantes, orientando su incorporación al mundo laboral a través de un itinerario personalizado de integración.
        </p>

        <h2>Objetivo General 1</h2>
        <p>Llevar a cabo un proceso dinámico y participativo en el que se realice una evaluación y posterior diagnóstico de la situación actual de cada participante, orientando su incorporación al mercado laboral a través de un itinerario personalizado de integración.</p>
        <button class="toggle-btn" onclick="toggleVisibility('obj1')">Ver más</button>
        <ul id="obj1" class="hidden">
            <li>Objetivo Específico 1.1: Realizar evaluaciones iniciales para identificar la situación profesional y personal actual de cada participante.</li>
            <li>Objetivo Específico 1.2: Desarrollar itinerarios personalizados de integración adaptados a las necesidades y capacidades de cada individuo.</li>
            <li>Objetivo Específico 1.3: Supervisar y evaluar el progreso de los participantes a lo largo de su proceso de integración.</li>
        </ul>

        <h2>Objetivo General 2</h2>
        <p>Proporcionar a los participantes un nivel suficiente de autonomía personal y los recursos necesarios para realizar una búsqueda de empleo efectiva, empoderándolos para que tomen un papel activo en su integración en el mercado laboral.</p>
        <button class="toggle-btn" onclick="toggleVisibility('obj2')">Ver más</button>
        <ul id="obj2" class="hidden">
            <li>Objetivo Específico 2.1: Impartir sesiones de formación sobre técnicas y herramientas de búsqueda de empleo.</li>
            <li>Objetivo Específico 2.2: Mejorar la comprensión de los participantes sobre el mercado laboral, particularmente en el sector aeronáutico.</li>
            <li>Objetivo Específico 2.3: Facilitar talleres para mejorar el perfil profesional de los participantes con habilidades y competencias relevantes.</li>
        </ul>

        <h2>Objetivo General 3</h2>
        <p>Fomentar la integración sociolaboral de personas con discapacidad en todos los sectores, con un enfoque particular en el sector aeronáutico.</p>
        <button class="toggle-btn" onclick="toggleVisibility('obj3')">Ver más</button>
        <ul id="obj3" class="hidden">
            <li>Objetivo Específico 3.1: Promover colaboraciones entre empresas del sector aeronáutico y los participantes del programa para crear oportunidades de empleo.</li>
            <li>Objetivo Específico 3.2: Implementar itinerarios intensivos de búsqueda de empleo que inculquen rutinas efectivas en los participantes.</li>
            <li>Objetivo Específico 3.3: Proporcionar formación especializada para mejorar la empleabilidad de los participantes en el sector aeronáutico.</li>
        </ul>

        <button class="toggle-btn" onclick="toggleDarkMode()">Alternar Modo Oscuro</button>
    </div>

    <script>
        function toggleVisibility(id) {
            const element = document.getElementById(id);
            element.classList.toggle('hidden');
        }

        function toggleDarkMode() {
            document.body.classList.toggle('dark-mode');
        }
    </script>
</body>
