
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Magno do Dario São José da Varginha</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* Custom CSS for elements that need more specific styling */
        .video-container {
            position: relative;
            padding-bottom: 56.25%;
            height: 0;
            overflow: hidden;
        }
        .video-container iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }
        .tab-content {
            display: none;
        }
        .tab-content.active {
            display: block;
            animation: fadeIn 0.5s;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        .mobile-menu {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease-out;
        }
        .mobile-menu.open {
            max-height: 500px;
        }
    </style>
</head>
<body class="bg-gray-50 font-sans">
    <!-- Header with Navigation -->
    <header class="bg-blue-800 text-white shadow-lg">
        <div class="container mx-auto px-4 py-4">
            <div class="flex justify-between items-center">
                <div class="flex items-center space-x-4">
                    <div class="bg-white p-2 rounded-full">
                        <i class="fas fa-landmark text-blue-800 text-2xl"></i>
                    </div>
                    <div>
                        <h1 class="text-xl md:text-2xl font-bold">Magno Do Dario</h1>
                        <p class="text-sm">Vereador de São José da Varginha</p>
                    </div>
                </div>
                
                <!-- Desktop Navigation -->
                <nav class="hidden md:block">
                    <ul class="flex space-x-6">
                        <li><a href="#" class="nav-link active" data-tab="home">Início</a></li>
                        <li><a href="#" class="nav-link" data-tab="about">Sobre</a></li>
                        <li><a href="#" class="nav-link" data-tab="projects">Projetos</a></li>
                        <li><a href="#" class="nav-link" data-tab="news">Notícias</a></li>
                        <li><a href="#" class="nav-link" data-tab="meetings">Reuniões</a></li>
                        <li><a href="#" class="nav-link" data-tab="contact">Contato</a></li>
                    </ul>
                </nav>
                
                <!-- Mobile menu button -->
                <button id="mobile-menu-button" class="md:hidden text-white focus:outline-none">
                    <i class="fas fa-bars text-2xl"></i>
                </button>
            </div>
            
            <!-- Mobile Navigation -->
            <div id="mobile-menu" class="mobile-menu md:hidden mt-2">
                <ul class="py-2 space-y-2">
                    <li><a href="#" class="block px-4 py-2 nav-link active" data-tab="home">Início</a></li>
                    <li><a href="#" class="block px-4 py-2 nav-link" data-tab="about">Sobre</a></li>
                    <li><a href="#" class="block px-4 py-2 nav-link" data-tab="projects">Projetos</a></li>
                    <li><a href="#" class="block px-4 py-2 nav-link" data-tab="news">Notícias</a></li>
                    <li><a href="#" class="block px-4 py-2 nav-link" data-tab="meetings">Reuniões</a></li>
                    <li><a href="#" class="block px-4 py-2 nav-link" data-tab="contact">Contato</a></li>
                </ul>
            </div>
        </div>
    </header>

    <!-- Main Content -->
    <main class="container mx-auto px-4 py-8">
        <!-- Home Tab -->
        <div id="home" class="tab-content active">
            <section class="mb-12">
                <div class="bg-blue-700 text-white rounded-lg p-6 md:p-8 shadow-lg">
                    <div class="flex flex-col md:flex-row items-center">
                        <div class="md:w-1/3 mb-6 md:mb-0">
                            <img src="https://via.placeholder.com/300x400" alt="Foto do Vereador" class="rounded-lg shadow-md w-full max-w-xs mx-auto">
                        </div>
                        <div class="md:w-2/3 md:pl-8">
                            <h2 class="text-2xl md:text-3xl font-bold mb-4">João Magno de Almeida</h2>
                            <p class="mb-4 text-lg">Trabalhando por São José da Varginha</p>
                            <p class="mb-6">Mandato pautado pela transparência, compromisso com a população e trabalho constante por uma cidade melhor. A atuação no Legislativo Municipal é guiada pela escuta das demandas da comunidade e pela busca de soluções reais nas áreas da saúde, educação, infraestrutura e inclusão social. Com diálogo, responsabilidade e presença ativa no dia a dia do povo, seguimos firmes na construção de um futuro mais justo e digno para todos.</p>
                            <div class="flex space-x-4">
                                <a href="#" class="bg-white text-blue-700 px-6 py-2 rounded-lg font-semibold hover:bg-gray-100 transition">Conheça meus projetos</a>
                                <a href="#" class="border-2 border-white text-white px-6 py-2 rounded-lg font-semibold hover:bg-blue-600 transition">Entre em contato</a>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <section class="mb-12">
                <h2 class="text-2xl font-bold mb-6 text-blue-800 border-b pb-2">Destaques</h2>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                    <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition">
                        <img src="https://via.placeholder.com/400x250" alt="Destaque 1" class="w-full">
                        <div class="p-4">
                            <h3 class="font-bold text-lg mb-2">Projeto de Lei Aprovado</h3>
                            <p class="text-gray-600 mb-4">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam in dui mauris.</p>
                            <a href="#" class="text-blue-600 font-semibold hover:underline">Saiba mais</a>
                        </div>
                    </div>
                    <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition">
                        <img src="https://via.placeholder.com/400x250" alt="Destaque 2" class="w-full">
                        <div class="p-4">
                            <h3 class="font-bold text-lg mb-2">Visita à Comunidade</h3>
                            <p class="text-gray-600 mb-4">Vivamus hendrerit arcu sed erat molestie vehicula. Sed auctor neque eu tellus rhoncus.</p>
                            <a href="#" class="text-blue-600 font-semibold hover:underline">Saiba mais</a>
                        </div>
                    </div>
                    <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition">
                        <img src="https://via.placeholder.com/400x250" alt="Destaque 3" class="w-full">
                        <div class="p-4">
                            <h3 class="font-bold text-lg mb-2">Próximas Audiências</h3>
                            <p class="text-gray-600 mb-4">Ut eleifend nibh porttitor. Nullam in dui mauris. Vivamus hendrerit arcu sed erat.</p>
                            <a href="#" class="text-blue-600 font-semibold hover:underline">Saiba mais</a>
                        </div>
                    </div>
                </div>
            </section>

            <section class="mb-12">
                <h2 class="text-2xl font-bold mb-6 text-blue-800 border-b pb-2">Últimas Notícias</h2>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                    <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition">
                        <img src="https://via.placeholder.com/600x300" alt="Notícia 1" class="w-full">
                        <div class="p-4">
                            <div class="flex justify-between items-center mb-2">
                                <span class="text-sm text-gray-500">10/06/2023</span>
                                <span class="bg-blue-100 text-blue-800 text-xs px-2 py-1 rounded">Câmara Municipal</span>
                            </div>
                            <h3 class="font-bold text-xl mb-2">Título da Notícia Importante</h3>
                            <p class="text-gray-600 mb-4">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam in dui mauris. Vivamus hendrerit arcu sed erat molestie vehicula. Sed auctor neque eu tellus rhoncus ut eleifend nibh porttitor.</p>
                            <a href="#" class="text-blue-600 font-semibold hover:underline">Ler notícia completa</a>
                        </div>
                    </div>
                    <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition">
                        <img src="https://via.placeholder.com/600x300" alt="Notícia 2" class="w-full">
                        <div class="p-4">
                            <div class="flex justify-between items-center mb-2">
                                <span class="text-sm text-gray-500">05/06/2023</span>
                                <span class="bg-green-100 text-green-800 text-xs px-2 py-1 rounded">Comunidade</span>
                            </div>
                            <h3 class="font-bold text-xl mb-2">Outra Notícia Relevante</h3>
                            <p class="text-gray-600 mb-4">Vivamus hendrerit arcu sed erat molestie vehicula. Sed auctor neque eu tellus rhoncus ut eleifend nibh porttitor. Nullam in dui mauris. Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                            <a href="#" class="text-blue-600 font-semibold hover:underline">Ler notícia completa</a>
                        </div>
                    </div>
                </div>
                <div class="text-center mt-6">
                    <a href="#" class="inline-block bg-blue-700 text-white px-6 py-2 rounded-lg font-semibold hover:bg-blue-800 transition">Ver todas as notícias</a>
                </div>
            </section>
        </div>

        <!-- About Tab -->
        <div id="about" class="tab-content">
            <section class="mb-12">
                <h2 class="text-2xl font-bold mb-6 text-blue-800 border-b pb-2">Sobre o Vereador</h2>
                <div class="flex flex-col md:flex-row">
                    <div class="md:w-1/3 mb-6 md:mb-0 md:pr-6">
                        <img src="https://via.placeholder.com/400x500" alt="Foto do Vereador" class="rounded-lg shadow-md w-full">
                    </div>
                    <div class="md:w-2/3">
                        <h3 class="text-xl font-bold mb-4">[Nome Completo do Vereador]</h3>
                        <p class="mb-4">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam in dui mauris. Vivamus hendrerit arcu sed erat molestie vehicula. Sed auctor neque eu tellus rhoncus ut eleifend nibh porttitor. Ut in nulla enim. Phasellus molestie magna non est bibendum non venenatis nisl tempor.</p>
                        <p class="mb-4">Suspendisse eget ligula. Aliquam erat volutpat. Donec quis nibh at felis congue commodo. Etiam auctor fringilla ante. Phasellus ligula dolor, viverra eget, tincidunt eget, varius ac, justo.</p>
                        
                        <h4 class="font-bold text-lg mt-6 mb-3">Formação Acadêmica</h4>
                        <ul class="list-disc pl-5 mb-6 space-y-2">
                            <li>Graduação em Direito - Universidade Federal</li>
                            <li>Pós-graduação em Gestão Pública - Faculdade XYZ</li>
                            <li>Curso de Especialização em Políticas Sociais</li>
                        </ul>
                        
                        <h4 class="font-bold text-lg mt-6 mb-3">Experiência Profissional</h4>
                        <ul class="list-disc pl-5 mb-6 space-y-2">
                            <li>Advogado - 10 anos de experiência</li>
                            <li>Consultor em Gestão Pública - 5 anos</li>
                            <li>Vereador - 2 mandatos</li>
                        </ul>
                        
                        <h4 class="font-bold text-lg mt-6 mb-3">Principais Bandearas</h4>
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                            <div class="flex items-start">
                                <div class="bg-blue-100 p-2 rounded-full mr-3">
                                    <i class="fas fa-home text-blue-700"></i>
                                </div>
                                <div>
                                    <h5 class="font-semibold">Moradia Popular</h5>
                                    <p class="text-sm text-gray-600">Defesa de políticas habitacionais</p>
                                </div>
                            </div>
                            <div class="flex items-start">
                                <div class="bg-green-100 p-2 rounded-full mr-3">
                                    <i class="fas fa-heartbeat text-green-700"></i>
                                </div>
                                <div>
                                    <h5 class="font-semibold">Saúde Pública</h5>
                                    <p class="text-sm text-gray-600">Melhoria dos serviços de saúde</p>
                                </div>
                            </div>
                            <div class="flex items-start">
                                <div class="bg-yellow-100 p-2 rounded-full mr-3">
                                    <i class="fas fa-graduation-cap text-yellow-700"></i>
                                </div>
                                <div>
                                    <h5 class="font-semibold">Educação</h5>
                                    <p class="text-sm text-gray-600">Valorização dos professores</p>
                                </div>
                            </div>
                            <div class="flex items-start">
                                <div class="bg-red-100 p-2 rounded-full mr-3">
                                    <i class="fas fa-briefcase text-red-700"></i>
                                </div>
                                <div>
                                    <h5 class="font-semibold">Geração de Empregos</h5>
                                    <p class="text-sm text-gray-600">Incentivo ao empreendedorismo</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
            
            <section class="mb-12">
                <h2 class="text-2xl font-bold mb-6 text-blue-800 border-b pb-2">Histórico Político</h2>
                <div class="relative">
                    <!-- Timeline -->
                    <div class="border-l-2 border-blue-500 absolute h-full left-4 md:left-1/2"></div>
                    
                    <!-- Timeline items -->
                    <div class="mb-8">
                        <div class="flex flex-col md:flex-row items-center md:justify-between">
                            <div class="md:w-5/12 md:text-right md:pr-8 mb-4 md:mb-0">
                                <h3 class="font-bold text-lg">Primeiro Mandato</h3>
                                <p class="text-gray-600">2017 - 2020</p>
                            </div>
                            <div class="w-8 h-8 bg-blue-500 rounded-full z-10 flex-shrink-0"></div>
                            <div class="md:w-5/12 md:pl-8 mt-4 md:mt-0">
                                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam in dui mauris. Vivamus hendrerit arcu sed erat molestie vehicula.</p>
                            </div>
                        </div>
                    </div>
                    
                    <div class="mb-8">
                        <div class="flex flex-col md:flex-row items-center md:justify-between">
                            <div class="md:w-5/12 md:text-right md:pr-8 mb-4 md:mb-0">
                                <h3 class="font-bold text-lg">Reeleição</h3>
                                <p class="text-gray-600">2021 - 2024</p>
                            </div>
                            <div class="w-8 h-8 bg-blue-500 rounded-full z-10 flex-shrink-0"></div>
                            <div class="md:w-5/12 md:pl-8 mt-4 md:mt-0">
                                <p>Sed auctor neque eu tellus rhoncus ut eleifend nibh porttitor. Ut in nulla enim. Phasellus molestie magna non est bibendum non venenatis nisl tempor.</p>
                            </div>
                        </div>
                    </div>
                    
                    <div class="mb-8">
                        <div class="flex flex-col md:flex-row items-center md:justify-between">
                            <div class="md:w-5/12 md:text-right md:pr-8 mb-4 md:mb-0">
                                <h3 class="font-bold text-lg">Principais Conquistas</h3>
                                <p class="text-gray-600">2017 - Presente</p>
                            </div>
                            <div class="w-8 h-8 bg-blue-500 rounded-full z-10 flex-shrink-0"></div>
                            <div class="md:w-5/12 md:pl-8 mt-4 md:mt-0">
                                <ul class="list-disc pl-5 space-y-2">
                                    <li>Aprovação do Plano Diretor Municipal</li>
                                    <li>Criação do Programa de Moradia Popular</li>
                                    <li>Reforma das Escolas Municipais</li>
                                    <li>Ampliação do Posto de Saúde Central</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
        </div>

        <!-- Projects Tab -->
        <div id="projects" class="tab-content">
            <section class="mb-12">
                <h2 class="text-2xl font-bold mb-6 text-blue-800 border-b pb-2">Projetos em Andamento</h2>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                    <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition">
                        <div class="p-4">
                            <div class="flex justify-between items-center mb-2">
                                <span class="bg-blue-100 text-blue-800 text-xs px-2 py-1 rounded">Infraestrutura</span>
                                <span class="text-sm text-gray-500">Em tramitação</span>
                            </div>
                            <h3 class="font-bold text-xl mb-2">PL 123/2023 - Reforma das Vias Públicas</h3>
                            <p class="text-gray-600 mb-4">Projeto de lei que prevê a reforma e manutenção das principais vias públicas do município, com foco na acessibilidade e segurança viária.</p>
                            <div class="flex justify-between items-center">
                                <span class="text-sm text-gray-500">Data de entrada: 15/03/2023</span>
                                <a href="#" class="text-blue-600 font-semibold hover:underline">Detalhes</a>
                            </div>
                        </div>
                    </div>
                    <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition">
                        <div class="p-4">
                            <div class="flex justify-between items-center mb-2">
                                <span class="bg-green-100 text-green-800 text-xs px-2 py-1 rounded">Educação</span>
                                <span class="text-sm text-gray-500">Em tramitação</span>
                            </div>
                            <h3 class="font-bold text-xl mb-2">PL 156/2023 - Merenda Escolar de Qualidade</h3>
                            <p class="text-gray-600 mb-4">Projeto que estabelece diretrizes para a melhoria da qualidade nutricional da merenda escolar nas escolas municipais.</p>
                            <div class="flex justify-between items-center">
                                <span class="text-sm text-gray-500">Data de entrada: 02/05/2023</span>
                                <a href="#" class="text-blue-600 font-semibold hover:underline">Detalhes</a>
                            </div>
                        </div>
                    </div>
                    <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition">
                        <div class="p-4">
                            <div class="flex justify-between items-center mb-2">
                                <span class="bg-yellow-100 text-yellow-800 text-xs px-2 py-1 rounded">Saúde</span>
                                <span class="text-sm text-gray-500">Em tramitação</span>
                            </div>
                            <h3 class="font-bold text-xl mb-2">PL 178/2023 - Ampliação do Posto de Saúde</h3>
                            <p class="text-gray-600 mb-4">Proposta de ampliação do Posto de Saúde Central, com a criação de novas especialidades e aumento do horário de atendimento.</p>
                            <div class="flex justify-between items-center">
                                <span class="text-sm text-gray-500">Data de entrada: 10/06/2023</span>
                                <a href="#" class="text-blue-600 font-semibold hover:underline">Detalhes</a>
                            </div>
                        </div>
                    </div>
                    <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition">
                        <div class="p-4">
                            <div class="flex justify-between items-center mb-2">
                                <span class="bg-red-100 text-red-800 text-xs px-2 py-1 rounded">Assistência Social</span>
                                <span class="text-sm text-gray-500">Em tramitação</span>
                            </div>
                            <h3 class="font-bold text-xl mb-2">PL 201/2023 - Programa de Moradia Popular</h3>
                            <p class="text-gray-600 mb-4">Criação de programa municipal de moradia popular com subsídios para famílias de baixa renda.</p>
                            <div class="flex justify-between items-center">
                                <span class="text-sm text-gray-500">Data de entrada: 22/06/2023</span>
                                <a href="#" class="text-blue-600 font-semibold hover:underline">Detalhes</a>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
            
            <section class="mb-12">
                <h2 class="text-2xl font-bold mb-6 text-blue-800 border-b pb-2">Projetos Aprovados</h2>
                <div class="overflow-x-auto">
                    <table class="min-w-full bg-white rounded-lg overflow-hidden">
                        <thead class="bg-gray-100">
                            <tr>
                                <th class="py-3 px-4 text-left">Número</th>
                                <th class="py-3 px-4 text-left">Título</th>
                                <th class="py-3 px-4 text-left">Área</th>
                                <th class="py-3 px-4 text-left">Data</th>
                                <th class="py-3 px-4 text-left">Status</th>
                            </tr>
                        </thead>
                        <tbody class="divide-y divide-gray-200">
                            <tr class="hover:bg-gray-50">
                                <td class="py-3 px-4">PL 45/2022</td>
                                <td class="py-3 px-4">Reforma da Praça Central</td>
                                <td class="py-3 px-4">Urbanismo</td>
                                <td class="py-3 px-4">10/11/2022</td>
                                <td class="py-3 px-4"><span class="bg-green-100 text-green-800 px-2 py-1 rounded text-xs">Aprovado</span></td>
                            </tr>
                            <tr class="hover:bg-gray-50">
                                <td class="py-3 px-4">PL 78/2022</td>
                                <td class="py-3 px-4">Programa de Coleta Seletiva</td>
                                <td class="py-3 px-4">Meio Ambiente</td>
                                <td class="py-3 px-4">05/09/2022</td>
                                <td class="py-3 px-4"><span class="bg-green-100 text-green-800 px-2 py-1 rounded text-xs">Aprovado</span></td>
                            </tr>
                            <tr class="hover:bg-gray-50">
                                <td class="py-3 px-4">PL 112/2021</td>
                                <td class="py-3 px-4">Incentivo ao Esporte Juvenil</td>
                                <td class="py-3 px-4">Esporte</td>
                                <td class="py-3 px-4">15/07/2021</td>
                                <td class="py-3 px-4"><span class="bg-green-100 text-green-800 px-2 py-1 rounded text-xs">Aprovado</span></td>
                            </tr>
                            <tr class="hover:bg-gray-50">
                                <td class="py-3 px-4">PL 89/2021</td>
                                <td class="py-3 px-4">Criação da Feira do Produtor</td>
                                <td class="py-3 px-4">Economia</td>
                                <td class="py-3 px-4">22/05/2021</td>
                                <td class="py-3 px-4"><span class="bg-green-100 text-green-800 px-2 py-1 rounded text-xs">Aprovado</span></td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </section>
            
            <section class="mb-12">
                <h2 class="text-2xl font-bold mb-6 text-blue-800 border-b pb-2">Projetos Rejeitados</h2>
                <div class="bg-white rounded-lg shadow-md overflow-hidden">
                    <div class="p-4">
                        <div class="flex justify-between items-center mb-2">
                            <span class="bg-blue-100 text-blue-800 text-xs px-2 py-1 rounded">Infraestrutura</span>
                            <span class="text-sm text-gray-500">Rejeitado em 10/03/2023</span>
                        </div>
                        <h3 class="font-bold text-xl mb-2">PL 101/2022 - Ampliação do Estacionamento Municipal</h3>
                        <p class="text-gray-600 mb-4">Projeto que previa a ampliação do estacionamento público central com construção de novo pavimento.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-sm text-gray-500">Votos: 8 a favor, 12 contra</span>
                            <a href="#" class="text-blue-600 font-semibold hover:underline">Detalhes da votação</a>
                        </div>
                    </div>
                </div>
            </section>
        </div>

        <!-- News Tab -->
        <div id="news" class="tab-content">
            <section class="mb-12">
                <h2 class="text-2xl font-bold mb-6 text-blue-800 border-b pb-2">Últimas Notícias</h2>
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                    <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition">
                        <img src="https://via.placeholder.com/400x250" alt="Notícia 1" class="w-full">
                        <div class="p-4">
                            <div class="flex justify-between items-center mb-2">
                                <span class="text-sm text-gray-500">10/06/2023</span>
                                <span class="bg-blue-100 text-blue-800 text-xs px-2 py-1 rounded">Câmara</span>
                            </div>
                            <h3 class="font-bold text-xl mb-2">Vereador apresenta projeto para reforma de escolas</h3>
                            <p class="text-gray-600 mb-4">O vereador [Nome] apresentou na sessão desta semana projeto que prevê a reforma de todas as escolas municipais...</p>
                            <a href="#" class="text-blue-600 font-semibold hover:underline">Ler mais</a>
                        </div>
                    </div>
                    <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition">
                        <img src="https://via.placeholder.com/400x250" alt="Notícia 2" class="w-full">
                        <div class="p-4">
                            <div class="flex justify-between items-center mb-2">
                                <span class="text-sm text-gray-500">05/06/2023</span>
                                <span class="bg-green-100 text-green-800 text-xs px-2 py-1 rounded">Comunidade</span>
                            </div>
                            <h3 class="font-bold text-xl mb-2">Visita ao bairro Jardim das Flores</h3>
                            <p class="text-gray-600 mb-4">O vereador [Nome] esteve nesta segunda-feira no bairro Jardim das Flores para ouvir as demandas da comunidade...</p>
                            <a href="#" class="text-blue-600 font-semibold hover:underline">Ler mais</a>
                        </div>
                    </div>
                    <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition">
                        <img src="https://via.placeholder.com/400x250" alt="Notícia 3" class="w-full">
                        <div class="p-4">
                            <div class="flex justify-between items-center mb-2">
                                <span class="text-sm text-gray-500">01/06/2023</span>
                                <span class="bg-yellow-100 text-yellow-800 text-xs px-2 py-1 rounded">Saúde</span>
                            </div>
                            <h3 class="font-bold text-xl mb-2">Debate sobre ampliação do posto de saúde</h3>
                            <p class="text-gray-600 mb-4">Foi realizado na Câmara Municipal um debate sobre a necessidade de ampliação do posto de saúde central...</p>
                            <a href="#" class="text-blue-600 font-semibold hover:underline">Ler mais</a>
                        </div>
                    </div>
                    <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition">
                        <img src="https://via.placeholder.com/400x250" alt="Notícia 4" class="w-full">
                        <div class="p-4">
                            <div class="flex justify-between items-center mb-2">
                                <span class="text-sm text-gray-500">28/05/2023</span>
                                <span class="bg-red-100 text-red-800 text-xs px-2 py-1 rounded">Eventos</span>
                            </div>
                            <h3 class="font-bold text-xl mb-2">Participação na Feira do Empreendedor</h3>
                            <p class="text-gray-600 mb-4">O vereador [Nome] participou como palestrante da 5ª Feira do Empreendedor de São José da Varginha...</p>
                            <a href="#" class="text-blue-600 font-semibold hover:underline">Ler mais</a>
                        </div>
                    </div>
                    <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition">
                        <img src="https://via.placeholder.com/400x250" alt="Notícia 5" class="w-full">
                        <div class="p-4">
                            <div class="flex justify-between items-center mb-2">
                                <span class="text-sm text-gray-500">22/05/2023</span>
                                <span class="bg-purple-100 text-purple-800 text-xs px-2 py-1 rounded">Educação</span>
                            </div>
                            <h3 class="font-bold text-xl mb-2">Entrega de kits escolares</h3>
                            <p class="text-gray-600 mb-4">O vereador [Nome] participou da entrega de kits escolares para crianças carentes do município...</p>
                            <a href="#" class="text-blue-600 font-semibold hover:underline">Ler mais</a>
                        </div>
                    </div>
                    <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition">
                        <img src="https://via.placeholder.com/400x250" alt="Notícia 6" class="w-full">
                        <div class="p-4">
                            <div class="flex justify-between items-center mb-2">
                                <span class="text-sm text-gray-500">15/05/2023</span>
                                <span class="bg-blue-100 text-blue-800 text-xs px-2 py-1 rounded">Legislativo</span>
                            </div>
                            <h3 class="font-bold text-xl mb-2">Sessão solene homenageia professores</h3>
                            <p class="text-gray-600 mb-4">A Câmara Municipal realizou sessão solene para homenagear professores destaque do município...</p>
                            <a href="#" class="text-blue-600 font-semibold hover:underline">Ler mais</a>
                        </div>
                    </div>
                </div>
                
                <div class="mt-8 flex justify-center">
                    <nav class="inline-flex rounded-md shadow">
                        <a href="#" class="px-4 py-2 rounded-l-md border border-gray-300 bg-white text-blue-700 font-medium hover:bg-gray-50">Anterior</a>
                        <a href="#" class="px-4 py-2 border-t border-b border-gray-300 bg-white text-blue-700 font-medium hover:bg-gray-50">1</a>
                        <a href="#" class="px-4 py-2 border-t border-b border-gray-300 bg-blue-700 text-white font-medium">2</a>
                        <a href="#" class="px-4 py-2 border-t border-b border-gray-300 bg-white text-blue-700 font-medium hover:bg-gray-50">3</a>
                        <a href="#" class="px-4 py-2 rounded-r-md border border-gray-300 bg-white text-blue-700 font-medium hover:bg-gray-50">Próxima</a>
                    </nav>
                </div>
            </section>
            
            <section class="mb-12">
                <h2 class="text-2xl font-bold mb-6 text-blue-800 border-b pb-2">Galeria de Fotos</h2>
                <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4">
                    <a href="#" class="group">
                        <img src="https://via.placeholder.com/300x200" alt="Foto 1" class="w-full h-40 object-cover rounded-lg group-hover:opacity-75 transition">
                    </a>
                    <a href="#" class="group">
                        <img src="https://via.placeholder.com/300x200" alt="Foto 2" class="w-full h-40 object-cover rounded-lg group-hover:opacity-75 transition">
                    </a>
                    <a href="#" class="group">
                        <img src="https://via.placeholder.com/300x200" alt="Foto 3" class="w-full h-40 object-cover rounded-lg group-hover:opacity-75 transition">
                    </a>
                    <a href="#" class="group">
                        <img src="https://via.placeholder.com/300x200" alt="Foto 4" class="w-full h-40 object-cover rounded-lg group-hover:opacity-75 transition">
                    </a>
                    <a href="#" class="group">
                        <img src="https://via.placeholder.com/300x200" alt="Foto 5" class="w-full h-40 object-cover rounded-lg group-hover:opacity-75 transition">
                    </a>
                    <a href="#" class="group">
                        <img src="https://via.placeholder.com/300x200" alt="Foto 6" class="w-full h-40 object-cover rounded-lg group-hover:opacity-75 transition">
                    </a>
                    <a href="#" class="group">
                        <img src="https://via.placeholder.com/300x200" alt="Foto 7" class="w-full h-40 object-cover rounded-lg group-hover:opacity-75 transition">
                    </a>
                    <a href="#" class="group">
                        <img src="https://via.placeholder.com/300x200" alt="Foto 8" class="w-full h-40 object-cover rounded-lg group-hover:opacity-75 transition">
                    </a>
                </div>
            </section>
        </div>

        <!-- Meetings Tab -->
        <div id="meetings" class="tab-content">
            <section class="mb-12">
                <h2 class="text-2xl font-bold mb-6 text-blue-800 border-b pb-2">Reuniões Transmitidas</h2>
                
                <div class="mb-8">
                    <h3 class="text-xl font-bold mb-4">Última Sessão</h3>
                    <div class="video-container rounded-lg shadow-lg">
                        <!-- Replace with actual YouTube embed code -->
                        <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>
                    <div class="mt-4">
                        <h4 class="font-bold text-lg">Sessão Ordinária - 12/06/2023</h4>
                        <p class="text-gray-600 mt-2">Transmissão da sessão ordinária da Câmara Municipal de São José da Varginha realizada em 12 de junho de 2023.</p>
                        <div class="mt-4">
                            <a href="#" class="inline-block bg-blue-700 text-white px-4 py-2 rounded hover:bg-blue-800">Ver pauta completa</a>
                        </div>
                    </div>
                </div>
                
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                    <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition">
                        <div class="video-container">
                            <!-- Replace with actual YouTube embed code -->
                            <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                        </div>
                        <div class="p-4">
                            <h4 class="font-bold">Sessão Ordinária - 05/06/2023</h4>
                            <p class="text-sm text-gray-600 mt-1">Duração: 2h 45min</p>
                            <div class="mt-3">
                                <a href="#" class="text-blue-600 text-sm font-semibold hover:underline">Assistir completo</a>
                            </div>
                        </div>
                    </div>
                    <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition">
                        <div class="video-container">
                            <!-- Replace with actual YouTube embed code -->
                            <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                        </div>
                        <div class="p-4">
                            <h4 class="font-bold">Sessão Extraordinária - 29/05/2023</h4>
                            <p class="text-sm text-gray-600 mt-1">Duração: 1h 30min</p>
                            <div class="mt-3">
                                <a href="#" class="text-blue-600 text-sm font-semibold hover:underline">Assistir completo</a>
                            </div>
                        </div>
                    </div>
                    <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition">
                        <div class="video-container">
                            <!-- Replace with actual YouTube embed code -->
                            <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                        </div>
                        <div class="p-4">
                            <h4 class="font-bold">Sessão Ordinária - 22/05/2023</h4>
                            <p class="text-sm text-gray-600 mt-1">Duração: 3h 15min</p>
                            <div class="mt-3">
                                <a href="#" class="text-blue-600 text-sm font-semibold hover:underline">Assistir completo</a>
                            </div>
                        </div>
                    </div>
                    <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition">
                        <div class="video-container">
                            <!-- Replace with actual YouTube embed code -->
                            <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                        </div>
                        <div class="p-4">
                            <h4 class="font-bold">Audiência Pública - 15/05/2023</h4>
                            <p class="text-sm text-gray-600 mt-1">Duração: 4h 20min</p>
                            <div class="mt-3">
                                <a href="#" class="text-blue-600 text-sm font-semibold hover:underline">Assistir completo</a>
                            </div>
                        </div>
                    </div>
                    <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition">
                        <div class="video-container">
                            <!-- Replace with actual YouTube embed code -->
                            <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                        </div>
                        <div class="p-4">
                            <h4 class="font-bold">Sessão Ordinária - 08/05/2023</h4>
                            <p class="text-sm text-gray-600 mt-1">Duração: 2h 50min</p>
                            <div class="mt-3">
                                <a href="#" class="text-blue-600 text-sm font-semibold hover:underline">Assistir completo</a>
                            </div>
                        </div>
                    </div>
                    <div class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition">
                        <div class="video-container">
                            <!-- Replace with actual YouTube embed code -->
                            <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                        </div>
                        <div class="p-4">
                            <h4 class="font-bold">Sessão Solene - 01/05/2023</h4>
                            <p class="text-sm text-gray-600 mt-1">Duração: 1h 40min</p>
                            <div class="mt-3">
                                <a href="#" class="text-blue-600 text-sm font-semibold hover:underline">Assistir completo</a>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="mt-8 text-center">
                    <a href="#" class="inline-block bg-blue-700 text-white px-6 py-3 rounded-lg font-semibold hover:bg-blue-800 transition">Ver mais reuniões</a>
                </div>
            </section>
            
            <section class="mb-12">
                <h2 class="text-2xl font-bold mb-6 text-blue-800 border-b pb-2">Próximas Reuniões</h2>
                <div class="bg-white rounded-lg shadow-md overflow-hidden">
                    <div class="divide-y divide-gray-200">
                        <div class="p-4 hover:bg-gray-50 transition">
                            <div class="flex flex-col md:flex-row md:items-center md:justify-between">
                                <div>
                                    <h3 class="font-bold text-lg">Sessão Ordinária</h3>
                                    <p class="text-gray-600">Pauta: Discussão do PL 123/2023 e PL 156/2023</p>
                                </div>
                                <div class="mt-2 md:mt-0">
                                    <div class="flex items-center">
                                        <i class="fas fa-calendar-day text-blue-700 mr-2"></i>
                                        <span class="font-semibold">19/06/2023</span>
                                        <i class="fas fa-clock text-blue-700 ml-4 mr-2"></i>
                                        <span class="font-semibold">19:00h</span>
                                    </div>
                                    <div class="mt-2">
                                        <span class="bg-blue-100 text-blue-800 px-2 py-1 rounded text-xs">Presencial e Online</span>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="p-4 hover:bg-gray-50 transition">
                            <div class="flex flex-col md:flex-row md:items-center md:justify-between">
                                <div>
                                    <h3 class="font-bold text-lg">Audiência Pública</h3>
                                    <p class="text-gray-600">Plano Diretor Municipal - Revisão 2023</p>
                                </div>
                                <div class="mt-2 md:mt-0">
                                    <div class="flex items-center">
                                        <i class="fas fa-calendar-day text-blue-700 mr-2"></i>
                                        <span class="font-semibold">26/06/2023</span>
                                        <i class="fas fa-clock text-blue-700 ml-4 mr-2"></i>
                                        <span class="font-semibold">14:00h</span>
                                    </div>
                                    <div class="mt-2">
                                        <span class="bg-green-100 text-green-800 px-2 py-1 rounded text-xs">Câmara Municipal</span>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="p-4 hover:bg-gray-50 transition">
                            <div class="flex flex-col md:flex-row md:items-center md:justify-between">
                                <div>
                                    <h3 class="font-bold text-lg">Sessão Extraordinária</h3>
                                    <p class="text-gray-600">Votação de vetos do Executivo</p>
                                </div>
                                <div class="mt-2 md:mt-0">
                                    <div class="flex items-center">
                                        <i class="fas fa-calendar-day text-blue-700 mr-2"></i>
                                        <span class="font-semibold">03/07/2023</span>
                                        <i class="fas fa-clock text-blue-700 ml-4 mr-2"></i>
                                        <span class="font-semibold">09:00h</span>
                                    </div>
                                    <div class="mt-2">
                                        <span class="bg-blue-100 text-blue-800 px-2 py-1 rounded text-xs">Presencial e Online</span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
            
            <section>
                <h2 class="text-2xl font-bold mb-6 text-blue-800 border-b pb-2">Canal Oficial no YouTube</h2>
                <div class="bg-white rounded-lg shadow-md p-6">
                    <div class="flex flex-col md:flex-row items-center">
                        <div class="md:w-1/3 mb-6 md:mb-0">
                            <img src="https://via.placeholder.com/300x200" alt="YouTube Channel" class="rounded-lg shadow-md w-full">
                        </div>
                        <div class="md:w-2/3 md:pl-8">
                            <h3 class="text-xl font-bold mb-2">Câmara Municipal de São José da Varginha</h3>
                            <p class="text-gray-600 mb-4">Acompanhe todas as sessões, audiências e eventos oficiais da Câmara Municipal através do nosso canal no YouTube.</p>
                            <div class="flex items-center">
                                <i class="fab fa-youtube text-red-600 text-2xl mr-3"></i>
                                <a href="#" class="text-blue-600 font-semibold hover:underline">Acessar Canal</a>
                            </div>
                            <div class="mt-4 flex flex-wrap gap-2">
                                <span class="bg-gray-100 text-gray-800 px-3 py-1 rounded-full text-sm">+500 inscritos</span>
                                <span class="bg-gray-100 text-gray-800 px-3 py-1 rounded-full text-sm">150 vídeos</span>
                                <span class="bg-gray-100 text-gray-800 px-3 py-1 rounded-full text-sm">Notificações ativadas</span>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
        </div>

        <!-- Contact Tab -->
        <div id="contact" class="tab-content">
            <section class="mb-12">
                <h2 class="text-2xl font-bold mb-6 text-blue-800 border-b pb-2">Entre em Contato</h2>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                    <div>
                        <h3 class="text-xl font-bold mb-4">Envie sua mensagem</h3>
                        <form class="space-y-4">
                            <div>
                                <label for="name" class="block text-gray-700 mb-1">Nome completo</label>
                                <input type="text" id="name" class="w-full px-4 py-2 border border-gray-300 rounded focus:outline-none focus:ring-2 focus:ring-blue-500">
                            </div>
                            <div>
                                <label for="email" class="block text-gray-700 mb-1">E-mail</label>
                                <input type="email" id="email" class="w-full px-4 py-2 border border-gray-300 rounded focus:outline-none focus:ring-2 focus:ring-blue-500">
                            </div>
                            <div>
                                <label for="phone" class="block text-gray-700 mb-1">Telefone</label>
                                <input type="tel" id="phone" class="w-full px-4 py-2 border border-gray-300 rounded focus:outline-none focus:ring-2 focus:ring-blue-500">
                            </div>
                            <div>
                                <label for="subject" class="block text-gray-700 mb-1">Assunto</label>
                                <select id="subject" class="w-full px-4 py-2 border border-gray-300 rounded focus:outline-none focus:ring-2 focus:ring-blue-500">
                                    <option value="">Selecione um assunto</option>
                                    <option value="suggestion">Sugestão</option>
                                    <option value="complaint">Reclamação</option>
                                    <option value="request">Solicitação</option>
                                    <option value="other">Outro</option>
                                </select>
                            </div>
                            <div>
                                <label for="message" class="block text-gray-700 mb-1">Mensagem</label>
                                <textarea id="message" rows="5" class="w-full px-4 py-2 border border-gray-300 rounded focus:outline-none focus:ring-2 focus:ring-blue-500"></textarea>
                            </div>
                            <div>
                                <button type="submit" class="bg-blue-700 text-white px-6 py-2 rounded font-semibold hover:bg-blue-800 transition">Enviar mensagem</button>
                            </div>
                        </form>
                    </div>
                    
                    <div>
                        <h3 class="text-xl font-bold mb-4">Informações de Contato</h3>
                        <div class="bg-white rounded-lg shadow-md p-6">
                            <div class="space-y-6">
                                <div class="flex items-start">
                                    <div class="bg-blue-100 p-3 rounded-full mr-4">
                                        <i class="fas fa-map-marker-alt text-blue-700"></i>
                                    </div>
                                    <div>
                                        <h4 class="font-bold text-lg mb-1">Endereço</h4>
                                        <p class="text-gray-600">Câmara Municipal de São José da Varginha<br>Praça da Matriz, 123 - Centro<br>São José da Varginha - MG</p>
                                    </div>
                                </div>
                                
                                <div class="flex items-start">
                                    <div class="bg-green-100 p-3 rounded-full mr-4">
                                        <i class="fas fa-phone-alt text-green-700"></i>
                                    </div>
                                    <div>
                                        <h4 class="font-bold text-lg mb-1">Telefones</h4>
                                        <p class="text-gray-600">
                                            Gabinete: (35) 1234-5678<br>
                                            Assessoria: (35) 9876-5432<br>
                                            Fax: (35) 1234-5678
                                        </p>
                                    </div>
                                </div>
                                
                                <div class="flex items-start">
                                    <div class="bg-yellow-100 p-3 rounded-full mr-4">
                                        <i class="fas fa-envelope text-yellow-700"></i>
                                    </div>
                                    <div>
                                        <h4 class="font-bold text-lg mb-1">E-mails</h4>
                                        <p class="text-gray-600">
                                            Gabinete: gabinete@vereador.com.br<br>
                                            Assessoria: assessoria@vereador.com.br<br>
                                            Imprensa: imprensa@vereador.com.br
                                        </p>
                                    </div>
                                </div>
                                
                                <div class="flex items-start">
                                    <div class="bg-red-100 p-3 rounded-full mr-4">
                                        <i class="fas fa-clock text-red-700"></i>
                                    </div>
                                    <div>
                                        <h4 class="font-bold text-lg mb-1">Atendimento</h4>
                                        <p class="text-gray-600">
                                            Segunda a Sexta: 08:00 - 18:00<br>
                                            Sábado: 08:00 - 12:00
                                        </p>
                                    </div>
                                </div>
                            </div>
                            
                            <div class="mt-8">
                                <h4 class="font-bold text-lg mb-3">Redes Sociais</h4>
                                <div class="flex space-x-4">
                                    <a href="#" class="bg-blue-600 text-white p-3 rounded-full hover:bg-blue-700 transition">
                                        <i class="fab fa-facebook-f"></i>
                                    </a>
                                    <a href="#" class="bg-blue-400 text-white p-3 rounded-full hover:bg-blue-500 transition">
                                        <i class="fab fa-twitter"></i>
                                    </a>
                                    <a href="#" class="bg-pink-600 text-white p-3 rounded-full hover:bg-pink-700 transition">
                                        <i class="fab fa-instagram"></i>
                                    </a>
                                    <a href="#" class="bg-red-600 text-white p-3 rounded-full hover:bg-red-700 transition">
                                        <i class="fab fa-youtube"></i>
                                    </a>
                                    <a href="#" class="bg-green-600 text-white p-3 rounded-full hover:bg-green-700 transition">
                                        <i class="fab fa-whatsapp"></i>
                                    </a>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
            
            <section>
                <h2 class="text-2xl font-bold mb-6 text-blue-800 border-b pb-2">Localização</h2>
                <div class="bg-white rounded-lg shadow-md overflow-hidden">
                    <!-- Replace with actual Google Maps embed code -->
                    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d12345.678901234567!2d-46.12345678901234!3d-23.123456789012345!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zMjPCsDA3JzI0LjQiUyA0NsKwMDcnMjQuNCJX!5e0!3m2!1sen!2sbr!4v1234567890123!5m2!1sen!2sbr" width="100%" height="450" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
                </div>
            </section>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-8">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <div>
                    <h3 class="text-xl font-bold mb-4">Vereador</h3>
                    <p class="mb-4">Trabalhando por São José da Varginha</p>
                    <div class="flex space-x-4">
                        <a href="#" class="text-gray-400 hover:text-white transition"><i class="fab fa-facebook-f"></i></a>
                        <a href="#" class="text-gray-400 hover:text-white transition"><i class="fab fa-twitter"></i></a>
                        <a href="#" class="text-gray-400 hover:text-white transition"><i class="fab fa-instagram"></i></a>
                        <a href="#" class="text-gray-400 hover:text-white transition"><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                <div>
                    <h3 class="text-xl font-bold mb-4">Links Úteis</h3>
                    <ul class="space-y-2">
                        <li><a href="#" class="hover:text-blue-300 transition">Câmara Municipal</a></li>
                        <li><a href="#" class="hover:text-blue-300 transition">Prefeitura Municipal</a></li>
                        <li><a href="#" class="hover:text-blue-300 transition">Legislação Municipal</a></li>
                        <li><a href="#" class="hover:text-blue-300 transition">Transparência</a></li>
                        <li><a href="#" class="hover:text-blue-300 transition">Ouvidoria</a></li>
                    </ul>
                </div>
                <div>
                    <h3 class="text-xl font-bold mb-4">Atendimento</h3>
                    <ul class="space-y-2">
                        <li class="flex items-start">
                            <i class="fas fa-map-marker-alt mt-1 mr-2 text-blue-300"></i>
                            <span>Praça da Matriz, 123 - Centro</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-phone-alt mt-1 mr-2 text-blue-300"></i>
                            <span>(35) 1234-5678</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-envelope mt-1 mr-2 text-blue-300"></i>
                            <span>contato@vereador.com.br</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-clock mt-1 mr-2 text-blue-300"></i>
                            <span>Seg-Sex: 08:00 - 18:00</span>
                        </li>
                    </ul>
                </div>
                <div>
                    <h3 class="text-xl font-bold mb-4">Newsletter</h3>
                    <p class="mb-4">Receba nossas atualizações por e-mail</p>
                    <form class="flex">
                        <input type="email" placeholder="Seu e-mail" class="px-4 py-2 rounded-l text-gray-800 w-full focus:outline-none">
                        <button type="submit" class="bg-blue-700 px-4 py-2 rounded-r hover:bg-blue-800 transition">
                            <i class="fas fa-paper-plane"></i>
                        </button>
                    </form>
                </div>
            </div>
            <div class="border-t border-gray-700 mt-8 pt-6 text-center text-gray-400">
                <p>&copy; 2023 Vereador de São José da Varginha. Todos os direitos reservados.</p>
                <p class="mt-2">Desenvolvido com <i class="fas fa-heart text-red-400"></i> para a comunidade</p>
            </div>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        document.getElementById('mobile-menu-button').addEventListener('click', function() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('open');
        });

        // Tab functionality
        const navLinks = document.querySelectorAll('.nav-link');
        
        navLinks.forEach(link => {
            link.addEventListener('click', function(e) {
                e.preventDefault();
                
                // Remove active class from all links
                navLinks.forEach(l => l.classList.remove('active'));
                
                // Add active class to clicked link
                this.classList.add('active');
                
                // Hide all tab contents
                const tabContents = document.querySelectorAll('.tab-content');
                tabContents.forEach(content => content.classList.remove('active'));
                
                // Show the selected tab content
                const tabId = this.getAttribute('data-tab');
                document.getElementById(tabId).classList.add('active');
                
                // Close mobile menu if open
                const mobileMenu = document.getElementById('mobile-menu');
                if (mobileMenu.classList.contains('open')) {
                    mobileMenu.classList.remove('open');
                }
                
                // Scroll to top
                window.scrollTo(0, 0);
            });
        });

        // Form submission (example)
        const contactForm = document.querySelector('form');
        if (contactForm) {
            contactForm.addEventListener('submit', function(e) {
                e.preventDefault();
                alert('Mensagem enviada com sucesso! Entraremos em contato em breve.');
                this.reset();
            });
        }
    </script>
</body>
</html>
Adicionando index.html
