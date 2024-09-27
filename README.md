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
            <p>1. Se você tivesse que planejar uma festa, qual das Greludas você chamaria para ajudar?</p>
            <label class="option"><input type="radio" name="question1" value="Marlene"> Marlene (ela sempre tem ideias mirabolantes)</label>
            <label class="option"><input type="radio" name="question1" value="Benedita"> Benedita (ela traz os melhores petiscos)</label>
            <label class="option"><input type="radio" name="question1" value="Márcia"> Márcia (ela sempre anima a galera)</label>
        </div>
        <div class="question">
            <p>2. Qual Greluda você escolheria para uma competição de dança?</p>
            <label class="option"><input type="radio" name="question2" value="Marlene"> Marlene (ela tem passos únicos)</label>
            <label class="option"><input type="radio" name="question2" value="Lucinda"> Lucinda (ela dança do jeito dela)</label>
            <label class="option"><input type="radio" name="question2" value="Márcia"> Márcia (a palhaça sempre arrasa)</label>
        </div>
        <div class="question">
            <p>3. Se você estivesse em apuros, quem você chamaria para te ajudar?</p>
            <label class="option"><input type="radio" name="question3" value="Benedita"> Benedita (ela sempre dá um jeito)</label>
            <label class="option"><input type="radio" name="question3" value="Josefa"> Josefa (ela conhece todos os esquemas)</label>
            <label class="option"><input type="radio" name="question3" value="Lucinda"> Lucinda (mesmo sem querer, ela acaba ajudando)</label>
        </div>
        <div class="question">
            <p>4. Qual Greluda é a mais engraçada e sempre conta piadas?</p>
            <label class="option"><input type="radio" name="question4" value="Márcia"> Márcia (a palhaça do grupo)</label>
            <label class="option"><input type="radio" name="question4" value="Marlene"> Marlene (com suas histórias malucas)</label>
            <label class="option"><input type="radio" name="question4" value="Benedita"> Benedita (sempre com uma piada na ponta da língua)</label>
        </div>
        <div class="question">
            <p>5. Se você pudesse fazer uma viagem com uma das Greludas, quem seria?</p>
            <label class="option"><input type="radio" name="question5" value="Lucinda"> Lucinda (as aventuras dela são inesquecíveis)</label>
            <label class="option"><input type="radio" name="question5" value="Marlene"> Marlene (sempre arranja confusão)</label>
            <label class="option"><input type="radio" name="question5" value="Josefa"> Josefa (os trambiques são garantidos)</label>
        </div>
        <button onclick="submitQuiz()">Enviar Respostas</button>
    </div>

    <footer>
        <p>Divirta-se e participe com a Tropa das Greludas!</p>
    </footer>

    <script>
        function submitQuiz() {
            const answers = {
                "Marlene": 0,
                "Benedita": 0,
                "Lucinda": 0,
                "Márcia": 0,
                "Josefa": 0
            };

            const question1 = document.querySelector('input[name="question1"]:checked');
            const question2 = document.querySelector('input[name="question2"]:checked');
            const question3 = document.querySelector('input[name="question3"]:checked');
            const question4 = document.querySelector('input[name="question4"]:checked');
            const question5 = document.querySelector('input[name="question5"]:checked');

            if (question1) answers[question1.value]++;
            if (question2) answers[question2.value]++;
            if (question3) answers[question3.value]++;
            if (question4) answers[question4.value]++;
            if (question5) answers[question5.value]++;

            const result = Object.keys(answers).reduce((a, b) => answers[a] > answers[b] ? a : b);
            alert(`Você se identifica mais com: ${result}!`);
        }
    </script>
</body>
</html>
