<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>اختبار الانفرتر و الزوايا</title>
  <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;700&display=swap" rel="stylesheet" />
  <style>
    body {
      font-family: 'Cairo', sans-serif;
      background: #e3f2fd;
      padding: 20px;
      color: #333;
    }

    h2 {
      text-align: center;
      color: #1565c0;
      margin-bottom: 30px;
    }

    .question {
      background: #ffffff;
      padding: 20px;
      margin-bottom: 20px;
      border-radius: 15px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
      transition: transform 0.3s;
    }

    .question:hover {
      transform: scale(1.01);
    }

    .question p {
      font-weight: bold;
      color: #0d47a1;
    }

    .question label {
      display: block;
      margin: 8px 0;
      cursor: pointer;
    }

    input[type="text"],
    textarea {
      width: 100%;
      padding: 10px;
      margin-top: 10px;
      border-radius: 8px;
      border: 1px solid #ccc;
    }

    input[type="radio"] {
      margin-left: 8px;
    }

    textarea {
      resize: vertical;
      min-height: 100px;
    }

    button {
      display: block;
      margin: 30px auto;
      padding: 14px 28px;
      background: #1976d2;
      color: #fff;
      border: none;
      border-radius: 10px;
      font-size: 18px;
      cursor: pointer;
      transition: background 0.3s, transform 0.2s;
    }

    button:hover {
      background: #0d47a1;
      transform: scale(1.03);
    }

    #resultBox {
      text-align: center;
      font-weight: bold;
      margin-top: 20px;
      color: #1b5e20;
      background: #c8e6c9;
      padding: 20px;
      border-radius: 12px;
      border: 2px solid #66bb6a;
      display: none;
    }

    @media (max-width: 600px) {
      button {
        width: 100%;
      }
    }
  </style>
</head>
<body>

<!-- زر العودة -->
<div style="text-align: center; margin-bottom: 20px;">
  <a href="https://najy-hub.github.io/Solar-Professional-Engineer/"
     style="display: inline-block; padding: 12px 24px; background-color: #1976d2; color: white; border-radius: 10px; text-decoration: none; font-weight: bold;">
    ⬅️ العودة إلى صفحة الكورس
  </a>
</div>

<h2>📘 اختبار حول الانفرترات وزاوية الميل</h2>

