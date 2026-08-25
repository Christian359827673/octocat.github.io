# octocat.github.io
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Quiz - Ecossistemas do Mundo</title>

    <style>
        body {
            font-family: Arial, Helvetica, sans-serif;
            margin: 0;
            background: #eaf6f3;
            color: #263238;
        }

        header {
            background: #00695c;
            color: white;
            text-align: center;
            padding: 35px 20px;
        }

        header h1 {
            margin: 0;
            font-size: 34px;
        }

        header p {
            font-size: 17px;
            margin-top: 10px;
        }

        .container {
            max-width: 900px;
            margin: 30px auto;
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.15);
        }

        .questao {
            margin-bottom: 30px;
            padding: 22px;
            border-radius: 12px;
            background: #f8fffd;
            border: 1px solid #b2dfdb;
        }

        .questao h2 {
            font-size: 19px;
            color: #00695c;
            margin-top: 0;
        }

        .tema {
            display: inline-block;
            background: #80cbc4;
            color: #004d40;
            padding: 5px 10px;
            border-radius: 20px;
            font-size: 13px;
            font-weight: bold;
            margin-bottom: 10px;
        }

        label {
            display: block;
            padding: 12px;
            margin: 7px 0;
            border-radius: 8px;
            cursor: pointer;
            transition: 0.2s;
        }

        label:hover {
            background: #e0f2f1;
        }

        input[type="radio"] {
            margin-right: 10px;
        }

        .feedback {
            display: none;
            margin-top: 15px;
            padding: 12px;
            border-radius: 8px;
            font-weight: bold;
        }

        .correto {
            display: block;
            background: #dcedc8;
            color: #33691e;
        }

        .incorreto {
            display: block;
            background: #ffcdd2;
            color: #b71c1c;
        }

        button {
            display: block;
            margin: 35px auto 10px;
            padding: 16px 35px;
            border: none;
            border-radius: 10px;
            background: #00695c;
            color: white;
            font-size: 18px;
            font-weight: bold;
            cursor: pointer;
        }

        button:hover {
            background: #004d40;
        }

        #resultado {
            display: none;
            margin-top: 35px;
            padding: 30px;
            text-align: center;
            border-radius: 12px;
            background: #e0f2f1;
        }

        #resultado h2 {
            color: #00695c;
        }

        #pontuacao {
            font-size: 32px;
            font-weight: bold;
            color: #00695c;
        }

        .barra {
            width: 100%;
            height: 25px;
            background: #cfd8dc;
            border-radius: 20px;
            overflow: hidden;
            margin: 20px 0;
        }

        #progresso {
            height: 100%;
            width: 0%;
            background: #26a69a;
            transition: width 1s;
        }

        footer {
            text-align: center;
            padding: 25px;
            color: #607d8b;
        }
    </style>
</head>

<body>

<header>

    <h1>🌎 Quiz: Ecossistemas do Nosso Planeta</h1>

    <p>
        Vida marinha, florestas, manguezais, rios, recifes de coral
        e biodiversidade
    </p>

</header>


