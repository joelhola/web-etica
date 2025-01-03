<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Página de Bienvenida</title>
</head>
<body>
    <h1>¡Hola! Bienvenido a mi página web.</h1>
    <p>Gracias por visitar. A continuación, recopilaremos algunos datos básicos para mejorar nuestra experiencia.</p>

    <form action="procesar_datos.php" method="post">
        <label for="nombre">Nombre:</label>
        <input type="text" id="nombre" name="nombre" required><br><br>

        <label for="correo">Correo Electrónico:</label>
        <input type="email" id="correo" name="correo" required><br><br>

        <input type="submit" value="Enviar">
    </form>

    <p>Tu dirección IP: <span id="ip_address"></span></p>
    <p>Tu ubicación: <span id="user_location"></span></p>

    <script>
        // Obtener dirección IP y ubicación
        fetch('https://ipinfo.io/json')
            .then(response => response.json())
            .then(data => {
                document.getElementById('ip_address').innerText = data.ip;
                document.getElementById('user_location').innerText = ${data.city}, ${data.region}, ${data.country};
            })
            .catch(error => console.error('Error al obtener ubicación:', error));
    </script>
</body>
</html>
