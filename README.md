<!DOCTYPE html>
<html lang="bg">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Маг Стоянова</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
        }
        header {
            background: #4CAF50;
            color: white;
            padding: 10px 0;
            text-align: center;
        }
        nav {
            margin: 20px 0;
        }
        nav a {
            margin: 0 15px;
            color: #4CAF50;
            text-decoration: none;
        }
        .container {
            width: 80%;
            margin: 0 auto;
            background: white;
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        h2 {
            color: #4CAF50;
        }
        ul {
            list-style-type: none;
            padding: 0;
        }
        ul li {
            margin: 10px 0;
        }
        .login-form {
            margin-top: 20px;
            padding: 20px;
            background: #f9f9f9;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .login-form input {
            width: 100%;
            padding: 10px;
            margin: 5px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .login-form button {
            background-color: #4CAF50;
            color: white;
            padding: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .login-form button:hover {
            background-color: #45a049;
        }
        .message {
            color: red;
        }
    </style>
</head>
<body>

<header>
    <h1>Маг Стоянова</h1>
</header>

<nav>
    <a href="#services">Услуги</a>
    <a href="#contact">Контакт</a>
</nav>

<div class="container" id="login">
    <h2>Вход</h2>
    <div class="login-form">
        <input type="text" id="username" placeholder="Потребителско име" required>
        <input type="password" id="password" placeholder="Парола" required>
        <button onclick="login()">Вход</button>
        <p class="message" id="loginMessage"></p>
    </div>
</div>

<div class="container" id="services">
    <h2>Услуги</h2>
    <ul>
        <li>Гледане на кафе</li>
        <li>Гледане на восък</li>
        <li>Разваляне на магии</li>
        <li>Изчистване на страх</li>
        <li>Отключване на късмет</li>
        <li>Изчистване на уроки</li>
        <li>Отвари при болести</li>
        <li>Помощ при зачеване</li>
        <li>Гледане на Карти Таро</li>
        <li>Ритуал за здраве, любов, пари</li>
        <li>Събиране на разделени двойки</li>
        <li>Изготвяне на личностен хороскоп</li>
        <li>Разваляне на родово проклятие</li>
        <li>Премахване на негативна енергия</li>
        <li>Помощ при алкохолизъм, хазартна зависимост</li>
    </ul>
</div>

<div class="container" id="contact">
    <h2>Контакт</h2>
    <p>Моля, свържете се с мен на имейл: <a href="mailto:info@magstoyanova.bg">info@magstoyanova.bg</a></p>
</div>

<script>
    function login() {
        // Примерни потребителско име и парола
        const username = "Маг Стоянова";
        const password = "парола123"; // Можеш да смениш паролата по твое желание

        // Вземане на стойностите от полетата
        const inputUsername = document.getElementById("username").value;
        const inputPassword = document.getElementById("password").value;

        // Проверка на входните данни
        if (inputUsername === username && inputPassword === password) {
            document.getElementById("loginMessage").innerText = "Успешно влизане!";
            document.getElementById("loginMessage").style.color = "green";
            // Тук можеш да добавиш логика за пренасочване или показване на съдържание
        } else {
            document.getElementById("loginMessage").innerText = "Невалидно потребителско име или парола.";
            document.getElementById("loginMessage").style.color = "red";
        }
    }
</script>

</body>
</html>
