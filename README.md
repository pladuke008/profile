<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>โปรไฟล์ - อัฟฮัม อินทโช (ปลาดุก)</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Kanit:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root {
            --kuromi-black: #2b2633;
            --kuromi-purple: #8e6cd3;
            --kuromi-dark-purple: #6c47b5;
            --kuromi-pink: #ff85be;
            --kuromi-light-pink: #ffd3e8;
            --kuromi-lavender: #e5daf5;
            --text-dark: #2d2345;
            --text-muted: #796a91;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Kanit', sans-serif;
        }

        body {
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            padding: 20px;
            position: relative;
            overflow-x: hidden;
            
            /* แสดงรูปภาพน้องคุโรมิหลายๆ ตัวกระจายรอบหน้าจอ โดยรองรับทั้งชื่อไทยและรหัสเข้ารหัสบน GitHub */
            background-color: #d8c8f0;
            background-image: 
                url("%E0%B8%81%E0%B8%B2%E0%B8%A3%E0%B9%8C%E0%B8%95%E0%B8%B5%E0%B8%99%E0%B8%84%E0%B8%B5%E0%B8%A3%E0%B8%B5%E0%B8%A1%E0%B8%B4.jpg"), /* การ์ตูนคีรีมิ */
                url("%E0%B8%81%E0%B8%B2%E0%B8%A3%E0%B9%8C%E0%B8%95%E0%B8%B5%E0%B8%99%E0%B8%84%E0%B8%B5%E0%B8%A3%E0%B8%B5%E0%B8%A1%E0%B8%B4.jpg"), /* รองรับกรณีพิมพ์ต่างกัน */
                url("การ์ตูนคุรุมิ.jpg"),
                url("images%20(1).jpg"),
                url("images (1).jpg"),
                url("oEDD0pG0LAq79j6rAb1NJEb7yfeEIoAeAPR7CI~tplv-sdweummd6v-text-logo-v1_QGF1bW51Y2hzaG9w_q75.jpeg"),
                url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='100' height='100' viewBox='0 0 100 100'%3E%3Cg fill='%23bca5e3' fill-opacity='0.25'%3E%3Ccircle cx='80' cy='25' r='3'/%3E%3Ccircle cx='25' cy='75' r='4'/%3E%3Cpath d='M85,80 L90,85 L85,90 L80,85 Z'/%3E%3C/g%3E%3C/svg%3E");
            
            background-size: 280px, 280px, 280px, 240px, 240px, 320px, auto;
            background-repeat: repeat;
            background-position: top left, bottom right, center, center;
            background-attachment: fixed;
        }

        .sparkle {
            position: absolute;
            background: white;
            border-radius: 50%;
            pointer-events: none;
            opacity: 0.8;
            animation: floatSparkle 6s infinite linear;
        }

        @keyframes floatSparkle {
            0% { transform: translateY(100vh) scale(0); opacity: 0; }
            50% { opacity: 0.8; }
            100% { transform: translateY(-10vh) scale(1); opacity: 0; }
        }

        .profile-card {
            background: rgba(255, 255, 255, 0.94);
            backdrop-filter: blur(15px);
            -webkit-backdrop-filter: blur(15px);
            border: 4px solid var(--kuromi-purple);
            border-radius: 32px;
            box-shadow: 0 20px 50px rgba(110, 71, 181, 0.35);
            width: 100%;
            max-width: 430px;
            padding: 50px 24px 35px 24px;
            text-align: center;
            z-index: 10;
            position: relative;
            margin-top: 40px;
            transition: all 0.3s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }

        .profile-card:hover {
            transform: translateY(-5px) scale(1.01);
            box-shadow: 0 25px 60px rgba(110, 71, 181, 0.45);
        }

        .kuromi-ears {
            position: absolute;
            top: -45px;
            left: 0;
            right: 0;
            height: 50px;
            pointer-events: none;
            display: flex;
            justify-content: space-between;
            padding: 0 45px;
        }

        .ear-left, .ear-right {
            width: 55px;
            height: 55px;
            background: var(--kuromi-black);
            border: 4px solid var(--kuromi-purple);
            border-bottom: none;
        }

        .ear-left {
            border-top-left-radius: 60px;
            border-top-right-radius: 15px;
            transform: rotate(-15deg);
        }

        .ear-right {
            border-top-right-radius: 60px;
            border-top-left-radius: 15px;
            transform: rotate(15deg);
        }

        .kuromi-skull-badge {
            position: absolute;
            top: -20px;
            left: 50%;
            transform: translateX(-50%);
            background: var(--kuromi-pink);
            color: white;
            width: 38px;
            height: 38px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            border: 3px solid var(--kuromi-black);
            box-shadow: 0 4px 10px rgba(255, 133, 190, 0.5);
            font-size: 16px;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% { transform: translateX(-50%) scale(1); }
            50% { transform: translateX(-50%) scale(1.1); }
            100% { transform: translateX(-50%) scale(1); }
        }

        .avatar-container {
            position: relative;
            width: 170px;
            height: 170px;
            margin: 0 auto 25px auto;
        }

        .avatar-circle {
            width: 100%;
            height: 100%;
            border-radius: 50%;
            border: 6px solid var(--kuromi-purple);
            padding: 5px;
            background: white;
            box-shadow: 0 10px 25px rgba(110, 71, 181, 0.3);
            display: flex;
            align-items: center;
            justify-content: center;
            overflow: hidden;
            position: relative;
        }

        .avatar-img {
            width: 100%;
            height: 100%;
            border-radius: 50%;
            object-fit: cover;
            display: block;
        }

        /* อวาตาร์สำรองเมื่อไฟล์รูปโปรไฟล์แตกหรือไม่เจอรูปภาพ */
        .avatar-fallback {
            width: 100%;
            height: 100%;
            border-radius: 50%;
            background: linear-gradient(135deg, var(--kuromi-purple), var(--kuromi-black));
            display: none;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 65px;
        }

        .name-wrapper {
            margin-bottom: 8px;
        }

        .profile-name {
            font-size: 24px;
            font-weight: 700;
            color: var(--kuromi-black);
            display: inline-flex;
            align-items: center;
            justify-content: center;
            gap: 5px;
            flex-wrap: wrap;
        }

        .nickname-badge {
            background: var(--kuromi-pink);
            color: white;
            font-size: 13px;
            font-weight: 600;
            padding: 2px 10px;
            border-radius: 12px;
            border: 1px solid var(--kuromi-black);
            margin-left: 5px;
            display: inline-block;
        }

        .id-badge {
            background: var(--kuromi-lavender);
            color: var(--kuromi-dark-purple);
            font-size: 14px;
            font-weight: 600;
            padding: 6px 18px;
            border-radius: 50px;
            display: inline-block;
            border: 2px dashed var(--kuromi-purple);
            margin-bottom: 25px;
        }

        .info-list {
            text-align: left;
            margin-bottom: 25px;
        }

        .info-card {
            background: rgba(255, 255, 255, 0.7);
            border: 2px solid var(--kuromi-lavender);
            border-radius: 20px;
            padding: 14px 18px;
            display: flex;
            align-items: center;
            margin-bottom: 12px;
            transition: all 0.25s ease;
        }

        .info-card:hover {
            background: white;
            border-color: var(--kuromi-pink);
            transform: translateX(5px);
        }

        .info-icon {
            width: 42px;
            height: 42px;
            border-radius: 14px;
            background: var(--kuromi-lavender);
            color: var(--kuromi-dark-purple);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 18px;
            margin-right: 15px;
            flex-shrink: 0;
            border: 2px solid transparent;
            transition: all 0.25s ease;
        }

        .info-card:hover .info-icon {
            background: var(--kuromi-light-pink);
            color: var(--kuromi-pink);
            border-color: var(--kuromi-pink);
        }

        .info-content {
            flex-grow: 1;
        }

        .info-title {
            font-size: 11px;
            color: var(--text-muted);
            text-transform: uppercase;
            letter-spacing: 0.5px;
            font-weight: 600;
            display: block;
        }

        .info-text {
            font-size: 15px;
            color: var(--text-dark);
            font-weight: 500;
            word-break: break-all;
        }

        .info-text a {
            color: var(--kuromi-dark-purple);
            text-decoration: none;
            font-weight: 600;
        }

        .info-text a:hover {
            color: var(--kuromi-pink);
            text-decoration: underline;
        }

        .call-btn {
            background: linear-gradient(135deg, var(--kuromi-purple), var(--kuromi-black));
            color: white;
            border: 3px solid var(--kuromi-black);
            border-radius: 18px;
            font-size: 16px;
            font-weight: 600;
            padding: 14px;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
            box-shadow: 0 6px 15px rgba(110, 71, 181, 0.3);
            text-decoration: none;
            width: 100%;
        }

        .call-btn i {
            margin-right: 10px;
            font-size: 18px;
            animation: ring 1.5s infinite;
        }

        @keyframes ring {
            0%, 100% { transform: rotate(0); }
            10%, 30% { transform: rotate(-10deg); }
            20%, 40% { transform: rotate(10deg); }
            50% { transform: rotate(0); }
        }

        .call-btn:hover {
            background: linear-gradient(135deg, var(--kuromi-pink), var(--kuromi-black));
            box-shadow: 0 8px 25px rgba(255, 133, 190, 0.4);
            transform: translateY(-3px);
        }
    </style>
