<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Panel SEO - SEM - Visibilidad</title>

    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background: #f5f5f5;
        }
        header {
            background: #1e3a8a;
            color: white;
            padding: 20px;
            text-align: center;
            font-size: 24px;
            font-weight: bold;
        }
        .container {
            display: flex;
            height: calc(100vh - 120px);
        }
        .sidebar {
            width: 250px;
            background: #0f172a;
            color: white;
            padding: 20px;
            display: flex;
            flex-direction: column;
            gap: 15px;
        }
        .sidebar button {
            padding: 12px;
            background: #1e293b;
            border: none;
            color: white;
            cursor: pointer;
            text-align: left;
            border-radius: 5px;
            transition: 0.3s;
        }
        .sidebar button:hover {
            background: #334155;
        }
        .content {
            flex: 1;
            padding: 30px;
            background: white;
            overflow-y: auto;
            font-size: 18px;
        }
        footer {
            background: #1e3a8a;
            color: white;
            text-align: center;
            padding: 15px;
            font-size: 14px;
        }
    </style>
</head>
<body>

<header>
  Posicionamiento Web
</header>

<div class="container">
    <div class="sidebar">
        <button onclick="mostrar('seo')">SEO</button>
        <button onclick="mostrar('sem')">SEM</button>
        <button onclick="mostrar('visibilidad')">Visibilidad en Web</button>
    </div>

  <div class="content" id="contenido">
    <p> Haz clic en un botón para mostrar la información aquí.&nbsp;</p>
    <p>Nota: No me dejó poner imagenes porque lo toma como texto.&nbsp;</p>
  </div>
</div>

<footer>
Troncoso Pérez Oscar Alexis - Viernes 7:00 pm - 10:00 pm </footer>

