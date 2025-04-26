# irteqi-everyday
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ارتقِ كل يوم</title>
    <style>
        body {
            background-color: #f9f7f7;
            font-family: 'Tajawal', sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            color: #5c4d7d;
        }
        header {
            background-color: #ffffff;
            padding: 20px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        header img {
            width: 80px;
        }
        h1 {
            margin-top: 10px;
            color: #7f56d9;
        }
        main {
            padding: 40px 20px;
        }
        .challenge {
            background-color: #ffffff;
            padding: 20px;
            margin: 20px auto;
            width: 90%;
            max-width: 500px;
            border-radius: 12px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }
        .start-button {
            background-color: #7f56d9;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 25px;
            font-size: 18px;
            cursor: pointer;
            margin-top: 20px;
        }
        .start-button:hover {
            background-color: #6842b7;
        }
    </style>
</head>
<body>

<header>
    <img src="logo.png" alt="شعار ارتقِ كل يوم">
    <h1>ارتقِ كل يوم</h1>
    <p>ارتقِ بذاتك، كل يوم بخطوة بسيطة ✨</p>
</header>

<main>
    <div class="challenge">
        <h2>تحدي اليوم</h2>
        <p id="challenge-text">💡 تحدى نفسك: ابتسم لخمسة أشخاص اليوم!</p>
        <button class="start-button" onclick="nextChallenge()">ابدأ تحديك الآن</button>
    </div>
</main>

<script>
    const challenges = [
        "💡 تحدى نفسك: ابتسم لخمسة أشخاص اليوم!",
        "💡 تحدى نفسك: اشرب لترين من الماء.",
        "💡 تحدى نفسك: خصص 10 دقائق للتأمل.",
        "💡 تحدى نفسك: اقرأ صفحة من كتاب تحبه.",
        "💡 تحدى نفسك: ساعد شخصاً دون أن تخبره.",
        "💡 تحدى نفسك: سجل ثلاثة أشياء أنت ممتن لها.",
        "💡 تحدى نفسك: اكتب هدفك لهذا الأسبوع.",
        "💡 تحدى نفسك: مارس رياضة خفيفة 15 دقيقة.",
        "💡 تحدى نفسك: اتصل بصديق قديم.",
        "💡 تحدى نفسك: نم قبل منتصف الليل اليوم.",
        "💡 تحدى نفسك: قل شكراً بصدق لشخص ساعدك.",
        "💡 تحدى نفسك: خصص وقتاً اليوم للاسترخاء الكامل.",
        "💡 تحدى نفسك: تعلم كلمة جديدة بلغة أجنبية.",
        "💡 تحدى نفسك: ابتعد عن مواقع التواصل 4 ساعات.",
        "💡 تحدى نفسك: جرب أكلة صحية جديدة.",
        "💡 تحدى نفسك: رتب غرفتك بالكامل.",
        "💡 تحدى نفسك: شاهد فيديو تحفيزي قصير.",
        "💡 تحدى نفسك: امشِ 5000 خطوة على الأقل.",
        "💡 تحدى نفسك: اكتُب فكرة مشروع صغيرة.",
        "💡 تحدى نفسك: تبرع بشيء قديم لشخص محتاج."
    ];

    function nextChallenge() {
        const randomIndex = Math.floor(Math.random() * challenges.length);
        document.getElementById('challenge-text').textContent = challenges[randomIndex];
    }
</script>

</body>
</html>
