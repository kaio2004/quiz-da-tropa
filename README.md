<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Qual Greluda Você É?</h1>
        <h2>Descubra com este divertido quiz!</h2>
    </header>
    <main>
        <form id="quizForm">
            <div class="question">
                <p>1. Como você prefere passar o tempo livre?</p>
                <label><input type="radio" name="timeLivre" value="Festejando com amigos"> Festejando com amigos</label><br>
                <label><input type="radio" name="timeLivre" value="Contando histórias"> Contando histórias</label><br>
                <label><input type="radio" name="timeLivre" value="Vendo vídeos engraçados"> Vendo vídeos engraçados</label><br>
            </div>
            <div class="question">
                <p>2. Qual é sua sobremesa favorita?</p>
                <label><input type="radio" name="sobremesa" value="Bolo de chocolate"> Bolo de chocolate</label><br>
                <label><input type="radio" name="sobremesa" value="Gelatina colorida"> Gelatina colorida</label><br>
                <label><input type="radio" name="sobremesa" value="Doce de leite"> Doce de leite</label><br>
            </div>
            <div class="question">
                <p>3. O que você faria se encontrasse um golpista?</p>
                <label><input type="radio" name="golpista" value="Daria risada e faria uma piada"> Daria risada e faria uma piada</label><br>
                <label><input type="radio" name="golpista" value="Tentaria enganá-lo de volta"> Tentaria enganá-lo de volta</label><br>
                <label><input type="radio" name="golpista" value="Contaria para os amigos"> Contaria para os amigos</label><br>
            </div>
            <button type="button" onclick="calcularResultado()">Descubra!</button>
        </form>
        <div id="resultado" class="resultado"></div>
    </main>
    <footer>
        <p>© 2024 Tropa das Greludas. Todos os direitos reservados.</p>
    </footer>
    <script src="script.js"></script>
</body>
</html>