<div class="container">

    <p>
        <strong>Instruções:</strong>
        escolha uma alternativa em cada questão.
        Cada questão vale <strong>1 ponto</strong>.
        A resposta correta somente será revelada depois que você clicar
        em <strong>Corrigir Questionário</strong>.
    </p>


    <form id="quiz">


        <!-- QUESTÃO 1 -->

        <div class="questao">

            <span class="tema">🌊 Vida Marinha</span>

            <h2>
                1. Por que os oceanos são importantes para o equilíbrio
                do planeta?
            </h2>

            <label>
                <input type="radio" name="q1" value="A">
                A) Porque produzem apenas água doce.
            </label>

            <label>
                <input type="radio" name="q1" value="B">
                B) Porque participam da regulação do clima e abrigam
                grande parte da biodiversidade.
            </label>

            <label>
                <input type="radio" name="q1" value="C">
                C) Porque não possuem influência sobre o clima.
            </label>

            <label>
                <input type="radio" name="q1" value="D">
                D) Porque são formados apenas por animais.
            </label>

            <div id="feedback1" class="feedback"></div>

        </div>


        <!-- QUESTÃO 2 -->

        <div class="questao">

            <span class="tema">🪸 Recifes de Coral</span>

            <h2>
                2. Qual é uma das principais ameaças aos recifes de coral?
            </h2>

            <label>
                <input type="radio" name="q2" value="A">
                A) Aumento da biodiversidade.
            </label>

            <label>
                <input type="radio" name="q2" value="B">
                B) Crescimento das algas marinhas.
            </label>

            <label>
                <input type="radio" name="q2" value="C">
                C) Aquecimento dos oceanos e acidificação da água.
            </label>

            <label>
                <input type="radio" name="q2" value="D">
                D) Aumento da quantidade de peixes.
            </label>

            <div id="feedback2" class="feedback"></div>

        </div>


        <!-- QUESTÃO 3 -->

        <div class="questao">

            <span class="tema">🐠 Animais Marinhos</span>

            <h2>
                3. Qual animal é conhecido por realizar longas migrações
                pelos oceanos?
            </h2>

            <label>
                <input type="radio" name="q3" value="A">
                A) Baleia-jubarte.
            </label>

            <label>
                <input type="radio" name="q3" value="B">
                B) Tatu.
            </label>

            <label>
                <input type="radio" name="q3" value="C">
                C) Tamanduá.
            </label>

            <label>
                <input type="radio" name="q3" value="D">
                D) Capivara.
            </label>

            <div id="feedback3" class="feedback"></div>

        </div>


        <!-- QUESTÃO 4 -->

        <div class="questao">

            <span class="tema">🌳 Florestas</span>

            <h2>
                4. Qual é uma função importante das florestas?
            </h2>

            <label>
                <input type="radio" name="q4" value="A">
                A) Impedir completamente a formação de chuvas.
            </label>

            <label>
                <input type="radio" name="q4" value="B">
                B) Abrigar espécies e participar do ciclo da água e
                do carbono.
            </label>

            <label>
                <input type="radio" name="q4" value="C">
                C) Produzir apenas madeira.
            </label>

            <label>
                <input type="radio" name="q4" value="D">
                D) Eliminar todos os gases da atmosfera.
            </label>

            <div id="feedback4" class="feedback"></div>

        </div>


        <!-- QUESTÃO 5 -->

        <div class="questao">

            <span class="tema">🌿 Floresta Amazônica</span>

            <h2>
                5. Qual característica é marcante na Floresta Amazônica?
            </h2>

            <label>
                <input type="radio" name="q5" value="A">
                A) Baixa diversidade de espécies.
            </label>

            <label>
                <input type="radio" name="q5" value="B">
                B) Predomínio de clima extremamente seco.
            </label>

            <label>
                <input type="radio" name="q5" value="C">
                C) Grande biodiversidade e elevada quantidade de
                florestas tropicais.
            </label>

            <label>
                <input type="radio" name="q5" value="D">
                D) Ausência de rios.
            </label>

            <div id="feedback5" class="feedback"></div>

        </div>


        <!-- QUESTÃO 6 -->

        <div class="questao">

            <span class="tema">🌱 Manguezais</span>

            <h2>
                6. Por que os manguezais são importantes para a vida marinha?
            </h2>

            <label>
                <input type="radio" name="q6" value="A">
                A) Porque funcionam como áreas de abrigo e reprodução
                para diversas espécies.
            </label>

            <label>
                <input type="radio" name="q6" value="B">
                B) Porque não possuem animais.
            </label>

            <label>
                <input type="radio" name="q6" value="C">
                C) Porque transformam água salgada em petróleo.
            </label>

            <label>
                <input type="radio" name="q6" value="D">
                D) Porque existem somente em desertos.
            </label>

            <div id="feedback6" class="feedback"></div>

        </div>


        <!-- QUESTÃO 7 -->

        <div class="questao">

            <span class="tema">🦀 Manguezais</span>

            <h2>
                7. Qual animal pode ser encontrado em áreas de manguezal?
            </h2>

            <label>
                <input type="radio" name="q7" value="A">
                A) Caranguejo.
            </label>

            <label>
                <input type="radio" name="q7" value="B">
                B) Urso-polar.
            </label>

            <label>
                <input type="radio" name="q7" value="C">
                C) Pinguim-imperador.
            </label>

            <label>
                <input type="radio" name="q7" value="D">
                D) Rena.
            </label>

            <div id="feedback7" class="feedback"></div>

        </div>


        <!-- QUESTÃO 8 -->

        <div class="questao">

            <span class="tema">🐟 Rios e Lagos</span>

            <h2>
                8. O que pode acontecer quando um rio recebe grande
                quantidade de poluentes?
            </h2>

            <label>
                <input type="radio" name="q8" value="A">
                A) A água sempre fica mais saudável.
            </label>

            <label>
                <input type="radio" name="q8" value="B">
                B) A biodiversidade pode diminuir e os organismos
                aquáticos podem ser prejudicados.
            </label>

            <label>
                <input type="radio" name="q8" value="C">
                C) Todos os peixes ficam maiores.
            </label>

            <label>
                <input type="radio" name="q8" value="D">
                D) O rio deixa imediatamente de existir.
            </label>

            <div id="feedback8" class="feedback"></div>

        </div>


        <!-- QUESTÃO 9 -->

        <div class="questao">

            <span class="tema">🦋 Polinização</span>

            <h2>
                9. Qual é a importância das abelhas para muitos
                ecossistemas?
            </h2>

            <label>
                <input type="radio" name="q9" value="A">
                A) Elas realizam a polinização de muitas plantas.
            </label>

            <label>
                <input type="radio" name="q9" value="B">
                B) Elas eliminam todas as pragas.
            </label>

            <label>
                <input type="radio" name="q9" value="C">
                C) Elas produzem oxigênio por meio da fotossíntese.
            </label>

            <label>
                <input type="radio" name="q9" value="D">
                D) Elas vivem exclusivamente dentro dos oceanos.
            </label>

            <div id="feedback9" class="feedback"></div>

        </div>


        <!-- QUESTÃO 10 -->

        <div class="questao">

            <span class="tema">🐊 Pantanal</span>

            <h2>
                10. Qual característica destaca o Pantanal?
            </h2>

            <label>
                <input type="radio" name="q10" value="A">
                A) É uma região sem água.
            </label>

            <label>
                <input type="radio" name="q10" value="B">
                B) Possui ciclos de cheias e secas que influenciam
                a vida dos organismos.
            </label>

            <label>
                <input type="radio" name="q10" value="C">
                C) É formado somente por desertos.
            </label>

            <label>
                <input type="radio" name="q10" value="D">
                D) Não possui animais.
            </label>

            <div id="feedback10" class="feedback"></div>

        </div>


        <!-- QUESTÃO 11 -->

        <div class="questao">

            <span class="tema">🏜️ Desertos</span>

            <h2>
                11. Como muitos organismos de regiões desérticas
                conseguem sobreviver?
            </h2>

            <label>
                <input type="radio" name="q11" value="A">
                A) Adaptando-se à escassez de água e às temperaturas
                extremas.
            </label>

            <label>
                <input type="radio" name="q11" value="B">
                B) Dependendo de chuvas constantes durante todo o ano.
            </label>

            <label>
                <input type="radio" name="q11" value="C">
                C) Vivendo exclusivamente dentro de rios.
            </label>

            <label>
                <input type="radio" name="q11" value="D">
                D) Evitando completamente qualquer adaptação.
            </label>

            <div id="feedback11" class="feedback"></div>

        </div>


        <!-- QUESTÃO 12 -->

        <div class="questao">

            <span class="tema">🦈 Cadeia Alimentar Marinha</span>

            <h2>
                12. Em uma cadeia alimentar marinha, qual organismo
                pode atuar como consumidor de outros animais?
            </h2>

            <label>
                <input type="radio" name="q12" value="A">
                A) Fitoplâncton.
            </label>

            <label>
                <input type="radio" name="q12" value="B">
                B) Alga.
            </label>

            <label>
                <input type="radio" name="q12" value="C">
                C) Tubarão.
            </label>

            <label>
                <input type="radio" name="q12" value="D">
                D) Planta aquática.
            </label>

            <div id="feedback12" class="feedback"></div>

        </div>


        <!-- QUESTÃO 13 -->

        <div class="questao">

            <span class="tema">🌎 Biodiversidade</span>

            <h2>
                13. O que pode acontecer quando uma espécie desaparece
                de um ecossistema?
            </h2>

            <label>
                <input type="radio" name="q13" value="A">
                A) Nunca ocorre nenhuma consequência.
            </label>

            <label>
                <input type="radio" name="q13" value="B">
                B) As relações alimentares e o equilíbrio do ecossistema
                podem ser alterados.
            </label>

            <label>
                <input type="radio" name="q13" value="C">
                C) Todas as outras espécies desaparecem imediatamente.
            </label>

            <label>
                <input type="radio" name="q13" value="D">
                D) O ecossistema sempre fica mais saudável.
            </label>

            <div id="feedback13" class="feedback"></div>

        </div>


        <!-- QUESTÃO 14 -->

        <div class="questao">

            <span class="tema">♻️ Conservação</span>

            <h2>
                14. Qual atitude contribui para a conservação dos
                ecossistemas?
            </h2>

            <label>
                <input type="radio" name="q14" value="A">
                A) Jogar lixo em rios.
            </label>

            <label>
                <input type="radio" name="q14" value="B">
                B) Destruir áreas de vegetação nativa.
            </label>

            <label>
                <input type="radio" name="q14" value="C">
                C) Preservar habitats e reduzir a poluição.
            </label>

            <label>
                <input type="radio" name="q14" value="D">
                D) Retirar animais silvestres da natureza.
            </label>

            <div id="feedback14" class="feedback"></div>

        </div>


        <!-- QUESTÃO 15 -->

        <div class="questao">

            <span class="tema">🌡️ Mudanças Climáticas</span>

            <h2>
                15. Como as mudanças climáticas podem afetar os ecossistemas?
            </h2>

            <label>
                <input type="radio" name="q15" value="A">
                A) Não provocam nenhuma alteração nos seres vivos.
            </label>

            <label>
                <input type="radio" name="q15" value="B">
                B) Podem alterar habitats, temperaturas, disponibilidade
                de água e distribuição de espécies.
            </label>

            <label>
                <input type="radio" name="q15" value="C">
                C) Fazem todas as espécies se adaptarem imediatamente.
            </label>

            <label>
                <input type="radio" name="q15" value="D">
                D) Afetam somente os desertos.
            </label>

            <div id="feedback15" class="feedback"></div>

        </div>


        <button type="button" onclick="corrigirQuiz()">
            ✅ Corrigir Questionário
        </button>

    </form>


    <!-- RESULTADO -->

    <div id="resultado">

        <h2>🏆 Resultado do Questionário</h2>

        <p id="pontuacao"></p>

        <div class="barra">
            <div id="progresso"></div>
        </div>

        <p id="porcentagem"></p>

        <p id="mensagem"></p>

    </div>

