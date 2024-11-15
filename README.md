<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Site</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
        }
        .container {
            text-align: center;
        }
        input[type="text"] {
            margin-top: 10px;
            padding: 8px;
            width: 200px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        button {
            margin-top: 10px;
            padding: 8px 16px;
            background-color: #007BFF;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Welcome to My Simple Site</h1>
        <input type="text" id="nameInput" placeholder="Enter your name">
        <br>
        <button onclick="greetUser()">Submit</button>
    </div>

<script>
    document.querySelector('button').addEventListener('click', function() {
        const name = document.getElementById('nameInput').value;
        if (name) {
            alert('Hello, ' + name + '! Welcome to the site!');
        } else {
            alert('Please enter your name.');
        }
    });
</script>

</body>
</html>
