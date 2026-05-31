<!DOCTYPE html>  
<html lang="ru">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">  
    <title>С 21 годом, Митя! 🎉</title>  
    <style>  
        * {  
            margin: 0;  
            padding: 0;  
            box-sizing: border-box;  
        }  
  
        body {  
            background-color: #0a0a0a;  
            font-family: system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', sans-serif;  
            color: white;  
            overflow-x: hidden;  
        }  
  
        /* Чёрный + розовый + красный фон */  
        .bg {  
            position: fixed;  
            top: 0;  
            left: 0;  
            width: 100%;  
            height: 100%;  
            background: radial-gradient(circle at 30% 20%, #1a0000, #000000);  
            z-index: -2;  
        }  
        .bg::after {  
            content: '';  
            position: absolute;  
            top: 0;  
            left: 0;  
            width: 100%;  
            height: 100%;  
            background: repeating-linear-gradient(45deg, rgba(255,20,147,0.08) 0px, rgba(255,20,147,0.08) 2px, transparent 2px, transparent 10px);  
        }  
  
        .container {  
            max-width: 700px;  
            margin: 0 auto;  
            padding: 2rem 1.5rem 4rem;  
            position: relative;  
            z-index: 2;  
        }  
  
        /* Имена при скролле */  
        .name-card {  
            background: rgba(0,0,0,0.6);  
            backdrop-filter: blur(10px);  
            border-radius: 50px;  
            padding: 1.5rem;  
            margin: 1rem 0;  
            text-align: center;  
            transform: translateY(40px);  
            opacity: 0;  
            transition: all 0.6s ease-out;  
            border-left: 5px solid #ff1493;  
            border-right: 5px solid #ff3366;  
        }  
        .name-card.visible {  
            transform: translateY(0);  
            opacity: 1;  
        }  
        .name-card h1 {  
            font-size: 2.8rem;  
            background: linear-gradient(135deg, #ff69b4, #ff3366);  
            -webkit-background-clip: text;  
            background-clip: text;  
            color: transparent;  
        }  
  
        .age {  
            text-align: center;  
            font-size: 1.8rem;  
            font-weight: bold;  
            background: rgba(255,51,102,0.2);  
            border-radius: 60px;  
            padding: 1rem;  
            margin: 2rem 0;  
        }  
  
        .section-title {  
            font-size: 1.8rem;  
            text-align: center;  
            margin: 2rem 0 1rem;  
            color: #ff6699;  
        }  
  
        .fact-card {  
            background: rgba(30,30,30,0.8);  
            border-radius: 28px;  
            padding: 1rem 1.5rem;  
            margin: 0.8rem 0;  
            border: 1px solid #ff3366;  
            display: flex;  
            gap: 12px;  
            align-items: center;  
        }  
        .fact-emoji {  
            font-size: 1.8rem;  
        }  
  
        /* Галерея */  
        .gallery {  
            display: grid;  
            grid-template-columns: repeat(2, 1fr);  
            gap: 1rem;  
            margin: 1.5rem 0;  
        }  
        .photo-placeholder {  
            background: #1a1a1a;  
            border-radius: 24px;  
            aspect-ratio: 1;  
            display: flex;  
            flex-direction: column;  
            align-items: center;  
            justify-content: center;  
            border: 2px dashed #ff3366;  
            color: #ff6699;  
            font-size: 0.8rem;  
            text-align: center;  
        }  
        .photo-placeholder i {  
            font-size: 2rem;  
            margin-bottom: 8px;  
        }  
  
        .surprise-btn {  
            background: linear-gradient(90deg, #ff1493, #ff3366);  
            width: 100%;  
            padding: 1rem;  
            font-size: 1.3rem;  
            font-weight: bold;  
            border: none;  
            border-radius: 50px;  
            color: white;  
            margin: 2rem 0;  
            cursor: pointer;  
        }  
  
        .music-widget {  
            position: fixed;  
            bottom: 20px;  
            right: 20px;  
            background: black;  
            padding: 10px 18px;  
            border-radius: 40px;  
            display: flex;  
            align-items: center;  
            gap: 8px;  
            border: 1px solid #ff1493;  
            z-index: 100;  
        }  
  
        footer {  
            text-align: center;  
            margin-top: 2rem;  
            opacity: 0.7;  
            font-size: 0.8rem;  
        }  
    </style>  
</head>  
<body>  
<div class="bg"></div>  
  
<div class="container">  
    <!-- Имена -->  
    <div class="name-card"><h1>Митя</h1><p>он же...</p></div>  
    <div class="name-card"><h1>Асфальтина</h1><p>легенда...</p></div>  
    <div class="name-card"><h1>Лукреция</h1><p>она же...</p></div>  
    <div class="name-card"><h1>Малой</h1><p>🔥 21 год — огонь! 🔥</p></div>  
  
    <div class="age">🎂 21 год 🎂</div>  
  
    <!-- Факты -->  
    <div class="section-title">📌 ФАКТЫ ПРО МИТЮ</div>  
    <div class="fact-card"><div class="fact-emoji">🌅</div> амбасадор шоу в 7 утра, когда все уже спят</div>  
    <div class="fact-card"><div class="fact-emoji">😴</div> призер в соревновании длительности сна на асфальте и в метро</div>  
    <div class="fact-card"><div class="fact-emoji">⭐</div> главная звездочка клуба «Центральная станция»</div>  
    <div class="fact-card"><div class="fact-emoji">🤝</div> самая лучшая поддержка на свете</div>  
    <div class="fact-card"><div class="fact-emoji">🎃</div> специалист по приготовлению блюд из тыквы</div>  
    <div class="fact-card"><div class="fact-emoji">🚂</div> мастер по переездам в питер и обратно (не дай бог ты еще раз переедешь)</div>  
  
    <!-- Галерея -->  
    <div class="section-title">📸 ФОТО</div>  
    <div class="gallery" id="gallery">  
        <div class="photo-placeholder" onclick="alert('Как добавить фото: загрузите фото на любой хостинг (например, tg:// или imgbb) и пришлите ссылку — я поменяю код')">📷 <span>фото 1</span></div>  
        <div class="photo-placeholder" onclick="alert('Как добавить фото: загрузите фото на любой хостинг и пришлите ссылку')">📷 <span>фото 2</span></div>  
        <div class="photo-placeholder" onclick="alert('Как добавить фото: загрузите фото и пришлите ссылку')">📷 <span>фото 3</span></div>  
        <div class="photo-placeholder" onclick="alert('Как добавить фото: загрузите фото и пришлите ссылку')">📷 <span>фото 4</span></div>  
    </div>  
  
    <button class="surprise-btn" id="surpriseBtn">🎁 СЮРПРИЗ 🎁</button>  
  
    <footer>  
        ❤️ с любовью от Мамы ❤️<br>  
        Митя, Асфальтина, Лукреция, Малой — с днём рождения!  
    </footer>  
</div>  
  
<div class="music-widget" id="musicBtn">  
    🎵 <span>Включить музыку</span>  
</div>  
  
<audio id="song" loop preload="auto">  
    <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3">  
</audio>  
  
<script>  
    // Музыка после клика  
    let musicPlaying = false;  
    const audio = document.getElementById('song');  
    const musicBtn = document.getElementById('musicBtn');  
  
    function startMusic() {  
        audio.play().then(() => {  
            musicPlaying = true;  
            musicBtn.innerHTML = '🎧 <span>Пати играет 🎵</span>';  
        }).catch(() => {});  
    }  
  
    document.body.addEventListener('click', function firstClick() {  
        startMusic();  
        document.body.removeEventListener('click', firstClick);  
    }, { once: true });  
  
    musicBtn.addEventListener('click', function(e) {  
        e.stopPropagation();  
        if (!musicPlaying) {  
            startMusic();  
        } else {  
            if (audio.paused) {  
                audio.play();  
                musicBtn.innerHTML = '🎧 <span>Пати играет 🎵</span>';  
            } else {  
                audio.pause();  
                musicBtn.innerHTML = '🎵 <span>Включить музыку</span>';  
            }  
        }  
    });  
  
    // Появление имён  
    const cards = document.querySelectorAll('.name-card');  
    function checkVisible() {  
        cards.forEach(c => {  
            const rect = c.getBoundingClientRect();  
            if (rect.top < window.innerHeight - 80) c.classList.add('visible');  
        });  
    }  
    window.addEventListener('scroll', checkVisible);  
    checkVisible();  
  
    // Сюрприз + конфетти  
    document.getElementById('surpriseBtn').addEventListener('click', () => {  
        canvasConfetti({ particleCount: 200, spread: 100, origin: { y: 0.6 }, colors: ['#ff1493', '#ff3366', '#000'] });  
        canvasConfetti({ particleCount: 100, spread: 120, origin: { y: 0.5, x: 0.2 } });  
        canvasConfetti({ particleCount: 100, spread: 120, origin: { y: 0.5, x: 0.8 } });  
        alert('🎉 СЮРПРИЗ! 🎉\n\nМитя, ты лучший! С 21 годом!\nОбнимаю, Мама ❤️');  
    });  
</script>  
<script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1"></script>  
</body>  
</html>  
