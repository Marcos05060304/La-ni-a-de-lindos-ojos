<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Quieres ser mi San Valentín?</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: #ffe6f2;
        }
        .container {
            position: relative;
            max-width: 500px;
            margin: 50px auto;
            padding: 20px;
            background: white;
            border-radius: 15px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .gerberas {
            width: 100%;
            border-radius: 10px;
        }
        h1 {
            color: #d63384;
        }
        .buttons {
            margin-top: 20px;
            position: relative;
        }
        button {
            font-size: 18px;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            cursor: pointer;
            border-radius: 10px;
            transition: 0.3s;
        }
        .yes-btn {
            background-color: #ff4081;
            color: white;
        }
        .no-btn {
            background-color: #ccc;
            color: black;
            position: absolute;
        }
    </style>
</head>
<body>
    <div class="container">
        <img class="gerberas" src="https://upload.wikimedia.org/wikipedia/commons/7/7a/Gerbera_Orange_Yellow.jpg" alt="Gerberas">
        <h1>¿Quieres ser mi San Valentín? 💖</h1>
        <div class="buttons">
            <button class="yes-btn" onclick="alert('¡Sabía que dirías que sí! 💕 Nos vemos el 14 de febrero.')">Sí</button>
            <button class="no-btn" onmouseover="moverBoton()">No</button>
        </div>
    </div>

    <script>
        function moverBoton() {
            let botonNo = document.querySelector('.no-btn');
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 100);
            botonNo.style.left = `${x}px`;
            botonNo.style.top = `${y}px`;
        }
    </script>
</body>
</html>