</head>
<body>

    <div class="sparkle" style="left: 10%; width: 8px; height: 8px; animation-delay: 0s;"></div>
    <div class="sparkle" style="left: 30%; width: 12px; height: 12px; animation-delay: 2s;"></div>
    <div class="sparkle" style="left: 70%; width: 10px; height: 10px; animation-delay: 4s;"></div>
    <div class="sparkle" style="left: 85%; width: 6px; height: 6px; animation-delay: 1s;"></div>
    <div class="sparkle" style="left: 50%; width: 14px; height: 14px; animation-delay: 5s;"></div>

    <div class="profile-card">
        
        <!-- ขอบหูคุโรมิติดตั้งบนตัวการ์ด -->
        <div class="kuromi-ears">
            <div class="ear-left"></div>
            <div class="ear-right"></div>
        </div>
        <div class="kuromi-skull-badge">
            <i class="fa-solid fa-heart"></i>
        </div>

        <!-- โซนรูปถ่ายโปรไฟล์คุณปลาดุก -->
        <div class="avatar-container">
            <div class="avatar-circle">
                <img id="user-profile-img" src="1781770654106.jpg" alt="รูปโปรไฟล์อัฟฮัม" class="avatar-img" onerror="handleImageLoadError()">
                
                <!-- ตัวสัญลักษณ์แมวสำรองกรณีหารูปไม่เจอ -->
                <div id="fallback-avatar" class="avatar-fallback">
                    <i class="fa-solid fa-cat"></i>
                </div>
            </div>
        </div>

        <!-- ชื่อและชื่อเล่นของคุณปลาดุก -->
        <div class="name-wrapper">
            <h1 class="profile-name">
                คุณอัฟฮัม อินทโช <span class="nickname-badge">ปลาดุก</span>
            </h1>
        </div>
        <div class="id-badge">รหัสนักศึกษา: 694245015</div>

        <div class="info-list">
            
            <!-- คณะ -->
            <div class="info-card">
                <div class="info-icon">
                    <i class="fa-solid fa-graduation-cap"></i>
                </div>
                <div class="info-content">
                    <span class="info-title">คณะ</span>
                    <span class="info-text">วิทยาศาสตร์และเทคโนโลยี</span>
                </div>
            </div>

            <!-- สาขาวิชา -->
            <div class="info-card">
                <div class="info-icon">
                    <i class="fa-solid fa-laptop-code"></i>
                </div>
                <div class="info-content">
                    <span class="info-title">สาขาวิชา</span>
                    <span class="info-text">วิทยาการคอมพิวเตอร์</span>
                </div>
            </div>

            <!-- มหาวิทยาลัย -->
            <div class="info-card">
                <div class="info-icon">
                    <i class="fa-solid fa-university"></i>
                </div>
                <div class="info-content">
                    <span class="info-title">สถาบันการศึกษา</span>
                    <span class="info-text">มหาวิทยาลัยราชภัฏหมู่บ้านจอมบึง</span>
                </div>
            </div>

            <!-- เบอร์โทร -->
            <div class="info-card">
                <div class="info-icon">
                    <i class="fa-solid fa-phone"></i>
                </div>
                <div class="info-content">
                    <span class="info-title">เบอร์โทรศัพท์</span>
                    <span class="info-text"><a href="tel:0986979273">098-697-9273</a></span>
                </div>
            </div>

            <!-- อีเมล -->
            <div class="info-card">
                <div class="info-icon">
                    <i class="fa-solid fa-envelope"></i>
                </div>
                <div class="info-content">
                    <span class="info-title">อีเมล</span>
                    <span class="info-text"><a href="mailto:xafhamxinthcho@gmail.com">xafhamxinthcho@gmail.com</a></span>
                </div>
            </div>

        </div>

        <!-- ปุ่มโทรออกทันที -->
        <a href="tel:0986979273" class="call-btn" onclick="playBubbleSound()">
            <i class="fa-solid fa-phone-volume"></i> โทรติดต่อคุณปลาดุก
        </a>

    </div>

    <script>
        // ระบบสร้างเสียงตอนกดปุ่ม (Web Audio API)
        let audioCtx = null;
        function playBubbleSound() {
            try {
                if (!audioCtx) {
                    audioCtx = new (window.AudioContext || window.webkitAudioContext)();
                }
                const osc = audioCtx.createOscillator();
                const gain = audioCtx.createGain();
                osc.type = 'sine';
                osc.frequency.setValueAtTime(450, audioCtx.currentTime);
                osc.frequency.exponentialRampToValueAtTime(1100, audioCtx.currentTime + 0.15);
                
                gain.gain.setValueAtTime(0.15, audioCtx.currentTime);
                gain.gain.exponentialRampToValueAtTime(0.01, audioCtx.currentTime + 0.15);
                
                osc.connect(gain);
                gain.connect(audioCtx.destination);
                
                osc.start();
                osc.stop(audioCtx.currentTime + 0.15);
            } catch(e) {
                // ข้ามไปเพื่อป้องกันบราวเซอร์บล็อกเสียงเริ่มต้น
            }
        }

        // รายการนามสกุลรูปและชื่อไฟล์สำรองที่ระบบจะพยายามไล่สุ่มหาบน GitHub Pages
        const availableImagePaths = [
            '1781770654106.jpg',
            '1781770654106.JPG',
            '1781770654106.png',
            '1781770654106.PNG',
            '1781770654106.jpeg',
            '1781770654106.JPEG',
            'f15e75df-5cc0-4133-9c0f-ff1cedd104ec.jpg',
            'f15e75df-5cc0-4133-9c0f-ff1cedd104ec.JPG',
            'f15e75df-5cc0-4133-9c0f-ff1cedd104ec.jpeg',
            'f15e75df-5cc0-4133-9c0f-ff1cedd104ec.png'
        ];
        let currentTryIndex = 0;

        function handleImageLoadError() {
            const imgElement = document.getElementById('user-profile-img');
            const fallbackElement = document.getElementById('fallback-avatar');
            
            if (currentTryIndex < availableImagePaths.length - 1) {
                currentTryIndex++;
                imgElement.src = availableImagePaths[currentTryIndex];
            } else {
                // หากพยายามหาทุกรูปแล้วรูปแตกจริงๆ จะดึงตัวอวตาร์แมวสีม่วงพาสเทลขึ้นโชว์อย่างน่ารักแทนครับ
                imgElement.style.display = 'none';
                fallbackElement.style.display = 'flex';
            }
        }
    </script>
</body>
</html>
