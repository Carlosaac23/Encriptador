<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="./CSS/style.css">
    <script type="text/javascript" src="./JS/main.js"></script>
    <title>Encriptador - Carlos Acosta</title>
</head>
<body>
    <header>
        <img src="./IMG/logo.png" alt="logo alura"> 
    </header>

    <main>
        <section class="seccion_izquierda">
            <input type="text" placeholder="Escribe tu texto aquí" id="textoEncriptado">
            <div class="contenedor_botones">
                <button type="button" id="botonEncriptado">Encriptar</button>
                <button type="button" id="botonDesencriptado">Desencriptar</button>
                <button type="button" id="botonCopiar">Copiar</button>
            </div>
        </section>
        <section class="seccion_derecha">
            <textarea name="resultado" class="textarea" placeholder="Texto encriptado/desencriptado" id="textoDesencriptado"></textarea>
        </section>
    </main>

    <footer class="footer">                                                     <!-----FOOTER----->
        <div class="footer__container container grid">
            <div>
                <h1 class="footer__title">
                    Carlos <span>Acosta</span>
                </h1>

                <h2 class="footer__education">
                    Desarrollador Back-end
                </h2>
            </div>

            <span class="footer__copy">
                &#169; Copyright Carlos Acosta. Derechos reservados
            </span>
        </div>
    </footer>

    
    <script>
        var btn = document.querySelector('#botonEncriptado');
        btn.onclick = encriptar;

        var btn2 = document.querySelector('#botonDesencriptado');
        btn2.onclick = desencriptar;

        var btn3 = document.querySelector('#botonCopiar');
        btn3.onclick = copiar;
    </script>
</body>
</html>
