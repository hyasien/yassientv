# yassientv
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>قنوات البث المباشر</title>
    <style>
        /* التصميم العام */
        body {
            font-family: 'Tajawal', Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #1a1a1a;
            color: #fff;
        }

        h1 {
            text-align: center;
            font-size: 1.0rem;
            margin: 20px 0;
            color: #ff4757;
        }

        /* الشاشة الكبيرة */
        .big-screen {
            width: 90%;
            max-width: 1800px;
            height: 60vh;
            background: #000;
            border-radius: 15px;
            margin: 20px auto;
            overflow: hidden;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
        }

        #mainFrame {
            width: 100%;
            height: 100%;
            border: none;
        }

        /* قائمة القنوات */
        .container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        .channel {
            position: relative;
            background: #2c3e50;
            border-radius: 15px;
            overflow: hidden;
            cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
            aspect-ratio: 16/9;
        }

        .channel:hover {
            transform: translateY(-10px);
            box-shadow: 0 12px 24px rgba(0, 0, 0, 0.5);
        }

        .channel iframe {
            width: 100%;
            height: 100%;
            border: none;
            pointer-events: none;
        }

        .channel::after {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            border: 3px solid transparent;
            border-radius: 15px;
            transition: border-color 0.3s;
        }

        .channel.active::after {
            border-color: #ff4757;
        }

        .channel .channel-name {
            position: absolute;
            bottom: 10px;
            left: 10px;
            background: rgba(0, 0, 0, 0.7);
            padding: 5px 10px;
            border-radius: 5px;
            font-size: 1rem;
            color: #fff;
        }

        /* التذييل */
        footer {
            text-align: center;
            padding: 20px;
            background: #2c3e50;
            margin-top: 40px;
            font-size: 0.9rem;
            color: #bdc3c7;
        }

        footer a {
            color: #ff4757;
            text-decoration: none;
        }

        footer a:hover {
            text-decoration: underline;
        }
    </style>
    <!-- خط Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@400;700&display=swap" rel="stylesheet">
</head>
<body>
    <h1>قنوات البث المباشر</h1>

    <!-- الشاشة الكبيرة -->
    <div class="big-screen">
        <iframe id="mainFrame" src="https://www.youtube.com/embed/xxxxxxxxxxx" allowfullscreen></iframe>
    </div>

    <!-- قائمة القنوات -->
    <div class="container">
        <div class="channel" data-src="http://www.elahmad.com/tv/mobiletv/glarb.php?id=manartv2">
            <iframe src="http://www.elahmad.com/tv/mobiletv/glarb.php?id=manartv2" allowfullscreen muted></iframe>
            <div class="channel-name">قناة المنار</div>
        </div>

	<div class="channel" data-src="https://www.elahmad.com/tv/watchtv.php?id=lbc">
            <iframe width="560" height="315" src="https://www.elahmad.com/tv/watchtv.php?id=lbc" style="border:none;" allowfullscreen allow="autoplay; fullscreen; picture-in-picture; xr-spatial-tracking; encrypted-media"></iframe>
            <div class="channel-name">قناة ال بي سي</div>
        </div>

	<div class="channel" data-src="https://www.elahmad.com/tv/watchtv.php?id=aljadeed">
            <iframe width="560" height="315" src="https://www.elahmad.com/tv/watchtv.php?id=aljadeed" style="border:none;" allowfullscreen allow="autoplay; fullscreen; picture-in-picture; xr-spatial-tracking; encrypted-media"></iframe>
            <div class="channel-name">قناة الجديد</div>
   	 </div>

	<div class="channel" data-src="https://www.elahmad.com/tv/mtvlebanon.htm">
           <iframe width="560" height="315" src="https://www.elahmad.com/tv/watchtv.php?id=otv_lebanon" style="border:none;" allowfullscreen allow="autoplay; fullscreen; picture-in-picture; xr-spatial-tracking; encrypted-media">	</iframe>
            <div class="channel-name">قناة ام تي في</div>
	</div>	
	<div class="channel" data-src="https://www.elahmad.com/tv/watchtv.php?id=otv_lebanon">
           <iframe width="560" height="315" src="https://www.elahmad.com/tv/watchtv.php?id=otv_lebanon" style="border:none;" allowfullscreen allow="autoplay; fullscreen; 	picture-in-picture; xr-spatial-tracking; encrypted-media">	</iframe>
            <div class="channel-name">قناة OTV</div>
  	</div>
	<div class="channel" data-src="https://www.elahmad.com/tv/mobiletv/glarb.php?id=nbn">
	<iframe width="560" height="315" src="https://www.elahmad.com/tv/mobiletv/glarb.php?id=nbn" style="border:none;" allowfullscreen allow="autoplay; fullscreen; picture-	in-picture; xr-spatial-tracking; encrypted-media"></iframe>
	<div class="channel-name">قناة ان بي ان</div>
	</div>
	<div class="channel" data-src="https://www.elahmad.com/tv/mobiletv/glarb.php?id=teleliban">
	<iframe width="560" height="315" src="https://www.elahmad.com/tv/mobiletv/glarb.php?id=teleliban" style="border:none;" allowfullscreen allow="autoplay; fullscreen; 	picture-in-picture; xr-spatial-tracking; encrypted-media"></iframe>
	<div class="channel-name">تلفزيون لبنان</div>
	</div>

        <div class="channel" data-src="http://www.elahmad.com/tv/mobiletv/glarb.php?id=almayadeen1">
            <iframe src="http://www.elahmad.com/tv/mobiletv/glarb.php?id=almayadeen1" allowfullscreen muted></iframe>
            <div class="channel-name">قناة الميادين</div>
        </div>

        <div class="channel" data-src="https://www.elahmad.com/tv/mobiletv/glarb.php?id=aljazeer_ar1">
            <iframe src="https://www.elahmad.com/tv/mobiletv/glarb.php?id=aljazeer_ar1" allowfullscreen muted></iframe>
            <div class="channel-name">قناة الجزيرة</div>

        </div>
