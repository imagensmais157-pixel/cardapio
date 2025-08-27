<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cardápios Profissionais - Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
        body { font-family: 'Poppins', sans-serif; }
        .gradient-bg { background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); }
        .card-hover { transition: transform 0.3s ease, box-shadow 0.3s ease; }
        .card-hover:hover { transform: translateY(-10px); box-shadow: 0 20px 40px rgba(0,0,0,0.1); }
        .whatsapp-float { position: fixed; bottom: 20px; right: 20px; z-index: 1000; }
        .mockup-phone { background: #333; border-radius: 25px; padding: 8px; }
        .mockup-screen { border-radius: 20px; overflow: hidden; }
    </style>
</head>
<body class="bg-gray-50">
    <!-- Header -->
    <nav class="bg-white shadow-lg fixed w-full top-0 z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <div class="flex items-center">
                    <i class="fas fa-utensils text-2xl text-purple-600 mr-2"></i>
                    <span class="text-xl font-bold text-gray-800">CardápiosPro</span>
                </div>
                <div class="hidden md:flex space-x-8">
                    <a href="#home" class="text-gray-700 hover:text-purple-600 transition">Início</a>
                    <a href="#portfolio" class="text-gray-700 hover:text-purple-600 transition">Portfólio</a>
                    <a href="#beneficios" class="text-gray-700 hover:text-purple-600 transition">Benefícios</a>
                    <a href="#precos" class="text-gray-700 hover:text-purple-600 transition">Preços</a>
                    <a href="#contato" class="text-gray-700 hover:text-purple-600 transition">Contato</a>
                </div>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="gradient-bg text-white pt-20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-20">
            <div class="text-center">
                <h1 class="text-5xl md:text-6xl font-bold mb-6">
                    Cardápios Profissionais<br>
                    <span class="text-yellow-300">que Vendem Mais</span>
                </h1>
                <p class="text-xl md:text-2xl mb-8 max-w-3xl mx-auto">
                    Crio cardápios digitais, impressos e com QR Code para restaurantes, lanchonetes e bares.
                </p>
                <button onclick="abrirWhatsApp()" class="bg-green-500 hover:bg-green-600 text-white font-bold py-4 px-8 rounded-full text-lg transition transform hover:scale-105">
                    <i class="fab fa-whatsapp mr-2"></i>
                    Fale comigo no WhatsApp
                </button>
            </div>
        </div>
    </section>

    <!-- Portfolio Section -->
    <section id="portfolio" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">Meus Trabalhos</h2>
                <p class="text-xl text-gray-600">Confira alguns exemplos de cardápios que já criei</p>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Pizzaria -->
                <div class="card-hover bg-white rounded-lg shadow-lg overflow-hidden">
                    <div class="mockup-phone mx-auto w-48 mt-6">
                        <div class="mockup-screen bg-red-600 h-80 flex flex-col">
                            <div class="bg-red-700 p-4 text-white text-center">
                                <h3 class="font-bold text-lg">🍕 Pizzaria Bella</h3>
                                <p class="text-sm">Cardápio Digital</p>
                            </div>
                            <div class="flex-1 p-4 bg-white text-gray-800">
                                <div class="mb-4">
                                    <h4 class="font-semibold text-red-600">PIZZAS TRADICIONAIS</h4>
                                    <div class="text-sm mt-2">
                                        <div class="flex justify-between">
                                            <span>Margherita</span>
                                            <span class="font-bold">R$ 35</span>
                                        </div>
                                        <div class="flex justify-between mt-1">
                                            <span>Calabresa</span>
                                            <span class="font-bold">R$ 38</span>
                                        </div>
                                    </div>
                                </div>
                                <div class="text-center">
                                    <div class="w-16 h-16 bg-gray-200 rounded mx-auto flex items-center justify-center">
                                        <i class="fas fa-qrcode text-2xl text-gray-600"></i>
                                    </div>
                                    <p class="text-xs mt-1">QR Code</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-gray-800 mb-2">Pizzaria Bella</h3>
                        <p class="text-gray-600 mb-4">Cardápio completo com QR Code para mesas</p>
                        <button onclick="verDetalhes('pizzaria')" class="text-purple-600 hover:text-purple-800 font-semibold">
                            Ver detalhes <i class="fas fa-arrow-right ml-1"></i>
                        </button>
                    </div>
                </div>

                <!-- Hamburgueria -->
                <div class="card-hover bg-white rounded-lg shadow-lg overflow-hidden">
                    <div class="mockup-phone mx-auto w-48 mt-6">
                        <div class="mockup-screen bg-yellow-500 h-80 flex flex-col">
                            <div class="bg-yellow-600 p-4 text-white text-center">
                                <h3 class="font-bold text-lg">🍔 Burger House</h3>
                                <p class="text-sm">Menu Premium</p>
                            </div>
                            <div class="flex-1 p-4 bg-white text-gray-800">
                                <div class="mb-4">
                                    <h4 class="font-semibold text-yellow-600">BURGERS ESPECIAIS</h4>
                                    <div class="text-sm mt-2">
                                        <div class="flex justify-between">
                                            <span>Classic Burger</span>
                                            <span class="font-bold">R$ 28</span>
                                        </div>
                                        <div class="flex justify-between mt-1">
                                            <span>BBQ Bacon</span>
                                            <span class="font-bold">R$ 32</span>
                                        </div>
                                    </div>
                                </div>
                                <div class="bg-yellow-100 p-2 rounded text-center">
                                    <p class="text-xs font-semibold text-yellow-800">COMBO + BATATA + REFRI</p>
                                    <p class="text-lg font-bold text-yellow-600">R$ 45</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-gray-800 mb-2">Burger House</h3>
                        <p class="text-gray-600 mb-4">Design moderno com foco em combos</p>
                        <button onclick="verDetalhes('burger')" class="text-purple-600 hover:text-purple-800 font-semibold">
                            Ver detalhes <i class="fas fa-arrow-right ml-1"></i>
                        </button>
                    </div>
                </div>

                <!-- Sushi -->
                <div class="card-hover bg-white rounded-lg shadow-lg overflow-hidden">
                    <div class="mockup-phone mx-auto w-48 mt-6">
                        <div class="mockup-screen bg-gray-800 h-80 flex flex-col">
                            <div class="bg-black p-4 text-white text-center">
                                <h3 class="font-bold text-lg">🍣 Sushi Zen</h3>
                                <p class="text-sm">Cardápio Elegante</p>
                            </div>
                            <div class="flex-1 p-4 bg-white text-gray-800">
                                <div class="mb-4">
                                    <h4 class="font-semibold text-gray-800">COMBINADOS</h4>
                                    <div class="text-sm mt-2">
                                        <div class="flex justify-between">
                                            <span>Combo Salmão</span>
                                            <span class="font-bold">R$ 45</span>
                                        </div>
                                        <div class="flex justify-between mt-1">
                                            <span>Combo Especial</span>
                                            <span class="font-bold">R$ 65</span>
                                        </div>
                                    </div>
                                </div>
                                <div class="bg-red-600 text-white p-2 rounded text-center">
                                    <p class="text-xs font-semibold">DELIVERY GRÁTIS</p>
                                    <p class="text-sm">Pedidos acima de R$ 80</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-gray-800 mb-2">Sushi Zen</h3>
                        <p class="text-gray-600 mb-4">Layout minimalista e sofisticado</p>
                        <button onclick="verDetalhes('sushi')" class="text-purple-600 hover:text-purple-800 font-semibold">
                            Ver detalhes <i class="fas fa-arrow-right ml-1"></i>
                        </button>
                    </div>
                </div>

                <!-- Bar -->
                <div class="card-hover bg-white rounded-lg shadow-lg overflow-hidden">
                    <div class="mockup-phone mx-auto w-48 mt-6">
                        <div class="mockup-screen bg-amber-700 h-80 flex flex-col">
                            <div class="bg-amber-800 p-4 text-white text-center">
                                <h3 class="font-bold text-lg">🍺 Bar do João</h3>
                                <p class="text-sm">Drinks & Petiscos</p>
                            </div>
                            <div class="flex-1 p-4 bg-white text-gray-800">
                                <div class="mb-4">
                                    <h4 class="font-semibold text-amber-700">CERVEJAS</h4>
                                    <div class="text-sm mt-2">
                                        <div class="flex justify-between">
                                            <span>Brahma 600ml</span>
                                            <span class="font-bold">R$ 8</span>
                                        </div>
                                        <div class="flex justify-between mt-1">
                                            <span>Heineken 600ml</span>
                                            <span class="font-bold">R$ 12</span>
                                        </div>
                                    </div>
                                </div>
                                <div class="bg-amber-100 p-2 rounded text-center">
                                    <p class="text-xs font-semibold text-amber-800">HAPPY HOUR</p>
                                    <p class="text-sm text-amber-700">17h às 19h - 20% OFF</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-gray-800 mb-2">Bar do João</h3>
                        <p class="text-gray-600 mb-4">Cardápio descontraído com promoções</p>
                        <button onclick="verDetalhes('bar')" class="text-purple-600 hover:text-purple-800 font-semibold">
                            Ver detalhes <i class="fas fa-arrow-right ml-1"></i>
                        </button>
                    </div>
                </div>

                <!-- Café -->
                <div class="card-hover bg-white rounded-lg shadow-lg overflow-hidden">
                    <div class="mockup-phone mx-auto w-48 mt-6">
                        <div class="mockup-screen bg-amber-600 h-80 flex flex-col">
                            <div class="bg-amber-700 p-4 text-white text-center">
                                <h3 class="font-bold text-lg">☕ Café Central</h3>
                                <p class="text-sm">Cafés & Doces</p>
                            </div>
                            <div class="flex-1 p-4 bg-white text-gray-800">
                                <div class="mb-4">
                                    <h4 class="font-semibold text-amber-700">CAFÉS ESPECIAIS</h4>
                                    <div class="text-sm mt-2">
                                        <div class="flex justify-between">
                                            <span>Cappuccino</span>
                                            <span class="font-bold">R$ 8</span>
                                        </div>
                                        <div class="flex justify-between mt-1">
                                            <span>Café Gelado</span>
                                            <span class="font-bold">R$ 10</span>
                                        </div>
                                    </div>
                                </div>
                                <div class="text-center">
                                    <p class="text-xs text-gray-600">🥐 CROISSANTS FRESCOS</p>
                                    <p class="text-sm font-semibold text-amber-700">Todos os dias às 8h</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-gray-800 mb-2">Café Central</h3>
                        <p class="text-gray-600 mb-4">Ambiente acolhedor e menu matinal</p>
                        <button onclick="verDetalhes('cafe')" class="text-purple-600 hover:text-purple-800 font-semibold">
                            Ver detalhes <i class="fas fa-arrow-right ml-1"></i>
                        </button>
                    </div>
                </div>

                <!-- Pastelaria -->
                <div class="card-hover bg-white rounded-lg shadow-lg overflow-hidden">
                    <div class="mockup-phone mx-auto w-48 mt-6">
                        <div class="mockup-screen bg-orange-500 h-80 flex flex-col">
                            <div class="bg-orange-600 p-4 text-white text-center">
                                <h3 class="font-bold text-lg">🥟 Pastel da Vovó</h3>
                                <p class="text-sm">Tradição & Sabor</p>
                            </div>
                            <div class="flex-1 p-4 bg-white text-gray-800">
                                <div class="mb-4">
                                    <h4 class="font-semibold text-orange-600">PASTÉIS DOCES</h4>
                                    <div class="text-sm mt-2">
                                        <div class="flex justify-between">
                                            <span>Carne</span>
                                            <span class="font-bold">R$ 6</span>
                                        </div>
                                        <div class="flex justify-between mt-1">
                                            <span>Queijo</span>
                                            <span class="font-bold">R$ 5</span>
                                        </div>
                                    </div>
                                </div>
                                <div class="bg-orange-100 p-2 rounded text-center">
                                    <p class="text-xs font-semibold text-orange-800">CALDO DE CANA</p>
                                    <p class="text-lg font-bold text-orange-600">R$ 4</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-gray-800 mb-2">Pastel da Vovó</h3>
                        <p class="text-gray-600 mb-4">Visual tradicional com toque moderno</p>
                        <button onclick="verDetalhes('pastel')" class="text-purple-600 hover:text-purple-800 font-semibold">
                            Ver detalhes <i class="fas fa-arrow-right ml-1"></i>
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Benefícios Section -->
    <section id="beneficios" class="py-20 bg-gray-100">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">Por que escolher meus cardápios?</h2>
                <p class="text-xl text-gray-600">Soluções completas para o seu negócio</p>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
                <div class="text-center bg-white p-8 rounded-lg shadow-lg">
                    <div class="bg-blue-100 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
                        <i class="fas fa-mobile-alt text-2xl text-blue-600"></i>
                    </div>
                    <h3 class="text-xl font-bold text-gray-800 mb-4">Versão Digital</h3>
                    <p class="text-gray-600">PDF otimizado para WhatsApp e redes sociais. Fácil de compartilhar!</p>
                </div>
                
                <div class="text-center bg-white p-8 rounded-lg shadow-lg">
                    <div class="bg-green-100 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
                        <i class="fas fa-qrcode text-2xl text-green-600"></i>
                    </div>
                    <h3 class="text-xl font-bold text-gray-800 mb-4">QR Code</h3>
                    <p class="text-gray-600">QR Code personalizado para mesas. Prático, moderno e sem contato!</p>
                </div>
                
                <div class="text-center bg-white p-8 rounded-lg shadow-lg">
                    <div class="bg-purple-100 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
                        <i class="fas fa-print text-2xl text-purple-600"></i>
                    </div>
                    <h3 class="text-xl font-bold text-gray-800 mb-4">Pronto para Impressão</h3>
                    <p class="text-gray-600">Arquivo em alta resolução, pronto para impressão em qualquer gráfica.</p>
                </div>
                
                <div class="text-center bg-white p-8 rounded-lg shadow-lg">
                    <div class="bg-yellow-100 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
                        <i class="fas fa-chart-line text-2xl text-yellow-600"></i>
                    </div>
                    <h3 class="text-xl font-bold text-gray-800 mb-4">Design Estratégico</h3>
                    <p class="text-gray-600">Layout que destaca os pratos que mais lucram e aumenta suas vendas.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Preços Section -->
    <section id="precos" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">Pacotes e Preços</h2>
                <p class="text-xl text-gray-600">Escolha o pacote ideal para o seu negócio</p>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8 max-w-5xl mx-auto">
                <!-- Pacote Inicial -->
                <div class="bg-white border-2 border-gray-200 rounded-lg p-8 text-center hover:border-purple-500 transition">
                    <h3 class="text-2xl font-bold text-gray-800 mb-4">Pacote Inicial</h3>
                    <div class="text-4xl font-bold text-purple-600 mb-6">R$ 100</div>
                    <ul class="text-left space-y-3 mb-8">
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Cardápio digital (PDF)</li>
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> QR Code personalizado</li>
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Até 20 itens</li>
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> 2 revisões incluídas</li>
                    </ul>
                    <button onclick="abrirWhatsApp('inicial')" class="w-full bg-purple-600 hover:bg-purple-700 text-white font-bold py-3 px-6 rounded-lg transition">
                        Escolher Pacote
                    </button>
                </div>
                
                <!-- Pacote Completo -->
                <div class="bg-white border-2 border-purple-500 rounded-lg p-8 text-center relative">
                    <div class="absolute -top-4 left-1/2 transform -translate-x-1/2 bg-purple-500 text-white px-4 py-1 rounded-full text-sm font-bold">
                        MAIS POPULAR
                    </div>
                    <h3 class="text-2xl font-bold text-gray-800 mb-4">Pacote Completo</h3>
                    <div class="text-4xl font-bold text-purple-600 mb-6">R$ 200</div>
                    <ul class="text-left space-y-3 mb-8">
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Tudo do pacote inicial</li>
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Arquivo para impressão</li>
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Até 50 itens</li>
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Design personalizado</li>
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> 5 revisões incluídas</li>
                    </ul>
                    <button onclick="abrirWhatsApp('completo')" class="w-full bg-purple-600 hover:bg-purple-700 text-white font-bold py-3 px-6 rounded-lg transition">
                        Escolher Pacote
                    </button>
                </div>
                
                <!-- Pacote Premium -->
                <div class="bg-white border-2 border-gray-200 rounded-lg p-8 text-center hover:border-purple-500 transition">
                    <h3 class="text-2xl font-bold text-gray-800 mb-4">Pacote Premium</h3>
                    <div class="text-4xl font-bold text-purple-600 mb-6">R$ 300</div>
                    <ul class="text-left space-y-3 mb-8">
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Tudo do pacote completo</li>
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Itens ilimitados</li>
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Múltiplas versões</li>
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Consultoria de preços</li>
                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Revisões ilimitadas</li>
                    </ul>
                    <button onclick="abrirWhatsApp('premium')" class="w-full bg-purple-600 hover:bg-purple-700 text-white font-bold py-3 px-6 rounded-lg transition">
                        Escolher Pacote
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- Contato Section -->
    <section id="contato" class="py-20 bg-gray-100">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h2 class="text-4xl font-bold text-gray-800 mb-8">Vamos conversar?</h2>
            <p class="text-xl text-gray-600 mb-8">Entre em contato e vamos criar o cardápio perfeito para o seu negócio!</p>
            
            <div class="flex flex-col md:flex-row justify-center items-center space-y-4 md:space-y-0 md:space-x-8">
                <button onclick="abrirWhatsApp()" class="bg-green-500 hover:bg-green-600 text-white font-bold py-4 px-8 rounded-full text-lg transition transform hover:scale-105">
                    <i class="fab fa-whatsapp mr-2"></i>
                    WhatsApp: (11) 99999-9999
                </button>
                
                <div class="flex items-center text-gray-600">
                    <i class="fas fa-envelope mr-2"></i>
                    <span>contato@cardapiospro.com</span>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-8">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <div class="flex items-center justify-center mb-4">
                <i class="fas fa-utensils text-2xl text-purple-400 mr-2"></i>
                <span class="text-xl font-bold">CardápiosPro</span>
            </div>
            <p class="text-gray-400">© 2024 CardápiosPro. Todos os direitos reservados.</p>
        </div>
    </footer>

    <!-- WhatsApp Float Button -->
    <div class="whatsapp-float">
        <button onclick="abrirWhatsApp()" class="bg-green-500 hover:bg-green-600 text-white p-4 rounded-full shadow-lg transition transform hover:scale-110">
            <i class="fab fa-whatsapp text-2xl"></i>
        </button>
    </div>

    <script>
        function abrirWhatsApp(pacote = '') {
            let mensagem = 'Olá! Tenho interesse em criar um cardápio profissional para meu negócio.';
            
            if (pacote === 'inicial') {
                mensagem += ' Gostaria de saber mais sobre o Pacote Inicial (R$ 100).';
            } else if (pacote === 'completo') {
                mensagem += ' Tenho interesse no Pacote Completo (R$ 200).';
            } else if (pacote === 'premium') {
                mensagem += ' Gostaria de contratar o Pacote Premium (R$ 300).';
            }
            
            const numeroWhatsApp = '5511999999999'; // Substitua pelo seu número
            const url = `https://wa.me/${numeroWhatsApp}?text=${encodeURIComponent(mensagem)}`;
            window.open(url, '_blank');
        }

        function verDetalhes(tipo) {
            let mensagem = `Olá! Vi o exemplo do cardápio de ${tipo} no seu portfólio e gostei muito! Gostaria de saber mais detalhes sobre como criar algo similar para meu negócio.`;
            
            const numeroWhatsApp = '5511999999999'; // Substitua pelo seu número
            const url = `https://wa.me/${numeroWhatsApp}?text=${encodeURIComponent(mensagem)}`;
            window.open(url, '_blank');
        }

        // Smooth scroll para navegação
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Animação de entrada dos cards
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);

        document.querySelectorAll('.card-hover').forEach(card => {
            card.style.opacity = '0';
            card.style.transform = 'translateY(30px)';
            card.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
            observer.observe(card);
        });
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'975e7658f06df502',t:'MTc1NjMyODA0Ny4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