<form action="https://script.google.com/macros/s/AKfycbzeO4zPScDZIi6FSjCo4ZEDJaJ8KOXFghSfaUhcF1Yb785kc56VuIgvoZTBjC9XOrkjVA/exec"
      method="POST"
      target="hidden_iframe"
      onsubmit="return handleSubmit();">

  <div class="question">
    <p>🧑‍🎓 الاسم الكامل:</p>
    <input type="text" name="name" required placeholder="أدخل اسمك الثلاثي">
  </div>

  <!-- الأسئلة -->
  <div class="question">
  <p>1. لا يتم تركيب نظام تتبع ميكانيكي (Tilt angle tracking) بسبب:</p>
    <label><input type="radio" name="q1" value="الصيانة"> الحاجة لصيانة دورية</label>
    <label><input type="radio" name="q1" value="الغيوم"> تأثير الطقس الغائم</label>
    <label><input type="radio" name="q1" value="كل ماذكر صحيح"> كل ماذكر صحيح</label>
  </div>

  <div class="question">
    <p>2. أيهما أفضل في الأنظمة الثابتة (Fixed Angle)؟</p>
    <label><input type="radio" name="q2" value="Constant yearly"> زاوية ثابتة طوال العام</label>
    <label><input type="radio" name="q2" value="Adjusted Seasonally"> زاوية متغيرة موسمياً</label>
  </div>

  <div class="question">
    <p>3. أي نوع من الانفرترات أفضل للأجواء الريفية أو الخلوية؟</p>
    <label><input type="radio" name="q3" value="Hyper inverter"> Hyper inverter</label>
    <label><input type="radio" name="q3" value="Battery inverter"> Battery inverter</label>
  </div>

  <div class="question">
    <p>4. في المحطات، أي انفرتر يسبب فقداً أكبر في القدرة بسبب خسائر النحاس؟</p>
    <label><input type="radio" name="q4" value="String inverter"> String inverter</label>
    <label><input type="radio" name="q4" value="Central inverter"> Central inverter</label>
  </div>

  <div class="question">
    <p>5. يستخدم Micro Inverter في حالة:</p>
    <label><input type="radio" name="q5" value="اختلاف الزوايا"> اختلاف الزوايا</label>
    <label><input type="radio" name="q5" value="وجود الظلال"> وجود ظلال</label>
    <label><input type="radio" name="q5" value="كل ماذكر صحيح"> كل ماذكر صحيح</label>
  </div>

  <div class="question">
    <p>6. ما هو البديل الأفضل لحالات Micro Inverter؟</p>
    <label><input type="radio" name="q6" value="Battery inverter"> Battery inverter</label>
    <label><input type="radio" name="q6" value="Hyper inverter"> Hyper inverter</label>
    <label><input type="radio" name="q6" value="Power Optimizer"> Power Optimizer</label>
    <label><input type="radio" name="q6" value="String inverter"> String inverter</label>
  </div>

  <div class="question">
    <p>7. ما هو Dry contact؟</p>
    <label><input type="radio" name="q7" value="ضبط الانفرتر"> مخرج ضبط الانفرتر</label>
    <label><input type="radio" name="q7" value="تشغيل المولد"> مخرج لتشغيل المولد الاحتياطي</label>
    <label><input type="radio" name="q7" value="تبريد الانفرتر"> مخرج تبريد الانفرتر</label>
  </div>

  <div class="question">
    <p>8. أي مرحلة MPPT لا تُستخدم مع كل البطاريات؟</p>
    <label><input type="radio" name="q8" value="Bulk Stage"> Bulk Stage</label>
    <label><input type="radio" name="q8" value="Absorpating Stage"> Absorpating Stage</label>
    <label><input type="radio" name="q8" value="Equalize Stage"> Equalize Stage</label>
    <label><input type="radio" name="q8" value="Floating Stage"> Floating Stage</label>
  </div>

  <div class="question">
    <p>9. لا يتأثر الانفرتر بدرجة الحرارة المحيطة؟</p>
    <label><input type="radio" name="q9" value="نعم"> نعم</label>
    <label><input type="radio" name="q9" value="لا"> لا</label>
  </div>

  <div class="question">
    <p>10. لتقليل التكلفة يمكن ضبط Output Mode على:</p>
    <label><input type="radio" name="q10" value="Utility mode"> Utility mode</label>
    <label><input type="radio" name="q10" value="Inverter Mode"> Inverter Mode</label>
  </div>

  <div class="question">
    <p>✍️ ملاحظاتك أو تعليقك (اختياري):</p>
    <textarea name="note" placeholder="اكتب أي ملاحظة أو تعليق هنا..."></textarea>
  </div>

  <input type="hidden" name="score" id="scoreField">
  <button type="submit">إرسال الإجابات</button>
</form>

<div id="resultBox"></div>
<iframe name="hidden_iframe" style="display:none;"></iframe>

<script>
function handleSubmit() {
  const correct = {
    q1: "كل ماذكر صحيح",
    q2: "Adjusted Seasonally",
    q3: "Battery inverter",
    q4: "Central inverter",
    q5: "كل ماذكر صحيح",
    q6: "Power Optimizer",
    q7:  "تشغيل المولد",
    q8: "Equalize Stage",
    q9: "لا",
    q10: "Inverter Mode"
  };

  let score = 0;
  for (let i = 1; i <= 10; i++) {
    const selected = document.querySelector(`input[name="q${i}"]:checked`);
    if (selected && selected.value === correct[`q${i}`]) {
      score++;
    }
  }

  const percentage = Math.round((score / 10) * 100);
  const resultText = `${score} من 10 (${percentage}%)`;
  document.getElementById("scoreField").value = resultText;

  setTimeout(() => {
    const name = document.querySelector('input[name="name"]').value;
    const note = document.querySelector('textarea[name="note"]').value;
    const box = document.getElementById("resultBox");
    box.style.display = "block";
    box.innerHTML = `✅ مرحبًا ${name}<br> نتيجتك: ${resultText}<br><br>✍️ ملاحظتك:<br>${note}`;
  }, 1000);

  return true;
}
</script>

</body>
</html>