<div class="channel" data-src="https://www.elahmad.com/tv/mobiletv/glarb.php?id=alarabiya1">
        <iframe width="560" height="315" src="https://www.elahmad.com/tv/mobiletv/glarb.php?id=alarabiya1" style="border:none;" allowfullscreen allow="autoplay; fullscreen; picture-in-picture; xr-spatial-tracking; encrypted-media"></iframe>
	<div class="channel-name">قناة العربية</div>
 	
</div>
<div class="channel" data-src="https://www.elahmad.com/tv/mobiletv/glarb.php?id=alarabytv">
           <iframe width="560" height="315" src="https://www.elahmad.com/tv/mobiletv/glarb.php?id=alarabytv" style="border:none;" allowfullscreen allow="autoplay; fullscreen; picture-in-picture; xr-spatial-tracking; encrypted-media"></iframe>
            <div class="channel-name">قناة العربي</div>
  </div>
<div class="channel" data-src="https://www.elahmad.com/tv/mobiletv/glarb.php?id=alhurra">
           <iframe width="560" height="315" src="https://www.elahmad.com/tv/mobiletv/glarb.php?id=alhurra" style="border:none;" allowfullscreen allow="autoplay; fullscreen; picture-in-picture; xr-spatial-tracking; encrypted-media"></iframe>
            <div class="channel-name">قناة الحرة</div>
  </div>
<div class="channel" data-src="https://www.elahmad.com/tv/mobiletv/glarb.php?id=skynews_ar1">
           <iframe width="560" height="315" src="https://www.elahmad.com/tv/mobiletv/glarb.php?id=skynews_ar1" style="border:none;" allowfullscreen allow="autoplay; fullscreen; picture-in-picture; xr-spatial-tracking; encrypted-media"></iframe>
            <div class="channel-name">قناة سكاي نيوز</div>
  </div>

  
    <script>
        // تحديد جميع القنوات
        const channels = document.querySelectorAll('.channel');
        const mainFrame = document.getElementById('mainFrame');

        // إضافة حدث النقر لكل قناة
        channels.forEach(channel => {
            channel.addEventListener('click', () => {
                // إزالة النشاط من جميع القنوات
                channels.forEach(c => c.classList.remove('active'));
                // إضافة مؤشر النشاط للقناة المختارة
                channel.classList.add('active');
                // تغيير مصدر الشاشة الكبيرة
                const newSrc = channel.getAttribute('data-src');
                mainFrame.src = newSrc;
            });
        });

        // تشغيل أول قناة افتراضيًا
        channels[0].click();
    </script>
</body>
</html>
