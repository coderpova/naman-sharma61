# naman-sharma61
this is my 18th repository
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JioHotstar Style UI</title>
    <style>
        :root {
            --hotstar-bg: #0f1014;
            --hotstar-blue: #1f80e0;
            --hotstar-nav: rgba(15, 16, 20, 0.95);
        }

        body {
            font-family: 'Roboto', sans-serif;
            background-color: var(--hotstar-bg);
            color: #fff;
            margin: 0;
            overflow-x: hidden;
        }

        /* Side Navigation Mockup */
        .sidebar {
            position: fixed;
            left: 0;
            top: 0;
            width: 80px;
            height: 100vh;
            background-color: var(--hotstar-nav);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding-top: 40px;
            z-index: 100;
            gap: 30px;
        }

        .nav-icon { font-size: 24px; color: #8f98b2; cursor: pointer; }
        .nav-icon:hover { color: #fff; }

        /* Main Content */
        .main { margin-left: 80px; }

        /* Hero Banner */
        .hero {
            position: relative;
            width: 100%;
            height: 75vh;
            background: #000;
        }

        .hero iframe {
            width: 100%;
            height: 100%;
            border: none;
            opacity: 0.7;
        }

        .hero-overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(to right, #0f1014 10%, transparent 60%),
                        linear-gradient(to top, #0f1014 5%, transparent 30%);
            display: flex;
            flex-direction: column;
            justify-content: center;
            padding-left: 60px;
        }

        .hero-title { font-size: 3rem; font-weight: 800; margin-bottom: 10px; }
        .hero-meta { color: #8f98b2; margin-bottom: 20px; font-size: 14px; }
        
        .btn-watch {
            background-color: var(--hotstar-blue);
            color: white;
            border: none;
            padding: 12px 40px;
            border-radius: 8px;
            font-weight: bold;
            font-size: 16px;
            cursor: pointer;
            transition: transform 0.2s;
        }

        /* Tray Row */
        .tray { padding: 40px 60px; }
        .tray-title { font-size: 20px; font-weight: 600; margin-bottom: 20px; }
        
        .card-container {
            display: flex;
            gap: 15px;
            overflow-x: auto;
        }
        .card-container::-webkit-scrollbar { display: none; }

        .poster-card {
            min-width: 160px;
            height: 230px;
            background: #1e212a;
            border-radius: 10px;
            overflow: hidden;
            transition: transform 0.3s;
            cursor: pointer;
        }

        .poster-card:hover { transform: scale(1.1); z-index: 10; border: 2px solid #fff; }
        .poster-card iframe { width: 100%; height: 100%; border: none; pointer-events: none; }

    </style>
</head>
<body>

    <div class="sidebar">
        <div class="nav-icon">👤</div>
        <div class="nav-icon">🔍</div>
        <div class="nav-icon">🏠</div>
        <div class="nav-icon">📺</div>
        <div class="nav-icon">⚽</div>
    </div>

    <div class="main">
        <div class="hero">
            <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ?autoplay=1&mute=1&controls=0&loop=1&playlist=dQw4w9WgXcQ" allow="autoplay"></iframe>
            <div class="hero-overlay">
                <div class="hero-title">Monostable Ops</div>
                <div class="hero-meta">Engineering · Hindi · 2026 · U/A 13+</div>
                <p style="max-width: 450px; line-height: 1.6;">Follow a B.Tech student from Dadri as they navigate the complex world of C++ coding and 555 timers before the big interview.</p>
                <button class="btn-watch">Watch Now</button>
            </div>
        </div>

        <div class="tray">
            <div class="tray-title">Trending for You</div>
            <div class="card-container">
                <div class="poster-card"><iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ?controls=0"></iframe></div>
                <div class="poster-card"><iframe src="https://www.youtube.com/embed/377pxMNUTwo?controls=0"></iframe></div>
                <div class="poster-card"><iframe src="https://www.youtube.com/embed/5PXg2paw4f0?controls=0"></iframe></div>
                <div class="poster-card"><iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ?controls=0"></iframe></div>
                <div class="poster-card"><iframe src="https://www.youtube.com/embed/377pxMNUTwo?controls=0"></iframe></div>
            </div>
        </div>
    </div>

</body>
</html>
