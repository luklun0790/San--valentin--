<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Quieres ser mi San Valentín?</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #ffe6e6;
            position: relative;
            overflow: hidden;
        }
        .container {
            margin-top: 50px;
        }
        h1 {
            color: #ff4d4d;
        }
        .btn {
            padding: 10px 20px;
            font-size: 18px;
            margin: 10px;
            cursor: pointer;
            border: none;
            border-radius: 5px;
        }
        .yes {
            background-color: #ff4d4d;
            color: white;
        }
        .no {
            background-color: #aaa;
            color: white;
            position: absolute;
        }
        .hidden {
            display: none;
            font-size: 20px;
            color: #ff4d4d;
            margin-top: 20px;
        }
        .images {
            margin-top: 30px;
        }
        .images img {
            width: 150px;
            height: auto;
            margin: 10px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>¿Quieres ser mi San Valentín? 💖</h1>
        <button class="btn yes" onclick="aceptar()">¡Sí!</button>
        <button class="btn no" onmouseover="moverBoton()">No</button>
        
        <p id="mensaje" class="hidden">Gracias por dejarme ser parte de tu camino ninja. 🥷❤️</p>
        <div class="images hidden" id="imagenes">
            <img src="https://upload.wikimedia.org/wikipedia/en/9/94/Naruto_Uzumaki.png" alt="Naruto">
            <img src="https://upload.wikimedia.org/wikipedia/en/4/47/Hinata.png" alt="Hinata">
        </div>
    </div>

    <script>
        function aceptar() {
            document.getElementById("mensaje").style.display = "block";
            document.getElementById("imagenes").style.display = "block";
        }

        function moverBoton() {
            const noBtn = document.querySelector('.no');
            const frases = ["Por favor 🥺", "Piénsalo bien 🤔", "Por fiiiii 😘"];
            noBtn.innerText = frases[Math.floor(Math.random() * frases.length)];

            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 50);
            noBtn.style.left = `${x}px`;
            noBtn.style.top = `${y}px`;
        }
    </script>
</body>
</html># San--valentin--
