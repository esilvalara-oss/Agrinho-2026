<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Monster Eco-High: Desafio Agrinho</title>
    <link href="https://fonts.googleapis.com/css2?family=Creepster&family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            background-color: #121212;
            color: #ffffff;
            margin: 0;
            padding: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
            background-image: radial-gradient(circle, #2a0845 0%, #121212 80%);
            min-height: 100vh;
        }

        header {
            text-align: center;
            margin-bottom: 30px;
        }

        h1 {
            font-family: 'Creepster', cursive;
            color: #ff1493;
            font-size: 3.5rem;
            margin: 0;
            text-shadow: 3px 3px #39ff14;
            letter-spacing: 2px;
        }

        h2 {
            font-size: 1.2rem;
            color: #39ff14;
            margin-top: 5px;
        }

        .game-container {
            background-color: #1e1e1e;
            border: 4px solid #ff1493;
            border-radius: 15px;
            padding: 30px;
            max-width: 600px;
            width: 100%;
            box-shadow: 0 0 20px rgba(57, 255, 20, 0.5);
            text-align: center;
        }

        /* Estilo da imagem da personagem */
        .character-img {
            width: 150px;
            height: 150px;
            object-fit: cover;
            border-radius: 50%;
            border: 4px solid #39ff14;
            margin-bottom: 20px;
            box-shadow: 0 0 15px #ff1493;
            display: none; /* Escondido por padrão até o jogo começar */
        }

        .question-text {
            font-size: 1.5rem;
            margin-bottom: 20px;
            color: #fff;
        }

        .btn-container {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .btn {
            background-color: #2a2a2a;
            color: #ff1493;
            border: 2px solid #ff1493;
            padding: 15px;
            font-size: 1.1rem;
            font-weight: bold;
            border-radius: 8px;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .btn:hover {
            background-color: #ff1493;
            color: #fff;
            box-shadow: 0 0 10px #ff1493;
        }

        .btn.correct {
            background-color: #39ff14;
            color: #000;
            border-color: #39ff14;
        }

        .btn.wrong {
            background-color: #ff0000;
            color: #fff;
            border-color: #ff0000;
        }

        .hide {
            display: none !important;
        }

        #next-btn, #restart-btn {
            margin-top: 20px;
            background-color: #39ff14;
            color: #000;
            border: none;
            padding: 10px 20px;
            font-size: 1.2rem;
            font-weight: bold;
            border-radius: 5px;
            cursor: pointer;
        }

        #next-btn:hover, #restart-btn:hover {
            background-color: #2eb80f;
        }

        .score-section {
            font-size: 2rem;
            font-family: 'Creepster', cursive;
            color: #ff1493;
        }
    </style>
