<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Love Question</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            text-align: center;
            margin: 20vh auto;
        }

        #love-question {
            font-size: 24px;
            margin-bottom: 20px;
        }

        #yes-btn, #no-btn {
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
        }

        #no-btn {
            transition: transform 0.0s ease-in-out;
        }

        #no-btn.clicked {
            transform: translateY(-50vh);
        }
    </style>
</head>
<body>
    <div id="love-question">Do you love me? </div>
    <button id="yes-btn" onclick="alert('Jnisilu ai tumii yes koba buliii ❤🌚 ')">Yes</button>
    <button id="no-btn" onclick="moveNoButton()">No</button>

    <script>
        function moveNoButton() {
            var noBtn = document.getElementById('no-btn');
            noBtn.classList.add('clicked');
            setTimeout(function() {
                noBtn.classList.remove('clicked'); // Reset the button position
            }, 500);
        }
    </script>
</body>
</html>
