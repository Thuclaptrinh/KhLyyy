// define questions and answers
const questions = [
    {
        question: 'Ngay ki niem la bn : ',
        answers: ['13/12', '1/12', '15/12', '4/12'],
        correctAnswer: 0
    },
    {
        question: 'Anh Thực thích cai gi ? ',
        answers: ['Tien', 'K.ly', 'laptop', 'Dien thoai'],
        correctAnswer: 2
    },
    {
        question: 'Sau nay anh Thuc se song o dau',
        answers: ['Thanh Hoa', 'Nam Dinh', 'Ha Noi'],
        correctAnswer: 2
    },
    {
        question: 'Nha anh Thuc co bn thanh vien?',
        answers: ['3', '4', '5', '6'],
        correctAnswer: 1
    },
    {
        question: 'Có yêu không ?',
        answers: ['Chac chan r', 'khong'],
        correctAnswer: 0
    },

];

// define game state
let currentQuestionIndex = 0;
let score = 0;

// define functions to update game state and display
function displayQuestion() {
    const currentQuestion = questions[currentQuestionIndex];
    const questionElement = document.getElementById('question');
    questionElement.textContent = currentQuestion.question;

    const answersElement = document.getElementById('answers');
    answersElement.innerHTML = '';
    currentQuestion.answers.forEach((answer, index) => {
        const answerElement = document.createElement('button');
        answerElement.textContent = answer;
        answerElement.addEventListener('click', () => {
            checkAnswer(index);
        });
        answersElement.appendChild(answerElement);
    });
}

function checkAnswer(answerIndex) {
    const currentQuestion = questions[currentQuestionIndex];
    if (answerIndex === currentQuestion.correctAnswer) {
        alert('Yeah chuan day');
        score++;
    } else {
        alert('Nguoi la ai ???');
    }
    currentQuestionIndex++;
    if (currentQuestionIndex < questions.length) {
        displayQuestion();
    } else {
        displayScore();
    }
}

function displayScore() {
    alert(`Your score: ${score}`);
    if(score == 5) {
        alert("Hello iuuu . ");

    }
    else {
        alert(" Do gia mao !! cut ngay !!!")
    }
}

// start game
displayQuestion();
