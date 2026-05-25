<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Proyecto Redes Interactivo</title>

    <style>

        body{
            font-family: Arial;
            background: #f0f4f8;
            margin: 0;
            padding: 20px;
        }

        h1{
            text-align: center;
            color: #003366;
        }

        .boton{
            background: #003366;
            color: white;
            padding: 15px;
            margin-top: 10px;
            cursor: pointer;
            border-radius: 10px;
            text-align: center;
            font-size: 18px;
        }

        .contenido{
            display: none;
            background: white;
            padding: 15px;
            border-radius: 10px;
            margin-top: 5px;
        }

        img{
            width: 100%;
            border-radius: 10px;
            margin-top: 10px;
        }

    </style>

</head>

<body>

    <h1>REDES INFORMÁTICAS</h1>

    <!-- TOPOLOGIAS -->

    <div class="boton" onclick="mostrar('topologias')">
        Topologías de Red
    </div>

    <div class="contenido" id="topologias">
        <p>
            Las topologías de red son la forma en que los dispositivos
            están conectados.
        </p>

        <ul>
            <li>Estrella</li>
            <li>Bus</li>
            <li>Anillo</li>
            <li>Malla</li>
        </ul>
    </div>

    <!-- CABLEADO -->

    <div class="boton" onclick="mostrar('cableado')">
        Cableado Estructurado
    </div>

    <div class="contenido" id="cableado">
        <p>
            Organiza los cables y conexiones de una red.
        </p>

        <ul>
            <li>UTP</li>
            <li>STP</li>
            <li>Fibra Óptica</li>
        </ul>
    </div>

    <!-- DIRECCIONES IP -->

    <div class="boton" onclick="mostrar('ip')">
        Direcciones IP
    </div>

    <div class="contenido" id="ip">
        <p>
            Una dirección IP identifica un dispositivo en la red.
        </p>

        <p>
            Ejemplo IPv4: 192.168.1.1
        </p>
    </div>

    <!-- PROTOCOLOS -->

    <div class="boton" onclick="mostrar('protocolos')">
        Protocolos
    </div>

    <div class="contenido" id="protocolos">
        <p>
            Los protocolos permiten la comunicación entre equipos.
        </p>

        <ul>
            <li>HTTP</li>
            <li>HTTPS</li>
            <li>FTP</li>
            <li>TCP/IP</li>
        </ul>
    </div>

    <!-- INTERNET -->

    <div class="boton" onclick="mostrar('internet')">
        Internet
    </div>

    <div class="contenido" id="internet">
        <p>
            Internet conecta millones de dispositivos en todo el mundo.
        </p>

        <img src="https://picsum.photos/600/250">
    </div>

    <!-- SEGURIDAD -->

    <div class="boton" onclick="mostrar('seguridad')">
        Seguridad Informática
    </div>

    <div class="contenido" id="seguridad">
        <p>
            Protege la información y los equipos de amenazas.
        </p>

        <ul>
            <li>Antivirus</li>
            <li>Firewall</li>
            <li>Contraseñas Seguras</li>
        </ul>
    </div>

    <!-- WIFI -->

    <div class="boton" onclick="mostrar('wifi')">
        Redes Inalámbricas
    </div>

    <div class="contenido" id="wifi">
        <p>
            Permiten conexión sin cables.
        </p>

        <ul>
            <li>WiFi</li>
            <li>Bluetooth</li>
            <li>Hotspot</li>
        </ul>
    </div>

    <script>

        function mostrar(id){

            let contenido = document.getElementById(id);

            if(contenido.style.display == "block"){
                contenido.style.display = "none";
            }
            else{
                contenido.style.display = "block";
            }

        }

    </script>

</body>
</html>
