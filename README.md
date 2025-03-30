# Color-Changer
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Change Background Color</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            transition: background-color 0.5s;
        }
        button {
            padding: 10px 20px;
            font-size: 18px;
            cursor: pointer;
            border: none;
            background-color: blue;
            color: white;
            border-radius: 5px;
            margin-top: 20px;
        }
        button:hover {
            background-color: darkblue;
        }
    </style>
</head>
<body>

    <h1>Click the Button to Change Background Color</h1>
    <button onclick="changeColor()">Change Color</button>

    <script>
        function changeColor() {
            const colors = ["#FF5733", "#33FF57", "#3357FF", "#F1C40F", "#9B59B6"];
            document.body.style.backgroundColor = colors[Math.floor(Math.random() * colors.length)];
        }
    </script>

</body>
</html>
