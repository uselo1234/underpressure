<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Under Pressure Team | Buceo y Aventura Submarina</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f4f8;
            color: #333;
            line-height: 1.7;
        }
        header {
            background-color: #003063;
            padding: 25px 0;
            text-align: center;
            position: relative;
        }
        header .logo {
            position: absolute;
            left: 20px;
            top: 20px;
            /* Añadido para el fondo azul */
            background-color: #003063;
            padding: 5px; /* Ajusta el padding según sea necesario */
            border-radius: 5px; /* Opcional: para redondear las esquinas del fondo */
        }
        header .logo img {
            height: 60px;
        }
        header h1 {
            color: #ffffff;
            font-size: 2.5em;
            margin-bottom: 0;
            font-weight: 700;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
        }
        header p {
            color: #b8c6d3;
            font-size: 1.1em;
            margin-top: 10px;
            font-weight: 400;
        }
        nav {
            background-color: #003063;
            padding: 10px 0;
            text-align: center;
        }
        nav ul {
            list-style: none;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
        }
        nav ul li {
            margin: 0 20px;
        }
        nav ul li a {
            color: #ffffff;
            text-decoration: none;
            font-size: 1.2em;
            font-weight: 600;
            text-transform: uppercase;
            transition: color 0.3s ease;
        }
        nav ul li a:hover {
            color: #ff6600;
        }
        .hero-section {
            background-image: url('https://images.unsplash.com/photo-1552767059-b165140681ce?q=80&w=3270&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D');
            background-size: cover;
            background-position: center;
            padding: 150px 0;
            text-align: center;
            color: #ffffff;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        .hero-section h2 {
            font-size: 3em;
            margin-bottom: 20px;
            font-weight: 700;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }
        .hero-section p {
            font-size: 1.3em;
            margin-bottom: 30px;
            max-width: 800px;
            line-height: 1.8;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.3);
        }
        .cta-button {
            background-color: #ff6600;
            color: #ffffff;
            padding: 15px 30px;
            text-decoration: none;
            font-size: 1.2em;
            font-weight: 600;
            border-radius: 10px;
            transition: background-color 0.3s ease, color 0.3s ease;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        .cta-button:hover {
            background-color: #cc5200;
            color: #ffffff;
            box-shadow: 0 6px 8px rgba(0, 0, 0, 0.15);
        }
        .experiencia-section {
            padding: 80px 0;
            text-align: center;
        }
        .experiencia-section h2 {
            font-size: 2.5em;
            margin-bottom: 40px;
            color: #003063;
            font-weight: 700;
        }
        .experiencia-section p{
            font-size: 1.2em;
            color: #555;
            max-width: 800px;
            margin: 0 auto 30px auto;
            line-height: 1.8;
        }
        .galeria-section {
            padding: 80px 0;
            text-align: center;
            background-color: #f0f4f8;
        }
        .galeria-section h2 {
            font-size: 2.5em;
            margin-bottom: 40px;
            color: #003063;
            font-weight: 700;
        }
        .galeria-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin: 0 auto;
            max-width: 1200px;
        }
        .galeria-grid img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 10px;
            transition: transform 0.3s ease;
        }
        .galeria-grid img:hover {
            transform: scale(1.1);
        }
        .testimonios-section {
            padding: 80px 0;
            text-align: center;
            background-color: #f0f4f8;
        }
        .testimonios-section h2 {
            font-size: 2.5em;
            margin-bottom: 40px;
            color: #003063;
            font-weight: 700;
        }
        .testimonio-card {
            background-color: #ffffff;
            border-radius: 15px;
            padding: 30px;
            margin: 20px;
            text-align: left;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .testimonio-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 8px 12px rgba(0, 0, 0, 0.15);
        }
        .testimonio-card p {
            font-size: 1.1em;
            color: #555;
            margin-bottom: 20px;
            line-height: 1.7;
            font-style: italic;
        }
        .testimonio-card h3 {
            font-size: 1.2em;
            color: #003063;
            font-weight: 600;
            margin-top: 10px;
        }
        .contacto-section {
            padding: 80px 0;
            text-align: center;
            background-color: #ffffff;
        }
        .contacto-section h2 {
            font-size: 2.5em;
            margin-bottom: 40px;
            color: #003063;
            font-weight: 700;
        }
        .contacto-form {
            max-width: 600px;
            margin: 0 auto;
            text-align: left;
            padding: 20px;
            border-radius: 15px;
            background-color: #f0f4f8;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        .contacto-form label {
            display: block;
            margin-top: 20px;
            font-size: 1.1em;
            color: #333;
            font-weight: 600;
        }
        .contacto-form input, .contacto-form textarea {
            width: 100%;
            padding: 12px;
            margin-top: 5px;
            border: 1px solid #ccc;
            border-radius: 8px;
            font-size: 1em;
            transition: border-color 0.3s ease;
        }
        .contacto-form input:focus, .contacto-form textarea:focus {
            outline: none;
            border-color: #ff6600;
        }
        .contacto-form textarea {
            height: 150px;
            resize: vertical;
        }
        .contacto-form button {
            background-color: #ff6600;
            color: #ffffff;
            padding: 12px 30px;
            border: none;
            border-radius: 8px;
            font-size: 1.1em;
            font-weight: 600;
            margin-top: 20px;
            cursor: pointer;
            transition: background-color 0.3s ease, color 0.3s ease;
            width: 100%;
        }
        .contacto-form button:hover {
            background-color: #cc5200;
            color: #ffffff;
        }
        footer {
            background-color: #003063;
            color: #ffffff;
            padding: 20px;
            text-align: center;
            margin-top: 80px;
        }
        footer p {
            font-size: 1em;
            font-weight: 400;
        }
        @media (max-width: 1200px) {
            .experiencia-section p, .consultoria-section ul {
                max-width: 95%;
            }
        }
        @media (max-width: 992px) {
            nav ul li {
                margin: 0 10px;
            }
            .hero-section h2 {
                font-size: 2.5em;
            }
            .hero-section p {
                font-size: 1.2em;
            }
            .testimonio-card {
                margin: 15px;
            }
        }
        @media (max-width: 768px) {
            header h1 {
                font-size: 2em;
            }
            header p {
                font-size: 1em;
            }
            nav ul {
                flex-direction: column;
            }
            nav ul li {
                margin: 10px 0;
            }
            .hero-section {
                padding: 100px 0;
            }
            .hero-section h2 {
                font-size: 2em;
            }
            .hero-section p {
                font-size: 1.1em;
            }
            .experiencia-section h2, .testimonios-section h2, .contacto-section h2 {
                font-size: 2em;
            }
            .testimonio-card {
                padding: 20px;
            }
        }
        @media (max-width: 576px) {
            header .logo img {
                height: 50px;
            }
            header h1 {
                font-size: 1.7em;
            }
            header p {
                font-size: 0.9em;
            }
            .hero-section {
                padding: 80px 0;
            }
            .hero-section h2 {
                font-size: 1.7em;
            }
            .hero-section p {
                font-size: 1em;
            }
            .cta-button {
                padding: 10px 20px;
                font-size: 1em;
            }
            .testimonio-card {
                margin: 10px;
            }
            .contacto-form {
                padding: 15px;
            }
            .contacto-form input, .contacto-form textarea {
                font-size: 0.9em;
            }
            .contacto-form button {
                font-size: 1em;
                padding: 10px 20px;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">
            <img src="https://res.cloudinary.com/dhls4wqxb/image/upload/v1747707886/WhatsApp_Image_2025-05-19_at_21.22.55_zu3pge.jpg" alt="Logo de Under Pressure Team">
        </div>
        <h1>Under Pressure Team</h1>
        <p>Explora el mundo submarino con nosotros</p>
    </header>
    <nav>
        <ul>
            <li><a href="#experiencia">Experiencia</a></li>
            <li><a href="#galeria">Galería</a></li>
            <li><a href="#testimonios">Testimonios</a></li>
            <li><a href="#contacto">Contacto</a></li>
        </ul>
    </nav>
    <section class="hero-section">
        <h2>Tu Aventura Submarina Comienza Aquí</h2>
        <p>
            Descubre la belleza del océano y vive experiencias inolvidables.
            Ofrecemos inmersiones guiadas y cursos para todos los niveles.
        </p>
        <a href="#contacto" class="cta-button">Reserva tu Inmersión</a>
    </section>
    <section id="experiencia" class="experiencia-section">
        <h2>Descubre la Experiencia</h2>
        <p>
            Sumérgete en un mundo fascinante y explora la vida marina de cerca.
            Nuestras inmersiones guiadas te llevarán a los mejores puntos de la zona,
            donde podrás admirar paisajes impresionantes y especies únicas.
        </p>
    </section>
    <section id="galeria" class="galeria-section">
        <h2>Galería de Fotos</h2>
        <div class="galeria-grid">
            <img src="https://res.cloudinary.com/dhls4wqxb/image/upload/v1747707490/WhatsApp_Image_2025-05-19_at_21.12.38_1_vzotxk.jpg" alt="Foto de buceo 1">
            <img src="https://res.cloudinary.com/dhls4wqxb/image/upload/v1747707496/WhatsApp_Image_2025-05-19_at_21.12.40_zobrxp.jpg" alt="Foto de buceo 2">
            <img src="https://res.cloudinary.com/dhls4wqxb/image/upload/v1747707499/WhatsApp_Image_2025-05-19_at_21.12.40_1_bizww9.jpg" alt="Foto de buceo 3">
            <img src="https://res.cloudinary.com/dhls4wqxb/image/upload/v1747707501/WhatsApp_Image_2025-05-19_at_21.12.39_1_fqq8fw.jpg" alt="Foto de buceo 4">
            <img src="https://res.cloudinary.com/dhls4wqxb/image/upload/v1747707502/WhatsApp_Image_2025-05-19_at_21.12.38_pzxgt0.jpg" alt="Foto de buceo 5">
            <img src="https://res.cloudinary.com/dhls4wqxb/image/upload/v1747707507/WhatsApp_Image_2025-05-19_at_21.12.39_aqvm6o.jpg" alt="Foto de buceo 6">
        </div>
    </section>
    <section id="testimonios" class="testimonios-section">
        <h2>Testimonios</h2>
        <div class="testimonios-cards-container">
            <div class="testimonio-card">
                <p>"Una experiencia increíble. El equipo es muy profesional y te hacen sentir seguro en todo momento."</p>
                <h3>Pedro Gómez</h3>
            </div>
            <div class="testimonio-card">
                <p>"Los paisajes submarinos son impresionantes. ¡Definitivamente volveré a bucear con ellos!"</p>
                <h3>Ana Martínez</h3>
            </div>
        </div>
    </section>
    <section id="contacto" class="contacto-section">
        <h2>Contáctanos</h2>
        <form class="contacto-form" id="contacto-form">
            <label for="nombre">Nombre:</label>
            <input type="text" id="nombre" name="nombre" placeholder="Tu nombre" required>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" placeholder="Tu email" required>
            <label for="mensaje">Mensaje:</label>
            <textarea id="mensaje" name="mensaje" placeholder="Tu mensaje" required></textarea>
            <button type="submit">Enviar Mensaje</button>
        </form>
    </section>
    <footer>
        <p>© 2025 Under Pressure Team. Todos los derechos reservados.</p>
    </footer>
    <script>
        const form = document.getElementById('contacto-form');

        form.addEventListener('submit', (event) => {
            event.preventDefault(); // Evita que el formulario se envíe de la manera tradicional

            const formData = new FormData(form);

            fetch('/enviar_correo', {  // La ruta debe coincidir con la definida en tu script de backend
                method: 'POST',
                body: formData
            })
            .then(response => response.json())
            .then(data => {
                if (data.success) {
                    alert(data.message); // Muestra un mensaje de éxito
                    form.reset(); // Opcional: Resetea el formulario
                } else {
                    alert(data.message); // Muestra un mensaje de error
                }
            })
            .catch(error => {
                console.error('Error:', error);
                alert('Ocurrió un error al enviar el mensaje. Por favor, inténtalo de nuevo más tarde.');
            });
        });
    </script>
</body>
</html>
