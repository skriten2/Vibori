<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Выборы Президента Школы</title>
    <style>
        body {
            margin: 0;
            background-color: #1a1a1a;
            color: white;
            font-family: Arial, sans-serif;
            overflow-y: scroll;
            perspective: 1000px; /* Перспектива для 3D эффекта */
        }
        header {
            background: linear-gradient(90deg, #8B5CF6, #6D28D9);
            padding: 20px;
            text-align: center;
            position: relative;
            z-index: 1;
        }
        h1 {
            font-size: 3em;
            margin: 0;
            text-shadow: 0 0 20px #ffffff;
        }
        .subtitle {
            font-size: 1.5em;
            margin-top: 10px;
        }
        nav {
            margin: 20px 0;
        }
        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            font-size: 1.2em;
        }
        nav a:hover {
            text-decoration: underline;
        }
        .content {
            padding: 20px;
            width: 80%;
            margin: auto;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            backdrop-filter: blur(10px);
        }
        section {
            margin-bottom: 30px;
        }
        h2 {
            color: #8B5CF6;
        }
        .team-intro {
            text-align: center;
            margin-top: 30px;
            font-size: 1.2em;
            color: white;
            text-shadow: 0 0 10px #8B5CF6;
        }
        footer {
            text-align: center;
            padding: 10px;
            background: rgba(255, 255, 255, 0.1);
            position: relative;
            bottom: 0;
            width: 100%;
            z-index: 1;
        }
        .shape {
            position: absolute;
            width: 100px;
            height: 100px;
            background: rgba(139, 92, 246, 0.5);
            backdrop-filter: blur(10px);
            border-radius: 10px;
            transition: transform 0.2s;
            z-index: 5;
        }
        .shape:nth-child(1) {
            animation: float 3s ease-in-out infinite;
        }
        .shape:nth-child(2) {
            animation: float 5s ease-in-out infinite;
        }
        .shape:nth-child(3) {
            animation: float 4s ease-in-out infinite;
        }
        @keyframes float {
            0% { transform: translateY(0); }
            50% { transform: translateY(-20px); }
            100% { transform: translateY(0); }
        }
        .title {
            text-align: center;
            margin-top: 50px;
            font-size: 4em;
            color: white;
            text-shadow: 0 0 20px #8B5CF6;
            position: relative;
            z-index: 10;
            transform: translateZ(50px);
            transition: transform 0.1s;
        }
    </style>
</head>
<body>
    <header>
        <h1>Выборы Президента Школы</h1>
        <div class="subtitle">Поддержите своего кандидата!</div>
        <nav>
            <a href="#about">О кандидате</a>
            <a href="#news">Новости</a>
            <a href="#proposals">Предложения</a>
            <a href="#team">Наша команда</a>
        </nav>
    </header>

    <div class="content">
        <section id="about">
            <h2>О кандидате</h2>
            <p>Я, Портнягин Александр Александрович, стремлюсь сделать нашу школу лучше для всех. Я активно работаю над улучшением школьной среды.</p>
            <p>Мы вместе сможем создать лучшее учебное заведение!</p>
        </section>

        <section id="news">
            <h2>Последние новости</h2>
            <ul>
                <li>Александр принял участие в выборах 15.10.25.</li>
                <li>Новые инициативы для активных учеников будут реализованы.</li>
            </ul>
        </section>

        <section id="proposals">
            <h2>Предложения президента</h2>
            <ul>
                <li>Внедрение гибкого расписания уроков.</li>
                <li>Организация конкурсов и мероприятий.</li>
                <li>Создание комфортных условий в учебных кабинетах и туалетах.</li>
            </ul>
        </section>

        <section id="team">
            <h2>Наша команда</h2>
            <p>Я и мои помощники:</p>
            <p>Eфимов Степан Александрович, Данилов Валерий Сергеевич, Сапрыгин Никита Игоревич.</p>
            <p>Мы стремимся к улучшению условий обучения в школе.</p>
        </section>
    </div>

    <footer>
        <p>&copy; 2023 Выборы Президента Школы</p>
    </footer>

    <div class="title">ПОРТНЯГИН АЛЕКСАНДР АНАТОЛЬЕВИЧ</div>

    <script>
        const shapes = [];
        const numShapes = 15; // Увеличиваем количество фигур

        // Создаем абстракции
        for (let i = 0; i < numShapes; i++) {
            const shape = document.createElement('div');
            shape.className = 'shape';
            shape.style.left = Math.random() * window.innerWidth + 'px';
            shape.style.top = Math.random() * window.innerHeight + 'px';
            document.body.appendChild(shape);
            shapes.push(shape);
        }

        // Обработка движения мыши для 3D текста
        document.addEventListener('mousemove', (e) => {
            const mouseX = e.clientX / window.innerWidth - 0.5;
            const mouseY = e.clientY / window.innerHeight - 0.5;

            const title = document.querySelector('.title');
            title.style.transform = translateZ(50px) rotateY(${mouseX * 30}deg) rotateX(${-mouseY * 30}deg);

            shapes.forEach((shape) => {
                const offsetX = (Math.random() - 0.5) * 10;
                const offsetY = (Math.random() - 0.5) * 10;
                shape.style.transform = translate(${e.clientX + offsetX}px, ${e.clientY + offsetY}px);
            });
        });
    </script>
</body>
</html>
