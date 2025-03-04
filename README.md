<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ВАРЮХА Свистунова</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            background-image: url('https://github.com/Dasha00Ushakova1/Barbara/blob/e4f3c47f6f43eee041f72d6ceb9ee40c6b384dc7/%D1%84%D0%BE%D0%BD.jpg'); /* Замените на URL изображения фона */
            background-size: cover;
            background-position: center;
            color: white;
            margin: 0;
            padding: 0;
        }
        .button {
            margin: 10px;
            padding: 15px 30px;
            font-size: 16px;
            color: white;
            background-color: #007BFF;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
            width: 80%;
        }
        .button:hover {
            background-color: #0056b3;
        }
        .color-box {
            width: 80px;
            height: 80px;
            background-color: #ccc;
            margin: 10px;
            transition: background-color 0.5s;
        }
        .image-container {
            display: flex;
            flex-direction: row;
            justify-content: center;
            flex-wrap: wrap;
        }
        .image-placeholder {
            width: 45%;
            height: auto;
            border: 2px dashed #ccc;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 10px;
            font-weight: bold;
            color: #888;
        }
        .image-placeholder img {
            max-width: 100%;
            max-height: 100%;
            object-fit: cover;
        }
        #text-output {
            margin: 20px;
            font-size: 20px;
            color: #fff;
        }
    </style>
</head>
<body>
<h1>ВАРЮХА Свистунова</h1>

<div>
    <button class="button" onclick="showText('Тык сюда')">Кнопка 1</button>
    <button class="button" onclick="changeColor('box1')">Изменить цвет 1</button>
    <button class="button" onclick="showText('Сюда тоже можно тыкнуть')">Кнопка 2</button>
    <button class="button" onclick="changeColor('box2')">Изменить цвет 2</button>
</div>

<div id="text-output">ВаРьКа</div>

<div class="color-box" id="box1"></div>
<div class="color-box" id="box2"></div>

<div class="image-container">
    <div class="image-placeholder">
        <img src="https://github.com/Dasha00Ushakova1/Barbara/blob/e4f3c47f6f43eee041f72d6ceb9ee40c6b384dc7/%D0%98%D0%B7%D0%BE%D0%B1%D1%80%D0%B0%D0%B6%D0%B5%D0%BD%D0%B8%D0%B5%20WhatsApp%202025-03-04%20%D0%B2%2020.00.11_ae252489.jpg" alt="1"> <!-- Замените на путь к Вашему изображению -->
    </div>
    <div class="image-placeholder">
        <img src="https://github.com/Dasha00Ushakova1/Barbara/blob/e4f3c47f6f43eee041f72d6ceb9ee40c6b384dc7/%D0%98%D0%B7%D0%BE%D0%B1%D1%80%D0%B0%D0%B6%D0%B5%D0%BD%D0%B8%D0%B5%20WhatsApp%202025-03-04%20%D0%B2%2020.00.12_5b7921a0.jpg" alt="2"> <!-- Замените на путь к Вашему изображению -->
    </div>
    <div class="image-placeholder">
        <img src="https://github.com/Dasha00Ushakova1/Barbara/blob/e4f3c47f6f43eee041f72d6ceb9ee40c6b384dc7/%D0%98%D0%B7%D0%BE%D0%B1%D1%80%D0%B0%D0%B6%D0%B5%D0%BD%D0%B8%D0%B5%20WhatsApp%202025-03-04%20%D0%B2%2020.00.24_f890ac4f.jpg" alt="3"> <!-- Замените на путь к Вашему изображению -->
    </div>
</div>

<script>
    function showText(message) {
        document.getElementById('text-output').innerText = message;
    }

    function changeColor(boxId) {
        const box = document.getElementById(boxId);
        const randomColor = '#' + Math.floor(Math.random()*16777215).toString(16);
        box.style.backgroundColor = randomColor;
    }
</script>
</body>
</html>
