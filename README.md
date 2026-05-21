<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Get To Know Me - Kirani</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Fredoka:wght@300..700&family=Quicksand:wght@500;700&display=swap');

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Quicksand', sans-serif;
            background-color: #f4f9f4;
            background-image: 
                radial-gradient(#ffe3e3 15%, transparent 16%),
                radial-gradient(#e8f5e9 15%, transparent 16%);
            background-size: 40px 40px;
            background-position: 0 0, 20px 20px;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding: 20px;
        }

        .carrd-box {
            background: #ffffff;
            border: 4px solid #4caf50;
            border-radius: 24px;
            box-shadow: 8px 8px 0px #ff8a8a;
            width: 100%;
            max-width: 480px;
            overflow: hidden;
            animation: fadeIn 0.6s ease-out;
        }

        .carrd-header {
            background-color: #ff6b6b;
            padding: 12px;
            text-align: center;
            border-bottom: 4px solid #4caf50;
            display: flex;
            justify-content: space-between;
            align-items: center;
            color: white;
        }

        .header-dots {
            display: flex;
            gap: 6px;
            margin-left: 10px;
        }

        .dot {
            width: 12px;
            height: 12px;
            border-radius: 50%;
            background-color: white;
            opacity: 0.7;
        }

        .carrd-title {
            font-family: 'Fredoka', sans-serif;
            font-size: 1.3rem;
            letter-spacing: 1px;
            font-weight: 600;
            margin-right: auto;
            margin-left: 15px;
        }

        .carrd-banner {
            background-image: url('data:image/jpeg;base64,eUpsb2FkZWQ6MTAwMDAwMjMyMi5qcGctM2U3OTJmNGUtOGI3ZC00YzRlLTkValid_Base64_Will_Show_Directly');
            background-size: cover;
            background-position: center;
            height: 120px;
            position: relative;
            border-bottom: 4px solid #4caf50;
        }

        .avatar-container {
            position: absolute;
            bottom: -45px;
            left: 25px;
            background: white;
            border: 4px solid #ff6b6b;
            border-radius: 50%;
            width: 90px;
            height: 90px;
            overflow: hidden;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 3px 3px 0px rgba(0,0,0,0.1);
        }

        .avatar-container img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .carrd-body {
            padding: 60px 25px 25px 25px;
        }

        .profile-name {
            font-family: 'Fredoka', sans-serif;
            font-size: 1.8rem;
            color: #ff6b6b;
            margin-bottom: 2px;
        }

        .profile-tag {
            display: inline-block;
            background-color: #e8f5e9;
            color: #2e7d32;
            padding: 4px 10px;
            border-radius: 12px;
            font-size: 0.85rem;
            font-weight: 700;
            margin-bottom: 20px;
            border: 1px solid #c8e6c9;
        }

        .info-section {
            background-color: #fafafa;
            border: 2px solid #e0e0e0;
            border-radius: 16px;
            padding: 15px;
            margin-bottom: 15px;
        }

        .info-row {
            margin-bottom: 12px;
            font-size: 0.95rem;
            color: #424242;
            line-height: 1.5;
        }

        .info-row:last-child {
            margin-bottom: 0;
        }

        .label {
            font-weight: 700;
            color: #ff6b6b;
            display: inline-block;
            width: 95px;
            vertical-align: top;
        }

        .content-right {
            display: inline-block;
            width: calc(100% - 105px);
        }

        .badge-list {
            display: flex;
            flex-wrap: wrap;
            gap: 6px;
            margin-top: 5px;
        }

        .badge {
            background-color: #fff1f1;
            border: 1px solid #ffcdd2;
            color: #c62828;
            padding: 3px 10px;
            border-radius: 8px;
            font-size: 0.8rem;
            font-weight: 600;
        }

        .badge.green {
            background-color: #e8f5e9;
            border: 1px solid #c8e6c9;
            color: #2e7d32;
        }

        .badge.purple {
            background-color: #f3e5f5;
            border: 1px solid #e1bee7;
            color: #4a148c;
        }

        .badge.yellow {
            background-color: #fffde7;
            border: 1px solid #fff59d;
            color: #f57f17;
        }

        .badge.beloved {
            background-color: #ff8a8a;
            border: 1px solid #ff5252;
            color: #ffffff;
            animation: heartbeat 1.5s infinite;
        }

        .status-box {
            background-color: #e8f5e9;
            border-left: 5px solid #4caf50;
            padding: 12px;
            border-radius: 4px 12px 12px 4px;
            font-size: 0.9rem;
            color: #37474f;
            font-style: italic;
        }

        .carrd-footer {
            text-align: center;
            padding: 15px;
            background-color: #f9f9f9;
            border-top: 2px solid #eeeeee;
            font-size: 0.8rem;
            color: #9e9e9e;
        }

        .heart {
            color: #ff6b6b;
            display: inline-block;
            animation: heartbeat 1.2s infinite;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes heartbeat {
            0% { transform: scale(1); }
            20% { transform: scale(1.05); }
            40% { transform: scale(1); }
            60% { transform: scale(1.05); }
            80% { transform: scale(1); }
            100% { transform: scale(1); }
        }
    </style>
</head>
<body>
    <div class="carrd-box">
        <div class="carrd-header">
            <div class="header-dots">
                <div class="dot" style="background-color: #ff8a8a;"></div>
                <div class="dot" style="background-color: #a5d6a7;"></div>
                <div class="dot" style="background-color: #fff59d;"></div>
            </div>
            <div class="carrd-title">get to know me ♪</div>
        </div>
        <div class="carrd-banner" style="background-image: url('data:image/jpeg;base64,...(kode_banner_anda)...')">
            <div class="avatar-container">
                <img src="data:image/jpeg;base64,...(kode_avatar_anda)..." alt="Anon Chihaya Avatar">
            </div>
        </div>
        <div class="carrd-body">
            <h1 class="profile-name">Kirani</h1>
            <span class="profile-tag">Grade 10 • Age 17</span>
            <div class="info-section">
                <div class="info-row">
                    <span class="label">✨ Passion:</span>
                    <span class="content-right">Digital Art & Graphic Design</span>
                </div>
            </div>
            <div class="info-section" style="border-color: #c8e6c9;">
                <div class="info-row">
                    <span class="label" style="color: #4caf50;">👾 Fandoms:</span>
                    <div class="content-right">
                        <span style="font-size: 0.85rem; color: #757575;">(Mostly active)</span>
                        <div class="badge-list">
                            <span class="badge green">Limbus Company</span>
                            <span class="badge green">Reverse: 1999</span>
                            <span class="badge green">Uma Musume</span>
                            <span class="badge green">Wuthering Waves</span>
                            <span class="badge green">Tamon B-Side</span>
                            <span class="badge green">Kill Blue</span>
                            <span class="badge green">etc.</span>
                        </div>
                    </div>
                </div>
            </div>
            <div class="info-section">
                <div class="info-row">
                    <span class="label">💖 Fav Muse:</span>
                    <div class="content-right">
                        <div class="badge-list">
                            <span class="badge">Anon Chihaya</span>
                            <span class="badge">Ouri Sakaguchi</span>
                            <span class="badge">Acheron</span>
                            <span class="badge">Yi Sang</span>
                            <span class="badge">Natsuki Seba</span>
                            <span class="badge beloved">Nyamu Yuutenji (BELOVED)</span>
                            <span class="badge">Mutsumi Wakaba</span>
                        </div>
                    </div>
                </div>
            </div>
            <div class="info-section" style="border-color: #fff59d;">
                <div class="info-row">
                    <span class="label" style="color: #f57f17;">🎨 Fav Color:</span>
                    <div class="content-right">
                        <div class="badge-list">
                            <span class="badge green">Green</span>
                            <span class="badge purple">Purple</span>
                            <span class="badge yellow">Yellow</span>
                        </div>
                    </div>
                </div>
                <div class="info-row" style="margin-top: 10px;">
                    <span class="label" style="color: #f57f17;">🎵 Music:</span>
                    <div class="content-right" style="font-size: 0.85rem; font-weight: 700; color: #555; line-height: 1.5;">
                        TYLER THE CREATOR <br>
                        JOEY VALENCE & BRAE <br>
                        MILI FTW
                    </div>
                </div>
            </div>
            <div class="status-box">
                <strong>Current status:</strong> Currently busy working and improving. 🚀
            </div>
        </div>
        <div class="carrd-footer">
            Made with <span class="heart">❤</span> for Kirani
        </div>
    </div>
</body>
</html>
