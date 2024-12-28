<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Truth or Dare Game</title>
    <link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
</head>
<style>
/* Basic page styling */
body {
    font-family: 'Pacifico', cursive;
    margin: 0;
    padding: 0;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background: linear-gradient(45deg, #ffb3b3, #ffccff);
    animation: backgroundAnimation 6s infinite alternate;
    overflow: hidden;
    position: relative;
    flex-direction: column;
    text-align: center;
}

/* Button styling */
.button {
    background-color: #ff99cc;
    border: none;
    color: white;
    padding: 20px 40px;
    font-size: 1.5em;
    cursor: pointer;
    border-radius: 25px;
    box-shadow: 0 0 15px #ff80bf;
    transition: all 0.4s cubic-bezier(0.68, -0.55, 0.27, 1.55);
    position: relative;
    overflow: hidden;
    margin-top: 20px;
}

.button:hover {
    transform: scale(1.1);
    box-shadow: 0 0 25px #ff80bf, 0 0 35px #ff99cc;
    background-color: #ff80bf;
}

.button:before {
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    width: 300%;
    height: 300%;
    background: #fff;
    transition: width 0.4s, height 0.4s, top 0.4s, left 0.4s;
    border-radius: 50%;
    z-index: 0;
    transform: translate(-50%, -50%);
}

.button:hover:before {
    width: 0;
    height: 0;
    top: 50%;
    left: 50%;
}

.button span {
    position: relative;
    z-index: 1;
}

/* Game title */
h1 {
    font-size: 3em;
    color: #ff80bf;
    margin-bottom: 20px;
    font-weight: bold;
    text-shadow: 0 0 10px #fff, 0 0 20px #ff99cc;
}

/* Love emoji flying randomly */
.love-emojis {
    position: absolute;
    font-size: 30px;
    animation: loveFlow 4s linear infinite;
    z-index: -1;
}

@keyframes loveFlow {
    0% {
        top: -100px;
        left: -100px;
        opacity: 1;
    }
    100% {
        top: 100vh;
        left: 100vw;
        opacity: 0;
    }
}

/* Styling for truth and dare text */
.truth, .dare {
    display: none;
    color: #ff80bf;
    font-weight: bold;
    font-size: 1.8em;
    margin-top: 20px;
    animation: shine 1s infinite alternate;
    margin-bottom: 20px;
}

/* Shine effect */
@keyframes shine {
    0% {
        text-shadow: 0 0 10px #fff, 0 0 20px #ff99cc, 0 0 30px #ffccff;
    }
    100% {
        text-shadow: 0 0 20px #fff, 0 0 30px #ff99cc, 0 0 40px #ffccff;
    }
}

/* Input fields */
.input-container {
    text-align: center;
    margin-bottom: 20px;
}

input {
    padding: 10px;
    font-size: 1.2em;
    margin: 10px;
    width: 250px;
    border-radius: 10px;
    border: 1px solid #ff80bf;
}

/* VS section */
.vs {
    font-size: 2.5em;
    color: #ff80bf;
    font-weight: bold;
    margin-top: 20px;
    margin-bottom: 40px;
}

/* Flex container for game content */
.game-content {
    display: none;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

/* Buttons layout */
#nextButton, #truthButton, #dareButton {
    display: none;
}

/* Mobile responsiveness */
@media (max-width: 600px) {
    .button {
        padding: 15px 30px;
        font-size: 1.2em;
    }
    h1 {
        font-size: 2em;
    }
}

/* Background animation */
@keyframes backgroundAnimation {
    0% {
        background: linear-gradient(45deg, #ffb3b3, #ffccff);
    }
    50% {
        background: linear-gradient(45deg, #ffccff, #ff99cc);
    }
    100% {
        background: linear-gradient(45deg, #ffb3b3, #ffccff);
    }
}

/* Active button effect */
.button:active {
    opacity: 0.8;
}
</style>
<body>
    <!-- Love emojis flying randomly across the screen -->
    <div class="love-emojis">❤️</div>

    <div>
        <h1>Truth or Dare Game</h1>

        <!-- Language selection -->
        <div>
            <select id="languageSelect">
                <option value="en">English</option>
                <option value="te">Telugu</option>
            </select>
        </div>

        <!-- Player input section -->
        <div class="input-container">
            <input type="text" id="player1" placeholder="Enter Player 1 Name">
            <input type="text" id="player2" placeholder="Enter Player 2 Name">
            <button class="button" id="startButton"><span>Start Game</span></button>
        </div>

        <!-- Game content section -->
        <div class="game-content">
            <div id="vsDisplay" class="vs"></div>
            <div id="gameText" class="gameText"></div>
            <div id="truth" class="truth"></div>
            <div id="dare" class="dare"></div>
            <button class="button" id="nextButton"><span>Next Turn</span></button>
            <button class="button" id="truthButton"><span>Truth</span></button>
            <button class="button" id="dareButton"><span>Dare</span></button>
        </div>

        <!-- Scoreboard -->
        <div id="scoreDisplay" style="font-size: 1.5em; color: #ff80bf; margin-top: 20px;">
            Player 1: 0 | Player 2: 0
        </div>
    </div>

<script>
// Truth and Dare questions
const truths = [
    { "en": "What is the one thing you are most ashamed of?", "te": "మీరు అత్యంత లజ్జపడ్డ విషయమేమిటి?" },
    { "en": "Have you ever had a crush on someone in this room?", "te": "ఈ గదిలో ఉన్నవారిలో ఎవరిపై మీరు క్రష్ పడారూ?" },
    { "en": "If you could change one thing about your past, what would it be?", "te": "మీ భూతకాలం గురించి ఒక విషయం మార్చవలసిన పట్ల ఎంచుకోగలిగితే అది ఏమిటి?" },
    { "en": "Have you ever lied to get out of a situation?", "te": "ఏదైనా పరిస్థితి నుండి తప్పించడానికి మీరు నకిలీ చెప్పారు?" },
    { "en": "What’s the most embarrassing thing you’ve ever done in front of someone?", "te": "మీరు ఎవరినీ ముందు చేసిన అత్యంత అవమానకరమైన విషయం ఏమిటి?" },
    { "en": "What’s something you’ve never told anyone?", "te": "మీరు ఎప్పటికీ చెప్పని విషయం ఏమిటి?" },
    { "en": "If you were invisible for a day, what would you do?", "te": "మీరు ఒక రోజు కనిపించకపోతే, మీరు ఏమి చేస్తారు?" },
    { "en": "What’s the worst date you’ve ever been on?", "te": "మీరు వెళ్లిన అత్యంత చెడు డేట్ ఏమిటి?" },
    { "en": "Who is your secret crush?", "te": "మీ రహస్య క్రష్ ఎవరు?" },
    { "en": "If you could switch lives with someone for a day, who would it be?", "te": "ఒక రోజు ఇతరుల జీవితాన్ని మార్చగలిగితే, ఎవరితో అది మారుస్తారు?" }
];

const dares = [
    { "en": "Dance for 1 minute without music.", "te": "సంగీతం లేకుండా 1 నిమిషం నృత్యం చేయండి." },
    { "en": "Text your crush and say you like them.", "te": "మీ క్రష్ కు సందేశం పంపించి వారిని మీరు ఇష్టపడతారని చెప్పండి." },
    { "en": "Do an impression of someone in the room.", "te": "గదిలో ఉన్న ఎవరి కాపీని మీరు చేయండి." },
    { "en": "Post an embarrassing photo on your social media.", "te": "మీ సోషల్ మీడియా లో ఒక అవమానకరమైన ఫోటో పోస్ట్ చేయండి." },
    { "en": "Speak in an accent until your next turn.", "te": "మీ తదుపరి టర్న్ వరకు ఒక లహిరి మాట్లాడండి." },
    { "en": "Try to lick your elbow.", "te": "మీ ఎల్బోను లిక్కు చేయాలని ప్రయత్నించండి." },
    { "en": "Let the person to your left draw on your face with a marker.", "te": "మీ ఎడమవైపున ఉన్న వ్యక్తికి మార్కర్‌తో మీ ముఖంపై గీయడానికి అనుమతించండి." },
    { "en": "Call your crush and sing them a song.", "te": "మీ క్రష్ కి కాల్ చేసి వారికీ ఒక పాట పాడండి." },
    { "en": "Do 20 push-ups.", "te": "20 పుష్-అప్స్ చేయండి." },
    { "en": "Imitate a celebrity until someone guesses who it is.", "te": "ఒక సెలబ్రిటి‌ను అనుకరించండి, ఎవరైనా దాన్ని అంచనా వేయించే వరకు." }
];

let player1Name, player2Name;
let player1Score = 0, player2Score = 0;
let currentPlayer = 1;  // 1 for Player 1, 2 for Player 2
let selectedLanguage = "en";

// Start game function
function startGame() {
    player1Name = document.getElementById("player1").value;
    player2Name = document.getElementById("player2").value;

    if (!player1Name || !player2Name) {
        alert("Please enter both player names.");
        return;
    }

    document.querySelector(".input-container").style.display = "none";
    document.querySelector(".game-content").style.display = "flex";
    document.getElementById("vsDisplay").innerHTML = `${player1Name} VS ${player2Name}`;
    document.getElementById("scoreDisplay").innerText = `Player 1: 0 | Player 2: 0`;

    updateGame();
}

// Update the game text based on the current player
function updateGame() {
    document.getElementById("truth").style.display = "none";
    document.getElementById("dare").style.display = "none";
    document.getElementById("gameText").innerHTML = `${currentPlayer === 1 ? player1Name : player2Name}'s Turn!`;
    document.getElementById("truthButton").style.display = "block";
    document.getElementById("dareButton").style.display = "block";
    document.getElementById("nextButton").style.display = "none";
}

// Select and show a truth or dare
function selectTruthOrDare(type) {
    let selectedOption;
    const availableList = type === 'truth' ? truths : dares;
    const randomIndex = Math.floor(Math.random() * availableList.length);
    selectedOption = availableList[randomIndex];

    if (selectedLanguage === "te") {
        selectedOption = selectedOption.te;
    } else {
        selectedOption = selectedOption.en;
    }

    // Display the result
    if (type === 'truth') {
        document.getElementById("truth").style.display = "block";
        document.getElementById("truth").innerHTML = selectedOption;
    } else {
        document.getElementById("dare").style.display = "block";
        document.getElementById("dare").innerHTML = selectedOption;
    }

    // Hide buttons and show next button
    document.getElementById("truthButton").style.display = "none";
    document.getElementById("dareButton").style.display = "none";
    document.getElementById("nextButton").style.display = "block";
}

// Move to the next turn
function nextTurn() {
    currentPlayer = currentPlayer === 1 ? 2 : 1;
    updateGame();
}

// Event listeners
document.getElementById("startButton").addEventListener("click", startGame);
document.getElementById("truthButton").addEventListener("click", () => selectTruthOrDare('truth'));
document.getElementById("dareButton").addEventListener("click", () => selectTruthOrDare('dare'));
document.getElementById("nextButton").addEventListener("click", nextTurn);

// Language change event
document.getElementById("languageSelect").addEventListener("change", function() {
    selectedLanguage = this.value;
});

</script>
</body>
</html>
