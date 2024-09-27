<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Quiz da Tropa das Greludas</title>
    <style>
        body {
            font-family: 'Comic Sans MS', cursive, sans-serif;
            background: linear-gradient(to right, #ffafbd, #ffc3a0);
            color: #333;
            margin: 0;
            padding: 20px;
        }

        h1 {
            color: #e63946;
            text-align: center;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
        }

        .quiz-container {
            background-color: #ffffff;
            border-radius: 10px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
            padding: 30px;
            max-width: 600px;
            margin: auto;
            border: 2px solid #457b9d;
        }

        .question {
            margin-bottom: 20px;
            padding: 10px;
            border-left: 5px solid #e63946;
            background-color: #f1faee;
        }

        .option {
            display: block;
            margin: 10px 0;
            padding: 12px;
            background-color: #a8dadc;
            border-radius: 8px;
            cursor: pointer;
            transition: background-color 0.3s, transform 0.3s;
        }

        .option:hover {
            background-color: #457b9d;
            transform: scale(1.05);
        }

        button {
            background-color: #2a9d8f;
            color: white;
            border: none;
            padding: 12px 20px;
            border-radius: 8px;
            cursor: pointer;
            font-size: 18px;
            margin-top: 20px;
            transition: background-color 0.3s;
        }

        button:hover {
            background-color: #264653;
        }

        footer {
            text-align: center;
            margin-top: 20px;
            color: #264653;
        }
    </style>
</head>
<body>
    <h1>Quiz da Tropa das Greludas</h1>
    <div class="quiz-container">
        <div class="question">
            <p>1. Qual é a especialidade da Marlene?</p>
            <label class="option"><input type="radio" name="question1" value="a"> Contar mentiras</label>
            <label class="option"><input type="radio" name="question1" value="b"> Cozinhar</label>
            <label class="option"><input type="radio" name="question1" value="c"> Dançar</label>
        </div>
        <div class="question">
            <p>2. O que a Benedita gosta de fazer?</p>
            <label class="option"><input type="radio" name="question2" value="a"> Jogar bingo</label>
            <label class="option"><input type="radio" name="question2" value="b"> Dar golpes</label>
            <label class="option"><input type="radio" name="question2" value="c"> Fazer crochê</label>
        </div>
        <button onclick="submitQuiz()">Enviar Respostas</button>
    </div>

    <footer>
        <p>Divirta-se e participe com a Tropa das Greludas!</p>
    </footer>

    <script>
        function submitQuiz() {
            alert("Obrigado por participar do quiz da Tropa das Greludas!");
        }
    </script>
</body>
</html>
