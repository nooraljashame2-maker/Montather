<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>تطبيق سراج التعليمي - الصف الثالث الابتدائي</title>
    <link rel="stylesheet" href="style.css">
    <!-- استيراد الخطوط والأيقونات -->
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700;900&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>

    <!-- رأس التطبيق -->
    <header class="app-header">
        <div class="user-welcome">
            <div class="avatar"><i class="fa-solid fa-graduation-cap"></i></div>
            <div>
                <h1>أهلاً بك يا بطلنا سراج! 🌟</h1>
                <p>الصف الثالث الابتدائي - رحلة التعلم المتفوقة</p>
            </div>
        </div>
        <div class="score-board">
            <span id="stars-count"><i class="fa-solid fa-star text-gold"></i> <span class="num">12</span> نجوم</span>
            <button class="btn-add-lesson" onclick="openAddLessonModal()"><i class="fa-solid fa-plus-circle"></i> إضافة درس</button>
        </div>
    </header>

    <!-- المحتوى الرئيسي -->
    <main class="container">
        <!-- قسم المواد الدراسية -->
        <section class="subjects-section">
            <h2><i class="fa-solid fa-book-open"></i> مواد الصف الثالث الابتدائي</h2>
            <div class="subjects-grid" id="subjects-grid">
                <!-- المواد الأساسية -->
                <div class="subject-card arabic" onclick="openSubject('القراءة العربية', 'arabic')">
                    <div class="icon-box"><i class="fa-solid fa-book-bookmark"></i></div>
                    <h3>القراءة العربية</h3>
                    <p>قواعد، محفوظات، ونصوص تفاعلية</p>
                </div>
                <div class="subject-card math" onclick="openSubject('الرياضيات', 'math')">
                    <div class="icon-box"><i class="fa-solid fa-calculator"></i></div>
                    <h3>الرياضيات</h3>
                    <p>جدول الضرب، الأرقام والتمارين</p>
                </div>
                <div class="subject-card science" onclick="openSubject('العلوم', 'science')">
                    <div class="icon-box"><i class="fa-solid fa-flask"></i></div>
                    <h3>العلوم</h3>
                    <p>الكائنات الحية، النباتات والبيئة</p>
                </div>
                <div class="subject-card english" onclick="openSubject('اللغة الإنجليزية', 'english')">
                    <div class="icon-box"><i class="fa-solid fa-language"></i></div>
                    <h3>English</h3>
                    <p>الحروف، الكلمات والمحادثة</p>
                </div>
                <div class="subject-card islamic" onclick="openSubject('التربية الإسلامية', 'islamic')">
                    <div class="icon-box"><i class="fa-solid fa-mosque"></i></div>
                    <h3>التربية الإسلامية</h3>
                    <p>القرآن الكريم والحديث الشريف</p>
                </div>
            </div>
        </section>

        <!-- منطقة عرض الدروس التفاعلية مع خاصية النطق -->
        <section class="lesson-viewer-section" id="lesson-viewer" style="display: none;">
            <div class="viewer-header">
                <button class="btn-back" onclick="closeSubject()"><i class="fa-solid fa-arrow-right"></i> عودة للمواد</button>
                <h2 id="current-subject-title">عنوان المادة</h2>
                <button class="btn-speak-all" onclick="speakFullLesson()"><i class="fa-solid fa-volume-high"></i> قراءة الدرس كاملاً</button>
            </div>
            
            <div class="lessons-list-container" id="lessons-list-container">
                <!-- سيتم تعبئة الدروس هنا ديناميكياً -->
            </div>
        </section>
    </main>

    <!-- نافذة منبثقة لإضافة درس جديد -->
    <div class="modal" id="add-lesson-modal" style="display: none;">
        <div class="modal-content">
            <span class="close-btn" onclick="closeAddLessonModal()">&times;</span>
            <h2><i class="fa-solid fa-pen-to-square"></i> إضافة درس جديد لسراج</h2>
            <form id="add-lesson-form" onsubmit="saveNewLesson(event)">
                <div class="form-group">
                    <label>اختر المادة:</label>
                    <select id="lesson-subject-select" required>
                        <option value="arabic">القراءة العربية</option>
                        <option value="math">الرياضيات</option>
                        <option value="science">العلوم</option>
                        <option value="english">اللغة الإنجليزية</option>
                        <option value="islamic">التربية الإسلامية</option>
                    </select>
                </div>
                <div class="form-group">
                    <label>عنوان الدرس:</label>
                    <input type="text" id="lesson-title-input" placeholder="مثال: محادثة والحواس الخمس" required>
                </div>
                <div class="form-group">
                    <label>نص الدرس (انقر على أي كلمة لاحقاً لتسمع نطقها):</label>
                    <textarea id="lesson-content-input" rows="5" placeholder="اكتب نص الدرس هنا بالتفصيل..." required></textarea>
                </div>
                <button type="submit" class="btn-save">حفظ الدرس في النظام <i class="fa-solid fa-check"></i></button>
            </form>
        </div>
    </div>

    <script>
        // قاعدة بيانات افتراضية ومخزنة محلياً للدروس
        let lessonsData = JSON.parse(localStorage.getItem('siraj_lessons')) || {
            arabic: [
                { title: "الدرس الأول: أداة الاستحمام والنظافة", content: "النظافة من الإيمان يا سراج. يحافظ التلميذ النظيف على كتبه وملابسه وكتب مدرسته يومياً." }
            ],
            math: [
                { title: "جدول الضرب (2)", content: "اثنان في واحد يساوي اثنان. اثنان في اثنان يساوي أربعة. اثنان في ثلاثة يساوي ستة." }
            ],
            science: [
                { title: "أجزاء النبات", content: "يتكون النبات من الجذر والسايق والورقة. الجذر يمتص الماء من الأرض ليتغذى النبات." }
            ],
            english: [
                { title: "Alphabet & Numbers", content: "Hello Siraj. Apple, Boy, Cat, Dog. One, Two, Three, Four, Five." }
            ],
            islamic: [
                { title: "سورة الفاتحة", content: "بسم الله الرحمن الرحيم. الحمد لله رب العالمين. الرحمن الرحيم. مالك يوم الدين." }
            ]
        };

        let currentActiveKey = '';

        function openSubject(subjectName, key) {
            currentActiveKey = key;
            document.getElementById('current-subject-title').innerText = subjectName;
            document.querySelector('.subjects-section').style.display = 'none';
            document.getElementById('lesson-viewer').style.display = 'block';
            renderLessons(key);
        }

        function closeSubject() {
            document.getElementById('lesson-viewer').style.display = 'none';
            document.querySelector('.subjects-section').style.display = 'block';
        }

        function renderLessons(key) {
            const container = document.getElementById('lessons-list-container');
            container.innerHTML = '';
            const list = lessonsData[key] || [];

            if(list.length === 0) {
                container.innerHTML = '<p class="no-lessons">لا توجد دروس مضافة لهذه المادة بعد. اضغط على (إضافة درس) لإضافة محتوى جديد.</p>';
                return;
            }

            list.forEach((lesson, index) => {
                let lessonCard = document.createElement('div');
                lessonCard.className = 'lesson-card';
                
                // تقسيم النص إلى كلمات قابلة للنقر والنطق الفردي
                let wordsHtml = lesson.content.split(' ').map(word => 
                    `<span class="speakable-word" onclick="speakWord(this, '${key === 'english' ? 'en-US' : 'ar-SA'}')">${word}</span>`
                ).join(' ');

                lessonCard.innerHTML = `
                    <h3><i class="fa-solid fa-bookmark"></i> ${lesson.title}</h3>
                    <div class="lesson-text-box">${wordsHtml}</div>
                `;
                container.appendChild(lessonCard);
            });
        }

        // خاصية نطق كلمة مفردة عند النقر عليها
        function speakWord(element, lang) {
            const wordText = element.innerText;
            if ('speechSynthesis' in window) {
                window.speechSynthesis.cancel(); // إيقاف أي نطق سابق
                let utterance = new SpeechSynthesisUtterance(wordText);
                utterance.lang = lang;
                utterance.rate = 0.9; // سرعة مناسبة للأطفال
                
                // تمييز الكلمة بصرياً أثناء النطق
                element.classList.add('highlight-word');
                utterance.onend = () => {
                    element.classList.remove('highlight-word');
                };
                
                window.speechSynthesis.speak(utterance);
            } else {
                alert('متصفحك لا يدعم خاصية النطق الصوتي.');
            }
        }

        // قراءة الدرس كاملاً
        function speakFullLesson() {
            const container = document.getElementById('lesson-viewer');
            let textElements = container.querySelectorAll('.speakable-word');
            let fullText = Array.from(textElements).map(el => el.innerText).join(' ');

            if ('speechSynthesis' in window) {
                window.speechSynthesis.cancel();
                let utterance = new SpeechSynthesisUtterance(fullText);
                utterance.lang = currentActiveKey === 'english' ? 'en-US' : 'ar-SA';
                utterance.rate = 0.85;
                window.speechSynthesis.speak(utterance);
            }
        }

        // إدارة النوافذ المنبثقة لإضافة الدروس
        function openAddLessonModal() {
            document.getElementById('add-lesson-modal').style.display = 'flex';
        }

        function closeAddLessonModal() {
            document.getElementById('add-lesson-modal').style.display = 'none';
        }

        function saveNewLesson(event) {
            event.preventDefault();
            const subjectKey = document.getElementById('lesson-subject-select').value;
            const title = document.getElementById('lesson-title-input').value;
            const content = document.getElementById('lesson-content-input').value;

            if(!lessonsData[subjectKey]) {
                lessonsData[subjectKey] = [];
            }

            lessonsData[subjectKey].push({ title, content });
            localStorage.setItem('siraj_lessons', JSON.stringify(lessonsData));

            alert('تم حفظ الدرس بنجاح يا أم سراج! 🌟');
            closeAddLessonModal();
            document.getElementById('add-lesson-form').reset();

            // إذا كانت المادة مفتوحة حالياً، قم بتحديث العرض
            if(document.getElementById('lesson-viewer').style.display === 'block' && currentActiveKey === subjectKey) {
                renderLessons(subjectKey);
            }
        }
    </script>
</body>
</html>
