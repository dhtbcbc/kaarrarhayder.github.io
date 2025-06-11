<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>كرار حيدر - موقع شخصي</title>
    <!-- Tailwind CSS for styling -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Cairo for body, Noto Kufi Arabic for headings -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;700&family=Noto+Kufi+Arabic:wght@600;800&display=swap" rel="stylesheet">
    <!-- Font Awesome for icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* --- General Styling --- */
        body {
            font-family: 'Cairo', sans-serif;
            background-color: #121212; /* Dark background for a premium feel */
            color: #E0E0E0;
        }

        /* --- Custom Colors --- */
        .text-gold { color: #D4AF37; }
        .bg-gold { background-color: #D4AF37; }
        .border-gold { border-color: #D4AF37; }
        .ring-gold:focus { --tw-ring-color: #D4AF37; }

        /* --- Typography --- */
        h1, h2 {
            font-family: 'Noto Kufi Arabic', sans-serif;
        }

        /* --- Header Styling --- */
        .header-container {
            position: relative;
            width: 100%;
            max-width: 500px; /* Control max width of the header */
            height: 100px; /* Adjust height as needed */
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 2rem auto;
        }
        .header-svg {
            position: absolute;
            width: 100%;
            height: 100%;
            z-index: 0;
        }
        .header-title {
            position: relative;
            z-index: 1;
            font-size: 3rem; /* 48px */
            font-weight: 800;
            color: #121212; /* Text color inside the banner */
            text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
        }

        /* --- Feature Card Styling --- */
        .feature-card {
            background-color: #1E1E1E;
            border: 1px solid #333;
            border-radius: 1rem; /* 16px */
            padding: 2rem; /* 32px */
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.2), 0 8px 10px -6px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            opacity: 0;
            animation: fadeIn 0.8s ease forwards;
        }
        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 30px -10px rgba(212, 175, 55, 0.15);
        }
        
        /* --- Form Elements Styling --- */
        .gemini-input {
            width: 100%;
            padding: 1rem;
            border-radius: 0.5rem;
            border: 1px solid #444;
            background-color: #2a2a2a;
            color: #E0E0E0;
            font-size: 1.125rem;
            text-align: right;
            transition: border-color 0.3s ease;
        }
        .gemini-input::placeholder { color: #888; }
        .gemini-input:focus {
            outline: none;
            border-color: #D4AF37;
            box-shadow: 0 0 0 2px rgba(212, 175, 55, 0.3);
        }
        .gemini-button {
            background: linear-gradient(145deg, #D4AF37, #B8860B);
            color: #121212;
            font-weight: bold;
            padding: 0.75rem 1.5rem;
            border-radius: 0.5rem;
            box-shadow: 0 4px 6px -1px rgba(0,0,0,0.2);
            transition: all 0.3s ease;
            transform: translateY(0);
            border: none;
            cursor: pointer;
        }
        .gemini-button:hover {
            transform: translateY(-3px) scale(1.05);
            box-shadow: 0 10px 15px -3px rgba(212, 175, 55, 0.2);
        }
        .gemini-button:disabled {
            background: #555;
            cursor: not-allowed;
            transform: none;
            box-shadow: none;
            color: #999;
        }

        /* --- Output Area Styling --- */
        .output-box {
            background-color: #121212;
            border: 1px dashed #444;
            border-radius: 0.75rem;
            padding: 1.5rem;
            min-height: 100px;
            width: 100%;
            font-size: 1.1rem;
            line-height: 1.8;
            white-space: pre-wrap;
            color: #f0f0f0;
        }
        
        /* --- Loading Spinner --- */
        .loader {
            width: 50px;
            height: 50px;
            border: 5px solid #444;
            border-bottom-color: #D4AF37;
            border-radius: 50%;
            display: inline-block;
            box-sizing: border-box;
            animation: rotation 1s linear infinite;
        }
        @keyframes rotation {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        
        /* Fade-in Animation */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        /* Staggered animation delays */
        .feature-card:nth-child(1) { animation-delay: 0.1s; }
        .feature-card:nth-child(2) { animation-delay: 0.2s; }
        .feature-card:nth-child(3) { animation-delay: 0.3s; }
        .feature-card:nth-child(4) { animation-delay: 0.4s; }
        .feature-card:nth-child(5) { animation-delay: 0.5s; }
        .feature-card:nth-child(6) { animation-delay: 0.6s; }


    </style>
</head>
<body class="flex justify-center p-4 sm:p-6">
    <div class="max-w-4xl w-full space-y-12">
        <!-- Header with integrated SVG Banner -->
        <header>
            <div class="header-container">
                <svg class="header-svg" viewBox="0 0 200 40" preserveAspectRatio="none">
                    <path d="M0,0 H190 L200,20 L190,40 H0 Z" fill="#D4AF37"/>
                </svg>
                <h1 class="header-title">كرار حيدر</h1>
            </div>
        </header>

        <main class="space-y-12">

            <!-- AI Image Generator -->
            <section class="feature-card">
                <h2 class="text-3xl font-bold text-gold mb-6 text-center">🖼️ مولّد الصور بالذكاء الاصطناعي</h2>
                <div class="flex flex-col items-center gap-4">
                    <textarea id="imagePromptInput" class="gemini-input" rows="3" placeholder="اكتب وصفًا للصورة التي تتخيلها (مثال: أسد يرتدي نظارات شمسية على سطح المريخ)..."></textarea>
                    <button id="generateImageBtn" class="gemini-button">حوّل الخيال إلى صورة ✨</button>
                    <div id="loadingImageIndicator" class="mt-4 hidden text-center flex-col items-center">
                        <div class="loader"></div>
                        <p class="text-gold mt-2">جاري رسم تحفتك الفنية...</p>
                    </div>
                    <div id="generatedImageContainer" class="mt-6 w-full max-w-lg p-2 bg-black rounded-lg shadow-inner">
                        <img id="generatedImage" src="" alt="الصورة التي تم إنشاؤها" class="w-full h-auto rounded-md hidden"/>
                    </div>
                    <div id="imageError" class="mt-4 text-red-500 hidden"></div>
                </div>
            </section>
            
            <!-- AI Quote Generator -->
            <section class="feature-card">
                <h2 class="text-3xl font-bold text-gold mb-6 text-center">✒️ مولّد الاقتباسات الشخصية</h2>
                <div class="flex flex-col items-center gap-4">
                    <textarea id="quoteTopicInput" class="gemini-input" rows="2" placeholder="اكتب كلمة تعبر عن حالتك أو اهتمامك (مثال: الأمل، القهوة، النجاح)..."></textarea>
                    <button id="generateQuoteBtn" class="gemini-button">ألهمني باقتباس 📜</button>
                    <div id="loadingQuoteIndicator" class="mt-4 hidden text-center flex-col items-center">
                        <div class="loader"></div>
                    </div>
                    <div id="generatedQuote" class="output-box mt-6 text-center"></div>
                    <div id="quoteError" class="mt-4 text-red-500 hidden"></div>
                </div>
            </section>

            <!-- Poem Generator -->
            <section class="feature-card">
                <h2 class="text-3xl font-bold text-gold mb-6 text-center">✍️ شعر بأسلوب جبار رشيد</h2>
                <div class="flex flex-col items-center gap-4">
                    <textarea id="poemTopicInput" class="gemini-input" rows="2" placeholder="اكتب موضوع الشعر الذي تريده..."></textarea>
                    <button id="generatePoemBtn" class="gemini-button">اكتب لي شعرًا</button>
                    <div id="loadingPoemIndicator" class="mt-4 hidden text-center"><div class="loader"></div></div>
                    <div id="generatedPoem" class="output-box mt-6 text-center"></div>
                    <div id="poemError" class="mt-4 text-red-500 hidden"></div>
                </div>
            </section>

            <!-- Dream Interpreter -->
            <section class="feature-card">
                <h2 class="text-3xl font-bold text-gold mb-6 text-center">🌙 مفسر الأحلام</h2>
                <div class="flex flex-col items-center gap-4">
                    <textarea id="dreamInput" class="gemini-input" rows="3" placeholder="اكتب وصفًا لحلمك هنا..."></textarea>
                    <button id="interpretDreamBtn" class="gemini-button">فسّر حلمي</button>
                    <div id="loadingDreamIndicator" class="mt-4 hidden text-center"><div class="loader"></div></div>
                    <div id="interpretedDream" class="output-box mt-6 text-center"></div>
                    <div id="dreamError" class="mt-4 text-red-500 hidden"></div>
                </div>
            </section>
            
            <!-- Wasit Itinerary Generator -->
            <section class="feature-card">
                <h2 class="text-3xl font-bold text-gold mb-6 text-center">🗺️ خطتك لزيارة واسط</h2>
                <div class="flex flex-col items-center gap-4">
                    <textarea id="itineraryInput" class="gemini-input" rows="3" placeholder="أدخل اهتماماتك لنصمم لك جولة! (مثال: التاريخ، الطعام، الطبيعة)..."></textarea>
                    <button id="generateItineraryBtn" class="gemini-button">أنشئ خطتي</button>
                    <div id="loadingItineraryIndicator" class="mt-4 hidden text-center"><div class="loader"></div></div>
                    <div id="itineraryResult" class="output-box mt-6 text-center"></div>
                    <div id="itineraryError" class="mt-4 text-red-500 hidden"></div>
                </div>
            </section>

            <!-- Collaboration Idea Generator -->
            <section class="feature-card">
                 <h2 class="text-3xl font-bold text-gold mb-6 text-center">💡 اقترح فكرة تعاون</h2>
                <div class="flex flex-col items-center gap-4">
                    <textarea id="skillsInput" class="gemini-input" rows="3" placeholder="أدخل مهاراتك أو اهتماماتك هنا..."></textarea>
                    <button id="generateIdeaBtn" class="gemini-button">اقترح فكرة!</button>
                    <div id="loadingIdeaIndicator" class="mt-4 hidden text-center"><div class="loader"></div></div>
                    <div id="collaborationIdea" class="output-box mt-6 text-center"></div>
                    <div id="ideaError" class="mt-4 text-red-500 hidden"></div>
                </div>
            </section>
        </main>

        <!-- Contact and Footer -->
        <footer class="text-center pt-8 space-y-6">
            <div class="feature-card">
                <h2 class="text-2xl font-bold text-gold mb-4">تواصل معي</h2>
                <div class="flex flex-wrap justify-center gap-x-8 gap-y-4 text-lg">
                    <a href="https://www.instagram.com/k9x9i" target="_blank" class="flex items-center gap-3 text-gray-300 hover:text-gold transition-colors">
                        <i class="fab fa-instagram text-2xl"></i>
                        <span>k9x9i</span>
                    </a>
                    <a href="https://t.me/K1_ar1" target="_blank" class="flex items-center gap-3 text-gray-300 hover:text-gold transition-colors">
                        <i class="fab fa-telegram-plane text-2xl"></i>
                        <span>@K1_ar1</span>
                    </a>
                </div>
            </div>
            <p class="text-sm text-gray-500 pt-4">جميع الحقوق محفوظة كرار حيدر 2024 ©️</p>
        </footer>
    </div>

    <script>
        // --- API Call Helper Functions ---
        
        /**
         * Generic handler for text generation with Gemini
         */
        async function callGeminiText(prompt, resultElement, loadingIndicator, errorElement, buttonElement) {
            if (!prompt) {
                errorElement.textContent = "الرجاء إدخال البيانات المطلوبة.";
                errorElement.classList.remove('hidden');
                resultElement.textContent = '';
                return;
            }
            errorElement.classList.add('hidden');
            loadingIndicator.classList.remove('hidden');
            resultElement.textContent = '';
            if (buttonElement) buttonElement.disabled = true;

            try {
                const payload = { contents: [{ role: "user", parts: [{ text: prompt }] }] };
                const apiKey = ""; 
                const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-flash:generateContent?key=${apiKey}`;
                const response = await fetch(apiUrl, {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify(payload)
                });

                if (!response.ok) throw new Error(`HTTP error! status: ${response.status}`);
                const result = await response.json();

                if (result.candidates && result.candidates[0]?.content?.parts?.[0]?.text) {
                    resultElement.textContent = result.candidates[0].content.parts[0].text;
                } else {
                    throw new Error("API response format is incorrect.");
                }
            } catch (error) {
                resultElement.textContent = "عذراً، حدث خطأ. يرجى المحاولة مرة أخرى.";
                console.error("Error calling Gemini API:", error);
            } finally {
                loadingIndicator.classList.add('hidden');
                if (buttonElement) buttonElement.disabled = false;
            }
        }

        /**
         * Handler for image generation with Imagen
         */
        async function callImagen(prompt, imageElement, loadingIndicator, errorElement, buttonElement) {
            if (!prompt) {
                errorElement.textContent = "الرجاء إدخال وصف للصورة.";
                errorElement.classList.remove('hidden');
                imageElement.classList.add('hidden');
                return;
            }
            errorElement.classList.add('hidden');
            loadingIndicator.classList.remove('hidden');
            imageElement.classList.add('hidden'); // Hide previous image
            if (buttonElement) buttonElement.disabled = true;

            try {
                const payload = { instances: [{ prompt: prompt }], parameters: { "sampleCount": 1 } };
                const apiKey = "";
                const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/imagen-3.0-generate-002:predict?key=${apiKey}`;
                const response = await fetch(apiUrl, {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify(payload)
                });
                
                if (!response.ok) throw new Error(`HTTP error! status: ${response.status}`);
                const result = await response.json();
                
                if (result.predictions && result.predictions[0]?.bytesBase64Encoded) {
                    imageElement.src = `data:image/png;base64,${result.predictions[0].bytesBase64Encoded}`;
                    imageElement.classList.remove('hidden');
                } else {
                    throw new Error("Image API response format is incorrect.");
                }
            } catch (error) {
                errorElement.textContent = "عذراً، لم نتمكن من إنشاء الصورة. حاول وصفًا مختلفًا.";
                errorElement.classList.remove('hidden');
                console.error("Error calling Imagen API:", error);
            } finally {
                loadingIndicator.classList.add('hidden');
                if (buttonElement) buttonElement.disabled = false;
            }
        }

        // --- Event Listeners ---

        // Image Generator
        document.getElementById('generateImageBtn').addEventListener('click', () => {
            const prompt = document.getElementById('imagePromptInput').value.trim();
            const creativePrompt = `digital art, cinematic lighting, ultra-detailed, 8k. prompt: ${prompt}`;
            callImagen(
                prompt ? creativePrompt : null,
                document.getElementById('generatedImage'),
                document.getElementById('loadingImageIndicator'),
                document.getElementById('imageError'),
                document.getElementById('generateImageBtn')
            );
        });

        // Quote Generator
        document.getElementById('generateQuoteBtn').addEventListener('click', () => {
            const topic = document.getElementById('quoteTopicInput').value.trim();
            const prompt = `اكتب اقتباسًا قصيرًا وعميقًا وملهمًا باللغة العربية حول موضوع "${topic}". يجب أن يكون الاقتباس أصيلًا ومبتكرًا.`;
            callGeminiText(
                topic ? prompt : null,
                document.getElementById('generatedQuote'),
                document.getElementById('loadingQuoteIndicator'),
                document.getElementById('quoteError'),
                document.getElementById('generateQuoteBtn')
            );
        });

        // Poem Generator
        document.getElementById('generatePoemBtn').addEventListener('click', () => {
            const topic = document.getElementById('poemTopicInput').value.trim();
            const prompt = `اكتب قصيدة رومانسية أو تأملية موجزة بأسلوب الشاعر العراقي جبار رشيد عن موضوع: ${topic}. استخدم مفردات وأساليب قريبة من أسلوبه المعروف في الشعر الحر والعاطفي. لا تتجاوز القصيدة 6 أسطر.`;
            callGeminiText(topic ? prompt : null, document.getElementById('generatedPoem'), document.getElementById('loadingPoemIndicator'), document.getElementById('poemError'), document.getElementById('generatePoemBtn'));
        });

        // Dream Interpreter
        document.getElementById('interpretDreamBtn').addEventListener('click', () => {
            const dream = document.getElementById('dreamInput').value.trim();
            const prompt = `بصفتك مفسر أحلام حكيم وشاعري، قم بتفسير الحلم التالي بطريقة إبداعية ومجازية، وليس بطريقة علمية. الحلم هو: "${dream}". اجعل التفسير قصيرًا وملهمًا وموجزًا.`;
            callGeminiText(dream ? prompt : null, document.getElementById('interpretedDream'), document.getElementById('loadingDreamIndicator'), document.getElementById('dreamError'), document.getElementById('interpretDreamBtn'));
        });
        
        // Wasit Itinerary
        document.getElementById('generateItineraryBtn').addEventListener('click', () => {
            const interests = document.getElementById('itineraryInput').value.trim();
            const prompt = `بصفتك مرشدًا محليًا ودودًا وخبيرًا في محافظة واسط، العراق، أنشئ خطة سياحية شخصية ومبتكرة ليوم واحد لزائر بناءً على الاهتمامات التالية: "${interests}". اقترح أماكن حقيقية أو معقولة، وأنشطة محلية، وأطعمة تقليدية. اجعل الخطة تبدو كدعوة شخصية ومرحبة.`;
            callGeminiText(interests ? prompt : null, document.getElementById('itineraryResult'), document.getElementById('loadingItineraryIndicator'), document.getElementById('itineraryError'), document.getElementById('generateItineraryBtn'));
        });

        // Collaboration Idea
        document.getElementById('generateIdeaBtn').addEventListener('click', () => {
            const skills = document.getElementById('skillsInput').value.trim();
            const prompt = `بصفتك مستشارًا إبداعيًا، اقترح فكرة مشروع مبتكرة للتعاون بين شخص يمتلك المهارات التالية: "${skills}"، وبين كرار حيدر. اجعل الفكرة موجزة ومثيرة للاهتمام وقابلة للتنفيذ.`;
            callGeminiText(skills ? prompt : null, document.getElementById('collaborationIdea'), document.getElementById('loadingIdeaIndicator'), document.getElementById('ideaError'), document.getElementById('generateIdeaBtn'));
        });
    </script>
</body>
</html>