<script>
    function mostrar(info) {
        const contenido = document.getElementById("contenido");

        const textos = {
            seo: `
                <h2>SEO (Search Engine Optimization)</h2>
                <h3>¿Qué es?</h3>
                <p>El SEO o Search Engine Optimization es el proceso de optimizar un sitio web para aparecer en los primeros resultados de búsqueda de manera orgánica, es decir, sin pagar por anuncios. Su funcionamiento se basa en mejorar la calidad del contenido, la relevancia de las palabras clave, la estructura de la página, la velocidad de carga, la experiencia del usuario y la autoridad del sitio mediante enlaces externos. Google rastrea, indexa y clasifica las páginas según estos factores, por lo que un buen SEO permite que un sitio sea más visible y aparezca como una respuesta confiable para las búsquedas de los usuarios. Aunque sus resultados toman tiempo, son estables, sostenibles y generan tráfico gratuito y constante.</p>

                <h3>¿Cómo funciona?</h3>
                <p>El funcionamiento del SEO se basa en cómo los motores de búsqueda, como Google, rastrean e interpretan las páginas web. Primero, Google utiliza bots que recorren Internet para encontrar páginas nuevas o actualizadas; luego indexa esa información en su base de datos y, finalmente, clasifica cada página según su relevancia, calidad y utilidad para el usuario. El SEO actúa optimizando todos los elementos que Google evalúa: desde el contenido y las palabras clave hasta la estructura interna, la velocidad, la accesibilidad y la autoridad externa que recibe una página mediante enlaces de otros sitios. De esta manera, el SEO permite que un sitio sea mejor comprendido por los buscadores y considerado como una respuesta valiosa para determinadas búsquedas. Algunos puntos a destacar son los siguientes:
                    <ul>
                        <li>Palabras clave</li>
                        <li>Contenido de calidad</li>
                        <li>Velocidad del sitio</li>
                        <li>Optimización móvil</li>
                        <li>Backlinks</li>
                    </ul>
                </p>

                <h3>¿Para qué sirve?</h3>
                <p>Su propósito principal es aumentar la visibilidad orgánica de un sitio, atraer tráfico de calidad sin pagar por cada visita, mejorar la reputación digital de una marca y convertir a los buscadores en una fuente constante y sostenible de clientes o lectores. También contribuye a crear una presencia a largo plazo, ya que una vez logrado un buen posicionamiento, los resultados tienden a mantenerse con un mantenimiento.
            `,

            sem: `
                <h2>SEM (Search Engine Marketing)</h2>
                <h3>¿Qué es?</h3>
                <p>El SEM o Search Engine Marketing se centra en campañas de publicidad pagada en motores de búsqueda, principalmente a través de Google Ads. Este método funciona mediante un sistema de pujas por palabras clave, donde los anunciantes compiten por aparecer en la parte superior de los resultados. Se suele pagar por clic (CPC), y Google determina qué anuncio mostrar según la combinación entre la puja y la calidad del anuncio y de la página de destino. El SEM ofrece resultados inmediatos, permite segmentar al público de forma precisa y es ideal para promocionar productos, lograr ventas rápidas o complementar estrategias de posicionamiento.</p>

                <h3>¿Cómo funciona?</h3>
                <p>Se basa en un sistema de publicidad pagada donde las empresas utilizan plataformas como Google Ads para mostrar anuncios cada vez que un usuario realiza una búsqueda relacionada con sus productos o servicios. Este proceso funciona mediante una subasta automática en la que los anunciantes pujan por palabras clave, establecen presupuestos diarios y crean anuncios relevantes. Google combina la puja, la calidad del anuncio y la experiencia de la página de destino para decidir qué anuncio mostrar y en qué posición. Como resultado, el SEM permite aparecer de forma inmediata en la parte superior de los resultados de búsqueda siempre que se cuente con un presupuesto y una estrategia de segmentación adecuadas.</p>

                <h3>¿Para qué sirve?</h3>
                <p>Sirve para obtener visibilidad inmediata, impulsar ventas o conversiones a corto plazo, promocionar productos o servicios recién lanzados, competir por palabras clave muy difíciles de posicionar orgánicamente y llegar a públicos altamente segmentados según su ubicación, intereses o comportamiento. Su principal utilidad es acelerar resultados y complementar el SEO, especialmente cuando se necesitan acciones rápidas o campañas temporales.</p>
            `,

            visibilidad: `
                <h2>Visibilidad en el Posicionamiento Web</h2>
                <h3>¿Qué es?</h3>
                <p>Es el nivel de exposición que una web obtiene cuando los usuarios buscan información relacionada con su contenido, productos o servicios. Esta visibilidad puede ser orgánica, proveniente del SEO, o pagada, proveniente del SEM, y se mide por cuántas veces aparece una página y en qué posición se muestra. Cuanto más alta sea la posición en Google, mayor será la probabilidad de recibir clics y atraer tráfico. La visibilidad es crucial porque determina la capacidad de una marca para ser encontrada por sus clientes potenciales, mejorar su reputación digital y aumentar sus oportunidades de conversión.</p>

                <h3>¿Cómo funciona?</h3>
                <p>La visibilidad de una web se refiere a qué tan fácil es que los usuarios la encuentren, principalmente en buscadores como Google. Funciona en tres pasos: primero, los motores de búsqueda rastrean e indexan tu página; segundo, determinan su relevancia y posición en los resultados según factores como contenido, palabras clave, enlaces, velocidad y experiencia del usuario; y tercero, la optimización mediante SEO (técnico, on-page y off-page) y la interacción de los usuarios mejora su ranking. Una web con buena visibilidad aparece en los primeros resultados, recibe más tráfico y, por tanto, mayor alcance y potencial de conversión.
                
Depende de múltiples factores como:
                    <ul>
                        <li>Relevancia del contenido</li>
                        <li>Autoridad del dominio</li>
                        <li>Optimización técnica</li>
                        <li>Competitividad de las palabras clave</li>
                    </ul>
                </p>

                <h3>¿Para qué sirve?</h3>
                <p>La visibilidad en buscadores sirve para que un sitio web logre ser encontrado fácilmente por los usuarios, aumente sus probabilidades de recibir clics, mejore su presencia de marca y genere oportunidades de venta o interacción. Tanto el SEO como el SEM existen precisamente para potenciar esa visibilidad: uno desde la optimización orgánica y sostenida, y el otro mediante la inversión en anuncios de alcance inmediato.</p>
            `
        };

        contenido.innerHTML = textos[info];
    }
	
</script>
</body>
</html>
