<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Мой первый сайт</title>
    <link rel="stylesheet" href=""> <!-- Подключаем CSS -->
</head>
<body>
    <header>
        <h1>Привет, мир!</h1>
        <nav>
            <a href="#">Главная</a>
            <a href="#">Обо мне</a>
            <a href="#">Контакты</a>
        </nav>
    </header>

    <main>
        <section>
            <h2>Обо мне</h2>
            <p>Здесь я расскажу немного о себе.</p>
            <img src="my-photo.jpg" alt="Мое фото" width="300"> <!-- положите свое изображение в папку -->
        </section>
    </main>

    <footer>
        <p>© 2024 Мой первый сайт</p>
    </footer>
</body><script src="script.js"></script>
</body>

<p id="demo"></p>

<button onclick="alert('Привет! Спасибо что нажали кнопку.')">Нажми на меня!</button>

  body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f0f0f0;
    line-height: 1.6;
}

header {
    background-color: #333;
    color: white;
    padding: 20px;
    text-align: center;
}

nav a {
    color: white;
    margin: 0 15px;
    text-decoration: none;
}

main {
    padding: 20px;
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px;
    position: fixed;
    bottom: 0;
    width: 100%;
}
// Находим кнопку и параграф по их id
const button = document.getElementById('myButton');
const demoParagraph = document.getElementById('demo');

// "Слушаем" событие "клик" на кнопке
button.addEventListener('click', function() {
    // Когда кнопка нажата, меняем текст в параграфе
    demoParagraph.textContent = 'Ура! Вы нажали на кнопку!';
});
