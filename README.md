#<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>JS & CSS Animation Project</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Animation and JS Demo</h1>

    <!-- Interactive Button -->
    <button id="animateBtn">Animate Box</button>

    <!-- Animated Box -->
    <div id="box"></div>

    <!-- JS Function Demonstration -->
    <button id="greetBtn">Greet Me</button>

    <script src="script.js"></script>
</body>
</html>
 index.html-
body {
    font-family: Arial, sans-serif;
    padding: 20px;
}

/* Box for animation */
#box {
    width: 100px;
    height: 100px;
    background-color: blue;
    margin-top: 20px;
    position: relative;
}

/* Transition Example */
#box.move {
    transition: transform 1s ease-in-out, background-color 1s ease-in-out;
    transform: translateX(300px);
    background-color: red;
}

/* Keyframe Animation Example */
@keyframes bounce {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-50px); }
}

#box.bounce {
    animation: bounce 1s ease infinite;
}
