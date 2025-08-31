<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Mountain Group Festive Page 🎉</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    /* Reset */
    * { margin: 0; padding: 0; box-sizing: border-box; }

    /* Background Video */
    .video-bg {
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      object-fit: cover;
      z-index: -2;
    }

    /* Overlay */
    .overlay {
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: linear-gradient(rgba(255,200,150,0.5), rgba(150,0,100,0.5));
      z-index: -1;
    }

    body {
      font-family: "Segoe UI", sans-serif;
      color: #fffbe8;
      text-align: center;
      overflow-x: hidden;
    }

    .header {
      margin-top: 40px;
      font-size: 3em;
      font-weight: bold;
      text-shadow: 0 4px 16px rgba(0,0,0,0.4);
      animation: bounceIn 1.5s ease;
    }

    @keyframes bounceIn {
      0% { transform: scale(0.8); opacity: 0; }
      100% { transform: scale(1); opacity: 1; }
    }

    .ganpati {
      margin: 30px auto;
      border-radius: 20px;
      border: 4px solid #ffd54f;
      box-shadow: 0 8px 30px rgba(0,0,0,0.3);
      max-width: 340px;
      transition: transform 0.3s;
    }
    .ganpati:hover {
      transform: scale(1.07) rotate(-2deg);
    }

    .section-title {
      font-size: 2em;
      margin: 40px 0 20px;
      color: #ffd54f;
      text-shadow: 0 4px 16px rgba(0,0,0,0.6);
    }

    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px,1fr));
      gap: 20px;
      margin: 0 auto;
      max-width: 900px;
      padding: 20px;
    }

    .item {
      background: rgba(255,255,255,0.15);
      border-radius: 15px;
      overflow: hidden;
      backdrop-filter: blur(6px);
      border: 2px solid #ffd54f;
      transition: transform 0.3s;
    }
    .item:hover { transform: scale(1.05); }

    .item img, .item video {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }
    .caption {
      padding: 10px;
      font-weight: bold;
      background: rgba(0,0,0,0.4);
    }

    .cta {
      margin: 50px 0;
    }
    .cta a {
      display: inline-block;
      padding: 14px 28px;
      font-size: 1.2em;
      border-radius: 30px;
      background: linear-gradient(45deg,#ffd54f,#ff7043);
      color: #ad1457;
      text-decoration: none;
      font-weight: bold;
      box-shadow: 0 6px 20px rgba(0,0,0,0.3);
      transition: transform 0.3s;
    }
    .cta a:hover { transform: scale(1.08); }

    /* Confetti */
    .confetti {
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      pointer-events: none;
      z-index: 9999;
    }
  </style>
</head>
<body>

  <!-- Background Video -->
  <video autoplay muted loop class="video-bg">
    <source src="assets/bg.mp4" type="video/mp4">
    <!-- fallback if video doesn’t load -->
  </video>
  <div class="overlay"></div>

  <!-- Confetti -->
  <canvas class="confetti"></canvas>

  <div class="header">🎉 Mountain Group 🎉</div>

  <img src="https://i.postimg.cc/65dt2Z8M/image.png"
       alt="Ganpati"
       class="ganpati">

  

  <h2 class="section-title">✨ Glimpse of Festive Years ✨</h2>
<div class="gallery" style="display: flex; flex-wrap: wrap; gap: 20px; justify-content: center; align-items: stretch;">
    <div class="item" style="flex: 1 1 250px; max-width: 350px; display: flex; flex-direction: column;">
        <a href="#" onclick="openGalleryModal(); return false;">
            <img src="https://i.postimg.cc/dVLg3kwb/IMG-20250827-190540.jpg" alt="">
        </a>
        <div class="caption">Ganpati Celebration 2025 🎈</div>
    </div>
    <!-- Gallery Modal -->
     <div id="galleryModal" style="display:none; position:fixed; top:0; left:0; width:100vw; height:100vh; background:rgba(0,0,0,0.85); z-index:10000; align-items:center; justify-content:center;">
        <span onclick="closeGalleryModal()" style="position:absolute;top:30px;right:40px;font-size:2em;color:#ffd54f;cursor:pointer;">&times;</span>
        <div style="max-width:90vw;max-height:80vh;display:flex;flex-wrap:wrap;gap:20px;justify-content:center;align-items:center; overflow-y:auto; position:relative;">
            <button onclick="scrollGallery(-1)" style="position:absolute;left:-50px;top:50%;transform:translateY(-50%);background:#ffd54f;color:#ad1457;border:none;border-radius:50%;width:40px;height:40px;font-size:2em;cursor:pointer;z-index:1;">&#8593;</button>
            <div id="galleryImages" style="display:flex;flex-wrap:wrap;gap:20px;justify-content:center;align-items:center;">
                <img src="https://i.postimg.cc/J4PWGCJk/IMG-20250827-144949.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
                <img src="https://i.postimg.cc/4dzDGDsn/IMG-20250827-145140.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
                <img src="https://i.postimg.cc/C1y3WhyW/IMG-20250827-190029.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
                <img src="https://i.postimg.cc/y8G4yhL6/IMG-20250827-190049.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
                <img src="https://i.postimg.cc/3NYPxtx1/IMG-20250827-190137.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
                <img src="https://i.postimg.cc/X7NRM1h7/IMG-20250827-190205.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
                <img src="https://i.postimg.cc/zXd9qSZw/IMG-20250827-190243.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
                <img src="https://i.postimg.cc/g2QQZz0n/IMG-20250827-190628.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
                <img src="https://i.postimg.cc/LsP7kcqv/IMG-20250827-190630.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
                <img src="https://i.postimg.cc/1XvY5PTR/IMG-20250827-194914.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
                <img src="https://i.postimg.cc/xj5ZPyCr/IMG-20250827-194948.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
                <img src="https://i.postimg.cc/QxMyY99F/IMG-20250827-200323.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
                <!-- Add more images as needed -->
            </div>
            <button onclick="scrollGallery(1)" style="position:absolute;right:-50px;top:50%;transform:translateY(-50%);background:#ffd54f;color:#ad1457;border:none;border-radius:50%;width:40px;height:40px;font-size:2em;cursor:pointer;z-index:1;">&#8595;</button>
        </div>
        <script>
            function scrollGallery(dir) {
                const container = document.querySelector('#galleryModal > div > #galleryImages').parentElement;
                container.scrollBy({ top: dir * 200, behavior: 'smooth' });
            }
        </script>
    </div>
    <script>
        function openGalleryModal() {
            document.getElementById('galleryModal').style.display = 'flex';
        }
        function closeGalleryModal() {
            document.getElementById('galleryModal').style.display = 'none';
        }
    </script>
    
    <div class="item" style="flex: 1 1 250px; max-width: 350px; display: flex; flex-direction: column;">
        <a href="#" onclick="openLogoModal(); return false;">
            <img src="https://i.postimg.cc/jSgd0b2c/Whats-App-Image-2025-08-30-at-3-23-41-PM-1.jpg" alt="">
        </a>
        <div class="caption">Ganpati Celebration 2024 🎈</div>
    </div>
    <!-- Logo Modal -->
    <div id="logoModal" style="display:none; position:fixed; top:0; left:0; width:100vw; height:100vh; background:rgba(0,0,0,0.85); z-index:10000; align-items:center; justify-content:center;">
        <span onclick="closeLogoModal()" style="position:absolute;top:30px;right:40px;font-size:2em;color:#ffd54f;cursor:pointer;">&times;</span>
        <div style="max-width:90vw;max-height:80vh;display:flex;flex-wrap:wrap;gap:20px;justify-content:center;align-items:center; overflow-y:auto; position:relative;">
            <button onclick="scrollLogoGallery(-1)" style="position:absolute;left:-50px;top:50%;transform:translateY(-50%);background:#ffd54f;color:#ad1457;border:none;border-radius:50%;width:40px;height:40px;font-size:2em;cursor:pointer;z-index:1;">&#8593;</button>
            <div id="logoGalleryImages" style="display:flex;flex-wrap:wrap;gap:20px;justify-content:center;align-items:center;">
                <img src="https://i.postimg.cc/9fDXcnqh/Whats-App-Image-2025-08-30-at-3-23-52-PM.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
                <img src="https://i.postimg.cc/TwmRD59N/Whats-App-Image-2025-08-30-at-3-23-55-PM.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
                <img src="https://i.postimg.cc/8Cxpcmhr/Whats-App-Image-2025-08-30-at-3-23-57-PM.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
                <img src="https://i.postimg.cc/cCB0DqPQ/Whats-App-Image-2025-08-30-at-3-24-03-PM.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
                <img src="https://i.postimg.cc/ry1VyWzK/Whats-App-Image-2025-08-30-at-3-24-06-PM.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
                <img src="https://i.postimg.cc/8PT175rw/Whats-App-Image-2025-08-30-at-3-24-09-PM-1.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
                <img src="https://i.postimg.cc/02Z9DsYv/Whats-App-Image-2025-08-30-at-3-24-12-PM.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
                <img src="https://i.postimg.cc/K8zx5HfM/Whats-App-Image-2025-08-30-at-3-24-16-PM.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
                <!-- Add more logo images as needed -->
            </div>
            <button onclick="scrollLogoGallery(1)" style="position:absolute;right:-50px;top:50%;transform:translateY(-50%);background:#ffd54f;color:#ad1457;border:none;border-radius:50%;width:40px;height:40px;font-size:2em;cursor:pointer;z-index:1;">&#8595;</button>
        </div>
        <script>
            function scrollLogoGallery(dir) {
                const container = document.querySelector('#logoModal > div > #logoGalleryImages').parentElement;
                container.scrollBy({ top: dir * 200, behavior: 'smooth' });
            }
        </script>
    </div>
    <script>
        function openLogoModal() {
            document.getElementById('logoModal').style.display = 'flex';
        }
        function closeLogoModal() {
            document.getElementById('logoModal').style.display = 'none';
        }
    </script>
    <div class="item" style="flex: 1 1 250px; max-width: 350px; display: flex; flex-direction: column;">
        <a href="#" onclick="openMountainModal(); return false;">
            <img src="https://i.postimg.cc/kGSzsLh7/mountain-group-logo.png" alt="">
        </a>
        <div class="caption">Some old Memorable pictures</div>
    </div>
   <!-- Mountain Modal -->
<div id="mountainModal" style="display:none; position:fixed; top:0; left:0; width:100vw; height:100vh; background:rgba(0,0,0,0.85); z-index:10000; align-items:center; justify-content:center;">
    <span onclick="closeMountainModal()" style="position:absolute;top:30px;right:40px;font-size:2em;color:#ffd54f;cursor:pointer;">&times;</span>
    <div style="max-width:90vw;max-height:80vh;display:flex;flex-wrap:wrap;gap:20px;justify-content:center;align-items:center; overflow-y:auto; position:relative;">
        <button onclick="scrollMountainGallery(-1)" style="position:absolute;left:-50px;top:50%;transform:translateY(-50%);background:#ffd54f;color:#ad1457;border:none;border-radius:50%;width:40px;height:40px;font-size:2em;cursor:pointer;z-index:1;">&#8593;</button>
        <div id="mountainGalleryImages" style="display:flex;flex-wrap:wrap;gap:20px;justify-content:center;align-items:center;">
            <img src="https://i.postimg.cc/43McG0BC/Whats-App-Image-2025-08-30-at-3-18-53-PM.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
            <img src="https://i.postimg.cc/rs2t0tBQ/Whats-App-Image-2025-08-30-at-3-18-56-PM.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
            <img src="https://i.postimg.cc/NF821jYY/Whats-App-Image-2025-08-30-at-3-19-05-PM.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
            <img src="https://i.postimg.cc/ZY6NkVNg/Whats-App-Image-2025-08-30-at-3-19-18-PM.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
            <img src="https://i.postimg.cc/PrhwdYzq/Whats-App-Image-2025-08-30-at-3-19-36-PM.jpg" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
            <!-- Add more mountain images as needed -->
        </div>
        <button onclick="scrollMountainGallery(1)" style="position:absolute;right:-50px;top:50%;transform:translateY(-50%);background:#ffd54f;color:#ad1457;border:none;border-radius:50%;width:40px;height:40px;font-size:2em;cursor:pointer;z-index:1;">&#8595;</button>
    </div>
</div>
<script>
    function openMountainModal() {
        document.getElementById('mountainModal').style.display = 'flex';
    }
    function closeMountainModal() {
        document.getElementById('mountainModal').style.display = 'none';
    }
    function scrollMountainGallery(dir) {
        const container = document.querySelector('#mountainModal > div > #mountainGalleryImages').parentElement;
        container.scrollBy({ top: dir * 200, behavior: 'smooth' });
    }
</script>

<div class="item" style="flex: 1 1 250px; max-width: 350px; display: flex; flex-direction: column;">
    <a href="#" onclick="Createdby(); return false;">
        <img src="https://i.postimg.cc/8Pjjp4fN/Handdrawn-Circle-Logo.png" alt="">
    </a>
    <div class="caption">Created By</div>
</div>
<!-- Created by Modal -->
<div id="Createdby" style="display:none; position:fixed; top:0; left:0; width:100vw; height:100vh; background:rgba(0,0,0,0.85); z-index:10000; align-items:center; justify-content:center;">
    <span onclick="closeCreatedbyModal()" style="position:absolute;top:30px;right:40px;font-size:2em;color:#ffd54f;cursor:pointer;">&times;</span>
    <div style="max-width:90vw;max-height:80vh;display:flex;flex-wrap:wrap;gap:20px;justify-content:center;align-items:center; overflow-y:auto; position:relative;">
        <button onclick="scrollCreatedbyGallery(-1)" style="position:absolute;left:-50px;top:50%;transform:translateY(-50%);background:#ffd54f;color:#ad1457;border:none;border-radius:50%;width:40px;height:40px;font-size:2em;cursor:pointer;z-index:1;">&#8593;</button>
        <div id="createdbyGalleryImages" style="display:flex;flex-wrap:wrap;gap:20px;justify-content:center;align-items:center;">
            <img src="https://i.postimg.cc/DyHm8G1s/Date-25th-august-2025-2.png" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
            <img src="https://i.postimg.cc/yxrxhg5M/1.png" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
            <img src="https://i.postimg.cc/pLjr8dBS/aagaman-shola-with-date.png" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
            <img src="https://i.postimg.cc/MGbGPrNb/path-pujan-post.png" alt="" style="max-width:350px;max-height:350px;border-radius:12px;">
            <!-- Add more mountain images as needed -->
        </div>
        <button onclick="scrollCreatedbyGallery(1)" style="position:absolute;right:-50px;top:50%;transform:translateY(-50%);background:#ffd54f;color:#ad1457;border:none;border-radius:50%;width:40px;height:40px;font-size:2em;cursor:pointer;z-index:1;">&#8595;</button>
    </div>
</div>
<script>
    function Createdby() {
        document.getElementById('Createdby').style.display = 'flex';
    }
    function closeCreatedbyModal() {
        document.getElementById('Createdby').style.display = 'none';
    }
    function scrollCreatedbyGallery(dir) {
        const container = document.querySelector('#Createdby > div > #createdbyGalleryImages').parentElement;
        container.scrollBy({ top: dir * 200, behavior: 'smooth' });
    }
</script>
</div>

  <div class="cta">
    <a href="https://docs.google.com/forms/d/e/1FAIpQLSdl2KTyULymW6zRVk4Xv-ox8Sfe1R9bea6HzHxeh9FsABjt3g/viewform?usp=header" target="_blank">
      📝 Fill Our Festive Feedback Form!
    </a>
  </div>

  <script>
    const canvas=document.querySelector('.confetti'),ctx=canvas.getContext('2d');
    let W=window.innerWidth,H=window.innerHeight;
    canvas.width=W;canvas.height=H;
    let confetti=[];
    for(let i=0;i<80;i++){
      confetti.push({x:Math.random()*W,y:Math.random()*H,r:Math.random()*6+4,d:Math.random()*W/2,color:['#ffd54f','#ff7043','#ad1457','#fffbe8'][Math.floor(Math.random()*4)],tilt:Math.random()*10-5,tiltAngle:Math.random()*Math.PI*2});
    }
    function drawConfetti(){
      ctx.clearRect(0,0,W,H);
      confetti.forEach(c=>{
        ctx.beginPath();
        ctx.arc(c.x,c.y,c.r,0,Math.PI*2);
        ctx.fillStyle=c.color;ctx.fill();
      });
      updateConfetti();
    }
    function updateConfetti(){
      confetti.forEach(c=>{
        c.y+=Math.cos(c.d)*0.3+1+c.r/8;
        c.x+=Math.sin(c.d)*0.5;
        c.tiltAngle+=0.05;
        c.x+=Math.sin(c.tiltAngle)*0.4;
        if(c.y>H){c.y=-10;c.x=Math.random()*W;}
      });
    }
    function animate(){drawConfetti();requestAnimationFrame(animate);}
    animate();
    window.addEventListener('resize',()=>{W=window.innerWidth;H=window.innerHeight;canvas.width=W;canvas.height=H;});
  </script>
</body>
</html>