</head>
<body>

    <header>
        <h1>Monster Eco-High</h1>
        <h2>Tema Agrinho: Agro forte, futuro sustentável</h2>
    </header>

    <div class="game-container">
        <div id="start-screen">
            <p class="question-text">As monstrinhas precisam da sua ajuda para tornar a fazenda da escola sustentável! Você consegue equilibrar a produção e salvar o meio ambiente?</p>
            <button class="btn" id="start-btn" style="background-color: #ff1493; color: white;">Iniciar Desafio!</button>
        </div>

        <div id="game-screen" class="hide">
            <img id="character-pic" class="character-img" src="" alt="Personagem">
            
            <div id="question" class="question-text">Pergunta aqui</div>
            <div id="answer-buttons" class="btn-container"></div>
            <button id="next-btn" class="hide">Próxima Pergunta</button>
        </div>

        <div id="result-screen" class="hide">
            <div class="score-section">
                Você acertou <span id="score">0</span> de <span id="total-questions">0</span> perguntas!
            </div>
            <p id="final-message" class="message"></p>
            <button id="restart-btn">Jogar Novamente</button>
        </div>
    </div>

    <script>
        const startButton = document.getElementById('start-btn');
        const nextButton = document.getElementById('next-btn');
        const restartButton = document.getElementById('restart-btn');
        const startScreen = document.getElementById('start-screen');
        const gameScreen = document.getElementById('game-screen');
        const resultScreen = document.getElementById('result-screen');
        const questionElement = document.getElementById('question');
        const answerButtonsElement = document.getElementById('answer-buttons');
        const scoreElement = document.getElementById('score');
        const totalQuestionsElement = document.getElementById('total-questions');
        const finalMessageElement = document.getElementById('final-message');
        const characterPicElement = document.getElementById('character-pic'); // Elemento da imagem

        let currentQuestionIndex = 0;
        let score = 0;

        // Perguntas com Imagens e Personagens
        const questions = [
            {
                character: "Frankie Stein",
                imgUrl: "https://placehold.co/150x150/2a0845/39ff14?text=Frankie", // Troque este link pela foto real da Frankie
                question: "A Frankie Stein quer gerar energia elétrica para as máquinas da fazenda sem poluir o ar. Qual a melhor escolha?",
                answers: [
                    { text: "Queimar carvão vegetal", correct: false },
                    { text: "Instalar painéis de energia solar e turbinas eólicas", correct: true },
                    { text: "Usar geradores a diesel o dia todo", correct: false }
                ]
            },
            {
                character: "Draculaura",
                imgUrl: "https://placehold.co/150x150/ff1493/ffffff?text=Draculaura", // Troque este link
                question: "Draculaura adora tomates, mas os prefere orgânicos e saudáveis. O que caracteriza uma plantação orgânica?",
                answers: [
                    { text: "Cultivo sem uso de agrotóxicos e adubos químicos prejudiciais", correct: true },
                    { text: "Plantar apenas tomates vermelhos em estufas de plástico", correct: false },
                    { text: "Usar muito inseticida para não ter nenhum bichinho", correct: false }
                ]
            },
            {
                character: "Lagoona Blue",
                imgUrl: "https://placehold.co/150x150/00ffff/000000?text=Lagoona", // Troque este link
                question: "Lagoona Blue está preocupada com o rio que passa perto das plantações. Como o agro sustentável protege as águas?",
                answers: [
                    { text: "Desmatando tudo até a beira da água", correct: false },
                    { text: "Preservando a mata ciliar (vegetação nas margens)", correct: true },
                    { text: "Jogando os restos de colheita na água", correct: false }
                ]
            },
            {
                character: "Cleo de Nile",
                imgUrl: "https://placehold.co/150x150/ffd700/000000?text=Cleo", // Troque este link
                question: "A Cleo de Nile quer aumentar a produção da fazenda, mas sabe que precisa cuidar do solo para o futuro. O que ela deve fazer?",
                answers: [
                    { text: "Plantar a mesma coisa todo ano até o solo esgotar", correct: false },
                    { text: "Fazer rotação de culturas e usar adubação verde", correct: true },
                    { text: "Queimar o solo antes de cada plantio", correct: false }
                ]
            },
            {
                character: "Clawdeen Wolf",
                imgUrl: "https://placehold.co/150x150/8a2be2/ffffff?text=Clawdeen", // Troque este link
                question: "Clawdeen Wolf está desenhando roupas e quer usar materiais agrícolas sustentáveis. O que ela deve escolher?",
                answers: [
                    { text: "Algodão agroecológico, que usa menos água e preserva o solo", correct: true },
                    { text: "Peles de animais silvestres", correct: false },
                    { text: "Plásticos descartáveis misturados na terra", correct: false }
                ]
            },
            {
                character: "Ghoulia Yelps",
                imgUrl: "https://placehold.co/150x150/ff0000/ffffff?text=Ghoulia", // Troque este link
                question: "Ghoulia Yelps calculou que a fazenda gasta muita água na irrigação tradicional. Qual tecnologia inteligente ela pode aplicar?",
                answers: [
                    { text: "Inundar a plantação todos os dias", correct: false },
                    { text: "Irrigação por gotejamento conectada a sensores de umidade", correct: true },
                    { text: "Esperar chover e não usar tecnologia alguma", correct: false }
                ]
            }
        ];

        startButton.addEventListener('click', startGame);
        nextButton.addEventListener('click', () => {
            currentQuestionIndex++;
            setNextQuestion();
        });
        restartButton.addEventListener('click', startGame);

        function startGame() {
            startScreen.classList.add('hide');
            resultScreen.classList.add('hide');
            gameScreen.classList.remove('hide');
            currentQuestionIndex = 0;
            score = 0;
            setNextQuestion();
        }

        function setNextQuestion() {
            resetState();
            showQuestion(questions[currentQuestionIndex]);
        }

        function showQuestion(question) {
            // Atualiza a imagem da monstrinha
            characterPicElement.src = question.imgUrl;
            characterPicElement.alt = question.character;
            characterPicElement.style.display = 'block';

            // Atualiza o texto da pergunta
            questionElement.innerText = question.question;
            
            // Gera os botões
            question.answers.forEach(answer => {
                const button = document.createElement('button');
                button.innerText = answer.text;
                button.classList.add('btn');
                if (answer.correct) {
                    button.dataset.correct = answer.correct;
                }
                button.addEventListener('click', selectAnswer);
                answerButtonsElement.appendChild(button);
            });
        }

        function resetState() {
            nextButton.classList.add('hide');
            while (answerButtonsElement.firstChild) {
                answerButtonsElement.removeChild(answerButtonsElement.firstChild);
            }
        }

        function selectAnswer(e) {
            const selectedButton = e.target;
            const correct = selectedButton.dataset.correct === "true";
            
            if (correct) {
                score++;
                selectedButton.classList.add('correct');
            } else {
                selectedButton.classList.add('wrong');
                Array.from(answerButtonsElement.children).forEach(button => {
                    if (button.dataset.correct === "true") {
                        button.classList.add('correct');
                    }
                });
            }

            Array.from(answerButtonsElement.children).forEach(button => {
                button.disabled = true;
                button.style.cursor = 'not-allowed';
            });

            if (questions.length > currentQuestionIndex + 1) {
                nextButton.classList.remove('hide');
            } else {
                setTimeout(showResults, 1500);
            }
        }

        function showResults() {
            gameScreen.classList.add('hide');
            resultScreen.classList.remove('hide');
            scoreElement.innerText = score;
            totalQuestionsElement.innerText = questions.length;

            if (score === questions.length) {
                finalMessageElement.innerText = "Assustadoramente Sustentável! Você entende tudo de equilíbrio ambiental!";
                finalMessageElement.style.color = "#39ff14";
            } else if (score >= questions.length / 2) {
                finalMessageElement.innerText = "Eletrizante! Você tem potencial, mas ainda pode aprender mais com as monstrinhas.";
                finalMessageElement.style.color = "#ffff00";
            } else {
                finalMessageElement.innerText = "Que desastre monstruoso! Precisamos estudar mais sobre sustentabilidade no agronegócio.";
                finalMessageElement.style.color = "#ff0000";
            }
        }
    </script>
</body>
</html>