</div>


<footer>
    Quiz educativo sobre ecossistemas 🌱🌊🐠🌳
</footer>


<script>

function corrigirQuiz() {

    // Gabarito
    const respostas = {

        q1: "B",
        q2: "C",
        q3: "A",
        q4: "B",
        q5: "C",
        q6: "A",
        q7: "A",
        q8: "B",
        q9: "A",
        q10: "B",
        q11: "A",
        q12: "C",
        q13: "B",
        q14: "C",
        q15: "B"

    };


    let pontuacao = 0;


    // Verificar cada questão
    for (let i = 1; i <= 15; i++) {

        const pergunta = "q" + i;

        const selecionada =
            document.querySelector(
                `input[name="${pergunta}"]:checked`
            );

        const feedback =
            document.getElementById(
                "feedback" + i
            );


        feedback.className = "feedback";


        // Questão não respondida
        if (!selecionada) {

            feedback.innerHTML =
                "⚠️ Não respondida. " +
                "A alternativa correta é: " +
                respostas[pergunta] + ".";

            feedback.classList.add("incorreto");

        }


        // Resposta correta
        else if (
            selecionada.value ===
            respostas[pergunta]
        ) {

            pontuacao++;

            feedback.innerHTML =
                "✅ Correto! " +
                "A alternativa " +
                respostas[pergunta] +
                " é a resposta correta.";

            feedback.classList.add("correto");

        }


        // Resposta errada
        else {

            feedback.innerHTML =
                "❌ Incorreto. " +
                "A alternativa correta é: " +
                respostas[pergunta] + ".";

            feedback.classList.add("incorreto");

        }

    }


    // Porcentagem
    const porcentagem =
        (pontuacao / 15) * 100;


    // Mostrar pontuação
    document.getElementById(
        "pontuacao"
    ).innerHTML =
        "🎯 " +
        pontuacao +
        " / 15 pontos";


    // Mostrar porcentagem
    document.getElementById(
        "porcentagem"
    ).innerHTML =
        "Você acertou " +
        porcentagem.toFixed(1) +
        "% das questões.";


    // Barra de progresso
    document.getElementById(
        "progresso"
    ).style.width =
        porcentagem + "%";


    // Mensagem de desempenho
    let mensagem;


    if (pontuacao === 15) {

        mensagem =
            "🌟 Perfeito! Você acertou todas as questões!";

    }

    else if (pontuacao >= 13) {

        mensagem =
            "🏆 Excelente! Você demonstra um conhecimento muito bom sobre os ecossistemas.";

    }

    else if (pontuacao >= 10) {

        mensagem =
            "👏 Muito bom! Você possui um ótimo conhecimento sobre os diferentes ecossistemas.";

    }

    else if (pontuacao >= 7) {

        mensagem =
            "👍 Bom trabalho! Você já conhece vários aspectos dos ecossistemas, mas pode continuar estudando.";

    }

    else {

        mensagem =
            "📚 Continue estudando! Revise os conteúdos sobre vida marinha, florestas, manguezais e biodiversidade.";

    }


    document.getElementById(
        "mensagem"
    ).innerHTML = mensagem;


    // Mostrar resultado
    document.getElementById(
        "resultado"
    ).style.display = "block";


    // Rolar até o resultado
    document.getElementById(
        "resultado"
    ).scrollIntoView({
        behavior: "smooth"
    });

}

</script>

</body>
</html>
