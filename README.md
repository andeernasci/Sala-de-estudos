# Sala-de-estudos
Rotina completa de estudos para concurso
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sala de Estudos</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: white;
            color: black;
            margin: 0;
            padding: 0;
            transition: all 0.3s ease;
        }
        body.dark-mode {
            background-color: #121212;
            color: white;
        }
        .container {
            padding: 20px;
        }
        header {
            text-align: center;
            margin-bottom: 20px;
        }
        .button {
            background-color: #4CAF50;
            color: white;
            padding: 10px 20px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }
        .button:hover {
            background-color: #45a049;
        }
        .discipline-list {
            list-style-type: none;
            padding: 0;
        }
        .discipline-list li {
            margin: 5px 0;
        }
        .discipline-link {
            text-decoration: none;
            color: #4CAF50;
        }
        .discipline-link:hover {
            text-decoration: underline;
        }
        .mode-toggle {
            display: flex;
            justify-content: center;
            margin-bottom: 20px;
        }
        .time-block {
            margin-bottom: 10px;
        }
        .note-box {
            margin-top: 20px;
        }
        .note-box textarea {
            width: 100%;
            height: 150px;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .footer {
            margin-top: 20px;
            text-align: center;
            color: #777;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>Sala de Estudos</h1>
            <button class="button mode-toggle" onclick="toggleMode()">Alternar Modo Claro/Escuro</button>
        </header>

        <div class="study-schedule">
            <h2>Quadro de Estudos</h2>
            <div class="time-block">
                <strong>Segunda-feira:</strong> Português | Português
            </div>
            <div class="time-block">
                <strong>Terça-feira:</strong> Legislação Municipal | Específica
            </div>
            <div class="time-block">
                <strong>Quarta-feira:</strong> Português | Específica
            </div>
            <div class="time-block">
                <strong>Quinta-feira:</strong> Legislação Municipal | Português
            </div>
            <div class="time-block">
                <strong>Sexta-feira:</strong> Português | Português
            </div>
            <div class="time-block">
                <strong>Sábado:</strong> Português | Específica
            </div>
        </div>

        <div class="discipline-list">
            <h2>Disciplinas</h2>
            <ul>
                <li><a class="discipline-link" href="#" onclick="openLink('portugues')">Português</a></li>
                <li><a class="discipline-link" href="#" onclick="openLink('legislacao')">Legislação Municipal</a></li>
                <li><a class="discipline-link" href="#" onclick="openLink('especifica')">Específica</a></li>
            </ul>
        </div>

        <div class="note-box">
            <h2>Bloco de Notas</h2>
            <textarea placeholder="Anote algo aqui..."></textarea>
        </div>

        <footer class="footer">
            <p>&copy; 2025 Sala de Estudos - Todos os direitos reservados</p>
        </footer>
    </div>

    <script>
        function toggleMode() {
            document.body.classList.toggle("dark-mode");
        }

        function openLink(discipline) {
            let url = "";
            switch(discipline) {
                case "portugues":
                    url = "https://www.exemplo.com/portugues";
                    break;
                case "legislacao":
                    url = "https://www.exemplo.com/legislacao";
                    break;
                case "especifica":
                    url = "https://www.exemplo.com/especifica";
                    break;
            }
            window.open(url, "_blank");
        }
    </script>
</body>
</html>
