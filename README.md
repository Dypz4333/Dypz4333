<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        *{
            padding: 0;
            margin: 0;
        }

        body{
            display: flex;
            flex-direction: column;
        }

        nav ul{
            display: flex;
        }

        nav{
            background-color: black;
            color:whitesmoke;
        }

        li{
            list-style: none;
            padding: 10px;
            padding-left: 20px;
            padding-right: 20px;
            background-color: rgb(66, 66, 66);
        }

        li:hover{
            background-color: gray;
        }
    </style>
</head>
<body>
    <nav>
        <ul>
            <li onclick="mostrarsobre()">Sobremim</li>
            <li onclick="mostrarlinks()">Links</li>
            <li onclick="mostrarstacks()">Habilidades</li>
        </ul>
    </nav>
    <article id="sobre">
        <h2>🚀 Sobre mim</h2>
        Me chamo Matheus Gabriel e sou um desenvolvedor front-end, atualmente estudando para futuramente me tornar um desenvolver do fullstack
        </article>
        
        <article id="link" style="display: none;">
        <h2>🔗 Links</h2>
        <img src="https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white">
        </article>
        
        <article id="stacks" style="display: none;">
        <h2>📕 Stacks</h2>
        <p align="left"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> <img href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer">  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-original.svg" alt="typescript" width="40" height="40"/> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="react" width="40" height="40"/> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/php/php-original.svg" alt="php" width="40" height="40"/>   <img src="https://www.vectorlogo.zone/logos/google_cloud/google_cloud-icon.svg" alt="gcp" width="40" height="40"/> </p>
    </article>     
    <script>
        var sobre = document.getElementById("sobre");
        var link = document.getElementById("link");
        var stacks = document.getElementById("stacks");

        function mostrarsobre(){
            sobre.style.display = "inline";
            link.style.display = "none";
            stacks.style.display = "none";
        }

        function mostrarlinks(){
            link.style.display = "inline";
            stacks.style.display = "none";
            sobre.style.display = "none";

        }

        function mostrarstacks(){
            stacks.style.display = "inline";
            sobre.style.display = "none";
            link.style.display = "none";
        }
        
    </script>
</body>
</html>

