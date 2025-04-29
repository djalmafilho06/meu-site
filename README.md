# meu-site<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Matemática com Djalma | Aulas e Materiais</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        .hero-gradient {
            background: linear-gradient(135deg, #3b82f6 0%, #1d4ed8 100%);
        }
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
        }
        .floating {
            animation: floating 3s ease-in-out infinite;
        }
        @keyframes floating {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }
        .nav-link {
            position: relative;
        }
        .nav-link:after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: 0;
            left: 0;
            background-color: #3b82f6;
            transition: width 0.3s ease;
        }
        .nav-link:hover:after {
            width: 100%;
        }
    </style>
</head>
<body class="font-sans bg-gray-50">
    <!-- Header/Navbar -->
    <header class="bg-white shadow-md sticky top-0 z-50">
        <div class="container mx-auto px-4 py-3 flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <div class="bg-blue-500 text-white p-2 rounded-lg">
                    <i class="fas fa-square-root-alt text-2xl"></i>
                </div>
                <h1 class="text-xl font-bold text-gray-800">Matemática com <span class="text-blue-600">Djalma</span></h1>
            </div>
            <nav class="hidden md:flex space-x-8">
                <a href="#inicio" class="nav-link text-gray-700 hover:text-blue-600 font-medium">Início</a>
                <a href="#materiais" class="nav-link text-gray-700 hover:text-blue-600 font-medium">Materiais</a>
                <a href="#aulas" class="nav-link text-gray-700 hover:text-blue-600 font-medium">Aulas</a>
                <a href="#sobre" class="nav-link text-gray-700 hover:text-blue-600 font-medium">Sobre</a>
                <a href="#contato" class="nav-link text-gray-700 hover:text-blue-600 font-medium">Contato</a>
            </nav>
            <div class="md:hidden">
                <button id="menu-btn" class="text-gray-700 focus:outline-none">
                    <i class="fas fa-bars text-2xl"></i>
                </button>
            </div>
        </div>
        <!-- Mobile menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white py-2 px-4 shadow-lg">
            <a href="#inicio" class="block py-2 text-gray-700 hover:text-blue-600">Início</a>
            <a href="#materiais" class="block py-2 text-gray-700 hover:text-blue-600">Materiais</a>
            <a href="#aulas" class="block py-2 text-gray-700 hover:text-blue-600">Aulas</a>
            <a href="#sobre" class="block py-2 text-gray-700 hover:text-blue-600">Sobre</a>
            <a href="#contato" class="block py-2 text-gray-700 hover:text-blue-600">Contato</a>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="inicio" class="hero-gradient text-white py-20">
        <div class="container mx-auto px-4 flex flex-col md:flex-row items-center">
            <div class="md:w-1/2 mb-10 md:mb-0">
                <h1 class="text-4xl md:text-5xl font-bold mb-6">Domine a Matemática com o Prof. Djalma</h1>
                <p class="text-xl mb-8">Materiais didáticos e suporte personalizado para todos os níveis, do básico ao avançado.</p>
                <div class="flex flex-col sm:flex-row space-y-4 sm:space-y-0 sm:space-x-4">
                    <a href="#materiais" class="bg-white text-blue-600 font-bold py-3 px-6 rounded-lg hover:bg-gray-100 transition duration-300 text-center">Ver Materiais</a>
                    <a href="#contato" class="bg-transparent border-2 border-white text-white font-bold py-3 px-6 rounded-lg hover:bg-white hover:text-blue-600 transition duration-300 text-center">Agendar Aula</a>
                </div>
            </div>
            <div class="md:w-1/2 flex justify-center">
                <img src="https://images.unsplash.com/photo-1635070041078-e363dbe005cb?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=800&q=80" alt="Matemática" class="rounded-lg shadow-2xl w-full max-w-md floating">
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-12">Como Posso Te Ajudar?</h2>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div class="bg-gray-50 p-8 rounded-xl shadow-md hover:shadow-lg transition duration-300 card-hover">
                    <div class="bg-blue-100 text-blue-600 w-16 h-16 rounded-full flex items-center justify-center mb-6 mx-auto">
                        <i class="fas fa-book text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-center mb-4">Materiais Exclusivos</h3>
                    <p class="text-gray-600 text-center">Apostilas, resumos e exercícios cuidadosamente elaborados para cada nível de aprendizado.</p>
                </div>
                <div class="bg-gray-50 p-8 rounded-xl shadow-md hover:shadow-lg transition duration-300 card-hover">
                    <div class="bg-blue-100 text-blue-600 w-16 h-16 rounded-full flex items-center justify-center mb-6 mx-auto">
                        <i class="fas fa-video text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-center mb-4">Videoaulas</h3>
                    <p class="text-gray-600 text-center">Explicações claras e objetivas em formato de vídeo para você assistir quando e onde quiser.</p>
                </div>
                <div class="bg-gray-50 p-8 rounded-xl shadow-md hover:shadow-lg transition duration-300 card-hover">
                    <div class="bg-blue-100 text-blue-600 w-16 h-16 rounded-full flex items-center justify-center mb-6 mx-auto">
                        <i class="fas fa-chalkboard-teacher text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-center mb-4">Aulas Personalizadas</h3>
                    <p class="text-gray-600 text-center">Suporte individualizado para tirar dúvidas e aprofundar nos temas que você mais precisa.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Materials Section -->
    <section id="materiais" class="py-16 bg-gray-50">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-4">Materiais Disponíveis</h2>
            <p class="text-xl text-center text-gray-600 mb-12">Escolha o material ideal para o seu nível de aprendizado</p>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Material 1 -->
                <div class="bg-white rounded-xl shadow-md overflow-hidden card-hover transition duration-300">
                    <div class="h-48 bg-blue-500 flex items-center justify-center">
                        <i class="fas fa-calculator text-white text-6xl"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2">Matemática Básica</h3>
                        <p class="text-gray-600 mb-4">Apostila completa com operações fundamentais, frações, porcentagens e introdução à álgebra.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-2xl font-bold text-blue-600">R$ 49,90</span>
                            <button class="bg-blue-600 text-white py-2 px-4 rounded-lg hover:bg-blue-700 transition duration-300">Comprar</button>
                        </div>
                    </div>
                </div>
                
                <!-- Material 2 -->
                <div class="bg-white rounded-xl shadow-md overflow-hidden card-hover transition duration-300">
                    <div class="h-48 bg-green-500 flex items-center justify-center">
                        <i class="fas fa-function text-white text-6xl"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2">Álgebra e Funções</h3>
                        <p class="text-gray-600 mb-4">Pacote completo com videoaulas e exercícios sobre equações, funções e sistemas lineares.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-2xl font-bold text-green-600">R$ 79,90</span>
                            <button class="bg-green-600 text-white py-2 px-4 rounded-lg hover:bg-green-700 transition duration-300">Comprar</button>
                        </div>
                    </div>
                </div>
                
                <!-- Material 3 -->
                <div class="bg-white rounded-xl shadow-md overflow-hidden card-hover transition duration-300">
                    <div class="h-48 bg-purple-500 flex items-center justify-center">
                        <i class="fas fa-shapes text-white text-6xl"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2">Geometria e Trigonometria</h3>
                        <p class="text-gray-600 mb-4">Kit completo com apostila e 10 videoaulas sobre geometria plana, espacial e trigonometria.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-2xl font-bold text-purple-600">R$ 69,90</span>
                            <button class="bg-purple-600 text-white py-2 px-4 rounded-lg hover:bg-purple-700 transition duration-300">Comprar</button>
                        </div>
                    </div>
                </div>
                
                <!-- Material 4 -->
                <div class="bg-white rounded-xl shadow-md overflow-hidden card-hover transition duration-300">
                    <div class="h-48 bg-yellow-500 flex items-center justify-center">
                        <i class="fas fa-chart-line text-white text-6xl"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2">Cálculo Diferencial</h3>
                        <p class="text-gray-600 mb-4">Material avançado com limites, derivadas e aplicações, ideal para estudantes universitários.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-2xl font-bold text-yellow-600">R$ 89,90</span>
                            <button class="bg-yellow-600 text-white py-2 px-4 rounded-lg hover:bg-yellow-700 transition duration-300">Comprar</button>
                        </div>
                    </div>
                </div>
                
                <!-- Material 5 -->
                <div class="bg-white rounded-xl shadow-md overflow-hidden card-hover transition duration-300">
                    <div class="h-48 bg-red-500 flex items-center justify-center">
                        <i class="fas fa-infinity text-white text-6xl"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2">Matemática Avançada</h3>
                        <p class="text-gray-600 mb-4">Pacote completo com cálculo integral, séries, equações diferenciais e números complexos.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-2xl font-bold text-red-600">R$ 99,90</span>
                            <button class="bg-red-600 text-white py-2 px-4 rounded-lg hover:bg-red-700 transition duration-300">Comprar</button>
                        </div>
                    </div>
                </div>
                
                <!-- Material 6 -->
                <div class="bg-white rounded-xl shadow-md overflow-hidden card-hover transition duration-300">
                    <div class="h-48 bg-indigo-500 flex items-center justify-center">
                        <i class="fas fa-graduation-cap text-white text-6xl"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2">Pacote Completo</h3>
                        <p class="text-gray-600 mb-4">Todos os materiais com desconto especial + 2 horas de consultoria individual.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-2xl font-bold text-indigo-600">R$ 299,90</span>
                            <button class="bg-indigo-600 text-white py-2 px-4 rounded-lg hover:bg-indigo-700 transition duration-300">Comprar</button>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-12">
                <button class="bg-blue-600 text-white font-bold py-3 px-8 rounded-lg hover:bg-blue-700 transition duration-300 inline-flex items-center">
                    Ver Todos os Materiais <i class="fas fa-arrow-right ml-2"></i>
                </button>
            </div>
        </div>
    </section>

    <!-- Classes Section -->
    <section id="aulas" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-4">Modalidades de Aulas</h2>
            <p class="text-xl text-center text-gray-600 mb-12">Escolha a forma de aprendizado que melhor se adapta a você</p>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Aula 1 -->
                <div class="bg-gray-50 p-8 rounded-xl shadow-md hover:shadow-lg transition duration-300 card-hover">
                    <div class="bg-blue-100 text-blue-600 w-16 h-16 rounded-full flex items-center justify-center mb-6 mx-auto">
                        <i class="fas fa-user-graduate text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-center mb-4">Aulas Individuais</h3>
                    <p class="text-gray-600 text-center mb-6">Atenção personalizada com foco nas suas dificuldades específicas.</p>
                    <ul class="space-y-2 mb-6">
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> 1 hora de duração</li>
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Material complementar</li>
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Agendamento flexível</li>
                    </ul>
                    <div class="text-center">
                        <span class="text-2xl font-bold text-blue-600">R$ 120/hora</span>
                    </div>
                </div>
                
                <!-- Aula 2 -->
                <div class="bg-gray-50 p-8 rounded-xl shadow-md hover:shadow-lg transition duration-300 card-hover border-2 border-blue-500 transform scale-105">
                    <div class="bg-blue-500 text-white w-16 h-16 rounded-full flex items-center justify-center mb-6 mx-auto">
                        <i class="fas fa-users text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-center mb-4">Aulas em Grupo</h3>
                    <p class="text-gray-600 text-center mb-6">Aprendizado colaborativo com turmas pequenas e temas específicos.</p>
                    <ul class="space-y-2 mb-6">
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> 1h30 de duração</li>
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Turmas de até 5 alunos</li>
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Material incluso</li>
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Preço mais acessível</li>
                    </ul>
                    <div class="text-center">
                        <span class="text-2xl font-bold text-blue-600">R$ 80/hora</span>
                    </div>
                </div>
                
                <!-- Aula 3 -->
                <div class="bg-gray-50 p-8 rounded-xl shadow-md hover:shadow-lg transition duration-300 card-hover">
                    <div class="bg-blue-100 text-blue-600 w-16 h-16 rounded-full flex items-center justify-center mb-6 mx-auto">
                        <i class="fas fa-laptop text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-center mb-4">Pacote de Videoaulas</h3>
                    <p class="text-gray-600 text-center mb-6">Acesso ilimitado a todas as videoaulas gravadas.</p>
                    <ul class="space-y-2 mb-6">
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Mais de 50 horas de conteúdo</li>
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Exercícios resolvidos</li>
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Acesso vitalício</li>
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Atualizações periódicas</li>
                    </ul>
                    <div class="text-center">
                        <span class="text-2xl font-bold text-blue-600">R$ 399,90</span>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-12">
                <a href="#contato" class="bg-blue-600 text-white font-bold py-3 px-8 rounded-lg hover:bg-blue-700 transition duration-300 inline-flex items-center">
                    Agendar Aula Experimental <i class="fas fa-calendar-check ml-2"></i>
                </a>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="sobre" class="py-16 bg-gray-50">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/3 mb-8 md:mb-0 flex justify-center">
                    <div class="relative">
                        <div class="w-64 h-64 bg-blue-500 rounded-full overflow-hidden shadow-xl">
                            <img src="https://images.unsplash.com/photo-1573497019940-1c28c88b4f3e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=800&q=80" alt="Professor Djalma" class="w-full h-full object-cover">
                        </div>
                        <div class="absolute -bottom-5 -right-5 bg-white p-4 rounded-full shadow-lg">
                            <div class="bg-blue-500 text-white w-12 h-12 rounded-full flex items-center justify-center">
                                <i class="fas fa-award text-xl"></i>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="md:w-2/3 md:pl-12">
                    <h2 class="text-3xl font-bold text-gray-800 mb-6">Djalma Manoel do Nascimento Filho</h2>
                    <p class="text-gray-600 mb-4 text-lg">Mestre em Matemática pela Universidade Federal do Rio de Janeiro (UFRJ) com mais de 15 anos de experiência no ensino de matemática em todos os níveis.</p>
                    <p class="text-gray-600 mb-6 text-lg">Minha missão é descomplicar a matemática e mostrar como ela pode ser fascinante e acessível para todos.</p>
                    
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-8">
                        <div class="flex items-start">
                            <div class="bg-blue-100 text-blue-600 p-3 rounded-full mr-4">
                                <i class="fas fa-university"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-gray-800">Formação Acadêmica</h4>
                                <p class="text-gray-600">Mestrado em Matemática - UFRJ</p>
                                <p class="text-gray-600">Licenciatura em Matemática - UERJ</p>
                            </div>
                        </div>
                        <div class="flex items-start">
                            <div class="bg-blue-100 text-blue-600 p-3 rounded-full mr-4">
                                <i class="fas fa-briefcase"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-gray-800">Experiência</h4>
                                <p class="text-gray-600">Professor Universitário - 8 anos</p>
                                <p class="text-gray-600">Professor de Ensino Médio - 7 anos</p>
                            </div>
                        </div>
                        <div class="flex items-start">
                            <div class="bg-blue-100 text-blue-600 p-3 rounded-full mr-4">
                                <i class="fas fa-star"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-gray-800">Especialidades</h4>
                                <p class="text-gray-600">Cálculo Diferencial e Integral</p>
                                <p class="text-gray-600">Álgebra Linear</p>
                                <p class="text-gray-600">Matemática Financeira</p>
                            </div>
                        </div>
                        <div class="flex items-start">
                            <div class="bg-blue-100 text-blue-600 p-3 rounded-full mr-4">
                                <i class="fas fa-trophy"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-gray-800">Conquistas</h4>
                                <p class="text-gray-600">Prêmio Melhor Professor - 2018</p>
                                <p class="text-gray-600">Autor de 3 livros didáticos</p>
                            </div>
                        </div>
                    </div>
                    
                    <div class="flex flex-wrap gap-4">
                        <a href="#" class="bg-blue-600 text-white px-6 py-2 rounded-full hover:bg-blue-700 transition duration-300 inline-flex items-center">
                            <i class="fab fa-linkedin-in mr-2"></i> LinkedIn
                        </a>
                        <a href="#" class="bg-gray-800 text-white px-6 py-2 rounded-full hover:bg-gray-900 transition duration-300 inline-flex items-center">
                            <i class="fab fa-github mr-2"></i> GitHub
                        </a>
                        <a href="#" class="bg-green-600 text-white px-6 py-2 rounded-full hover:bg-green-700 transition duration-300 inline-flex items-center">
                            <i class="fas fa-book-open mr-2"></i> Publicações
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-12">O Que Dizem Meus Alunos</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Depoimento 1 -->
                <div class="bg-gray-50 p-8 rounded-xl shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 bg-blue-500 rounded-full overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/women/32.jpg" alt="Aluna" class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-bold">Ana Carolina</h4>
                            <div class="flex text-yellow-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                            </div>
                        </div>
                    </div>
                    <p class="text-gray-600 italic">"Nunca imaginei que entenderia cálculo tão facilmente. As explicações do professor Djalma são claras e ele tem uma paciência incrível para tirar dúvidas."</p>
                </div>
                
                <!-- Depoimento 2 -->
                <div class="bg-gray-50 p-8 rounded-xl shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 bg-blue-500 rounded-full overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/men/45.jpg" alt="Aluno" class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-bold">Ricardo Almeida</h4>
                            <div class="flex text-yellow-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                            </div>
                        </div>
                    </div>
                    <p class="text-gray-600 italic">"Comprei o pacote de videoaulas e foi a melhor decisão que tomei. Consigo estudar no meu ritmo e o material é excelente. Recomendo muito!"</p>
                </div>
                
                <!-- Depoimento 3 -->
                <div class="bg-gray-50 p-8 rounded-xl shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 bg-blue-500 rounded-full overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/women/68.jpg" alt="Aluna" class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-bold">Juliana Santos</h4>
                            <div class="flex text-yellow-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star-half-alt"></i>
                            </div>
                        </div>
                    </div>
                    <p class="text-gray-600 italic">"As aulas em grupo são ótimas! O professor consegue dar atenção individual mesmo em turmas pequenas. Minhas notas melhoraram muito desde que comecei."</p>
                </div>
            </div>
            
            <div class="text-center mt-12">
                <button class="bg-blue-600 text-white font-bold py-3 px-8 rounded-lg hover:bg-blue-700 transition duration-300 inline-flex items-center">
                    Ver Mais Depoimentos <i class="fas fa-comments ml-2"></i>
                </button>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contato" class="py-16 bg-gray-50">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-4">Entre em Contato</h2>
            <p class="text-xl text-center text-gray-600 mb-12">Tire suas dúvidas ou agende uma aula experimental</p>
            
            <div class="flex flex-col md:flex-row">
                <div class="md:w-1/2 mb-8 md:mb-0 md:pr-8">
                    <form class="bg-white p-8 rounded-xl shadow-md">
                        <div class="mb-6">
                            <label for="name" class="block text-gray-700 font-medium mb-2">Nome Completo</label>
                            <input type="text" id="name" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500">
                        </div>
                        <div class="mb-6">
                            <label for="email" class="block text-gray-700 font-medium mb-2">E-mail</label>
                            <input type="email" id="email" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500">
                        </div>
                        <div class="mb-6">
                            <label for="subject" class="block text-gray-700 font-medium mb-2">Assunto</label>
                            <select id="subject" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500">
                                <option value="">Selecione...</option>
                                <option value="aulas">Aulas Particulares</option>
                                <option value="material">Dúvidas sobre Materiais</option>
                                <option value="outro">Outro Assunto</option>
                            </select>
                        </div>
                        <div class="mb-6">
                            <label for="message" class="block text-gray-700 font-medium mb-2">Mensagem</label>
                            <textarea id="message" rows="4" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500"></textarea>
                        </div>
                        <button type="submit" class="w-full bg-blue-600 text-white font-bold py-3 px-6 rounded-lg hover:bg-blue-700 transition duration-300">Enviar Mensagem</button>
                    </form>
                </div>
                
                <div class="md:w-1/2 md:pl-8">
                    <div class="bg-white p-8 rounded-xl shadow-md h-full">
                        <h3 class="text-xl font-bold text-gray-800 mb-6">Outras Formas de Contato</h3>
                        
                        <div class="space-y-6">
                            <div class="flex items-start">
                                <div class="bg-blue-100 text-blue-600 p-3 rounded-full mr-4">
                                    <i class="fas fa-envelope"></i>
                                </div>
                                <div>
                                    <h4 class="font-bold text-gray-800">E-mail</h4>
                                    <p class="text-gray-600">contato@djalmanatematica.com.br</p>
                                </div>
                            </div>
                            
                            <div class="flex items-start">
                                <div class="bg-blue-100 text-blue-600 p-3 rounded-full mr-4">
                                    <i class="fas fa-phone-alt"></i>
                                </div>
                                <div>
                                    <h4 class="font-bold text-gray-800">Telefone/WhatsApp</h4>
                                    <p class="text-gray-600">(21) 98765-4321</p>
                                </div>
                            </div>
                            
                            <div class="flex items-start">
                                <div class="bg-blue-100 text-blue-600 p-3 rounded-full mr-4">
                                    <i class="fas fa-map-marker-alt"></i>
                                </div>
                                <div>
                                    <h4 class="font-bold text-gray-800">Endereço</h4>
                                    <p class="text-gray-600">Rua da Matemática, 123 - Sala 3.14<br>Rio de Janeiro - RJ</p>
                                </div>
                            </div>
                            
                            <div class="flex items-start">
                                <div class="bg-blue-100 text-blue-600 p-3 rounded-full mr-4">
                                    <i class="fas fa-clock"></i>
                                </div>
                                <div>
                                    <h4 class="font-bold text-gray-800">Horário de Atendimento</h4>
                                    <p class="text-gray-600">Segunda a Sexta: 9h às 18h<br>Sábado: 9h às 12h</p>
                                </div>
                            </div>
                        </div>
                        
                        <div class="mt-8">
                            <h4 class="font-bold text-gray-800 mb-4">Redes Sociais</h4>
                            <div class="flex space-x-4">
                                <a href="#" class="bg-blue-600 text-white w-10 h-10 rounded-full flex items-center justify-center hover:bg-blue-700 transition duration-300">
                                    <i class="fab fa-facebook-f"></i>
                                </a>
                                <a href="#" class="bg-blue-400 text-white w-10 h-10 rounded-full flex items-center justify-center hover:bg-blue-500 transition duration-300">
                                    <i class="fab fa-twitter"></i>
                                </a>
                                <a href="#" class="bg-pink-600 text-white w-10 h-10 rounded-full flex items-center justify-center hover:bg-pink-700 transition duration-300">
                                    <i class="fab fa-instagram"></i>
                                </a>
                                <a href="#" class="bg-red-600 text-white w-10 h-10 rounded-full flex items-center justify-center hover:bg-red-700 transition duration-300">
                                    <i class="fab fa-youtube"></i>
                                </a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- FAQ Section -->
    <section class="py-16 bg-white">
        <div class="container mx-auto px-4 max-w-4xl">
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-12">Perguntas Frequentes</h2>
            
            <div class="space-y-4">
                <!-- Pergunta 1 -->
                <div class="border border-gray-200 rounded-lg overflow-hidden">
                    <button class="faq-btn w-full flex justify-between items-center p-6 bg-gray-50 hover:bg-gray-100 transition duration-300">
                        <h3 class="text-lg font-medium text-left text-gray-800">Como faço para adquirir os materiais?</h3>
                        <i class="fas fa-chevron-down text-blue-600 transition-transform duration-300"></i>
                    </button>
                    <div class="faq-content hidden px-6 pb-6 pt-2">
                        <p class="text-gray-600">Você pode adquirir os materiais diretamente pelo site, clicando no botão "Comprar" de cada produto. Após a confirmação do pagamento, você receberá um e-mail com os materiais em formato digital (PDF para apostilas e links para videoaulas). Para materiais físicos, informaremos o prazo de entrega.</p>
                    </div>
                </div>
                
                <!-- Pergunta 2 -->
                <div class="border border-gray-200 rounded-lg overflow-hidden">
                    <button class="faq-btn w-full flex justify-between items-center p-6 bg-gray-50 hover:bg-gray-100 transition duration-300">
                        <h3 class="text-lg font-medium text-left text-gray-800">Qual a diferença entre as aulas individuais e em grupo?</h3>
                        <i class="fas fa-chevron-down text-blue-600 transition-transform duration-300"></i>
                    </button>
                    <div class="faq-content hidden px-6 pb-6 pt-2">
                        <p class="text-gray-600">As aulas individuais são totalmente personalizadas, focadas nas suas necessidades específicas, com horários flexíveis. Já as aulas em grupo têm um programa definido, são mais econômicas e permitem a interação com outros alunos. Ambas incluem material de apoio, mas nas individuais o ritmo e conteúdo são totalmente adaptados a você.</p>
                    </div>
                </div>
                
                <!-- Pergunta 3 -->
                <div class="border border-gray-200 rounded-lg overflow-hidden">
                    <button class="faq-btn w-full flex justify-between items-center p-6 bg-gray-50 hover:bg-gray-100 transition duration-300">
                        <h3 class="text-lg font-medium text-left text-gray-800">Os materiais têm garantia?</h3>
                        <i class="fas fa-chevron-down text-blue-600 transition-transform duration-300"></i>
                    </button>
                    <div class="faq-content hidden px-6 pb-6 pt-2">
                        <p class="text-gray-600">Sim, todos os materiais têm garantia de 7 dias. Se você não ficar satisfeito com o conteúdo, basta nos enviar um e-mail dentro desse prazo que devolveremos 100% do valor pago, sem questionamentos.</p>
                    </div>
                </div>
                
                <!-- Pergunta 4 -->
                <div class="border border-gray-200 rounded-lg overflow-hidden">
                    <button class="faq-btn w-full flex justify-between items-center p-6 bg-gray-50 hover:bg-gray-100 transition duration-300">
                        <h3 class="text-lg font-medium text-left text-gray-800">Como funcionam as aulas online?</h3>
                        <i class="fas fa-chevron-down text-blue-600 transition-transform duration-300"></i>
                    </button>
                    <div class="faq-content hidden px-6 pb-6 pt-2">
                        <p class="text-gray-600">As aulas online são realizadas por plataformas como Zoom ou Google Meet. Você receberá um link de acesso após o agendamento. Recomendamos ter uma boa conexão de internet, microfone e webcam (opcional). Todas as aulas são gravadas (com sua permissão) e disponibilizadas para você revisar depois.</p>
                    </div>
                </div>
                
                <!-- Pergunta 5 -->
                <div class="border border-gray-200 rounded-lg overflow-hidden">
                    <button class="faq-btn w-full flex justify-between items-center p-6 bg-gray-50 hover:bg-gray-100 transition duration-300">
                        <h3 class="text-lg font-medium text-left text-gray-800">Posso parcelar os valores?</h3>
                        <i class="fas fa-chevron-down text-blue-600 transition-transform duration-300"></i>
                    </button>
                    <div class="faq-content hidden px-6 pb-6 pt-2">
                        <p class="text-gray-600">Sim, aceitamos pagamentos parcelados em até 12x no cartão de crédito para materiais e pacotes de aulas. Para aulas avulsas, o pagamento é feito por transferência bancária ou PIX antes de cada aula.</p>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-12">
                <p class="text-gray-600 mb-4">Não encontrou sua dúvida aqui?</p>
                <a href="#contato" class="bg-blue-600 text-white font-bold py-3 px-8 rounded-lg hover:bg-blue-700 transition duration-300 inline-flex items-center">
                    Entre em Contato <i class="fas fa-envelope ml-2"></i>
                </a>
            </div>
        </div>
    </section>

    <!-- Newsletter Section -->
    <section class="py-16 bg-blue-600 text-white">
        <div class="container mx-auto px-4 text-center">
            <h2 class="text-3xl font-bold mb-4">Receba Materiais Gratuitos!</h2>
            <p class="text-xl mb-8 max-w-2xl mx-auto">Cadastre-se para receber conteúdos exclusivos, dicas de estudo e promoções especiais diretamente no seu e-mail.</p>
            
            <form class="max-w-md mx-auto flex flex-col sm:flex-row gap-4">
                <input type="email" placeholder="Seu melhor e-mail" class="flex-grow px-4 py-3 rounded-lg focus:outline-none text-gray-800">
                <button type="submit" class="bg-white text-blue-600 font-bold py-3 px-6 rounded-lg hover:bg-gray-100 transition duration-300">Cadastrar</button>
            </form>
            
            <p class="mt-4 text-sm opacity-80">Não enviaremos spam. Você pode cancelar sua inscrição a qualquer momento.</p>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <div>
                    <div class="flex items-center space-x-2 mb-4">
                        <div class="bg-blue-500 text-white p-2 rounded-lg">
                            <i class="fas fa-square-root-alt text-xl"></i>
                        </div>
                        <h3 class="text-xl font-bold">Matemática com Djalma</h3>
                    </div>
                    <p class="text-gray-400">Transformando a maneira como você aprende matemática, do básico ao avançado.</p>
                </div>
                
                <div>
                    <h4 class="text-lg font-bold mb-4">Links Rápidos</h4>
                    <ul class="space-y-2">
                        <li><a href="#inicio" class="text-gray-400 hover:text-white transition duration-300">Início</a></li>
                        <li><a href="#materiais" class="text-gray-400 hover:text-white transition duration-300">Materiais</a></li>
                        <li><a href="#aulas" class="text-gray-400 hover:text-white transition duration-300">Aulas</a></li>
                        <li><a href="#sobre" class="text-gray-400 hover:text-white transition duration-300">Sobre</a></li>
                        <li><a href="#contato" class="text-gray-400 hover:text-white transition duration-300">Contato</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="text-lg font-bold mb-4">Materiais</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Matemática Básica</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Álgebra</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Geometria</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Cálculo</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Pacote Completo</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="text-lg font-bold mb-4">Contato</h4>
                    <ul class="space-y-2">
                        <li class="flex items-center">
                            <i class="fas fa-envelope mr-2 text-gray-400"></i>
                            <span>contato@djalmanatematica.com.br</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-phone-alt mr-2 text-gray-400"></i>
                            <span>(21) 98765-4321</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-map-marker-alt mr-2 text-gray-400"></i>
                            <span>Rio de Janeiro - RJ</span>
                        </li>
                    </ul>
                    <div class="flex space-x-4 mt-4">
                        <a href="#" class="bg-gray-700 text-white w-10 h-10 rounded-full flex items-center justify-center hover:bg-blue-600 transition duration-300">
                            <i class="fab fa-facebook-f"></i>
                        </a>
                        <a href="#" class="bg-gray-700 text-white w-10 h-10 rounded-full flex items-center justify-center hover:bg-blue-400 transition duration-300">
                            <i class="fab fa-twitter"></i>
                        </a>
                        <a href="#" class="bg-gray-700 text-white w-10 h-10 rounded-full flex items-center justify-center hover:bg-pink-600 transition duration-300">
                            <i class="fab fa-instagram"></i>
                        </a>
                        <a href="#" class="bg-gray-700 text-white w-10 h-10 rounded-full flex items-center justify-center hover:bg-red-600 transition duration-300">
                            <i class="fab fa-youtube"></i>
                        </a>
                    </div>
                </div>
            </div>
            
            <div class="border-t border-gray-800 mt-12 pt-8 flex flex-col md:flex-row justify-between items-center">
                <p class="text-gray-400 mb-4 md:mb-0">© 2023 Matemática com Djalma. Todos os direitos reservados.</p>
                <div class="flex space-x-6">
                    <a href="#" class="text-gray-400 hover:text-white transition duration-300">Termos de Uso</a>
                    <a href="#" class="text-gray-400 hover:text-white transition duration-300">Política de Privacidade</a>
                </div>
            </div>
        </div>
    </footer>

    <!-- Back to Top Button -->
    <button id="back-to-top" class="fixed bottom-8 right-8 bg-blue-600 text-white w-12 h-12 rounded-full flex items-center justify-center shadow-lg hover:bg-blue-700 transition duration-300 hidden">
        <i class="fas fa-arrow-up"></i>
    </button>

    <script>
        // Mobile menu toggle
        const menuBtn = document.getElementById('menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        
        menuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });
        
        // FAQ accordion
        const faqBtns = document.querySelectorAll('.faq-btn');
        
        faqBtns.forEach(btn => {
            btn.addEventListener('click', () => {
                const content = btn.nextElementSibling;
                const icon = btn.querySelector('i');
                
                // Close all other open FAQs
                document.querySelectorAll('.faq-content').forEach(item => {
                    if (item !== content && !item.classList.contains('hidden')) {
                        item.classList.add('hidden');
                        const otherIcon = item.previousElementSibling.querySelector('i');
                        otherIcon.classList.remove('fa-chevron-up');
                        otherIcon.classList.add('fa-chevron-down');
                    }
                });
                
                // Toggle current FAQ
                content.classList.toggle('hidden');
                
                // Toggle icon
                icon.classList.toggle('fa-chevron-down');
                icon.classList.toggle('fa-chevron-up');
            });
        });
        
        // Back to top button
        const backToTopBtn = document.getElementById('back-to-top');
        
        window.addEventListener('scroll', () => {
            if (window.pageYOffset > 300) {
                backToTopBtn.classList.remove('hidden');
            } else {
                backToTopBtn.classList.add('hidden');
            }
        });
        
        backToTopBtn.addEventListener('click', () => {
            window.scrollTo({
                top: 0,
                behavior: 'smooth'
            });
        });
        
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                    
                    // Close mobile menu if open
                    if (!mobileMenu.classList.contains('hidden')) {
                        mobileMenu.classList.add('hidden');
                    }
                }
            });
        });
    </script>
</body>
</html>
