<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cursos de Programação</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
        }
        header {
            background-color: #333;
            color: white;
            padding: 20px;
            font-size: 24px;
        }
        .container {
            padding: 20px;
        }
        .curso {
            border: 1px solid #ddd;
            margin: 10px;
            padding: 10px;
            display: inline-block;
            width: 200px;
        }
        .curso h3 {
            margin: 0;
        }
        .botao-inscricao, .botao-pix {
            display: block;
            margin-top: 10px;
            padding: 8px;
            background-color: #28a745;
            color: white;
            border: none;
            cursor: pointer;
        }
        .botao-inscricao:hover, .botao-pix:hover {
            background-color: #218838;
        }
    </style>
</head>
<body>
    <header>Cursos de Programação</header>
    <div class="container">
        <h2>Bem-vindo ao site de cursos!</h2>
        <p>Aqui você encontra cursos incríveis para aprender a programar.</p>
        
        <div class="curso">
            <h3>HTML e CSS</h3>
            <p>Aprenda a criar sites bonitos e responsivos.</p>
            <button class="botao-inscricao" onclick="inscrever('HTML e CSS')">Inscreva-se</button>
            <button class="botao-pix" onclick="copiarPix()">Pagar com Pix</button>
        </div>
        <div class="curso">
            <h3>JavaScript</h3>
            <p>Domine a linguagem que dá vida às páginas web.</p>
            <button class="botao-inscricao" onclick="inscrever('JavaScript')">Inscreva-se</button>
            <button class="botao-pix" onclick="copiarPix()">Pagar com Pix</button>
        </div>
        <div class="curso">
            <h3>Python</h3>
            <p>Entre no mundo da programação com uma linguagem poderosa.</p>
            <button class="botao-inscricao" onclick="inscrever('Python')">Inscreva-se</button>
            <button class="botao-pix" onclick="copiarPix()">Pagar com Pix</button>
        </div>
    </div>

    <script>
        function inscrever(curso) {
            alert('Você se inscreveu no curso de ' + curso + '!');
        }
        
        function copiarPix() {
            const chavePix = "157-543-066-52"; // Substitua pelo seu CPF ou chave Pix
            navigator.clipboard.writeText(chavePix).then(() => {
                alert("Chave Pix copiada! Agora, vá ao seu banco e cole para fazer o pagamento.");
            });
        }
    </script>
</body>
</html>
