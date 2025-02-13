# Valentine-Invite
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Valentine's Day Invite</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 50px;
        }
        .question {
            font-size: 24px;
            margin-bottom: 20px;
        }
        .buttons {
            margin-top: 20px;
        }
        .hidden {
            display: none;
        }
        .celebration {
            font-size: 28px;
            color: red;
        }
    </style>
</head>
<body>
    <div id="flowchart">
        <div id="question1" class="question">Will you be my Valentine? ❤️</div>
        <div class="buttons">
            <button onclick="answerYes()">Yes</button>
            <button onclick="answerNo()">No</button>
        </div>
    </div>
    
    <div id="celebration" class="hidden">
        <div class="celebration">🎉 Yay! Let's celebrate love! 🎉</div>
        <img src="https://i.imgur.com/w1aL67u.png" alt="Happy Mascot" width="200px">
    </div>
    
    <script>
        function answerYes() {
            document.getElementById('flowchart').style.display = 'none';
            document.getElementById('celebration').style.display = 'block';
        }
        
        function answerNo() {
            alert("Are you sure? 🥺");
        }
    </script>
</body>
</html>
