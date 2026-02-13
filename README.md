<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Enchanted Bloom · flower shop</title>
    <!-- Font Awesome for icons (optional but adds charm) -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Roboto, 'Helvetica Neue', sans-serif;
        }

        body {
            background-color: #faf3ea;  /* warm, soft background */
        }

        /* main container with a subtle paper texture feel */
        .shop-wrapper {
            max-width: 1300px;
            margin: 0 auto;
            padding: 2rem 1.5rem;
            background-color: #fffcf7;
            box-shadow: 0 20px 40px -15px rgba(100, 70, 40, 0.2);
        }

        /* ---------- EXTERIOR / HEADER SECTION ---------- */
        .exterior {
            background: #d9e6d4;  /* soft sage green base */
            background-image: radial-gradient(circle at 20% 30%, #e3f0dc 5%, transparent 15%),
                              radial-gradient(circle at 90% 70%, #f1f7e8 8%, transparent 20%);
            border-radius: 48px 48px 30px 30px;
            padding: 2rem 2rem 1.5rem 2rem;
            margin-bottom: 3rem;
            border: 6px solid #f1dbc0;  /* warm wood trim */
            box-shadow: 0 10px 0 #9f8b77;
            position: relative;
        }

        .exterior-content {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            align-items: center;
        }

        .shop-sign {
            background: #f7e5c2;
            padding: 1.2rem 2.2rem;
            border-radius: 60px 60px 30px 30px;
            box-shadow: 0 6px 0 #b89b7a, inset 0 2px 10px #fff9e6;
            border: 2px solid #e2c7a1;
            transform: rotate(-1deg);
        }

        .shop-sign h1 {
            font-size: 2.6rem;
            font-weight: 600;
            letter-spacing: 2px;
            color: #2f4d3c;
            text-shadow: 2px 2px 0 #ffefc0;
            font-family: 'Trebuchet MS', 'Lucida Grande', sans-serif;
        }

        .shop-sign h1 i {
            color: #c7385f;
            font-size: 2.2rem;
            margin: 0 6px;
        }

        .flower-box-bike {
            display: flex;
            gap: 1.5rem;
            align-items: flex-end;
            flex-wrap: wrap;
            justify-content: center;
        }

        .bike {
            background: #b7d6b2;
            padding: 1rem 1.5rem 0.5rem 1.5rem;
            border-radius: 80px 80px 30px 30px;
            border: 2px solid #7f9a7a;
            box-shadow: inset 0 -8px 0 #849f7e;
        }

        .bike i {
            font-size: 5rem;
            color: #516d4a;
            filter: drop-shadow(2px 6px 0 #3e5538);
        }

        .bike .sunflowers {
            font-size: 2rem;
            letter-spacing: 8px;
            color: #f3b33d;
            text-shadow: 0 3px 0 #b46118;
        }

        .window-boxes {
            background: #aec0a8;
            border-radius: 40px 40px 20px 20px;
            padding: 0.8rem 2rem;
            color: #233d26;
            font-weight: bold;
            display: flex;
            gap: 1.2rem;
            font-size: 1.5rem;
            border: 2px solid #728b6b;
        }

        .window-boxes i {
            background: #b93b5a;
            color: white;
            padding: 8px;
            border-radius: 50%;
        }

        /* ---------- RAINBOW WALL (interior feature) ---------- */
        .rainbow-wall {
            background: linear-gradient(145deg, #f9eec1, #fff2d4);
            border-radius: 40px 40px 20px 20px;
            padding: 2rem 1.5rem;
            margin-bottom: 2.5rem;
            border-left: 10px solid #f1b6c5;
            border-right: 10px solid #b3d9b0;
            box-shadow: inset 0 0 0 3px white, 0 10px 15px -8px #7f6e5b;
            display: flex;
            flex-wrap: wrap;
            justify-content: space-around;
            gap: 1.5rem;
        }

        .terrarium-group {
            display: flex;
            flex-wrap: wrap;
            gap: 1.2rem;
            justify-content: center;
        }

        .glass-item {
            background: rgba(255, 255, 255, 0.6);
            backdrop-filter: blur(3px);
            border-radius: 50% 50% 40% 40%;
            padding: 1rem 1rem 0.5rem 1rem;
            box-shadow: 0 12px 0 #d3c3a4, 0 0 0 3px #dabfa7;
            text-align: center;
            min-width: 90px;
        }

        .glass-item i {
            font-size: 2.5rem;
            color: #2b6e4f;
        }

        .glass-item span {
            display: block;
            background: #f7b1ab;
            padding: 0.3rem;
            border-radius: 30px;
            font-size: 0.8rem;
            font-weight: bold;
            color: #2c472c;
        }

        /* rustic tables */
        .rustic-tables {
            background: #ac8e68;  /* wood base */
            background-image: repeating-linear-gradient(90deg, #8b6f50 1px, #c9a87c 3px, #b48d5f 6px);
            border-radius: 60px 60px 30px 30px;
            padding: 1.8rem 1.2rem;
            margin: 2.5rem 0;
            border: 4px solid #6d4f32;
            box-shadow: 0 15px 0 #534433;
        }

        .table-grid {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 2rem 1.2rem;
        }

        .bucket {
            background: #c0b0a0;
            border: 3px solid #616247;
            border-radius: 20px 20px 40px 40px;
            padding: 0.6rem 0.4rem 1.2rem 0.4rem;
            min-width: 130px;
            text-align: center;
            box-shadow: inset 0 -6px 0 #7d705b, 0 6px 0 #4d453a;
            transform: rotate(0.5deg);
        }

        .bucket i {
            font-size: 2.2rem;
            margin: 0 3px;
            filter: drop-shadow(0 4px 2px #ba9f88);
        }

        .bucket .label {
            background: #fcf2cf;
            border-radius: 40px;
            padding: 0.2rem 0.5rem;
            font-size: 0.8rem;
            font-weight: 600;
            color: #1c3f29;
            margin-top: 5px;
            border: 1px solid #ed9e6c;
        }

        /* dried flower corner */
        .dried-corner {
            background: #ecdcc0;
            border-radius: 80px 20px 80px 20px;
            padding: 2rem 2rem;
            margin: 2rem 0;
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            justify-content: space-between;
            border: 3px dashed #b1946e;
        }

        .dried-hanging {
            font-size: 3rem;
            word-spacing: 20px;
            color: #866b49;
            text-shadow: 0 4px 0 #cfa26b;
        }

        .dried-corner p {
            font-size: 1.4rem;
            background: #ccb28b;
            padding: 0.6rem 1.2rem;
            border-radius: 100px;
            color: #2f3523;
            font-weight: 600;
        }

        /* design counter */
        .design-counter {
            background: #dad0c0;
            background: linear-gradient(145deg, #e5d7c3, #cfc1ad);
            border-radius: 50px 50px 20px 20px;
            padding: 1.5rem 2rem;
            margin: 2rem 0;
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            justify-content: space-between;
            border: 5px solid #ac9b84;
            box-shadow: 0 12px 0 #786a56;
        }

        .counter-items i {
            font-size: 2.2rem;
            background: white;
            padding: 12px;
            border-radius: 50%;
            color: #ad5a71;
            box-shadow: 0 4px 0 #af8b6b;
            margin: 0 5px;
        }

        .mirror {
            background: #bfd5e3;
            padding: 1rem 2.2rem;
            border-radius: 20px 20px 40px 40px;
            font-size: 2rem;
            border: 3px solid #5e7a94;
            box-shadow: inset 0 0 15px #b1d0e6;
            font-weight: bold;
            color: #2d4b65;
        }

        /* atmosphere card */
        .atmosphere {
            background: #fef6dd;
            background-image: radial-gradient(circle at 10% 20%, #fffde7 5%, transparent 30%),
                              radial-gradient(circle at 90% 70%, #fff0d4 10%, transparent 30%);
            border-radius: 130px 30px 130px 30px;
            padding: 2.2rem 2.5rem;
            margin: 2rem 0 0.5rem 0;
            border: 2px solid #eaccad;
            box-shadow: 0 15px 0 #e1ba93, inset 0 0 30px #fffaee;
            font-size: 1.3rem;
            line-height: 1.7;
            color: #4d4132;
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
            align-items: center;
        }

        .atmosphere i {
            font-size: 3rem;
            background: #b5d9b2;
            border-radius: 50%;
            padding: 0.7rem;
            color: #446b41;
        }

        .footer-note {
            text-align: center;
            margin-top: 3rem;
            font-size: 1.2rem;
            background: #ffe4c4;
            padding: 1rem;
            border-radius: 60px;
            border: 2px solid #f4b393;
            color: #233d2b;
        }

        .footer-note i {
            color: #cd4c6d;
        }

        hr {
            border: 2px solid #ebd5b0;
            margin: 2rem 0;
        }

        /* small extras */
        .flower-emoji-rainbow {
            font-size: 2rem;
            text-align: center;
            word-spacing: 15px;
        }

        /* responsive touches */
        @media (max-width: 700px) {
            .shop-sign h1 { font-size: 2rem; }
            .exterior-content { justify-content: center; }
        }
    </style>
</head>
<body>
    <div class="shop-wrapper">
        <!-- EXTERIOR section (with bike, sign, window boxes) -->
        <section class="exterior">
            <div class="exterior-content">
                <div class="shop-sign">
                    <h1>
                        <i class="fas fa-seedling"></i> 
                        The Enchanted Bloom 
                        <i class="fas fa-leaf"></i>
                    </h1>
                </div>
                <div class="flower-box-bike">
                    <div class="bike">
                        <i class="fas fa-bicycle"></i>
                        <div class="sunflowers">
                            <i class="fas fa-sun"></i> 🌻🌻🌻 
                        </div>
                    </div>
                    <div class="window-boxes">
                        <i class="fas fa-fan"></i> PETUNIAS 
                        <i class="fas fa-fan"></i> GERANIUMS 
                        <i class="fas fa-tree"></i>
                    </div>
                </div>
            </div>
            <!-- tiny flower box detail -->
            <div style="text-align: center; margin-top: 20px; color: #3f5c37; font-weight: 500;">
                <i class="fas fa-flower"></i>  vintage mint bike · overflowing blooms  <i class="fas fa-flower"></i>
            </div>
        </section>

        <!-- ENTRANCE bell & tile fragrance -->
        <div style="display: flex; justify-content: space-between; align-items: center; margin: 20px 0 10px; background: #f2e5d4; padding: 0.5rem 1.5rem; border-radius: 60px;">
            <span style="font-size: 2rem;">🔔 ✨</span>
            <span style="font-weight: 300; font-style: italic; color: #804e4e;"><i class="fas fa-rose"></i> the air is sweet with rose & eucalyptus <i class="fas fa-spray-can-sparkles"></i></span>
            <span style="background: #fad5d5; padding: 0.4rem 1rem; border-radius: 40px;">pastel tile floor</span>
        </div>

        <!-- RAINBOW WALL (hanging terrariums + geometric shelves) -->
        <section class="rainbow-wall">
            <div class="terrarium-group">
                <div class="glass-item"><i class="fas fa-leaf"></i><span>air plant</span></div>
                <div class="glass-item"><i class="fas fa-cactus"></i><span>cactus</span></div>
                <div class="glass-item"><i class="fas fa-tree"></i><span>kalanchoe</span></div>
                <div class="glass-item"><i class="fas fa-feather"></i><span>echeveria</span></div>
            </div>
            <div style="color:#4d3775; font-weight: bold; background: #fee3b8; border-radius: 50px; padding: 0.5rem 1.5rem;">
                <i class="fas fa-paint-roller"></i> A LIVING TAPESTRY OF COLOR
            </div>
        </section>

        <!-- RUSTIC TABLES with buckets and vases -->
        <section class="rustic-tables">
            <div class="table-grid">
                <!-- bucket 1 -->
                <div class="bucket"><i class="fas fa-leaf" style="color: #f2b0c6;"></i> <i class="fas fa-leaf" style="color: #f6e683;"></i> <i class="fas fa-leaf" style="color: #bbd9b4;"></i> <div class="label">calla lilies · white</div></div>
                <div class="bucket"><i class="fas fa-sun-plant-wilt" style="color: #edc13a;"></i> <i class="fas fa-sun-plant-wilt" style="color: #e5942a;"></i> <div class="label">sunflowers · yellow</div></div>
                <div class="bucket"><i class="fas fa-leaf" style="color: #f084b3;"></i> <i class="fas fa-leaf" style="color: #ef8fbc;"></i> <div class="label">peonies · pink</div></div>
                <div class="bucket"><i class="fas fa-leaf" style="color: #bf4343;"></i> <i class="fas fa-leaf" style="color: #cf5a5a;"></i> <div class="label">tulips · red</div></div>
                <div class="bucket"><i class="fas fa-leaf" style="color: #9b70cf;"></i> <i class="fas fa-leaf" style="color: #8a4ec4;"></i> <div class="label">irises · purple</div></div>
            </div>
            <p style="text-align: center; margin-top: 25px; background: #fef7ae; display: inline-block; padding: 0.4rem 2rem; border-radius: 60px; font-weight: 600; border: 2px solid #b0845c;">
                🌼 reclaimed barn wood · buckets & ceramic vases 🌼
            </p>
        </section>

        <!-- DRIED FLOWER CORNER -->
        <section class="dried-corner">
            <span class="dried-hanging">
                🌾 💐 🌿 🌸 🌾
            </span>
            <p>
                <i class="fas fa-dragon"></i> dried lavender · pampas · statice · wheat
            </p>
        </section>

        <!-- DESIGN COUNTER with mirror -->
        <section class="design-counter">
            <div class="counter-items">
                <i class="fas fa-twine"></i>
                <i class="fas fa-scroll"></i>
                <i class="fas fa-pencil"></i>
                <i class="fas fa-crop"></i>
            </div>
            <div class="mirror">
                <i class="fas fa-arrow-left"></i> MIRROR <i class="fas fa-arrow-right"></i>
            </div>
            <span style="background: #eccfaf; padding: 0.5rem 1rem; border-radius: 40px;">💐 friendly florist</span>
        </section>

        <!-- ATMOSPHERE (light, music, fountain) -->
        <section class="atmosphere">
            <i class="fas fa-sun"></i>
            <span>☀️ sunbeams catch the dust · colors glow</span>
            <i class="fas fa-music"></i>
            <span>soft music · trickling fountain</span>
            <i class="fas fa-heart"></i>
            <span>a pocket of joy</span>
        </section>

        <!-- small divider with quote -->
        <hr>
        <div class="flower-emoji-rainbow">
            🌷🌺🌸🌼🌻🌹🥀🌿🌾💐
        </div>

        <!-- footer note -->
        <div class="footer-note">
            <i class="fas fa-store"></i>  The Enchanted Bloom · a feast for the senses  <i class="fas fa-fan"></i>
        </div>

        <!-- tiny description (from original) -->
        <p style="margin-top: 2rem; text-align: center; font-size: 1rem; background: #e1dccd; padding: 1rem; border-radius: 40px; color:#2c4433;">
            ✨ a beautiful, colorful flower shop — where every bucket tells a story, and the walls bloom with joy. 
            hand-painted sign, sage green trim, and a vintage bicycle with sunflowers. ✨
        </p>
    </div>
</body>
</html>
