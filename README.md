<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jeff Barber - Barbearia a Domicílio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap');

        body {
            font-family: 'Poppins', sans-serif;
            scroll-behavior: smooth;
        }
        
        .hero {
            background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url('https://images.unsplash.com/photo-1595476108010-b4d1f102b1b1?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1480&q=80');
            background-size: cover;
            background-position: center;
        }
        
        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
        }
        
        .floating-button {
            animation: float 3s ease-in-out infinite;
        }
        
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-15px); }
            100% { transform: translateY(0px); }
        }
    </style>
</head>
<body class="bg-gray-100">
    <!-- Navigation -->
    <nav class="bg-black text-white shadow-lg fixed w-full z-50">
        <div class="container mx-auto px-4 py-3 flex justify-between items-center">
            <div class="flex items-center">
                <i class="fas fa-cut text-amber-500 text-2xl mr-2"></i>
                <span class="font-bold text-xl">JEFF BARBER</span>
            </div>
            <div class="hidden md:flex space-x-8">
                <a href="#home" class="hover:text-amber-500 transition">Início</a>
                <a href="#services" class="hover:text-amber-500 transition">Serviços</a>
                <a href="#about" class="hover:text-amber-500 transition">Sobre</a>
                <a href="#contact" class="hover:text-amber-500 transition">Contato</a>
            </div>
            <button class="md:hidden focus:outline-none" id="menu-btn">
                <i class="fas fa-bars text-2xl"></i>
            </button>
        </div>

        <!-- Mobile Menu -->
        <div class="md:hidden hidden bg-black w-full px-4 py-2" id="mobile-menu">
            <a href="#home" class="block py-2 hover:text-amber-500 transition">Início</a>
            <a href="#services" class="block py-2 hover:text-amber-500 transition">Serviços</a>
            <a href="#about" class="block py-2 hover:text-amber-500 transition">Sobre</a>
            <a href="#contact" class="block py-2 hover:text-amber-500 transition">Contato</a>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero text-white pt-32 pb-20 md:pt-40 md:pb-28 px-4" id="home">
        <div class="container mx-auto text-center">
            <h1 class="text-4xl md:text-6xl font-bold mb-6">ESTILO QUE <span class="text-amber-500">VAI ATÉ VOCÊ</span></h1>
            <p class="text-xl md:text-2xl mb-8 max-w-2xl mx-auto">Cortes profissionais no conforto da sua casa por apenas R$25</p>
            <div class="flex flex-col md:flex-row justify-center gap-4">
                <a href="https://wa.me/5511996681443" class="bg-amber-500 hover:bg-amber-600 text-black font-bold py-3 px-8 rounded-full text-lg transition flex items-center justify-center gap-2">
                    <i class="fab fa-whatsapp"></i> Agendar agora
                </a>
                <a href="#services" class="border-2 border-white hover:bg-white hover:text-black font-bold py-3 px-8 rounded-full text-lg transition">
                    Nossos serviços
                </a>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="py-16 px-4 bg-white" id="services">
        <div class="container mx-auto">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-4">NOSSOS SERVIÇOS</h2>
            <div class="w-20 h-1 bg-amber-500 mx-auto mb-12"></div>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Service 1 -->
                <div class="service-card bg-gray-50 rounded-lg overflow-hidden shadow-md transition duration-300">
                    <img src="https://images.unsplash.com/photo-1522337360788-8b13dee7a37e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="Corte de cabelo" class="w-full h-48 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2">Corte Social</h3>
                        <p class="text-gray-600 mb-4">Corte básico com máquina e tesoura, ideal para quem busca um visual limpo e bem cuidado.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-2xl font-bold text-amber-500">R$25</span>
                            <a href="https://wa.me/5511996681443" class="bg-black hover:bg-gray-800 text-white py-2 px-4 rounded-full text-sm transition">
                                Agendar <i class="fas fa-arrow-right ml-1"></i>
                            </a>
                        </div>
                    </div>
                </div>
                
                <!-- Service 2 -->
                <div class="service-card bg-gray-50 rounded-lg overflow-hidden shadow-md transition duration-300">
                    <img src="https://images.unsplash.com/photo-1599351431202-1e0f0137899a?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="Barba" class="w-full h-48 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2">Aparar Barba</h3>
                        <p class="text-gray-600 mb-4">Aparo e modelagem básica da barba para manter seu visual sempre alinhado.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-2xl font-bold text-amber-500">R$15</span>
                            <a href="https://wa.me/5511996681443" class="bg-black hover:bg-gray-800 text-white py-2 px-4 rounded-full text-sm transition">
                                Agendar <i class="fas fa-arrow-right ml-1"></i>
                            </a>
                        </div>
                    </div>
                </div>
                
                <!-- Service 3 -->
                <div class="service-card bg-gray-50 rounded-lg overflow-hidden shadow-md transition duration-300">
                    <img src="https://images.unsplash.com/photo-1592155931584-901ac15763e3?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="Corte infantil" class="w-full h-48 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2">Corte Infantil</h3>
                        <p class="text-gray-600 mb-4">Corte simples para crianças, com paciência e cuidado para deixar os pequenos à vontade.</p>
                        <div class="flex justify-between items-center">
                            <span class="text-2xl font-bold text-amber-500">R$20</span>
                            <a href="https://wa.me/5511996681443" class="bg-black hover:bg-gray-800 text-white py-2 px-4 rounded-full text-sm transition">
                                Agendar <i class="fas fa-arrow-right ml-1"></i>
                            </a>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="mt-16 bg-amber-50 rounded-xl p-8 md:p-12 flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 mb-6 md:mb-0 md:pr-8">
                    <h3 class="text-2xl font-bold mb-4">Pacote Iniciante</h3>
                    <p class="text-gray-700 mb-4">Corte + Aparar Barba com desconto especial para meus primeiros clientes.</p>
                    <div class="flex items-center">
                        <span class="text-3xl font-bold text-amber-500 mr-4">R$35</span>
                        <span class="line-through text-gray-500">R$40</span>
                    </div>
                </div>
                <div class="md:w-1/2">
                    <a href="https://wa.me/5511996681443" class="bg-black hover:bg-gray-800 text-white font-bold py-4 px-8 rounded-full text-lg transition flex items-center justify-center gap-2 w-full md:w-auto">
                        <i class="fab fa-whatsapp"></i> Quero o pacote
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section class="py-16 px-4 bg-gray-100" id="about">
        <div class="container mx-auto">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 mb-8 md:mb-0 md:pr-8">
                    <img src="https://images.unsplash.com/photo-1585747860715-2ba37e788b70?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1474&q=80" alt="Jeff Barber" class="rounded-lg shadow-xl w-full max-w-md mx-auto">
                </div>
                <div class="md:w-1/2">
                    <h2 class="text-3xl md:text-4xl font-bold mb-6">COMEÇANDO MINHA JORNADA</h2>
                    <div class="w-20 h-1 bg-amber-500 mb-6"></div>
                    <p class="text-gray-700 mb-4">Olá, sou o Jeff! Recentemente decidi transformar minha paixão por cortes de cabelo em profissão. Após concluir meu curso de barbeiro, estou animado para colocar em prática tudo que aprendi e construir minha clientela.</p>
                    <p class="text-gray-700 mb-6">Apesar de ser novo na área, trago dedicação, atenção aos detalhes e o compromisso de sempre ouvir atentamente o que cada cliente deseja. Estou oferecendo preços especiais enquanto ganho experiência e aperfeiçoo minhas técnicas.</p>
                    <div class="flex flex-wrap gap-4">
                        <div class="flex items-center bg-white px-4 py-2 rounded-full shadow">
                            <i class="fas fa-check-circle text-amber-500 mr-2"></i>
                            <span>Formação recente</span>
                        </div>
                        <div class="flex items-center bg-white px-4 py-2 rounded-full shadow">
                            <i class="fas fa-check-circle text-amber-500 mr-2"></i>
                            <span>Material esterilizado</span>
                        </div>
                        <div class="flex items-center bg-white px-4 py-2 rounded-full shadow">
                            <i class="fas fa-check-circle text-amber-500 mr-2"></i>
                            <span>Atendimento personalizado</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials -->
    <section class="py-16 px-4 bg-white">
        <div class="container mx-auto">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-4">PRIMEIRAS AVALIAÇÕES</h2>
            <div class="w-20 h-1 bg-amber-500 mx-auto mb-12"></div>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Testimonial 1 -->
                <div class="bg-gray-50 p-6 rounded-lg shadow">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-full bg-gray-300 overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="Cliente" class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-bold">Carlos Silva</h4>
                            <div class="flex text-amber-500">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                            </div>
                        </div>
                    </div>
                    <p class="text-gray-600">"Fiquei surpreso com a qualidade do trabalho do Jeff, especialmente por ser iniciante. Corte bem feito e muito atencioso!"</p>
                </div>
                
                <!-- Testimonial 2 -->
                <div class="bg-gray-50 p-6 rounded-lg shadow">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-full bg-gray-300 overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/men/44.jpg" alt="Cliente" class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-bold">Marcos Oliveira</h4>
                            <div class="flex text-amber-500">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star-half-alt"></i>
                            </div>
                        </div>
                    </div>
                    <p class="text-gray-600">"Ótimo custo-benefício. O Jeff é cuidadoso e se esforça para fazer um bom trabalho. Recomendo para quem quer economizar sem perder qualidade."</p>
                </div>
                
                <!-- Testimonial 3 -->
                <div class="bg-gray-50 p-6 rounded-lg shadow">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-full bg-gray-300 overflow-hidden mr-4">
                            <img src="https://randomuser.me/api/portraits/men/68.jpg" alt="Cliente" class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-bold">Ricardo Santos</h4>
                            <div class="flex text-amber-500">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="far fa-star"></i>
                            </div>
                        </div>
                    </div>
                    <p class="text-gray-600">"Bom atendimento e preço justo. Percebi que o Jeff tem potencial e com mais experiência vai ficar excelente!"</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="py-16 px-4 bg-gray-100" id="contact">
        <div class="container mx-auto">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-4">ENTRE EM CONTATO</h2>
            <div class="w-20 h-1 bg-amber-500 mx-auto mb-12"></div>
            
            <div class="flex flex-col md:flex-row gap-8">
                <div class="md:w-1/2">
                    <div class="bg-white p-6 rounded-lg shadow-lg">
                        <h3 class="text-xl font-bold mb-6">Informações de Contato</h3>
                        
                        <div class="flex items-start mb-6">
                            <div class="bg-amber-100 p-3 rounded-full mr-4">
                                <i class="fas fa-phone-alt text-amber-500"></i>
                            </div>
                            <div>
                                <h4 class="font-bold">Telefone/WhatsApp</h4>
                                <a href="tel:11996681443" class="text-gray-600 hover:text-amber-500 transition">(11) 99668-1443</a>
                            </div>
                        </div>
                        
                        <div class="flex items-start mb-6">
                            <div class="bg-amber-100 p-3 rounded-full mr-4">
                                <i class="fab fa-instagram text-amber-500"></i>
                            </div>
                            <div>
                                <h4 class="font-bold">Instagram</h4>
                                <a href="https://instagram.com/Jeffbarber2025" target="_blank" class="text-gray-600 hover:text-amber-500 transition">@Jeffbarber2025</a>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="bg-amber-100 p-3 rounded-full mr-4">
                                <i class="fas fa-map-marker-alt text-amber-500"></i>
                            </div>
                            <div>
                                <h4 class="font-bold">Área de Atendimento</h4>
                                <p class="text-gray-600">Grande São Paulo e região</p>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="md:w-1/2">
                    <div class="bg-white p-6 rounded-lg shadow-lg">
                        <h3 class="text-xl font-bold mb-6">Horário de Funcionamento</h3>
                        
                        <div class="space-y-4">
                            <div class="flex justify-between border-b pb-2">
                                <span>Segunda a Sexta</span>
                                <span class="font-bold">09:00 - 20:00</span>
                            </div>
                            <div class="flex justify-between border-b pb-2">
                                <span>Sábado</span>
                                <span class="font-bold">08:00 - 18:00</span>
                            </div>
                            <div class="flex justify-between">
                                <span>Domingo</span>
                                <span class="font-bold">10:00 - 15:00</span>
                            </div>
                        </div>
                        
                        <div class="mt-8">
                            <h4 class="font-bold mb-4">Formas de Pagamento</h4>
                            <div class="flex flex-wrap gap-3">
                                <div class="bg-gray-100 px-3 py-2 rounded">
                                    <i class="fas fa-money-bill-wave text-green-500"></i> Dinheiro
                                </div>
                                <div class="bg-gray-100 px-3 py-2 rounded">
                                    <i class="fab fa-pix text-blue-500"></i> Pix
                                </div>
                                <div class="bg-gray-100 px-3 py-2 rounded">
                                    <i class="fas fa-mobile-alt text-purple-500"></i> Transferência
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Floating WhatsApp Button -->
    <a href="https://wa.me/5511996681443" class="fixed bottom-6 right-6 bg-green-500 text-white p-4 rounded-full shadow-xl floating-button z-50">
        <i class="fab fa-whatsapp text-2xl"></i>
    </a>

    <!-- Footer -->
    <footer class="bg-black text-white py-8 px-4">
        <div class="container mx-auto">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="mb-4 md:mb-0">
                    <div class="flex items-center">
                        <i class="fas fa-cut text-amber-500 text-2xl mr-2"></i>
                        <span class="font-bold text-xl">JEFF BARBER</span>
                    </div>
                    <p class="text-gray-400 mt-2">Construindo minha carreira com dedicação e qualidade</p>
                </div>
                
                <div class="flex space-x-6">
                    <a href="https://instagram.com/Jeffbarber2025" target="_blank" class="text-gray-400 hover:text-amber-500 transition">
                        <i class="fab fa-instagram text-2xl"></i>
                    </a>
                    <a href="https://wa.me/5511996681443" class="text-gray-400 hover:text-amber-500 transition">
                        <i class="fab fa-whatsapp text-2xl"></i>
                    </a>
                </div>
            </div>
            
            <div class="border-t border-gray-800 mt-8 pt-6 text-center text-gray-400">
                <p>&copy; 2023 Jeff Barber. Todos os direitos reservados.</p>
            </div>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        const menuBtn = document.getElementById('menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        
        menuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });
        
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    // Close mobile menu if open
                    mobileMenu.classList.add('hidden');
                    
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });
        
        // Change navbar style on scroll
        window.addEventListener('scroll', function() {
            const navbar = document.querySelector('nav');
            if (window.scrollY > 50) {
                navbar.classList.add('shadow-xl');
            } else {
                navbar.classList.remove('shadow-xl');
            }
        });
    </script>
</body>
</html>
