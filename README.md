# landing
مشاوره تلفنی زانو درد

<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>مشاوره روانشناسی تلفنی | انتخاب بهترین مشاور</title>
    <meta name="description" content="در کمتر از ۳۰ ثانیه با پر کردن چند سوال ساده، مشاور مناسب شرایطت رو انتخاب کن.">
    <link href="https://cdn.jsdelivr.net/gh/rastikerdar/yekan-font@v3.0.0/dist/font-face.css" rel="stylesheet" type="text/css" />
    <style>
        body { font-family: 'Yekan Bakh', 'YekanBakh', 'Yekan', sans-serif; background: #fff; margin: 0; padding: 0; }
        .container { max-width: 500px; margin: auto; padding: 15px; }
        .question { background: #f0f4f8; padding: 15px; border-radius: 10px; margin-bottom: 120px; }
        .question h3 { margin: 0 0 10px; font-size: 18px; }
        .option label { display: flex; align-items: center; cursor: pointer; margin-bottom: 10px; }
        .option input[type="radio"] {
            appearance: none;
            width: 20px;
            height: 20px;
            border: 2px solid #333;
            border-radius: 2px;
            margin-left: 10px;
            position: relative;
        }
        .option input[type="radio"]:checked::before {
            content: "";
            position: absolute;
            top: 3px;
            left: 3px;
            width: 12px;
            height: 12px;
            background-color: #005de6;
        }
        .btn {
            font-family: inherit;
            display: block;
            width: 100%;
            padding: 10px;
            background: #005de6;
            color: white;
            border: none;
            border-radius: 8px;
            font-size: 16px;
            cursor: pointer;
            margin-top: 10px;
        }
        .btn-green {
            background: green;
            position: fixed;
            bottom: 80px;
            left: 50%;
            transform: translateX(-50%);
            width: calc(100% - 30px);
            max-width: 500px;
            padding: 10px;
            font-size: 16px;
            z-index: 1000;
            box-shadow: 0 6px 12px rgba(0,0,0,0.2), 0 0 10px rgba(0,128,0,0.3);
            border-radius: 8px;
            transition: background 0.3s ease;
        }
        .btn-green:hover { background: #009e00; }
        .highlight1 { background: #fff3cd; padding: 10px 15px; border-radius: 10px; margin: 10px 5px; }
        .highlight2 { background: #fff3cd; padding: 10px 15px; border-radius: 10px; margin: 10px 5px; }
        .video { width: 100%; border-radius: 10px; margin: 10px 0; }
        .form-input {
            padding: 10px 0px 10px 10px; /* افزایش ۴px پدینگ سمت راست */
            margin-bottom: 10px;
            border-radius: 8px;
            border: 1px solid #ccc;
            width: 100%;
        }
        .success {
            background: #cce5ff;
            padding: 20px;
            border-radius: 10px;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="container" id="top">
        <img src="https://cdn.hamkadeh.com/Kolii%D9%81%D9%84%D8%A7%D8%ADi%20(5).jpg" alt="مشاوره روانشناسی" style="width: 100%; border-radius: 12px;">
        
        <div class="highlight1">
            <strong>همین حالا پرسشنامه مشاوره روانشناسی رو پر کن تا متخصص مناسب شرایطت باهات تماس بگیره</strong><br>
            <a href="#q1" style="color: #005de6; font-weight: bold;">منم مشاوره میخوام  </a>
        </div>

        <div class="highlight2">
            <strong>اگر می‌خوای دقیق بدونی کدوم مشاور برای تو مناسبه و چه چیزی واقعاً بهت کمک می‌کنه، فقط کافیه چند سوال ساده رو جواب بدی.</strong>
            <br><br>
            <span>تو کمتر از ۳۰ ثانیه، مسیر مناسب مشاوره برات مشخص میشه. آخرش هم یه ویدیوی خیلی کوتاه برات داریم که ممکنه دیدگاهت رو کامل عوض کنه 👇</span>
        </div>

        <div style="background:#005de6; color:white; text-align:center; padding:10px 15px; border-radius:20px; font-weight:bold; font-size:15px; margin:15px 0;">
            فقط ۳۰ ثانیه وقت بذار تا بدونی دقیقاً چه مشاوره‌ای برای شرایط تو مناسبه – ببین و تصمیم بگیر 👇
        </div>

        <video class="video" controls playsinline preload="metadata" poster="https://cdn.hamkadeh.com/New-Landing-koli1%20(1).jpg">
        <source src="https://cdn.hamkadeh.com/falah2.mp4" type="video/mp4">
        مرورگر شما از ویدیو پشتیبانی نمی‌کند.
        </video>


        <form id="quiz">
            <div class="question" id="q1">
                <h3>سن شما در کدام بازه قرار دارد؟</h3>
                <div class="option"><label><input type="radio" name="age" value="20-30">۲۰ تا ۳۰ سال</label></div>
                <div class="option"><label><input type="radio" name="age" value="30-40">۳۰ تا ۴۰ سال</label></div>
                <div class="option"><label><input type="radio" name="age" value="40+">۴۰ سال به بالا</label></div>
                <button type="button" class="btn" onclick="next(2, 'age')">بعدی</button>
            </div>

            <div class="question" id="q2" style="display:none;">
                <h3>در حال حاضر چقدر احساس نیاز به مشاوره روانشناسی دارید؟</h3>
                <div class="option"><label><input type="radio" name="need" value="low">خیلی کم – فقط نیاز به شنیده شدن دارم</label></div>
                <div class="option"><label><input type="radio" name="need" value="medium">متوسط – گاهی اوقات فشار روحی زیادی دارم</label></div>
                <div class="option"><label><input type="radio" name="need" value="high">زیاد – نیاز به راهنمایی جدی دارم</label></div>
                <div class="option"><label><input type="radio" name="need" value="urgent">فوری – واقعاً به کمک تخصصی نیاز دارم</label></div>
                <button type="button" class="btn" onclick="next(3, 'need')">بعدی</button>
            </div>

            <div class="question" id="q3" style="display:none;">
                <h3>در چه زمینه‌ای بیشتر احساس نیاز به مشاوره دارید؟</h3>
                <div class="option"><label><input type="radio" name="area" value="family">روابط خانوادگی یا زناشویی</label></div>
                <div class="option"><label><input type="radio" name="area" value="anxiety">اضطراب، استرس یا بی‌قراری</label></div>
                <div class="option"><label><input type="radio" name="area" value="self">اعتماد به نفس یا شناخت خود</label></div>
                <div class="option"><label><input type="radio" name="area" value="other">سایر موارد روانشناختی</label></div>
                <button type="button" class="btn" onclick="next(4, 'area')">بعدی</button>
            </div>

            <div class="question" id="q4" style="display:none;">
                <h3>برای شروع مشاوره، لطفاً اطلاعات تماس خود را وارد کنید</h3>
                <input type="tel" name="phone" class="form-input" placeholder="شماره موبایل خود را وارد کنید" required>
                <button type="submit" class="btn">ارسال</button>
            </div>
        </form>

        <div id="success" class="success" style="display:none;">
            اطلاعات شما با موفقیت ثبت شد. منتظر تماس ما باشید.
            <br><br>
            <button class="btn" onclick="window.location.reload()">بازگشت به صفحه محصول</button>
        </div>
    </div>

    <button class="btn btn-green" onclick="scrollToTop()">همین حالا مشاوره‌تو شروع کن</button>

    <script>
        function next(step, fieldName) {
            const radios = document.getElementsByName(fieldName);
            let checked = false;
            for (let radio of radios) {
                if (radio.checked) {
                    checked = true;
                    break;
                }
            }
            if (!checked) {
                alert("لطفاً یکی از گزینه‌ها را انتخاب کنید");
                return;
            }
            for (let i = 1; i <= 4; i++) {
                document.getElementById("q" + i).style.display = (i === step) ? "block" : "none";
            }
        }

        function scrollToTop() {
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        document.getElementById("quiz").addEventListener("submit", function (e) {
            e.preventDefault();
            document.getElementById("quiz").style.display = "none";
            document.getElementById("success").style.display = "block";
        });
    </script>
</body>
</html>
