 <!DOCTYPE html>
<html lang="uk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>OptiMind - AI для автоматизації вашого бізнесу</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
        
        body {
            font-family: 'Inter', sans-serif;
            scroll-behavior: smooth;
        }
        
        .gradient-text {
            background: linear-gradient(90deg, #3b82f6, #10b981);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        
        .floating {
            animation: floating 3s ease-in-out infinite;
        }
        
        @keyframes floating {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-15px); }
            100% { transform: translateY(0px); }
        }
        
        .pulse {
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }
        
        .fade-in {
            animation: fadeIn 1s ease-in;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        .glow {
            box-shadow: 0 0 15px rgba(59, 130, 246, 0.5);
        }
        
        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1);
        }
        
        .testimonial-card {
            transition: all 0.3s ease;
        }
        
        .testimonial-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1);
        }
        
        .progress-bar {
            height: 6px;
            background-color: #e5e7eb;
            border-radius: 3px;
            overflow: hidden;
        }
        
        .progress-fill {
            height: 100%;
            background: linear-gradient(90deg, #3b82f6, #10b981);
            border-radius: 3px;
            transition: width 1s ease-in-out;
        }
        
        .step-number {
            min-width: 40px;
            height: 40px;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .pricing-card {
            transition: all 0.3s ease;
            border: 2px solid transparent;
        }
        
        .pricing-card:hover {
            transform: translateY(-10px);
            border-color: #3b82f6;
        }
        
        .pricing-card.popular {
            border-color: #10b981;
            position: relative;
        }
        
        .pricing-card.popular::before {
            content: "Популярний";
            position: absolute;
            top: -12px;
            left: 50%;
            transform: translateX(-50%);
            background: #10b981;
            color: white;
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 600;
        }
    </style>
</head>
<body class="bg-white text-gray-800">
    <!-- Sticky CTA Button -->
    <div class="fixed bottom-5 right-5 z-50">
        <button id="sticky-cta" class="bg-blue-600 hover:bg-blue-700 text-white font-bold py-3 px-6 rounded-full shadow-lg transform transition-all duration-300 hover:scale-105 flex items-center pulse glow">
            <i class="fas fa-calendar-check mr-2"></i>
            <span>Звʼязок</span>
        </button>
    </div>

    <!-- Hero Section -->
    <section class="py-20 px-4">
        <div class="container mx-auto flex flex-col md:flex-row items-center">
            <div class="md:w-1/2 mb-10 md:mb-0 fade-in">
                <h1 class="text-4xl md:text-5xl font-bold mb-6 leading-tight">
                    <span class="gradient-text">Автоматизуйте свій бізнес</span> <br>з допомогою штучного інтелекту
                </h1>
                <p class="text-xl text-gray-600 mb-8">OptiMind допомагає підприємствам збільшити прибуток на 30-150% завдяки автоматизації рутинних процесів та аналітиці даних у реальному часі.</p>
                <div class="flex space-x-4 mb-8">
                    <a href="https://t.me/dessigka" target="_blank" class="text-blue-500 hover:text-blue-700">
                        <i class="fab fa-telegram fa-2x"></i>
                    </a>
                    <a href="https://www.instagram.com/rockwel.capital?igsh=NnA4OGtzdmEzbmNx&utm_source=qr" target="_blank" class="text-pink-500 hover:text-pink-700">
                        <i class="fab fa-instagram fa-2x"></i>
                    </a>
                    <a href="https://wa.me/380661176745?text=Привіт Михайле!" target="_blank" class="text-green-500 hover:text-green-700">
                        <i class="fab fa-whatsapp fa-2x"></i>
                    </a>
                </div>
                <div class="mt-4">
                    <p class="text-gray-600">Email: <a href="mailto:rockwellcapital1@gmail.com" class="text-blue-600 hover:underline">rockwellcapital1@gmail.com</a></p>
                </div>
                <div class="flex flex-col sm:flex-row space-y-4 sm:space-y-0 sm:space-x-4">
                   
                    
                    </button>
                </div>
                <div class="mt-6 flex items-center">
                    <div class="flex -space-x-2">
                        <img src="https://randomuser.me/api/portraits/women/44.jpg" class="w-10 h-10 rounded-full border-2 border-white" alt="User">
                        <img src="https://randomuser.me/api/portraits/men/32.jpg" class="w-10 h-10 rounded-full border-2 border-white" alt="User">
                        <img src="https://randomuser.me/api/portraits/women/68.jpg" class="w-10 h-10 rounded-full border-2 border-white" alt="User">
                    </div>
                    <div class="ml-4">
                        <div class="flex items-center">
                            <div class="flex text-yellow-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                            </div>
                            <span class="ml-2 text-gray-600">5.0 (17 відгуків)</span>
                        </div>
                        <p class="text-sm text-gray-500">Понад 20 бізнесів вже використовують OptiMind</p>
                    </div>
                </div>
            </div>
            <div class="md:w-1/2 flex justify-center">
                <div class="relative">
                    <img src="https://illustrations.popsy.co/amber/artificial-intelligence.svg" alt="AI Illustration" class="w-full max-w-lg floating">
                    <div class="absolute -bottom-10 -left-10 bg-blue-100 rounded-full p-4 shadow-lg">
                        <div class="bg-white rounded-full p-3 shadow-md">
                            <i class="fas fa-chart-line text-blue-600 text-2xl"></i>
                        </div>
                        <p class="mt-2 text-sm font-semibold text-center">+150% ROI</p>
                    </div>
                    <div class="absolute -top-10 -right-10 bg-green-100 rounded-full p-4 shadow-lg">
                        <div class="bg-white rounded-full p-3 shadow-md">
                            <i class="fas fa-clock text-green-600 text-2xl">  Ші</i>
                        </div>
                        <p class="mt-2 text-sm font-semibold text-center">Економить 20 год/тиждень</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Problem Section -->
    <section id="problem" class="py-16 bg-gray-50 px-4">
        <div class="container mx-auto">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold mb-4">Ваш бізнес втрачає грощі через ці проблеми?</h2>
                <div class="w-20 h-1 bg-blue-600 mx-auto"></div>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8">
                <div class="bg-white p-8 rounded-xl shadow-md hover:shadow-xl transition-all duration-300 transform hover:-translate-y-2">
                    <div class="text-blue-600 text-4xl mb-4">
                        <i class="fas fa-clock"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Втрата часу на рутину</h3>
                    <p class="text-gray-600">Ваші співробітники витрачають години на повторювані завдання, які можна автоматизувати.</p>
                    <div class="mt-6">
                        <div class="flex justify-between mb-1">
                            <span class="text-sm font-medium text-gray-500">Продуктивність</span>
                            <span class="text-sm font-medium text-gray-500">40%</span>
                        </div>
                        <div class="progress-bar">
                            <div class="progress-fill" style="width: 40%"></div>
                        </div>
                    </div>
                </div>
                
                <div class="bg-white p-8 rounded-xl shadow-md hover:shadow-xl transition-all duration-300 transform hover:-translate-y-2">
                    <div class="text-blue-600 text-4xl mb-4">
                        <i class="fas fa-exclamation-triangle"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Людський фактор</h3>
                    <p class="text-gray-600">Помилки в обробці даних, пропущені клієнти, неякісні аналітичні звіти.</p>
                    <div class="mt-6">
                        <div class="flex justify-between mb-1">
                            <span class="text-sm font-medium text-gray-500">Точність</span>
                            <span class="text-sm font-medium text-gray-500">75%</span>
                        </div>
                        <div class="progress-bar">
                            <div class="progress-fill" style="width: 75%"></div>
                        </div>
                    </div>
                </div>
                
                <div class="bg-white p-8 rounded-xl shadow-md hover:shadow-xl transition-all duration-300 transform hover:-translate-y-2">
                    <div class="text-blue-600 text-4xl mb-4">
                        <i class="fas fa-chart-line"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Втрата прибутку</h3>
                    <p class="text-gray-600">Відсутність персоналізації пропозицій, невикористані можливості для апселу та крос-селу.</p>
                    <div class="mt-6">
                        <div class="flex justify-between mb-1">
                            <span class="text-sm font-medium text-gray-500">Прибутковість</span>
                            <span class="text-sm font-medium text-gray-500">60%</span>
                        </div>
                        <div class="progress-bar">
                            <div class="progress-fill" style="width: 60%"></div>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="mt-12 bg-gradient-to-r from-blue-600 to-green-500 rounded-xl p-8 text-white">
                <div class="flex flex-col md:flex-row items-center">
                    <div class="md:w-2/3 mb-6 md:mb-0">
                        <h3 class="text-2xl font-bold mb-2">Це коштує вашому бізнесу 1000$ щомісяця</h3>
                        <p>Дослідження показують, що бізнеси без автоматизації втрачають до 40% потенційного прибутку.</p>
                    </div>
                    <div class="md:w-1/3 flex justify-center md:justify-end">
                        <button class="bg-white text-blue-600 hover:bg-gray-100 font-bold py-3 px-6 rounded-lg shadow-lg transform transition-all duration-300 hover:scale-105">
                            Виправити це
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Solution Section -->
    <section id="solution" class="py-16 px-4">
        <div class="container mx-auto">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold mb-4">Як <span class="gradient-text">OptiMind</span> вирішує ваші проблеми</h2>
                <p class="text-xl text-gray-600 max-w-3xl mx-auto">Наш AI-асистент автоматизує ключові бізнес-процеси, даючи вам конкурентну перевагу</p>
                <div class="w-20 h-1 bg-green-500 mx-auto mt-4"></div>
            </div>
            
            <div class="flex flex-col md:flex-row items-center mb-16">
                <div class="md:w-1/2 mb-8 md:mb-0">
                    <img src="https://illustrations.popsy.co/amber/digital-nomad.svg" alt="Solution" class="w-full max-w-md mx-auto">
                </div>
                <div class="md:w-1/2 md:pl-12">
                    <div class="flex items-start mb-6">
                        <div class="bg-blue-100 p-3 rounded-full mr-4">
                            <i class="fas fa-robot text-blue-600 text-xl"></i>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold mb-2">Автоматизація процесів</h3>
                            <p class="text-gray-600">OptiMind бере на себе обробку замовлень, комунікацію з клієнтами, аналіз даних та інші рутинні завдання.</p>
                        </div>
                    </div>
                    
                    <div class="flex items-start mb-6">
                        <div class="bg-green-100 p-3 rounded-full mr-4">
                            <i class="fas fa-brain text-green-600 text-xl"></i>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold mb-2">Інтелектуальна аналітика</h3>
                            <p class="text-gray-600">Наш алгоритм аналізує дані у реальному часі, виявляючи приховані можливості для зростання продажів.</p>
                        </div>
                    </div>
                    
                    <div class="flex items-start">
                        <div class="bg-purple-100 p-3 rounded-full mr-4">
                            <i class="fas fa-user-tie text-purple-600 text-xl"></i>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold mb-2">Персоналізація</h3>
                            <p class="text-gray-600">Створення індивідуальних пропозицій для кожного клієнта на основі його поведінки та історії покупок.</p>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="bg-gray-50 rounded-xl p-8">
                <h3 class="text-2xl font-bold mb-6 text-center">Реальні результати наших клієнтів</h3>
                <div class="grid md:grid-cols-3 gap-8">
                    <div class="text-center">
                        <div class="text-4xl font-bold text-blue-600 mb-2">+47%</div>
                        <p class="text-gray-600">Зростання конверсії</p>
                        <div class="mt-4">
                            <div class="progress-bar mx-auto w-3/4">
                                <div class="progress-fill" style="width: 47%"></div>
                            </div>
                        </div>
                    </div>
                    <div class="text-center">
                        <div class="text-4xl font-bold text-green-600 mb-2">-47%</div>
                        <p class="text-gray-600">Скорочення витрат</p>
                        <div class="mt-4">
                            <div class="progress-bar mx-auto w-3/4">
                                <div class="progress-fill" style="width: 35%"></div>
                            </div>
                        </div>
                    </div>
                    <div class="text-center">
                        <div class="text-4xl font-bold text-purple-600 mb-2">+82%</div>
                        <p class="text-gray-600">Зростання повторних продажів</p>
                        <div class="mt-4">
                            <div class="progress-bar mx-auto w-3/4">
                                <div class="progress-fill" style="width: 82%"></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section id="features" class="py-16 bg-gray-50 px-4">
        <div class="container mx-auto">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold mb-4">Можливості <span class="gradient-text">OptiMind</span></h2>
                <p class="text-xl text-gray-600 max-w-3xl mx-auto">Все, що потрібно для автоматизації та масштабування вашого бізнесу</p>
                <div class="w-20 h-1 bg-blue-600 mx-auto mt-4"></div>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="bg-white p-8 rounded-xl shadow-md feature-card transition-all duration-300">
                    <div class="text-blue-600 text-4xl mb-4">
                        <i class="fas fa-comments"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">AI-чатботи</h3>
                    <p class="text-gray-600 mb-4">24/7 обслуговування клієнтів з персоналізованими відповідями на основі NLP.</p>
                    <ul class="space-y-2">
                        <li class="flex items-center">
                            <i class="fas fa-check-circle text-green-500 mr-2"></i>
                            <span>Відповіді на 95% запитів</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check-circle text-green-500 mr-2"></i>
                            <span>Інтеграція з соцмережами</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check-circle text-green-500 mr-2"></i>
                            <span>Навчання на ваших даних</span>
                        </li>
                    </ul>
                </div>
                
                <div class="bg-white p-8 rounded-xl shadow-md feature-card transition-all duration-300">
                    <div class="text-green-600 text-4xl mb-4">
                        <i class="fas fa-chart-pie"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Прогностична аналітика</h3>
                    <p class="text-gray-600 mb-4">Точні прогнози продажів, попиту та інших ключових показників бізнесу.</p>
                    <ul class="space-y-2">
                        <li class="flex items-center">
                            <i class="fas fa-check-circle text-green-500 mr-2"></i>
                            <span>Точність до 92%</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check-circle text-green-500 mr-2"></i>
                            <span>Автоматичні звіти</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check-circle text-green-500 mr-2"></i>
                            <span>Рекомендації щодо дій</span>
                        </li>
                    </ul>
                </div>
                
                <div class="bg-white p-8 rounded-xl shadow-md feature-card transition-all duration-300">
                    <div class="text-purple-600 text-4xl mb-4">
                        <i class="fas fa-shopping-cart"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Персоналізовані оферти</h3>
                    <p class="text-gray-600 mb-4">Автоматичне формування індивідуальних пропозицій для кожного клієнта.</p>
                    <ul class="space-y-2">
                        <li class="flex items-center">
                            <i class="fas fa-check-circle text-green-500 mr-2"></i>
                            <span>Аналіз поведінки</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check-circle text-green-500 mr-2"></i>
                            <span>Динамічні ціни</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check-circle text-green-500 mr-2"></i>
                            <span>Оптимальні часи для контакту</span>
                        </li>
                    </ul>
                </div>
                
                <div class="bg-white p-8 rounded-xl shadow-md feature-card transition-all duration-300">
                    <div class="text-yellow-600 text-4xl mb-4">
                        <i class="fas fa-tasks"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Автоматизація робочих процесів</h3>
                    <p class="text-gray-600 mb-4">Оптимізація внутрішніх бізнес-процесів без участі людини.</p>
                    <ul class="space-y-2">
                        <li class="flex items-center">
                            <i class="fas fa-check-circle text-green-500 mr-2"></i>
                            <span>Інтеграція з CRM/ERP</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check-circle text-green-500 mr-2"></i>
                            <span>Автоматичні нагадування</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check-circle text-green-500 mr-2"></i>
                            <span>Розподіл завдань</span>
                        </li>
                    </ul>
                </div>
                
                <div class="bg-white p-8 rounded-xl shadow-md feature-card transition-all duration-300">
                    <div class="text-red-600 text-4xl mb-4">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Захист від шахрайства</h3>
                    <p class="text-gray-600 mb-4">Виявлення підозрілих операцій та потенційних ризиків у реальному часі.</p>
                    <ul class="space-y-2">
                        <li class="flex items-center">
                            <i class="fas fa-check-circle text-green-500 mr-2"></i>
                            <span>Аналіз транзакцій</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check-circle text-green-500 mr-2"></i>
                            <span>Виявлення аномалій</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check-circle text-green-500 mr-2"></i>
                            <span>Попередження про ризики</span>
                        </li>
                    </ul>
                </div>
                
                <div class="bg-white p-8 rounded-xl shadow-md feature-card transition-all duration-300">
                    <div class="text-indigo-600 text-4xl mb-4">
                        <i class="fas fa-lightbulb"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Генерація ідей</h3>
                    <p class="text-gray-600 mb-4">AI-асистент пропонує нові ідеї для розвитку бізнесу на основі трендів.</p>
                    <ul class="space-y-2">
                        <li class="flex items-center">
                            <i class="fas fa-check-circle text-green-500 mr-2"></i>
                            <span>Аналіз ринку</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check-circle text-green-500 mr-2"></i>
                            <span>Прогнозування трендів</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check-circle text-green-500 mr-2"></i>
                            <span>Персоналізовані рекомендації</span>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

   
                
               
    <!-- Testimonials Section -->
    <section id="testimonials" class="py-16 px-4">
        <div class="container mx-auto">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold mb-4">Що кажуть наші клієнти</h2>
                <p class="text-xl text-gray-600 max-w-3xl mx-auto">Реальні результати реальних бізнесів</p>
                <div class="w-20 h-1 bg-green-500 mx-auto mt-4"></div>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="bg-white p-8 rounded-xl shadow-md testimonial-card">
                    <div class="flex items-center mb-4">
                        <img src="https://randomuser.me/api/portraits/women/43.jpg" alt="User" class="w-12 h-12 rounded-full mr-4">
                        <div>
                            <h4 class="font-bold">Олена</h4>
                            <p class="text-gray-600 text-sm">CEO</p>
                        </div>
                    </div>
                    <div class="flex mb-4 text-yellow-400">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                    <p class="text-gray-700 italic">"Завдяки OptiMind ми збільшили продажі на 65% за 3 місяці."</p>
                </div>
                
                <div class="bg-white p-8 rounded-xl shadow-md testimonial-card">
                    <div class="flex items-center mb-4">
                        <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="User" class="w-12 h-12 rounded-full mr-4">
                        <div>
                            <h4 class="font-bold">Іван</h4>
                            <p class="text-gray-600 text-sm">COO</p>
                        </div>
                    </div>
                    <div class="flex mb-4 text-yellow-400">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                    <p class="text-gray-700 italic">"Наші операційні витрати скоротилися на 40%, а ефективність команди зросла вдвічі. Найкраще рішення для автоматизації!"</p>
                </div>
                
                <div class="bg-white p-8 rounded-xl shadow-md testimonial-card">
                    <div class="flex items-center mb-4">
                        <img src="https://randomuser.me/api/portraits/women/68.jpg" alt="User" class="w-12 h-12 rounded-full mr-4">
                        <div>
                            <h4 class="font-bold">Марія</h4>
                            <p class="text-gray-600 text-sm">Marketing Director</p>
                        </div>
                    </div>
                    <div class="flex mb-4 text-yellow-400">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                    <p class="text-gray-700 italic">"Конверсія нашого сайту зросла з 2.3% до 4.7% завдяки персоналізованим рекомендаціям від OptiMind. ROI понад 300%!"</p>
                </div>
            </div>
        </div>
    </section>

    <!-- How It Works Section -->
    <section class="py-16 bg-gray-50 px-4">
        <div class="container mx-auto">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold mb-4">Як це працює?</h2>
                <p class="text-xl text-gray-600 max-w-3xl mx-auto">Простий процес інтеграції - від першого контакту до результатів</p>
                <div class="w-20 h-1 bg-blue-600 mx-auto mt-4"></div>
            </div>
            
            <div class="max-w-4xl mx-auto">
                <div class="flex flex-col md:flex-row items-center mb-12">
                    <div class="md:w-1/3 mb-6 md:mb-0 flex justify-center">
                        <div class="step-number bg-blue-600 text-white rounded-full font-bold text-xl">1</div>
                    </div>
                    <div class="md:w-2/3">
                        <h3 class="text-xl font-bold mb-2">Аналіз вашого бізнесу</h3>
                        <p class="text-gray-600">Наші експерти вивчають ваші процеси та визначають точки росту.</p>
                    </div>
                </div>
                
                <div class="flex flex-col md:flex-row items-center mb-12">
                    <div class="md:w-1/3 mb-6 md:mb-0 flex justify-center">
                        <div class="step-number bg-blue-600 text-white rounded-full font-bold text-xl">2</div>
                    </div>
                    <div class="md:w-2/3">
                        <h3 class="text-xl font-bold mb-2">Налаштування рішення</h3>
                        <p class="text-gray-600">Ми адаптуємо OptiMind під ваші конкретні потреби.</p>
                    </div>
                </div>
                
                <div class="flex flex-col md:flex-row items-center mb-12">
                    <div class="md:w-1/3 mb-6 md:mb-0 flex justify-center">
                        <div class="step-number bg-blue-600 text-white rounded-full font-bold text-xl">3</div>
                    </div>
                    <div class="md:w-2/3">
                        <h3 class="text-xl font-bold mb-2">Інтеграція з вашими системами</h3>
                        <p class="text-gray-600">Безболісне підключення до вашого CRM, ERP та інших систем.</p>
                    </div>
                </div>
                
                <div class="flex flex-col md:flex-row items-center mb-12">
                    <div class="md:w-1/3 mb-6 md:mb-0 flex justify-center">
                        <div class="step-number bg-blue-600 text-white rounded-full font-bold text-xl">4</div>
                    </div>
                    <div class="md:w-2/3">
                        <h3 class="text-xl font-bold mb-2">Навчання AI на ваших даних</h3>
                        <p class="text-gray-600">Наш алгоритм аналізує історію вашого бізнесу для максимальної ефективності.</p>
                    </div>
                </div>
                
                <div class="flex flex-col md:flex-row items-center">
                    <div class="md:w-1/3 mb-6 md:mb-0 flex justify-center">
                        <div class="step-number bg-blue-600 text-white rounded-full font-bold text-xl">5</div>
                    </div>
                    <div class="md:w-2/3">
                        <h3 class="text-xl font-bold mb-2">Отримання результатів</h3>
                        <p class="text-gray-600">Ви отримуєте зростання ефективності та прибутку вже в перший місяць.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- FAQ Section -->
    <section class="py-16 px-4">
        <div class="container mx-auto">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold mb-4">Поширені запитання</h2>
                <p class="text-xl text-gray-600 max-w-3xl mx-auto">Відповіді на питання, які ви могли б мати</p>
                <div class="w-20 h-1 bg-green-500 mx-auto mt-4"></div>
            </div>
            
            <div class="max-w-3xl mx-auto">
                <div class="mb-6 border-b border-gray-200 pb-6">
                    <button class="flex justify-between items-center w-full text-left font-bold text-lg focus:outline-none faq-btn">
                        <span>Скільки часу потрібно для впровадження OptiMind?</span>
                        <i class="fas fa-chevron-down text-blue-600 transition-transform duration-300"></i>
                    </button>
                    <div class="mt-4 text-gray-600 hidden faq-answer">
                        <p>Середній термін впровадження становить від 3 до 14 днів, залежно від складності вашого бізнесу та кількості інтеграцій.</p>
                    </div>
                </div>
                
                <div class="mb-6 border-b border-gray-200 pb-6">
                    <button class="flex justify-between items-center w-full text-left font-bold text-lg focus:outline-none faq-btn">
                        <span>Чи безпечно довіряти вам свої дані?</span>
                        <i class="fas fa-chevron-down text-blue-600 transition-transform duration-300"></i>
                    </button>
                    <div class="mt-4 text-gray-600 hidden faq-answer">
                        <p>Так, безпека даних - наш пріоритет. У нас з вами буде договір про нерозголошення. Всі дані шифруються та зберігаються у захищених дата-центрах.</p>
                    </div>
                </div>
                
                <div class="mb-6 border-b border-gray-200 pb-6">
                    <button class="flex justify-between items-center w-full text-left font-bold text-lg focus:outline-none faq-btn">
                        <span>Чи потрібні технічні знання для використання?</span>
                        <i class="fas fa-chevron-down text-blue-600 transition-transform duration-300"></i>
                    </button>
                    <div class="mt-4 text-gray-600 hidden faq-answer">
                        <p>Ні, інтерфейс OptiMind інтуїтивно зрозумілий і не вимагає технічних знань. Крім того, ми надаємо повний супровід та навчання для вашої команди.</p>
                    </div>
                </div>
                
                <div class="mb-6 border-b border-gray-200 pb-6">
                    <button class="flex justify-between items-center w-full text-left font-bold text-lg focus:outline-none faq-btn">
                        <span>Які галузі ви обслуговуєте?</span>
                        <i class="fas fa-chevron-down text-blue-600 transition-transform duration-300"></i>
                    </button>
                    <div class="mt-4 text-gray-600 hidden faq-answer">
                        <p>OptiMind працює з бізнесами будь-якого розміру в різних галузях: e-commerce, фінанси, нерухомість, охорона здоров'я, освіта, логістика та багато інших.</p>
                    </div>
                </div>
                
                <div class="mb-6">
                    <button class="flex justify-between items-center w-full text-left font-bold text-lg focus:outline-none faq-btn">
                        <span>Як часто оновлюється програмне забезпечення?</span>
                        <i class="fas fa-chevron-down text-blue-600 transition-transform duration-300"></i>
                    </button>
                    <div class="mt-4 text-gray-600 hidden faq-answer">
                        <p>ШІ автоматизує ключові рутинні процеси. Оновлення буде разом з оновленням від провідних AI компаній. Ми регулярно випускаємо нові функції та покращення.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Security Section -->
    <section class="py-16 bg-gray-50 px-4">
        <div class="container mx-auto">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold mb-4">Безпека даних</h2>
                <p class="text-xl text-gray-600 max-w-3xl mx-auto">Ваша конфіденційність - наш пріоритет</p>
                <div class="w-20 h-1 bg-blue-600 mx-auto mt-4"></div>
            </div>
            
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 mb-8 md:mb-0">
                    <img src="" alt="" class="w-full max-w-md mx-auto">
                </div>
                <div class="md:w-1/2 md:pl-12">
                    <div class="flex items-start mb-6">
                        <div class="bg-blue-100 p-3 rounded-full mr-4">
                            <i class="fas fa-lock text-blue-600 text-xl"></i>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold mb-2">Шифрування даних</h3>
                            <p class="text-gray-600">Всі дані шифруються за допомогою AES-256, як під час передачі, так і під час зберігання.</p>
                        </div>
                    </div>
                    
                    <div class="flex items-start mb-6">
                        <div class="bg-green-100 p-3 rounded-full mr-4">
                            <i class="fas fa-shield-alt text-green-600 text-xl"></i>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold mb-2">Сертифіковані центри даних</h3>
                            <p class="text-gray-600">Ваші дані зберігаються в надійних дата-центрах з сертифікацією ISO 27001 та SOC 2.</p>
                        </div>
                    </div>
                    
                    <div class="flex items-start mb-6">
                        <div class="bg-purple-100 p-3 rounded-full mr-4">
                            <i class="fas fa-user-shield text-purple-600 text-xl"></i>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold mb-2">Контроль доступу</h3>
                            <p class="text-gray-600">Детальні налаштування прав доступу для кожного користувача в вашій команді.</p>
                        </div>
                    </div>
                    
                    <div class="flex items-start">
                        <div class="bg-red-100 p-3 rounded-full mr-4">
                            <i class="fas fa-history text-red-600 text-xl"></i>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold mb-2">Резервне копіювання</h3>
                            <p class="text-gray-600">Автоматичне щоденне резервне копіювання всіх даних з можливістю відновлення на будь-яку дату.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section id="contact" class="py-16 bg-gradient-to-r from-blue-600 to-green-500 text-white px-4">
        <div class="container mx-auto">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold mb-4">Чекаємо Вас на консультації! </h2>
                <p class="text-xl max-w-3xl mx-auto">Раді кожному Вашому повідомленню</p>
            </div>
            
            <div class="flex flex-col items-center space-y-6">
                <div class="flex flex-wrap justify-center gap-6">
                    <a href="https://t.me/dessigka" target="_blank" class="bg-white text-blue-500 hover:bg-gray-100 font-bold py-4 px-8 rounded-lg shadow-lg transform transition-all duration-300 hover:scale-105 flex items-center">
                        <i class="fab fa-telegram fa-2x mr-3"></i>
                        <span>Telegram</span>
                    </a>
                    <a href="https://www.instagram.com/rockwel.capital?igsh=NnA4OGtzdmEzbmNx&utm_source=qr" target="_blank" class="bg-white text-pink-500 hover:bg-gray-100 font-bold py-4 px-8 rounded-lg shadow-lg transform transition-all duration-300 hover:scale-105 flex items-center">
                        <i class="fab fa-instagram fa-2x mr-3"></i>
                        <span>Instagram</span>
                    </a>
                    <a href="https://wa.me/380661176745?text=Привіт Михайле!" target="_blank" class="bg-white text-green-500 hover:bg-gray-100 font-bold py-4 px-8 rounded-lg shadow-lg transform transition-all duration-300 hover:scale-105 flex items-center">
                        <i class="fab fa-whatsapp fa-2x mr-3"></i>
                        <span>WhatsApp</span>
                    </a>
                </div>
                
                <div class="mt-8 text-center">
                    <p class="text-xl">Email: <a href="mailto:rockwellcapital1@gmail.com" class="underline hover:text-gray-200">rockwellcapital1@gmail.com</a></p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12 px-4">
        <div class="container mx-auto">
            <div class="grid md:grid-cols-4 gap-8">
                <div>
                    <div class="text-2xl font-bold text-white mb-4">Opti<span class="text-green-400">Mind</span></div>
                    <p class="text-gray-400 mb-4">Лідер у сфері AI-рішень для бізнесу з 2025 року.</p>
                    <div class="flex space-x-4">
                        
                       
                     
                    </div>
                </div>
                
                <div>
                    <h3 class="text-lg font-semibold mb-4">Продукт:Ші для бізнесу,створення власної моделі Ші </h3>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Функції:Автоматизація та оптимізація рутини!</a></li>
                        <li><a href="#pricing" class="text-gray-400 hover:text-white transition-colors">Ціни:Індивідуально</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors"></a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors"></a></li>
                    </ul>
                </div>
                
                <div>
                    <h3 class="text-lg font-semibold mb-4"></h3>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Про нас:Ми молода компанія що розвивається!Готові розглянути партнерство!</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors"></a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors"></a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Партнери:ФОП дзюбенко Микита Валерійович</a></li>
                    </ul>
                </div>
                
                <div>
                    <h3 class="text-lg font-semibold mb-4"></h3>
                    <ul class="space-y-2">
                        <li class="flex items-center">
                            <i class="fas fa-map-marker-alt text-gray-400 mr-2"></i>
                            <span class="text-gray-400">м. Київ,Україна</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-phone text-gray-400 mr-2"></i>
                            <span class="text-gray-400">+380 661176745</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-envelope text-gray-400 mr-2"></i>
                            <span class="text-gray-400">rockwellcapital1@gmail.com</span>
                        </li>
                    </ul>
                </div>
            </div>
            
            <div class="border-t border-gray-800 mt-12 pt-8 flex flex-col md:flex-row justify-between items-center">
                <p class="text-gray-400 mb-4 md:mb-0">© 2025 OptiMind. Усі права захищені.</p>
                <div class="flex space-x-6">
                    <a href="#privacy" class="text-gray-400 hover:text-white transition-colors">Політика конфіденційності</a>
                    <a href="#terms" class="text-gray-400 hover:text-white transition-colors">Умови використання</a>
                    <a href="#cookies" class="text-gray-400 hover:text-white transition-colors">Cookie</a>
                </div>
            </div>
        </div>
    </footer>

    <!-- Privacy Policy Modal -->
    <div id="privacy" class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center p-4 z-50 hidden">
        <div class="bg-white rounded-lg max-w-2xl w-full max-h-[80vh] overflow-y-auto">
            <div class="p-6">
                <h2 class="text-2xl font-bold mb-4">Політика конфіденційності</h2>
                <div class="space-y-4 text-gray-700">
                    <p>Останнє оновлення: 01.01.2025</p>
                    
                    <h3 class="font-bold">1. Збір інформації</h3>
                    <p>Ми збираємо інформацію, яку ви надаєте при реєстрації, заповненні форм або спілкуванні з нами. Це може включати ім'я, електронну пошту, телефон та інші контактні дані.</p>
                    
                    <h3 class="font-bold">2. Використання інформації</h3>
                    <p>Ваші дані використовуються для:</p>
                    <ul class="list-disc pl-5">
                        <li>Надання послуг та підтримки</li>
                        <li>Покращення якості наших продуктів</li>
                        <li>Комунікації з вами</li>
                        <li>Запобігання шахрайству</li>
                    </ul>
                    
                    <h3 class="font-bold">3. Захист даних</h3>
                    <p>Ми використовуємо стандартні засоби захисту для запобігання несанкціонованого доступу до ваших даних.</p>
                    
                    <h3 class="font-bold">4. Поширення даних</h3>
                    <p>Ми не продаємо та не передаємо ваші персональні дані третім особам без вашої згоди, за винятком випадків, передбачених законом.</p>
                </div>
                <button class="mt-6 bg-blue-600 text-white px-4 py-2 rounded hover:bg-blue-700 close-modal">Закрити</button>
            </div>
        </div>
    </div>

    <!-- Terms Modal -->
    <div id="terms" class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center p-4 z-50 hidden">
        <div class="bg-white rounded-lg max-w-2xl w-full max-h-[80vh] overflow-y-auto">
            <div class="p-6">
                <h2 class="text-2xl font-bold mb-4">Умови використання</h2>
                <div class="space-y-4 text-gray-700">
                    <p>Останнє оновлення: 01.01.2025</p>
                    
                    <h3 class="font-bold">1. Прийняття умов</h3>
                    <p>Використовуючи наші послуги, ви погоджуєтеся з цими умовами. Якщо ви не згодні, будь ласка, не використовуйте наші послуги.</p>
                    
                    <h3 class="font-bold">2. Інтелектуальна власність</h3>
                    <p>Усі матеріали на сайті, включаючи тексти, зображення, логотипи, є власністю OptiMind або її ліцензіарів.</p>
                    
                    <h3 class="font-bold">3. Обмеження відповідальності</h3>
                    <p>OptiMind не несе відповідальності за будь-які прямі, непрямі, випадкові збитки, пов'язані з використанням наших послуг.</p>
                    
                    <h3 class="font-bold">4. Зміни умов</h3>
                    <p>Ми залишаємо за собою право змінювати ці умови. Зміни набувають чинності після їх публікації на сайті.</p>
                </div>
                <button class="mt-6 bg-blue-600 text-white px-4 py-2 rounded hover:bg-blue-700 close-modal">Закрити</button>
            </div>
        </div>
    </div>

    <!-- Cookies Modal -->
    <div id="cookies" class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center p-4 z-50 hidden">
        <div class="bg-white rounded-lg max-w-2xl w-full max-h-[80vh] overflow-y-auto">
            <div class="p-6">
                <h2 class="text-2xl font-bold mb-4">Політика використання Cookie</h2>
                <div class="space-y-4 text-gray-700">
                    <p>Останнє оновлення: 01.01.2025</p>
                    
                    <h3 class="font-bold">1. Що таке cookie?</h3>
                    <p>Cookie - це невеликі текстові файли, які зберігаються на вашому пристрої при відвідуванні веб-сайтів.</p>
                    
                    <h3 class="font-bold">2. Як ми використовуємо cookie?</h3>
                    <p>Ми використовуємо cookie для:</p>
                    <ul class="list-disc pl-5">
                        <li>Забезпечення коректної роботи сайту</li>
                        <li>Аналізу відвідуваності</li>
                        <li>Персоналізації контенту</li>
                    </ul>
                    
                    <h3 class="font-bold">3. Управління cookie</h3>
                    <p>Ви можете керувати cookie через налаштування вашого браузера. Вимкнення cookie може вплинути на функціональність сайту.</p>
                    
                    <h3 class="font-bold">4. Види cookie</h3>
                    <p>Ми використовуємо:</p>
                    <ul class="list-disc pl-5">
                        <li>Необхідні cookie (для роботи сайту)</li>
                        <li>Аналітичні cookie (Google Analytics)</li>
                        <li>Функціональні cookie (для запам'ятовування налаштувань)</li>
                    </ul>
                </div>
                <button class="mt-6 bg-blue-600 text-white px-4 py-2 rounded hover:bg-blue-700 close-modal">Закрити</button>
            </div>
        </div>
    </div>

    <script>
        // Modal functionality
        document.querySelectorAll('[href="#privacy"], [href="#terms"], [href="#cookies"]').forEach(link => {
            link.addEventListener('click', function(e) {
                e.preventDefault();
                const modalId = this.getAttribute('href').substring(1);
                document.getElementById(modalId).classList.remove('hidden');
            });
        });

        document.querySelectorAll('.close-modal').forEach(button => {
            button.addEventListener('click', function() {
                this.closest('[id]').classList.add('hidden');
            });
        });

        document.querySelectorAll('[id="privacy"], [id="terms"], [id="cookies"]').forEach(modal => {
            modal.addEventListener('click', function(e) {
                if (e.target === this) {
                    this.classList.add('hidden');
                }
            });
        });

        // Mobile menu toggle
        document.getElementById('menu-btn').addEventListener('click', function() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        });

        // FAQ accordion
        const faqButtons = document.querySelectorAll('.faq-btn');
        faqButtons.forEach(button => {
            button.addEventListener('click', function() {
                const answer = this.nextElementSibling;
                const icon = this.querySelector('i');
                
                answer.classList.toggle('hidden');
                icon.classList.toggle('fa-chevron-down');
                icon.classList.toggle('fa-chevron-up');
            });
        });

        // Form submission
        document.getElementById('contact-form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('');
            this.reset();
        });

        // Sticky CTA button click
        document.getElementById('sticky-cta').addEventListener('click', function() {
            window.scrollTo({
                top: document.getElementById('contact').offsetTop - 100,
                behavior: 'smooth'
            });
        });

        // Animate progress bars on scroll
        function animateProgressBars() {
            const progressBars = document.querySelectorAll('.progress-fill');
            
            progressBars.forEach(bar => {
                const width = bar.style.width;
                bar.style.width = '0';
                
                setTimeout(() => {
                    bar.style.width = width;
                }, 100);
            });
        }

        // Run animation when page loads
        window.addEventListener('load', animateProgressBars);

        // Animate elements on scroll
        function animateOnScroll() {
            const elements = document.querySelectorAll('.feature-card, .testimonial-card');
            
            elements.forEach(element => {
                const elementPosition = element.getBoundingClientRect().top;
                const screenPosition = window.innerHeight / 1.3;
                
                if (elementPosition < screenPosition) {
                    element.style.opacity = "1";
                    element.style.transform = "translateY(0)";
                }
            });
        }

        // Set initial state for animated elements
        document.querySelectorAll('.feature-card, .testimonial-card').forEach(el => {
            el.style.opacity = "0";
            el.style.transform = "translateY(20px)";
            el.style.transition = "opacity 0.6s ease, transform 0.6s ease";
        });

        // Listen for scroll events
        window.addEventListener('scroll', animateOnScroll);
        window.addEventListener('load', animateOnScroll);
    </script>
</body>
</html>
