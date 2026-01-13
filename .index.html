<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>تطبيق فيزياء Tech - اختبار المتجهات</title>
    <style>
        :root { --primary-blue: #0033cc; --bg-dark: #121212; --card-bg: #1e1e1e; }
        body { background-color: var(--bg-dark); color: white; font-family: 'Segoe UI', Tahoma, sans-serif; margin: 0; display: flex; flex-direction: column; align-items: center; min-height: 100vh; }
        
        /* Header Style */
        .header { background-color: var(--primary-blue); width: 100%; padding: 40px 20px; text-align: center; border-bottom-left-radius: 30px; border-bottom-right-radius: 30px; box-shadow: 0 4px 15px rgba(0,0,0,0.3); box-sizing: border-box; }
        .header h1 { margin: 0; font-size: 28px; }
        .test-info { margin-top: 15px; font-size: 16px; color: #e0e0e0; line-height: 1.6; }

        /* Container */
        .container { width: 90%; max-width: 500px; margin: 30px 0; }
        .card { background-color: var(--card-bg); padding: 25px; border-radius: 20px; border: 1px solid #333; }

        /* Login Form */
        label { display: block; margin-bottom: 12px; font-size: 18px; }
        input[type="text"] { width: 100%; padding: 15px; border-radius: 12px; border: 1px solid #444; background: #2a2a2a; color: white; box-sizing: border-box; outline: none; margin-bottom: 10px; }
        .btn-action { width: 100%; padding: 15px; background-color: #1a53ff; color: white; border: none; border-radius: 15px; font-size: 18px; font-weight: bold; cursor: pointer; transition: 0.3s; }
        .btn-action:hover { background-color: #003ccb; }
        .error-msg { color: #ff4d4d; font-size: 14px; text-align: center; margin-top: 10px; display: none; }

        /* Quiz Style */
        .question-box { margin-bottom: 30px; padding-bottom: 15px; border-bottom: 1px solid #333; }
        .question-text { font-size: 17px; margin-bottom: 15px; color: #4dabff; font-weight: bold; }
        .options-list { list-style: none; padding: 0; }
        .option-item { background: #2a2a2a; padding: 12px; border-radius: 10px; margin-bottom: 8px; cursor: pointer; border: 1px solid transparent; transition: 0.2s; }
        .option-item:hover { border-color: #1a53ff; }
        .option-item input { margin-left: 10px; }
        
        /* Result Screen */
        .score-circle { width: 120px; height: 120px; border-radius: 50%; border: 5px solid #00ff00; display: flex; align-items: center; justify-content: center; font-size: 30px; margin: 20px auto; color: #00ff00; }
    </style>
</head>
<body>

<div class="header">
    <h1>تطبيق فيزياء Tech</h1>
    <div class="test-info">
        [span_1](start_span)تست الفيزياء رقم (2)[span_1](end_span)<br>
        [span_2](start_span)التاريخ: 13-01-2026[span_2](end_span)
    </div>
</div>

<div class="container" id="main-container">
    <div id="login-view" class="card">
        <label>اسم الطالب:</label>
        <input type="text" id="studentName" placeholder="أدخل اسمك للمتابعة...">
        <div id="login-error" class="error-msg"></div>
        <button class="btn-action" onclick="tryStartTest()">بدء الاختبار</button>
    </div>

    <div id="quiz-view" class="card" style="display: none;">
        <div id="questions-container"></div>
        <button class="btn-action" onclick="finishTest()">إنهاء الاختبار</button>
    </div>

    <div id="result-view" class="card" style="display: none; text-align: center;">
        <h2>انتهى الاختبار!</h2>
        <div class="score-circle" id="final-score">0/13</div>
        <p id="feedback-text"></p>
        <button class="btn-action" onclick="location.reload()">خروج</button>
    </div>
</div>

<script>
    const questions = [
        [span_3](start_span){ q: "اكتب المتجه A = (3, 4) بدلالة متجهات الوحدة الأساسية:[span_3](end_span)", options: ["3i + 4j", "4i + 3j", "3i - 4j", "7ij"], correct: 0 },
        [span_4](start_span){ q: "جسم يتحرك من P(1, -2, -3) إلى Q(4, 6, 1)، أوجد متجه الإزاحة:[span_4](end_span)", options: ["(3, 8, 4)", "(5, 4, -2)", "(3, 4, 4)", "(1, 1, 1)"], correct: 0 },
        [span_5](start_span){ q: "طائرة تطير بسرعة 200 شمالاً والرياح تهب شرقاً بسرعة h، أوجد المحصلة:[span_5](end_span)", options: ["206 كم/س", "250 كم/س", "150 كم/س", "200 كم/س"], correct: 0 },
        [span_6](start_span){ q: "إذا كان A=3i-2j و B=4i-j، أوجد A+B:[span_6](end_span)", options: ["7i - 3j", "7i + 3j", "-i + j", "i - j"], correct: 0 },
        [span_7](start_span){ q: "قيمة M التي تجعل المتجهين (3i+2j) و (Mi-6j) متعامدين:[span_7](end_span)", options: ["4", "2", "-4", "6"], correct: 0 },
        [span_8](start_span){ q: "الفرق الجوهري بين الكمية القياسية والكمية المتجهة هو:[span_8](end_span)", options: ["الاتجاه", "المقدار", "وحدة القياس", "الزمن"], correct: 0 },
        [span_9](start_span){ q: "نقطة تبعد عن الأصل مسافة R=10 وزاوية 60، إحداثياتها هي:[span_9](end_span)", options: ["(5, 8.66)", "(8.66, 5)", "(5, 5)", "(10, 60)"], correct: 0 },
        [span_10](start_span){ q: "متجه طوله 20 ويميل بزاوية 50 عن المحور الموجب، مركباته هي:[span_10](end_span)", options: ["Ax=12.8, Ay=15.3", "Ax=15.3, Ay=12.8", "Ax=10, Ay=10", "Ax=20, Ay=0"], correct: 0 },
        [span_11](start_span){ q: "متجهان متساويان (5 وحدات) والزاوية بينهما 90، أوجد المحصلة:[span_11](end_span)", options: ["7.07 وحدة", "10 وحدات", "5 وحدات", "25 وحدة"], correct: 0 }
    ];

    function tryStartTest() {
        const name = document.getElementById('studentName').value.trim();
        const errorDiv = document.getElementById('login-error');
        
        if (!name) {
            showError("يرجى إدخال اسمك!"); return;
        }

        // الحماية: منع تكرار الاسم أو إعادة الدخول
        let users = JSON.parse(localStorage.getItem('tech_users') || "[]");
        if (users.includes(name) || localStorage.getItem('tech_done_' + name)) {
            showError("عذراً، هذا الاسم مسجل مسبقاً أو انتهى من الاختبار.");
            return;
        }

        // بدء الاختبار
        users.push(name);
        localStorage.setItem('tech_users', JSON.stringify(users));
        localStorage.setItem('current_user', name);
        
        document.getElementById('login-view').style.display = 'none';
        showQuiz();
    }

    function showError(msg) {
        const errorDiv = document.getElementById('login-error');
        errorDiv.innerText = msg;
        errorDiv.style.display = 'block';
    }

    function showQuiz() {
        const container = document.getElementById('questions-container');
        document.getElementById('quiz-view').style.display = 'block';
        
        questions.forEach((item, i) => {
            let qHtml = `<div class="question-box">
                <div class="question-text">${i+1}. ${item.q}</div>
                <div class="options-list">`;
            item.options.forEach((opt, j) => {
                qHtml += `<label class="option-item">
                    <input type="radio" name="q${i}" value="${j}"> ${opt}
                </label>`;
            });
            qHtml += `</div></div>`;
            container.innerHTML += qHtml;
        });
    }

    function finishTest() {
        let score = 0;
        let currentUser = localStorage.getItem('current_user');

        questions.forEach((item, i) => {
            const selected = document.querySelector(`input[name="q${i}"]:checked`);
            if (selected && parseInt(selected.value) === item.correct) score++;
        });

        // منع الطالب من الدخول مرة أخرى
        localStorage.setItem('tech_done_' + currentUser, 'true');

        document.getElementById('quiz-view').style.display = 'none';
        document.getElementById('result-view').style.display = 'block';
        document.getElementById('final-score').innerText = `${score} / ${questions.length}`;
        document.getElementById('feedback-text').innerText = score >= (questions.length/2) ? "أحسنت، عمل رائع!" : "حاول مرة أخرى في المرة القادمة.";
    }

    // منع الخروج: إذا أغلق المتصفح بعد البدء سيعتبر "منتهي"
    window.onbeforeunload = function() {
        let user = localStorage.getItem('current_user');
        if (user) localStorage.setItem('tech_done_' + user, 'true');
    };
</script>
</body>
</html>
