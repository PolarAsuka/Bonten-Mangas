# Bonten-Mangas
Site de mangas
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Leitura de Mangás</title>
    <style>
        /* Definindo a paleta de cores */
        body {
            font-family: Arial, sans-serif;
            background-color: #1c1c1c; /* Tema escuro */
            color: #ffffff; /* Texto branco no tema escuro */
            margin: 0;
            padding: 0;
        }

        /* Tema claro */
        .light-theme {
            background-color: #eaeaea;
            color: #000000;
        }

        header {
            background-color: #5e2a8b; /* Roxo */
            padding: 20px;
            text-align: center;
            color: white;
        }

        header img {
            max-width: 150px;
        }

        nav {
            background-color: #3b1f56; /* Roxo mais escuro */
            padding: 10px;
            text-align: center;
        }

        nav a {
            color: white;
            padding: 10px;
            text-decoration: none;
            margin: 0 15px;
        }

        nav a:hover {
            background-color: #5e2a8b; /* Roxo ao passar o mouse */
        }

        .container {
            padding: 20px;
        }

        .manga-list {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }

        .manga-item {
            background-color: #333;
            border-radius: 8px;
            padding: 10px;
            text-align: center;
            width: 200px;
        }

        .manga-item img {
            width: 100%;
            border-radius: 8px;
        }

        .manga-item h3 {
            color: #5e2a8b;
        }

        footer {
            background-color: #1c1c1c;
            color: #bbb;
            text-align: center;
            padding: 10px;
        }

        .theme-toggle {
            position: absolute;
            top: 20px;
            right: 20px;
            padding: 10px;
            background-color: #5e2a8b;
            color: white;
            border: none;
            cursor: pointer;
        }

        .theme-toggle:hover {
            background-color: #3b1f56;
        }

    </style>
</head>
<body>

    <header>
        <img src="logo_roxy.png" alt="Logo do site"> <!-- Imagem de marca da Roxy Migurdia -->
        <h1>Leitura de Mangás</h1>
    </header>

    <button class="theme-toggle" onclick="toggleTheme()">Trocar Tema</button>

    <nav>
        <a href="#">Início</a>
        <a href="#">Mangás</a>
        <a href="#">Postar Mangá</a>
        <a href="#">Favoritos</a>
        <a href="#">Sobre</a>
    </nav>

    <div class="container">
        <h2>Últimos Mangás Postados</h2>
        <div class="manga-list">
            <div class="manga-item">
                <img src="manga_example1.jpg" alt="Mangá 1">
                <h3>Nome do Mangá</h3>
                <p>Descrição do mangá...</p>
            </div>
            <div class="manga-item">
                <img src="manga_example2.jpg" alt="Mangá 2">
                <h3>Nome do Mangá</h3>
                <p>Descrição do mangá...</p>
            </div>
            <!-- Adicione mais itens de mangá aqui -->
        </div>
    </div>

    <footer>
        <p>&copy; 2025 Leitura de Mangás | Todos os direitos reservados.</p>
        <p><a href="#">Termos de uso</a> | <a href="#">Política de privacidade</a></p>
    </footer>

    <script>
        // Função para alternar entre o tema claro e escuro
        function toggleTheme() {
            document.body.classList.toggle('light-theme');
        }
    </script>

</body>
</html>
