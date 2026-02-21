<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday JYOTI ❤️</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&family=Great+Vibes&family=Playfair+Display:ital@1&display=swap');
        
        :root { 
            --accent: #ff4d6d; 
            --gold: #ffd700; 
            --bg: #0d0d0d; 
            --pink-light: #ffb3c1;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }
        
        body { 
            font-family: 'Poppins', sans-serif; 
            background: var(--bg); 
            color: #fff; 
            overflow-x: hidden; 
            scroll-behavior: smooth; 
        }

        /* --- Screens --- */
        #start-screen { 
            position: fixed; 
            inset: 0; 
            background: radial-gradient(circle, #4a0e1c, #000); 
            display: flex; 
            justify-content: center; 
            align-items: center; 
            z-index: 9999; 
            cursor: pointer; 
            text-align: center; 
        }

        #start-text { 
            font-size: 1.8rem; 
            color: #fff; 
            font-family: 'Poppins', sans-serif; 
            font-weight: 400;
            letter-spacing: 1px;
            animation: pulse 1.5s infinite; 
            padding: 20px;
        }
        #start-text strong { 
            color: var(--accent); 
            font-weight: 600;
            display: block;
            font-size: 2.5rem;
            margin-top: 10px;
        }

        @keyframes pulse {
            0% { transform: scale(1); opacity: 0.8; }
            50% { transform: scale(1.05); opacity: 1; }
            100% { transform: scale(1); opacity: 0.8; }
        }

        #hero { 
            height: 100vh; 
            display: flex; 
            flex-direction: column; 
            justify-content: center; 
            align-items: center; 
            text-align: center; 
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('https://images.unsplash.com/photo-1513151233558-d860c5398176?auto=format&fit=crop&w=1500&q=80'); 
            background-size: cover; 
            background-position: center; 
        }

        #hero h1 { 
            font-family: 'Great Vibes', cursive; 
            font-size: clamp(3rem, 8vw, 6rem); 
            color: var(--accent); 
            text-shadow: 0 0 20px rgba(255,77,109,0.5); 
        }

        .countdown { display: flex; gap: 10px; margin-top: 20px; }
        .time-box { 
            background: var(--accent); 
            padding: 10px; 
            border-radius: 8px; 
            min-width: 70px; 
            box-shadow: 0 4px 15px rgba(255, 77, 109, 0.3);
        }
        .time-box span { display: block; font-size: 1.5rem; font-weight: bold; }

        .cake-section { padding: 80px 20px; text-align: center; background: #1a1a1a; }
        
        .cake {
            position: relative;
            width: 200px;
            height: 180px;
            margin: 60px auto;
            cursor: pointer;
        }

        .layer {
            position: absolute;
            left: 50%;
            transform: translateX(-50%);
            border-radius: 15px 15px 5px 5px;
            box-shadow: inset 0 -5px 10px rgba(0,0,0,0.2);
        }

        .layer-bottom { width: 200px; height: 70px; bottom: 0; background: linear-gradient(#ff4d6d, #a4133c); }
        .layer-middle { width: 160px; height: 60px; bottom: 70px; background: linear-gradient(#ff758f, #c9184a); }
        .layer-top { width: 120px; height: 50px; bottom: 130px; background: linear-gradient(#ff8fa3, #d6336c); }

        .layer-top::after {
            content: ""; position: absolute; top: 0; left: 0; width: 100%; height: 15px;
            background: #fff0f3; border-radius: 15px 15px 5px 5px;
        }

        .candle {
            position: absolute; bottom: 180px; left: 50%; transform: translateX(-50%);
            width: 10px; height: 35px; background: #fff; border-radius: 3px; z-index: 2;
        }

        .flame {
            position: absolute; bottom: 215px; left: 50%; transform: translateX(-50%);
            width: 14px; height: 24px; background: radial-gradient(#fff700, #ff8c00);
            border-radius: 50% 50% 20% 20%; box-shadow: 0 0 15px #ff8c00;
            animation: flicker 0.1s infinite alternate; z-index: 3;
        }

        @keyframes flicker {
            0% { transform: translateX(-50%) scale(1); }
            100% { transform: translateX(-50%) scale(1.1); }
        }

        .gallery { 
            display: grid; 
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); 
            gap: 30px; 
            padding: 50px; 
            background: #0d0d0d;
        }
        .card { 
            background: white; 
            padding: 12px 12px 35px; 
            transform: rotate(-2deg); 
            transition: 0.4s; 
            box-shadow: 0 10px 30px rgba(0,0,0,0.5);
        }
        .card:nth-child(even) { transform: rotate(3deg); }
        .card:hover { transform: rotate(0) scale(1.05); z-index: 10; }
        .card img { width: 100%; height: 350px; object-fit: cover; }
        .card p { color: #333; font-family: 'Playfair Display', serif; text-align: center; margin-top: 15px; font-size: 1.1rem; }

        #typewriter { font-size: 1.3rem; padding: 20px; font-style: italic; color: #ffe5ec; min-height: 120px; line-height: 1.6; max-width: 800px; margin: 0 auto; }
        
        .spark {
            position: fixed; width: 8px; height: 8px; border-radius: 50%; pointer-events: none;
            z-index: 100; animation: explode 1s ease-out forwards;
        }

        @keyframes explode {
            0% { transform: translate(0, 0) scale(1); opacity: 1; }
            100% { transform: translate(var(--dx), var(--dy)) scale(0.5); opacity: 0; }
        }

        .controls { position: fixed; bottom: 20px; left: 20px; display: flex; gap: 10px; z-index: 1000; }
        .btn { padding: 12px 20px; border: none; border-radius: 25px; background: var(--accent); color: white; cursor: pointer; font-weight: bold; transition: 0.3s; }
        .btn:hover { background: #ff758f; transform: scale(1.1); }

        .heart-float { position: fixed; color: var(--accent); pointer-events: none; animation: floatUp 4s linear forwards; z-index: 50; }
        @keyframes floatUp { 0% { transform: translateY(100vh); opacity: 1; } 100% { transform: translateY(-10vh); opacity: 0; } }
    </style>
</head>
<body>

<div id="start-screen" onclick="startSurprise()">
    <div id="start-text">Tap to Unveil the Magic for <br> <strong>JYOTI ❤️</strong></div>
</div>

<div id="main-content" style="display: none;">
    <section id="hero">
        <h1>Happy Birthday, JYOTI!</h1>
        <div class="countdown" id="timer">
            <div class="time-box"><span id="days">00</span>Days</div>
            <div class="time-box"><span id="hours">00</span>Hrs</div>
            <div class="time-box"><span id="mins">00</span>Min</div>
            <div class="time-box"><span id="secs">00</span>Sec</div>
        </div>
    </section>

    <section class="cake-section">
        <h2 style="color:var(--pink-light); margin-bottom: 20px;">Blow the Candle & Make a Wish! ✨</h2>
        <div class="cake" onclick="blowCandle()">
            <div id="flame" class="flame"></div>
            <div class="candle"></div>
            <div class="layer layer-top"></div>
            <div class="layer layer-middle"></div>
            <div class="layer layer-bottom"></div>
        </div>
        <p id="wish-msg" style="display:none; color:var(--accent); font-size:1.5rem; margin-top:20px; font-weight: bold; animation: pulse 1s infinite;">
            🎉 Timro dherai pragati hos. Timro aanuhar ma sadai khushi hos! 🎂
        </p>
    </section>

    <section class="gallery">
        <div class="card"><img src="https://via.placeholder.com/400x600?text=Jyoti+Photo+1"><p>My favorite smile 💕</p></div>
        <div class="card"><img src="https://via.placeholder.com/400x600?text=Jyoti+Photo+2"><p>Beautiful moment ✨</p></div>
        <div class="card"><img src="https://via.placeholder.com/400x600?text=Jyoti+Photo+3"><p>Simply Elegant 🌸</p></div>
    </section>

    <section style="text-align: center; padding: 60px 20px;">
        <h2 style="font-family:'Great Vibes'; font-size: 3.5rem; color: var(--accent);">To My Dearest...</h2>
        <div id="typewriter"></div>
        <button class="btn" onclick="generateWish()" style="margin-top:20px;">Generate Special Wish ✨</button>
        <p id="random-wish" style="color: var(--gold); margin-top: 20px; font-size: 1.2rem; min-height: 30px;"></p>
    </section>

    <footer style="text-align: center; padding: 60px 20px; border-top: 1px solid #333; background: #050505;">
        <p>I am the one who loves you the most. No matter what, I'm here. ❤️</p>
        <p style="font-family: 'Great Vibes'; font-size: 2rem; color: var(--gold); margin-top: 10px;">Forever Yours, Prince.</p>
    </footer>

    <div class="controls">
        <button class="btn" onclick="toggleMusic()" id="play-btn">⏸️ Pause Music</button>
    </div>
</div>

<audio id="bg-music" loop>
    <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mp3">
</audio>
<audio id="bday-song">
    <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-2.mp3" type="audio/mp3">
</audio>

<script>
    const music = document.getElementById('bg-music');
    const bdaySong = document.getElementById('bday-song');
    
    function startSurprise() {
        document.getElementById('start-screen').style.display = 'none';
        document.getElementById('main-content').style.display = 'block';
        music.play().catch(e => console.log("Audio blocked"));
        startTypewriter();
        setInterval(createHeart, 400);
    }

    function blowCandle() {
        const flame = document.getElementById('flame');
        if(flame.style.display !== 'none') {
            flame.style.display = 'none';
            document.getElementById('wish-msg').style.display = 'block';
            
            // Switch Music
            music.pause();
            bdaySong.play().catch(e => console.log("Song blocked"));
            document.getElementById('play-btn').innerText = "🎵 Playing B'Day Song";

            for(let i = 0; i < 50; i++) { createSpark(); }
        }
    }

    function startTypewriter() {
        const message = "Timi mero life ko tyo part hau jun bina sabai adhuro lagxa. Timi sangai huda jindagi sajilo ra ramailo lagxa. Ma timilai dherai maya garxu. 'Distance is just a test to see how far love can travel.' Ek din hami bhetnechhaun, ani tyo din pachi hami kahilyai chhutine chhainaun. Timro harek sapana pura hos ra hami sadai yesari nai sangai rahun. Happy Birthday, Jyoti! ❤️";
        let i = 0;
        const container = document.getElementById("typewriter");
        function type() {
            if (i < message.length) {
                container.innerHTML += message.charAt(i);
                i++; setTimeout(type, 50);
            }
        }
        type();
    }

    const wishes = [
        "Sadai khushi hunu, socheko sabai pugos! 🌸",
        "Ma timro sath kaile xodney xaina, promise. ❤️",
        "Distance is just a test to see how far love can travel. ✨",
        "Ek din hami bhetnechhaun, ani tyo din pachi hami kahilyai chhutine chhainaun. 💍",
        "Timi jasto swachha man bhayeko manche paunu mero bhagya ho! 😍"
    ];

    function generateWish() {
        const random = wishes[Math.floor(Math.random() * wishes.length)];
        document.getElementById('random-wish').innerText = random;
    }

    function createSpark() {
        const spark = document.createElement('div');
        spark.className = 'spark';
        const colors = ['#ff4d6d', '#ff758f', '#ffd166', '#ffffff'];
        spark.style.backgroundColor = colors[Math.floor(Math.random() * colors.length)];
        const rect = document.querySelector('.candle').getBoundingClientRect();
        spark.style.left = (rect.left + rect.width / 2) + 'px';
        spark.style.top = rect.top + 'px';
        const dx = (Math.random() - 0.5) * 400 + 'px';
        const dy = (Math.random() - 0.5) * 400 + 'px';
        spark.style.setProperty('--dx', dx);
        spark.style.setProperty('--dy', dy);
        document.body.appendChild(spark);
        setTimeout(() => spark.remove(), 1000);
    }

    function createHeart() {
        const heart = document.createElement('div');
        heart.className = 'heart-float';
        heart.innerHTML = '❤️';
        heart.style.left = Math.random() * 100 + 'vw';
        heart.style.fontSize = (Math.random() * 20 + 15) + 'px';
        document.body.appendChild(heart);
        setTimeout(() => heart.remove(), 4000);
    }

    function toggleMusic() {
        let currentAudio = bdaySong.paused ? music : bdaySong;
        if(currentAudio.paused) { 
            currentAudio.play(); 
            document.getElementById('play-btn').innerText = "⏸️ Pause Music"; 
        } else { 
            currentAudio.pause(); 
            document.getElementById('play-btn').innerText = "🎵 Play Music"; 
        }
    }

    const bday = new Date("March 6, 2026 00:00:00").getTime();
    setInterval(() => {
        const diff = bday - new Date().getTime();
        if(diff < 0) {
            document.getElementById("timer").innerHTML = "<h2 style='color:var(--gold)'>🎉 HAPPY BIRTHDAY, JYOTI! 🎉</h2>";
            return;
        }
        document.getElementById("days").innerText = String(Math.floor(diff / 86400000)).padStart(2, '0');
        document.getElementById("hours").innerText = String(Math.floor((diff % 86400000) / 3600000)).padStart(2, '0');
        document.getElementById("mins").innerText = String(Math.floor((diff % 3600000) / 60000)).padStart(2, '0');
        document.getElementById("secs").innerText = String(Math.floor((diff % 60000) / 1000)).padStart(2, '0');
    }, 1000);
</script>
# Birthday-suprise-for-special-person-