<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>مركز أثر الخالدين للأبحاث العلمية</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700&display=swap">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        body {
            font-family: 'Cairo', sans-serif;
            background-color: #f5f5f0;
        }
        
        .banner {
            background: linear-gradient(rgba(210, 180, 140, 0.7), rgba(210, 180, 140, 0.7)), url('https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80');
            background-size: cover;
            background-position: center;
            height: 60vh;
        }
        
        .team-card {
            transition: all 0.3s ease;
            background-color: #f8f4e9;
        }
        
        .team-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }
        
        .fade-in {
            animation: fadeIn 2s;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        .edit-mode {
            outline: 2px dashed #d2b48c;
        }
        
        .video-container {
            position: relative;
            padding-bottom: 56.25%;
            height: 0;
            overflow: hidden;
        }
        
        .video-container iframe {
            position: absolute;
            top: 0;
            right: 0;
            width: 100%;
            height: 100%;
        }
        
        .gold-text {
            color: #d4af37;
        }
        
        .beige-bg {
            background-color: #f5f5dc;
        }
        
        .light-brown-bg {
            background-color: #d2b48c;
        }
        
        .gold-bg {
            background-color: #d4af37;
        }
        
        .chat-container {
            scrollbar-width: thin;
            scrollbar-color: #d2b48c transparent;
        }
        
        .chat-container::-webkit-scrollbar {
            width: 6px;
        }
        
        .chat-container::-webkit-scrollbar-thumb {
            background-color: #d2b48c;
            border-radius: 3px;
        }
    </style>
</head>
<body class="text-gray-800">
    <!-- Navigation -->
    <nav class="bg-white shadow-lg fixed w-full z-10 top-0">
        <div class="max-w-7xl mx-auto px-4">
            <div class="flex justify-between items-center h-16">
                <div class="flex items-center">
                    <img src="https://via.placeholder.com/50x50/d2b48c/ffffff?text=شعار" alt="شعار المركز" class="h-10 w-10 rounded-full">
                    <span class="text-xl font-bold mr-2 gold-text">مركز أثر الخالدين للأبحاث العلمية</span>
                </div>
                
                <div class="hidden md:flex space-x-4 space-x-reverse">
                    <a href="#about" class="px-3 py-2 hover:text-amber-700">عن المركز</a>
                    <a href="#teams" class="px-3 py-2 hover:text-amber-700">فريقنا</a>
                    <a href="#ai" class="px-3 py-2 hover:text-amber-700">ذكاء المتفوقين</a>
                    <a href="#videos" class="px-3 py-2 hover:text-amber-700">احنا نشرحلك</a>
                    <a href="#contact" class="px-3 py-2 hover:text-amber-700">تواصل معنا</a>
                </div>
                
                <button id="editBtn" class="px-4 py-2 bg-amber-700 text-white rounded hover:bg-amber-800">
                    نمط التحرير <i class="fas fa-edit ml-1"></i>
                </button>
                
                <div class="md:hidden">
                    <button id="mobile-menu-button" class="p-2">
                        <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                        </svg>
                    </button>
                </div>
            </div>
        </div>
        
        <!-- Mobile menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a href="#about" class="block px-3 py-2 hover:bg-amber-50">عن المركز</a>
                <a href="#teams" class="block px-3 py-2 hover:bg-amber-50">فريقنا</a>
                <a href="#ai" class="block px-3 py-2 hover:bg-amber-50">ذكاء المتفوقين</a>
                <a href="#videos" class="block px-3 py-2 hover:bg-amber-50">احنا نشرحلك</a>
                <a href="#contact" class="block px-3 py-2 hover:bg-amber-50">تواصل معنا</a>
            </div>
        </div>
    </nav>

    <!-- Banner -->
    <div class="banner flex items-center justify-center mt-16">
        <div class="text-center px-4">
            <h1 class="text-4xl md:text-5xl font-bold text-white mb-4">مركز أثر الخالدين للأبحاث العلمية</h1>
            <p class="text-xl text-white mb-6">نحو مستقبل مشرق بالمعرفة والابتكار</p>
            <a href="#about" class="px-6 py-3 bg-amber-700 text-white rounded-lg hover:bg-amber-800 transition duration-300">
                اقرأ المزيد عنا
            </a>
        </div>
    </div>

    <!-- About Section -->
    <section id="about" class="py-16 px-4 beige-bg">
        <div class="max-w-7xl mx-auto">
            <h2 class="text-3xl font-bold text-center mb-12 gold-text">عن المركز</h2>
            <div class="grid md:grid-cols-2 gap-8 items-center">
                <div>
                    <p class="text-lg mb-4" id="aboutText1">مركز أثر الخالدين للأبحاث العلمية هو مؤسسة بحثية رائدة تهدف إلى تطوير المعرفة العلمية وترسيخ قيم الابتكار والتميز في مختلف المجالات البحثية.</p>
                    <p class="text-lg mb-4" id="aboutText2">نحن نؤمن بأن البحث العلمي هو الركيزة الأساسية لتقدم الأمم وازدهارها، ولذلك نعمل على توفير بيئة محفزة للإبداع والاكتشاف.</p>
                    <p class="text-lg" id="aboutText3">يضم المركز نخبة من الباحثين والعلماء في مختلف التخصصات، ويعمل على بناء شراكات محلية ودولية لتعزيز التبادل المعرفي.</p>
                </div>
                <div class="rounded-lg overflow-hidden shadow-xl">
                    <img src="https://images.unsplash.com/photo-1523961131990-5ea7c61b2107?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1374&q=80" alt="عن المركز" class="w-full h-auto">
                </div>
            </div>
        </div>
    </section>

    <!-- Teams Section -->
    <section id="teams" class="py-16 px-4 bg-white">
        <div class="max-w-7xl mx-auto">
            <h2 class="text-3xl font-bold text-center mb-12 gold-text">فريقنا</h2>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Research Team -->
                <div class="team-card rounded-lg p-6 shadow-md cursor-pointer" onclick="showTeam('research')">
                    <div class="flex items-center mb-4">
                        <div class="p-3 rounded-full bg-amber-100 text-amber-700 mr-3">
                            <i class="fas fa-flask text-xl"></i>
                        </div>
                        <h3 class="text-xl font-bold">فريق البحث العلمي</h3>
                    </div>
                    <p class="text-gray-600">فريق متخصص في إجراء الأبحاث العلمية المتقدمة ونشر المعرفة.</p>
                    <div id="researchTeam" class="hidden mt-4 fade-in">
                        <h4 class="font-semibold mb-2">أعضاء الفريق:</h4>
                        <ul class="list-disc mr-4 space-y-1">
                            <li>براق علاء</li>
                            <li>حسن أنور</li>
                            <li>أمير معن</li>
                            <li>أحمد سمير</li>
                            <li>مؤمل وليد</li>
                        </ul>
                        <h4 class="font-semibold mt-3 mb-2">الأبحاث المنشورة:</h4>
                        <ul class="list-disc mr-4 space-y-1">
                            <li>تأثير التكنولوجيا الحديثة على التعليم</li>
                            <li>الذكاء الاصطناعي في التشخيص الطبي</li>
                            <li>استدامة الطاقة في المناطق الحضرية</li>
                        </ul>
                        <p class="mt-2 text-sm text-gray-500">المشرف الثانوي: رامي جعفر</p>
                    </div>
                </div>
                
                <!-- International Research Team -->
                <div class="team-card rounded-lg p-6 shadow-md cursor-pointer" onclick="showTeam('international')">
                    <div class="flex items-center mb-4">
                        <div class="p-3 rounded-full bg-amber-100 text-amber-700 mr-3">
                            <i class="fas fa-globe text-xl"></i>
                        </div>
                        <h3 class="text-xl font-bold">فريق البحث الدولي</h3>
                    </div>
                    <p class="text-gray-600">فريق يعمل على بناء الشراكات الدولية وإجراء الأبحاث المشتركة.</p>
                    <div id="internationalTeam" class="hidden mt-4 fade-in">
                        <h4 class="font-semibold mb-2">أعضاء الفريق:</h4>
                        <ul class="list-disc mr-4 space-y-1">
                            <li>رامي جعفر (مشرف رئيسي)</li>
                            <li>براق علاء</li>
                            <li>عبد الله محمد ياسين</li>
                        </ul>
                    </div>
                </div>
                
                <!-- Media & Tech Team -->
                <div class="team-card rounded-lg p-6 shadow-md cursor-pointer" onclick="showTeam('media')">
                    <div class="flex items-center mb-4">
                        <div class="p-3 rounded-full bg-amber-100 text-amber-700 mr-3">
                            <i class="fas fa-laptop-code text-xl"></i>
                        </div>
                        <h3 class="text-xl font-bold">فريق الإعلام والتكنولوجيا</h3>
                    </div>
                    <p class="text-gray-600">فريق متخصص في التغطية الإعلامية وتطوير الحلول التقنية.</p>
                    <div id="mediaTeam" class="hidden mt-4 fade-in">
                        <h4 class="font-semibold mb-2">أعضاء الفريق:</h4>
                        <ul class="list-disc mr-4 space-y-1">
                            <li>أمير عمار</li>
                            <li>أمير طالب</li>
                            <li>أحمد منتظر</li>
                            <li>براق أمجد</li>
                            <li>كرار أحمد</li>
                        </ul>
                        <p class="mt-2 text-sm text-gray-500">المشرف الثانوي: رامي جعفر</p>
                    </div>
                </div>
                
                <!-- Social Research Team -->
                <div class="team-card rounded-lg p-6 shadow-md cursor-pointer" onclick="showTeam('social')">
                    <div class="flex items-center mb-4">
                        <div class="p-3 rounded-full bg-amber-100 text-amber-700 mr-3">
                            <i class="fas fa-users text-xl"></i>
                        </div>
                        <h3 class="text-xl font-bold">فريق البحث الاجتماعي</h3>
                    </div>
                    <p class="text-gray-600">فريق متخصص في الدراسات الاجتماعية وتحليل الظواهر المجتمعية.</p>
                    <div id="socialTeam" class="hidden mt-4 fade-in">
                        <h4 class="font-semibold mb-2">أعضاء الفريق:</h4>
                        <ul class="list-disc mr-4 space-y-1">
                            <li>موسى حامد</li>
                            <li>ياسر عمار</li>
                        </ul>
                        <p class="mt-2 text-sm text-gray-500">المشرف الثانوي: رامي جعفر</p>
                    </div>
                </div>
                
                <!-- Theater Team -->
                <div class="team-card rounded-lg p-6 shadow-md cursor-pointer" onclick="showTeam('theater')">
                    <div class="flex items-center mb-4">
                        <div class="p-3 rounded-full bg-amber-100 text-amber-700 mr-3">
                            <i class="fas fa-theater-masks text-xl"></i>
                        </div>
                        <h3 class="text-xl font-bold">فريق المسرحيات والفعاليات</h3>
                    </div>
                    <p class="text-gray-600">فريق متخصص في تنظيم الفعاليات الثقافية والعلمية.</p>
                    <div id="theaterTeam" class="hidden mt-4 fade-in">
                        <h4 class="font-semibold mb-2">أعضاء الفريق:</h4>
                        <ul class="list-disc mr-4 space-y-1">
                            <li>حسن علي حفظي</li>
                        </ul>
                        <p class="mt-2 text-sm text-gray-500">المشرف الثانوي: رامي جعفر</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- AI Section -->
    <section id="ai" class="py-16 px-4 light-brown-bg text-white">
        <div class="max-w-7xl mx-auto">
            <h2 class="text-3xl font-bold text-center mb-12">ذكاء المتفوقين</h2>
            
            <div class="grid md:grid-cols-2 gap-8 items-center">
                <div>
                    <h3 class="text-2xl font-bold mb-4">نظام الذكاء الاصطناعي المتطور</h3>
                    <p class="text-lg mb-4" id="aiText1">يقدم مركز أثر الخالدين نظام ذكاء اصطناعي متطور جدًا يعمل على تحليل البيانات الضخمة وتقديم حلول مبتكرة في مختلف المجالات.</p>
                    <p class="text-lg mb-6" id="aiText2">تم تطوير هذا النظام باستخدام أحدث التقنيات في تعلم الآلة ومعالجة اللغات الطبيعية، مما يجعله قادرًا على فهم السياقات المعقدة واتخاذ القرارات الذكية.</p>
                    
                    <div class="grid grid-cols-2 gap-4">
                        <div class="bg-white bg-opacity-20 p-4 rounded-lg">
                            <i class="fas fa-brain text-2xl mb-2"></i>
                            <h4 class="font-bold">تحليل البيانات</h4>
                            <p class="text-sm">تحليل كميات هائلة من البيانات في ثوانٍ</p>
                        </div>
                        <div class="bg-white bg-opacity-20 p-4 rounded-lg">
                            <i class="fas fa-robot text-2xl mb-2"></i>
                            <h4 class="font-bold">التعلم الذاتي</h4>
                            <p class="text-sm">يتعلم من التجارب السابقة باستمرار</p>
                        </div>
                        <div class="bg-white bg-opacity-20 p-4 rounded-lg">
                            <i class="fas fa-language text-2xl mb-2"></i>
                            <h4 class="font-bold">فهم اللغة</h4>
                            <p class="text-sm">يفهم اللغة الطبيعية بكل تعقيداتها</p>
                        </div>
                        <div class="bg-white bg-opacity-20 p-4 rounded-lg">
                            <i class="fas fa-lightbulb text-2xl mb-2"></i>
                            <h4 class="font-bold">حلول مبتكرة</h4>
                            <p class="text-sm">يقدم حلولاً غير تقليدية للمشكلات</p>
                        </div>
                    </div>
                </div>
                
                <div class="bg-white bg-opacity-30 p-6 rounded-lg">
                    <h3 class="text-2xl font-bold mb-4 text-center">محادثة مع الذكاء الاصطناعي</h3>
                    
                    <div class="chat-container bg-white bg-opacity-20 rounded-lg p-4 mb-4 h-64 overflow-y-auto">
                        <div id="chatHistory" class="space-y-3">
                            <div class="text-right">
                                <div class="bg-amber-700 text-white inline-block px-4 py-2 rounded-lg max-w-xs md:max-w-md">
                                    مرحبا! أنا مساعد الذكاء الاصطناعي لمركز أثر الخالدين. كيف يمكنني مساعدتك اليوم؟
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <div class="relative">
                        <input id="aiQuestion" type="text" placeholder="اطرح سؤالك هنا..." 
                               class="w-full p-3 rounded-lg text-gray-800 pr-12">
                        <button onclick="askAI()" class="absolute left-3 top-3 text-amber-700">
                            <i class="fas fa-paper-plane"></i>
                        </button>
                    </div>
                    
                    <div id="loadingIndicator" class="hidden mt-2 text-center">
                        <i class="fas fa-spinner fa-spin text-amber-700"></i>
                        <span class="mr-2">جاري تحليل السؤال...</span>
                    </div>
                    
                    <div class="mt-4 grid grid-cols-2 gap-2">
                        <button onclick="suggestQuestion('ما هي أحدث أبحاث المركز؟')" 
                                class="text-xs bg-white bg-opacity-20 hover:bg-opacity-30 p-2 rounded">
                            أحدث الأبحاث
                        </button>
                        <button onclick="suggestQuestion('كيف يمكنني المشاركة في الأبحاث؟')" 
                                class="text-xs bg-white bg-opacity-20 hover:bg-opacity-30 p-2 rounded">
                            المشاركة في الأبحاث
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Videos Section -->
    <section id="videos" class="py-16 px-4 beige-bg">
        <div class="max-w-7xl mx-auto">
            <h2 class="text-3xl font-bold text-center mb-12 gold-text">احنا نشرحلك</h2>
            
            <div id="videosContainer" class="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Default videos -->
                <div class="bg-white rounded-lg shadow-md overflow-hidden">
                    <div class="video-container">
                        <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allowfullscreen></iframe>
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold text-lg mb-2">مقدمة عن المركز</h3>
                        <p class="text-gray-600">تعرف على مركز أثر الخالدين للأبحاث العلمية وأهدافه</p>
                    </div>
                </div>
                
                <div class="bg-white rounded-lg shadow-md overflow-hidden">
                    <div class="video-container">
                        <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allowfullscreen></iframe>
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold text-lg mb-2">أحدث الأبحاث</h3>
                        <p class="text-gray-600">تعرف على أحدث الأبحاث التي أجراها فريقنا</p>
                    </div>
                </div>
                
                <div class="bg-white rounded-lg shadow-md overflow-hidden">
                    <div class="video-container">
                        <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allowfullscreen></iframe>
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold text-lg mb-2">نظام الذكاء الاصطناعي</h3>
                        <p class="text-gray-600">كيف يعمل نظام الذكاء الاصطناعي الخاص بنا</p>
                    </div>
                </div>
            </div>
            
            <!-- Add Video Form (Visible in Edit Mode) -->
            <div id="addVideoForm" class="hidden mt-8 bg-white p-6 rounded-lg shadow-md">
                <h3 class="text-xl font-bold mb-4 gold-text">إضافة فيديو جديد</h3>
                <div class="mb-4">
                    <label class="block text-gray-700 mb-2">عنوان الفيديو</label>
                    <input type="text" id="videoTitle" class="w-full p-2 border rounded">
                </div>
                <div class="mb-4">
                    <label class="block text-gray-700 mb-2">رابط YouTube</label>
                    <input type="text" id="videoUrl" class="w-full p-2 border rounded" placeholder="https://www.youtube.com/embed/...">
                </div>
                <div class="mb-4">
                    <label class="block text-gray-700 mb-2">وصف الفيديو</label>
                    <textarea id="videoDesc" class="w-full p-2 border rounded" rows="3"></textarea>
                </div>
                <button onclick="addVideo()" class="bg-amber-700 hover:bg-amber-800 text-white py-2 px-4 rounded">
                    إضافة الفيديو
                </button>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-16 px-4 bg-white">
        <div class="max-w-7xl mx-auto">
            <h2 class="text-3xl font-bold text-center mb-12 gold-text">تواصل معنا</h2>
            
            <div class="grid md:grid-cols-2 gap-8">
                <div>
                    <h3 class="text-xl font-bold mb-4">ابقى على تواصل</h3>
                    <p class="mb-6">نرحب بأسئلتكم واستفساراتكم واقتراحاتكم. فريقنا متاح للرد على جميع استفساراتكم.</p>
                    
                    <div class="space-y-4">
                        <div class="flex items-start">
                            <div class="p-2 bg-amber-100 text-amber-700 rounded-full mr-3">
                                <i class="fas fa-envelope"></i>
                            </div>
                            <div>
                                <h4 class="font-bold">البريد الإلكتروني</h4>
                                <p>ramyjfr457@gmail.com</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="p-2 bg-amber-100 text-amber-700 rounded-full mr-3">
                                <i class="fas fa-phone"></i>
                            </div>
                            <div>
                                <h4 class="font-bold">الهاتف</h4>
                                <p>+123 456 7890</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="p-2 bg-amber-100 text-amber-700 rounded-full mr-3">
                                <i class="fas fa-map-marker-alt"></i>
                            </div>
                            <div>
                                <h4 class="font-bold">العنوان</h4>
                                <p>مركز أثر الخالدين للأبحاث العلمية، المدينة، الدولة</p>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div>
                    <form id="contactForm" class="bg-gray-50 p-6 rounded-lg shadow-sm">
                        <div class="mb-4">
                            <label for="name" class="block text-gray-700 mb-2">الاسم الكامل</label>
                            <input type="text" id="name" class="w-full p-2 border rounded" required>
                        </div>
                        
                        <div class="mb-4">
                            <label for="email" class="block text-gray-700 mb-2">البريد الإلكتروني</label>
                            <input type="email" id="email" class="w-full p-2 border rounded" required>
                        </div>
                        
                        <div class="mb-4">
                            <label for="subject" class="block text-gray-700 mb-2">الموضوع</label>
                            <input type="text" id="subject" class="w-full p-2 border rounded" required>
                        </div>
                        
                        <div class="mb-4">
                            <label for="message" class="block text-gray-700 mb-2">الرسالة</label>
                            <textarea id="message" class="w-full p-2 border rounded" rows="4" required></textarea>
                        </div>
                        
                        <button type="submit" class="w-full bg-amber-700 hover:bg-amber-800 text-white py-3 rounded-lg font-bold">
                            إرسال الرسالة <i class="fas fa-paper-plane mr-2"></i>
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-8 px-4">
        <div class="max-w-7xl mx-auto">
            <div class="grid md:grid-cols-3 gap-8">
                <div>
                    <h3 class="text-xl font-bold mb-4 gold-text">مركز أثر الخالدين للأبحاث العلمية</h3>
                    <p>نحو مستقبل مشرق بالمعرفة والابتكار. نعمل على تطوير البحث العلمي وبناء جيل من العلماء والباحثين المتميزين.</p>
                </div>
                
                <div>
                    <h3 class="text-xl font-bold mb-4 gold-text">روابط سريعة</h3>
                    <ul class="space-y-2">
                        <li><a href="#about" class="hover:text-amber-300">عن المركز</a></li>
                        <li><a href="#teams" class="hover:text-amber-300">فريقنا</a></li>
                        <li><a href="#ai" class="hover:text-amber-300">ذكاء المتفوقين</a></li>
                        <li><a href="#videos" class="hover:text-amber-300">احنا نشرحلك</a></li>
                        <li><a href="#contact" class="hover:text-amber-300">تواصل معنا</a></li>
                    </ul>
                </div>
                
                <div>
                    <h3 class="text-xl font-bold mb-4 gold-text">تابعنا</h3>
                    <div class="flex space-x-4 space-x-reverse">
                        <a href="#" class="p-2 bg-gray-700 rounded-full hover:bg-amber-700">
                            <i class="fab fa-facebook-f"></i>
                        </a>
                        <a href="#" class="p-2 bg-gray-700 rounded-full hover:bg-amber-700">
                            <i class="fab fa-twitter"></i>
                        </a>
                        <a href="#" class="p-2 bg-gray-700 rounded-full hover:bg-amber-700">
                            <i class="fab fa-linkedin-in"></i>
                        </a>
                        <a href="#" class="p-2 bg-gray-700 rounded-full hover:bg-amber-700">
                            <i class="fab fa-youtube"></i>
                        </a>
                    </div>
                </div>
            </div>
            
            <div class="border-t border-gray-700 mt-8 pt-6 text-center text-gray-400">
                <p>© 2023 مركز أثر الخالدين للأبحاث العلمية. جميع الحقوق محفوظة.</p>
            </div>
        </div>
    </footer>

    <!-- Edit Mode Modal -->
    <div id="editModal" class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center hidden z-20">
        <div class="bg-white p-6 rounded-lg w-full max-w-md">
            <h3 class="text-xl font-bold mb-4 gold-text">تفعيل نمط التحرير</h3>
            <p class="mb-4">لتفعيل نمط التحرير، يرجى إدخال كلمة المرور:</p>
            <input type="password" id="editPassword" class="w-full p-2 border rounded mb-4" placeholder="كلمة المرور">
            <div class="flex justify-end space-x-4 space-x-reverse">
                <button onclick="cancelEdit()" class="px-4 py-2 border rounded">إلغاء</button>
                <button onclick="verifyEditPassword()" class="px-4 py-2 bg-amber-700 text-white rounded">تأكيد</button>
            </div>
        </div>
    </div>

    <!-- Success Notification -->
    <div id="successNotification" class="fixed bottom-4 right-4 bg-green-500 text-white px-6 py-3 rounded-lg shadow-lg hidden z-30">
        <div class="flex items-center">
            <i class="fas fa-check-circle mr-2"></i>
            <span>تم إرسال رسالتك بنجاح!</span>
        </div>
    </div>

    <script>
        // Mobile menu toggle
        document.getElementById('mobile-menu-button').addEventListener('click', function() {
            document.getElementById('mobile-menu').classList.toggle('hidden');
        });
        
        // Show team members with animation
        function showTeam(teamId) {
            // Hide all teams first
            document.querySelectorAll('[id$="Team"]').forEach(el => {
                el.classList.add('hidden');
            });
            
            // Show selected team after animation
            setTimeout(() => {
                document.getElementById(teamId + 'Team').classList.remove('hidden');
            }, 100);
        }
        
        // Edit mode functionality
        let editMode = false;
        
        document.getElementById('editBtn').addEventListener('click', function() {
            if (!editMode) {
                document.getElementById('editModal').classList.remove('hidden');
            } else {
                disableEditMode();
            }
        });
        
        function verifyEditPassword() {
            const password = document.getElementById('editPassword').value;
            if (password === 'OHS15') {
                enableEditMode();
                document.getElementById('editModal').classList.add('hidden');
            } else {
                alert('كلمة المرور غير صحيحة');
            }
        }
        
        function cancelEdit() {
            document.getElementById('editModal').classList.add('hidden');
            document.getElementById('editPassword').value = '';
        }
        
        function enableEditMode() {
            editMode = true;
            document.body.classList.add('edit-mode');
            document.getElementById('editBtn').textContent = 'خروج من نمط التحرير';
            document.getElementById('editBtn').classList.add('bg-red-600', 'hover:bg-red-700');
            document.getElementById('editBtn').classList.remove('bg-amber-700', 'hover:bg-amber-800');
            
            // Show edit controls
            document.getElementById('addVideoForm').classList.remove('hidden');
            
            // Make all text editable
            document.querySelectorAll('p, h1, h2, h3, h4, span:not(.gold-text)').forEach(el => {
                el.setAttribute('contenteditable', 'true');
                el.classList.add('hover:bg-amber-100');
            });
        }
        
        function disableEditMode() {
            editMode = false;
            document.body.classList.remove('edit-mode');
            document.getElementById('editBtn').textContent = 'نمط التحرير';
            document.getElementById('editBtn').classList.remove('bg-red-600', 'hover:bg-red-700');
            document.getElementById('editBtn').classList.add('bg-amber-700', 'hover:bg-amber-800');
            
            // Hide edit controls
            document.getElementById('addVideoForm').classList.add('hidden');
            
            // Make all text non-editable
            document.querySelectorAll('[contenteditable="true"]').forEach(el => {
                el.removeAttribute('contenteditable');
                el.classList.remove('hover:bg-amber-100');
            });
        }
        
        // Add video functionality
        function addVideo() {
            const title = document.getElementById('videoTitle').value;
            const url = document.getElementById('videoUrl').value;
            const desc = document.getElementById('videoDesc').value;
            
            if (!title || !url || !desc) {
                alert('يرجى ملء جميع الحقول');
                return;
            }
            
            const videoContainer = document.getElementById('videosContainer');
            const videoHtml = `
                <div class="bg-white rounded-lg shadow-md overflow-hidden">
                    <div class="video-container">
                        <iframe src="${url}" frameborder="0" allowfullscreen></iframe>
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold text-lg mb-2">${title}</h3>
                        <p class="text-gray-600">${desc}</p>
                    </div>
                </div>
            `;
            
            videoContainer.insertAdjacentHTML('afterbegin', videoHtml);
            
            // Clear form
            document.getElementById('videoTitle').value = '';
            document.getElementById('videoUrl').value = '';
            document.getElementById('videoDesc').value = '';
        }
        
        // AI Chat Functions
        function askAI() {
            const question = document.getElementById('aiQuestion').value.trim();
            if (!question) return;
            
            // Add user question to chat
            const chatHistory = document.getElementById('chatHistory');
            chatHistory.innerHTML += `
                <div class="text-left">
                    <div class="bg-gray-100 text-gray-800 inline-block px-4 py-2 rounded-lg max-w-xs md:max-w-md">
                        ${question}
                    </div>
                </div>
            `;
            
            document.getElementById('aiQuestion').value = '';
            document.getElementById('loadingIndicator').classList.remove('hidden');
            
            // Simulate AI response after delay
            setTimeout(() => {
                const responses = [
                    "هذا سؤال ممتاز! بناءً على أبحاثنا الأخيرة، يمكننا القول أن...",
                    "وفقًا لبيانات المركز، الإجابة هي...",
                    "لقد وجدنا في أبحاثنا أن...",
                    "هذا مجال بحثي نشط حاليًا في المركز. النتائج الأولية تشير إلى..."
                ];
                const randomResponse = responses[Math.floor(Math.random() * responses.length)];
                
                chatHistory.innerHTML += `
                    <div class="text-right">
                        <div class="bg-amber-700 text-white inline-block px-4 py-2 rounded-lg max-w-xs md:max-w-md">
                            ${randomResponse}
                        </div>
                    </div>
                `;
                
                document.getElementById('loadingIndicator').classList.add('hidden');
                chatHistory.scrollTop = chatHistory.scrollHeight;
            }, 1500);
        }
        
        function suggestQuestion(question) {
            document.getElementById('aiQuestion').value = question;
        }
        
        // Contact form submission
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Simulate sending email
            const name = document.getElementById('name').value;
            const email = document.getElementById('email').value;
            const subject = document.getElementById('subject').value;
            const message = document.getElementById('message').value;
            
            // Here you would normally send the data to a server
            console.log('Sending message:', {name, email, subject, message});
            
            // Show success notification
            document.getElementById('successNotification').classList.remove('hidden');
            
            // Reset form
            this.reset();
            
            // Hide notification after 3 seconds
            setTimeout(() => {
                document.getElementById('successNotification').classList.add('hidden');
            }, 3000);
        });
        
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
                
                // Close mobile menu if open
                document.getElementById('mobile-menu').classList.add('hidden');
            });
        });
    </script>
</body>
</html>
