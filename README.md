   <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>كرار حيدر فليح - شغف وإبداع</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts - Poppins & Lato for general text, Noto Sans Arabic for Arabic support -->
    <link href="https://fonts.googleapis.com/css2?family=Lato:wght@400;700&family=Noto+Sans+Arabic:wght@400;700&family=Poppins:wght@400;700&display=swap" rel="stylesheet">
    <!-- Font Awesome for icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* Custom styles for the chosen fonts and general body styling */
        body {
            font-family: 'Noto Sans Arabic', 'Poppins', 'Lato', sans-serif;
            background-color: #F8F8F8; /* Creamy light background */
            color: #333333; /* Darker text for readability */
            line-height: 1.7;
        }
        h1, h2, h3 {
            font-family: 'Poppins', 'Noto Sans Arabic', sans-serif;
            color: #1A202C; /* Elegant black for headings */
        }
        .text-gold-soft {
            color: #B8860B; /* A soft gold color */
        }
        .bg-cream-light {
            background-color: #F8F8F8;
        }
        .border-gold-subtle {
            border-color: #B8860B;
        }
        .ornament-divider {
            position: relative;
            height: 1px;
            background: linear-gradient(to right, transparent, #B8860B, transparent);
            margin: 3rem auto;
            max-width: 600px; /* Limit width of divider */
        }
        .ornament-divider::before,
        .ornament-divider::after {
            content: '';
            position: absolute;
            top: 50%;
            width: 8px;
            height: 8px;
            background-color: #B8860B;
            border-radius: 50%;
            transform: translateY(-50%);
        }
        .ornament-divider::before {
            left: 0;
        }
        .ornament-divider::after {
            right: 0;
        }
        /* Custom styles for loading spinner */
        .loader {
            border: 4px solid #f3f3f3;
            border-top: 4px solid #B8860B;
            border-radius: 50%;
            width: 40px;
            height: 40px;
            animation: spin 1s linear infinite;
            display: none; /* Hidden by default */
            margin: 20px auto;
        }
        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
    </style>
</head>
<body class="bg-cream-light font-sans text-gray-800 antialiased">
    <!-- Header Section -->
    <header class="bg-gray-900 text-white py-8 shadow-lg">
        <div class="container mx-auto px-4 text-center">
            <h1 class="text-4xl md:text-5xl font-bold mb-2 text-gold-soft">كرار حيدر فليح</h1>
            <p class="text-xl md:text-2xl font-light text-gray-300">طالب شغوف بالإبداع من العراق</p>
        </div>
    </header>

    <!-- Main Content Container -->
    <main class="container mx-auto px-4 py-12 max-w-4xl">

        <!-- About Me Section -->
        <section id="about" class="mb-16">
            <h2 class="text-3xl md:text-4xl font-semibold mb-6 text-gray-900 text-center">
                نبذة عني
            </h2>
            <p class="text-lg leading-relaxed text-center max-w-2xl mx-auto">
                اسمي كرار حيدر فليح، طالب سادس إعدادي علمي من العراق، أؤمن بأن الإبداع هو روح الحياة.
                أمتلك شغفًا عميقًا بالفن والتصميم، حيث أرى في كل فكرة فرصة لتحويلها إلى
                تصميم جذاب وذو معنى. أهتم بأدق التفاصيل الجمالية، وأبحث دائمًا عن
                التوازن المثالي بين البساطة الأنيقة والاحترافية المرنة.
                أنا مؤمن بالتفكير النقدي ومفتوح دائمًا على وجهات النظر المختلفة،
                مما يدفعني للتعلم والتطور المستمر.
            </p>
        </section>

        <!-- Artistic Divider -->
        <div class="ornament-divider mb-16"></div>

        <!-- Hobbies Section -->
        <section id="hobbies" class="mb-16">
            <h2 class="text-3xl md:text-4xl font-semibold mb-8 text-gray-900 text-center">
                هواياتي
            </h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Design Card -->
                <div class="bg-white rounded-lg shadow-md p-6 border-l-4 border-gold-subtle transform hover:scale-105 transition-transform duration-300">
                    <h3 class="text-xl font-bold mb-3 text-gray-900 text-center">التصميم الجرافيكي</h3>
                    <p class="text-gray-700 text-center">
                        أعشق تحويل الأفكار المجردة إلى تصاميم بصرية تحكي قصصًا.
                        التفاصيل الجمالية والتوازن في الألوان والأشكال هي ما يميز عملي.
                    </p>
                </div>
                <!-- Photography Card -->
                <div class="bg-white rounded-lg shadow-md p-6 border-l-4 border-gold-subtle transform hover:scale-105 transition-transform duration-300">
                    <h3 class="text-xl font-bold mb-3 text-gray-900 text-center">التصوير الفوتوغرافي</h3>
                    <p class="text-gray-700 text-center">
                        لدي عين فنية تلتقط الجمال من الزوايا الفريدة.
                        أبحث دائمًا عن وضعيات وإضاءات تبرز الصورة بطريقة فنية ومبتكرة.
                    </p>
                </div>
                <!-- Poetry Card -->
                <div class="bg-white rounded-lg shadow-md p-6 border-l-4 border-gold-subtle transform hover:scale-105 transition-transform duration-300">
                    <h3 class="text-xl font-bold mb-3 text-gray-900 text-center">الشعر والتأمل</h3>
                    <p class="text-gray-700 text-center">
                        أجد راحتي في الكلمات، وأميل للشعر الرومانسي والتأملي،
                        متأثراً بعمالقة مثل جبار رشيد وعبدالعزيز جويدة.
                    </p>
                </div>
                <!-- Religious Recitation Card -->
                <div class="bg-white rounded-lg shadow-md p-6 border-l-4 border-gold-subtle transform hover:scale-105 transition-transform duration-300">
                    <h3 class="text-xl font-bold mb-3 text-gray-900 text-center">الرادود الحسيني</h3>
                    <p class="text-gray-700 text-center">
                        فخور بانتمائي الديني كمسلم شيعي، وأخدم أهل البيت (عليهم السلام)
                        كرادود ألقي القصائد في المناسبات الدينية لإيصال رسالة الإسلام الأصيل.
                    </p>
                </div>
                <!-- Science Card -->
                <div class="bg-white rounded-lg shadow-md p-6 border-l-4 border-gold-subtle transform hover:scale-105 transition-transform duration-300">
                    <h3 class="text-xl font-bold mb-3 text-gray-900 text-center">الشغف العلمي</h3>
                    <p class="text-gray-700 text-center">
                        أرى في العلم سبيلاً للإبداع والابتكار.
                        تستهويني الأفكار الجريئة التي تغير العالم، مثل اكتشافات آينشتاين وتسلا.
                    </p>
                </div>
            </div>
        </section>

        <!-- Artistic Divider -->
        <div class="ornament-divider mb-16"></div>

        <!-- Poetry Generator Section -->
        <section id="poetry-generator" class="mb-16 bg-white rounded-lg shadow-md p-8">
            <h2 class="text-3xl md:text-4xl font-semibold mb-6 text-gray-900 text-center">
                إبداع شعري ✨
            </h2>
            <p class="text-lg leading-relaxed text-center max-w-2xl mx-auto mb-6">
                أدخل كلمة مفتاحية أو موضوعاً، ودع الذكاء الاصطناعي ينسج لك قصيدة
                رومانسية أو تأملية بأسلوب مستوحى من جبار رشيد وعبدالعزيز جويدة.
            </p>
            <div class="flex flex-col items-center gap-4">
                <textarea id="poetryInput" class="w-full md:w-3/4 p-4 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-gold-soft text-lg"
                    rows="4" placeholder="اكتب كلمة مفتاحية أو موضوعًا للشعر (مثال: الحب، الطبيعة، الأمل، الحنين)..."></textarea>
                <button id="generatePoetryBtn" class="bg-gold-soft text-white px-8 py-3 rounded-full text-lg font-bold hover:bg-yellow-700 transition-colors duration-300 shadow-lg flex items-center justify-center">
                    توليد قصيدة ✨
                </button>
                <div id="loadingSpinnerPoetry" class="loader"></div>
                <div id="poetryOutput" class="w-full md:w-3/4 bg-gray-50 p-6 rounded-lg border border-gray-200 mt-6 text-lg text-gray-800 leading-relaxed whitespace-pre-wrap text-center" style="min-height: 100px;">
                    <!-- Generated poetry will appear here -->
                </div>
                 <div id="errorMessagePoetry" class="text-red-600 text-center mt-4 hidden">
                    عذراً، حدث خطأ أثناء توليد القصيدة. الرجاء المحاولة مرة أخرى.
                </div>
            </div>
        </section>

        <!-- Artistic Divider -->
        <div class="ornament-divider mb-16"></div>

        <!-- Scientific Inspiration Section -->
        <section id="scientific-inspiration" class="mb-16 bg-white rounded-lg shadow-md p-8">
            <h2 class="text-3xl md:text-4xl font-semibold mb-6 text-gray-900 text-center">
                إلهام علمي ✨
            </h2>
            <p class="text-lg leading-relaxed text-center max-w-2xl mx-auto mb-6">
                هل لديك سؤال علمي أو فكرة تحتاج إلى استكشاف؟ أدخل موضوعاً يتعلق بالطاقة، الفيزياء، أو الابتكار، ودع الذكاء الاصطناعي يقدم لك أفكاراً ملهمة وتحديات محتملة.
            </p>
            <div class="flex flex-col items-center gap-4">
                <textarea id="scientificInput" class="w-full md:w-3/4 p-4 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-gold-soft text-lg"
                    rows="4" placeholder="اكتب سؤالك أو موضوعك العلمي (مثال: مستقبل الطاقة المتجددة، فيزياء الكم، الذكاء الاصطناعي في الفضاء)..."></textarea>
                <button id="getScientificInspirationBtn" class="bg-gold-soft text-white px-8 py-3 rounded-full text-lg font-bold hover:bg-yellow-700 transition-colors duration-300 shadow-lg flex items-center justify-center">
                    احصل على الإلهام ✨
                </button>
                <div id="loadingSpinnerScientific" class="loader"></div>
                <div id="scientificOutput" class="w-full md:w-3/4 bg-gray-50 p-6 rounded-lg border border-gray-200 mt-6 text-lg text-gray-800 leading-relaxed whitespace-pre-wrap text-center" style="min-height: 100px;">
                    <!-- Scientific inspiration will appear here -->
                </div>
                <div id="errorMessageScientific" class="text-red-600 text-center mt-4 hidden">
                    عذراً، حدث خطأ أثناء توليد الإلهام العلمي. الرجاء المحاولة مرة أخرى.
                </div>
            </div>
        </section>

        <!-- Artistic Divider -->
        <div class="ornament-divider mb-16"></div>

        <!-- Works/Design Gallery Section (Placeholder) -->
        <section id="works" class="mb-16">
            <h2 class="text-3xl md:text-4xl font-semibold mb-8 text-gray-900 text-center">
                أعمالي ومعرض التصاميم
            </h2>
            <div class="text-center">
                <p class="text-lg text-gray-700 text-center mb-4">
                    هنا سيتم عرض أحدث تصاميمي وأعمالي الفنية.
                    تابعني على وسائل التواصل الاجتماعي لتبقى على اطلاع دائم!
                </p>
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                    <!-- Placeholder for design images -->
                    <div class="bg-gray-200 rounded-lg overflow-hidden shadow-sm p-4 h-48 flex items-center justify-center text-gray-500">
                        <i class="fas fa-palette text-5xl"></i>
                    </div>
                    <div class="bg-gray-200 rounded-lg overflow-hidden shadow-sm p-4 h-48 flex items-center justify-center text-gray-500">
                        <i class="fas fa-camera-retro text-5xl"></i>
                    </div>
                    <div class="bg-gray-200 rounded-lg overflow-hidden shadow-sm p-4 h-48 flex items-center justify-center text-gray-500">
                        <i class="fas fa-pencil-ruler text-5xl"></i>
                    </div>
                </div>
            </div>
        </section>

        <!-- Artistic Divider -->
        <div class="ornament-divider mb-16"></div>

        <!-- Scientific Project Section (Existing, renamed from previous request to avoid confusion with new LLM feature) -->
        <section id="karrar-scientific-project" class="mb-16">
            <h2 class="text-3xl md:text-4xl font-semibold mb-6 text-gray-900 text-center">
                مشروعي العلمي الخاص بكرار
            </h2>
            <p class="text-lg leading-relaxed text-center max-w-2xl mx-auto">
                كطالب علمي، لدي طموح كبير في البحث والابتكار. أخوض حاليًا مشروعًا
                علميًا لاستكشاف طريقة جديدة لتوليد الطاقة من الفراغ، مستلهمًا
                من نظريات وعبقرية آينشتاين وتسلا. أؤمن بأن هذا المشروع يمكن أن
                يفتح آفاقًا جديدة في فهمنا للفيزياء والطاقة.
            </p>
        </section>

        <!-- Artistic Divider -->
        <div class="ornament-divider mb-16"></div>

        <!-- Contact Section -->
        <section id="contact" class="mb-16">
            <h2 class="text-3xl md:text-4xl font-semibold mb-8 text-gray-900 text-center">
                تواصل معي
            </h2>
            <div class="flex flex-col items-center space-y-4">
                <a href="tel:+9647816182503" class="flex items-center text-lg text-gray-700 hover:text-gold-soft transition-colors duration-300">
                    <i class="fas fa-phone-alt ml-3 text-gold-soft text-xl"></i>
                    <span>+964 781 618 2503</span>
                </a>
                <a href="https://instagram.com/k9x9i" target="_blank" rel="noopener noreferrer" class="flex items-center text-lg text-gray-700 hover:text-gold-soft transition-colors duration-300">
                    <i class="fab fa-instagram ml-3 text-gold-soft text-xl"></i>
                    <span>k9x9i</span>
                </a>
                <a href="https://t.me/K1_ar1" target="_blank" rel="noopener noreferrer" class="flex items-center text-lg text-gray-700 hover:text-gold-soft transition-colors duration-300">
                    <i class="fab fa-telegram-plane ml-3 text-gold-soft text-xl"></i>
                    <span>@K1_ar1</span>
                </a>
            </div>
        </section>
    </main>

    <!-- Footer Section -->
    <footer class="bg-gray-900 text-white py-8 mt-12">
        <div class="container mx-auto px-4 text-center">
            <p class="text-lg font-light text-gray-300">
                “أبحث عن الجمال في كل تفصيلة، وأؤمن أن كل فكرة عظيمة تبدأ من الشغف.”
            </p>
            <p class="text-sm text-gray-500 mt-4">&copy; 2024 كرار حيدر فليح. جميع الحقوق محفوظة.</p>
        </div>
    </footer>

    <script>
        // --- Poetry Generator Elements & Logic ---
        const poetryInput = document.getElementById('poetryInput');
        const generatePoetryBtn = document.getElementById('generatePoetryBtn');
        const poetryOutput = document.getElementById('poetryOutput');
        const loadingSpinnerPoetry = document.getElementById('loadingSpinnerPoetry');
        const errorMessagePoetry = document.getElementById('errorMessagePoetry');

        generatePoetryBtn.addEventListener('click', async () => {
            const userPrompt = poetryInput.value.trim();
            if (!userPrompt) {
                poetryOutput.textContent = 'الرجاء إدخال كلمة مفتاحية أو موضوع لتوليد القصيدة.';
                poetryOutput.classList.remove('text-gray-800');
                poetryOutput.classList.add('text-red-600');
                errorMessagePoetry.classList.add('hidden');
                return;
            }

            poetryOutput.textContent = '';
            poetryOutput.classList.remove('text-red-600');
            poetryOutput.classList.add('text-gray-800');
            loadingSpinnerPoetry.style.display = 'block';
            generatePoetryBtn.disabled = true;
            errorMessagePoetry.classList.add('hidden');

            try {
                let chatHistory = [];
                const promptText = `Generate a romantic or meditative poem in the style of Iraqi poets Jabar Rashid and Abdulaziz Jwaida, based on the following theme/keyword: "${userPrompt}". The poem should be in Arabic, evocative, and reflect deep emotions or contemplation.`;
                chatHistory.push({ role: "user", parts: [{ text: promptText }] });

                const payload = { contents: chatHistory };
                const apiKey = "";
                const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-flash:generateContent?key=${apiKey}`;

                const response = await fetch(apiUrl, {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify(payload)
                });

                if (!response.ok) {
                    throw new Error(`HTTP error! status: ${response.status}`);
                }

                const result = await response.json();

                if (result.candidates && result.candidates.length > 0 &&
                    result.candidates[0].content && result.candidates[0].content.parts &&
                    result.candidates[0].content.parts.length > 0) {
                    const generatedText = result.candidates[0].content.parts[0].text;
                    poetryOutput.textContent = generatedText;
                } else {
                    poetryOutput.textContent = 'عذراً، لم يتمكن الذكاء الاصطناعي من توليد قصيدة. الرجاء المحاولة بكلمة مفتاحية مختلفة.';
                    poetryOutput.classList.remove('text-gray-800');
                    poetryOutput.classList.add('text-red-600');
                }
            } catch (error) {
                console.error('Error generating poetry:', error);
                errorMessagePoetry.classList.remove('hidden');
                poetryOutput.textContent = '';
            } finally {
                loadingSpinnerPoetry.style.display = 'none';
                generatePoetryBtn.disabled = false;
            }
        });

        // --- Scientific Inspiration Elements & Logic ---
        const scientificInput = document.getElementById('scientificInput');
        const getScientificInspirationBtn = document.getElementById('getScientificInspirationBtn');
        const scientificOutput = document.getElementById('scientificOutput');
        const loadingSpinnerScientific = document.getElementById('loadingSpinnerScientific');
        const errorMessageScientific = document.getElementById('errorMessageScientific');

        getScientificInspirationBtn.addEventListener('click', async () => {
            const userPrompt = scientificInput.value.trim();
            if (!userPrompt) {
                scientificOutput.textContent = 'الرجاء إدخال سؤالك أو موضوعك العلمي للحصول على الإلهام.';
                scientificOutput.classList.remove('text-gray-800');
                scientificOutput.classList.add('text-red-600');
                errorMessageScientific.classList.add('hidden');
                return;
            }

            scientificOutput.textContent = '';
            scientificOutput.classList.remove('text-red-600');
            scientificOutput.classList.add('text-gray-800');
            loadingSpinnerScientific.style.display = 'block';
            getScientificInspirationBtn.disabled = true;
            errorMessageScientific.classList.add('hidden');

            try {
                let chatHistory = [];
                const promptText = `Provide scientific inspiration, brainstorming ideas, potential challenges, or related concepts for the following topic: "${userPrompt}". Focus on areas like energy generation, physics, innovation, or technology. The response should be in Arabic, insightful, and encourage further critical thinking.`;
                chatHistory.push({ role: "user", parts: [{ text: promptText }] });

                const payload = { contents: chatHistory };
                const apiKey = "";
                const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-flash:generateContent?key=${apiKey}`;

                const response = await fetch(apiUrl, {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify(payload)
                });

                if (!response.ok) {
                    throw new Error(`HTTP error! status: ${response.status}`);
                }

                const result = await response.json();

                if (result.candidates && result.candidates.length > 0 &&
                    result.candidates[0].content && result.candidates[0].content.parts &&
                    result.candidates[0].content.parts.length > 0) {
                    const generatedText = result.candidates[0].content.parts[0].text;
                    scientificOutput.textContent = generatedText;
                } else {
                    scientificOutput.textContent = 'عذراً، لم يتمكن الذكاء الاصطناعي من توليد إلهام علمي. الرجاء المحاولة بموضوع مختلف.';
                    scientificOutput.classList.remove('text-gray-800');
                    scientificOutput.classList.add('text-red-600');
                }
            } catch (error) {
                console.error('Error generating scientific inspiration:', error);
                errorMessageScientific.classList.remove('hidden');
                scientificOutput.textContent = '';
            } finally {
                loadingSpinnerScientific.style.display = 'none';
                getScientificInspirationBtn.disabled = false;
            }
        });
    </script>
</body>
</html>
