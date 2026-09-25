<!DOCTYPE html>
<html lang="pt-BR" class="h-full">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>MKS CLINIC | Estética Avançada</title>
    
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- FontAwesome CDN for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    
    <!-- Google Fonts: Cormorant Garamond & Montserrat -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600;700&family=Montserrat:wght@300;400;500;600;700&display=swap" rel="stylesheet">

    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        nude: {
                            50: '#FAF6F3',
                            100: '#F4ECE6',
                            200: '#E8D8CD',
                            300: '#DCBEB0',
                            400: '#C79A88',
                            500: '#A87A68',
                        },
                        gold: {
                            light: '#F7E7CE',
                            DEFAULT: '#D4AF37',
                            dark: '#AA771C',
                        },
                        charcoal: '#1A1817'
                    },
                    fontFamily: {
                        serif: ['"Cormorant Garamond"', 'serif'],
                        sans: ['"Montserrat"', 'sans-serif'],
                    }
                }
            }
        }
    </script>

    <style>
        body {
            background-color: #E6D5C7;
            background-image: 
                radial-gradient(circle at 50% 0%, rgba(255, 255, 255, 0.75) 0%, transparent 60%),
                radial-gradient(circle at 100% 100%, rgba(212, 175, 55, 0.18) 0%, transparent 50%),
                radial-gradient(circle at 0% 50%, rgba(168, 122, 104, 0.15) 0%, transparent 50%);
            background-attachment: fixed;
            font-family: 'Montserrat', sans-serif;
            color: #2D2725;
            -webkit-tap-highlight-color: transparent;
        }

        .gold-button-border {
            border: 1px solid rgba(212, 175, 55, 0.45);
            box-shadow: 0 4px 20px rgba(168, 122, 104, 0.12);
        }

        .gold-button-border:active {
            transform: scale(0.98);
        }

        /* Continuous Golden Star Shimmer Animation */
        @keyframes starGlow {
            0%, 100% {
                transform: scale(1);
                filter: drop-shadow(0 0 2px rgba(212, 175, 55, 0.4));
                color: #D4AF37;
            }
            50% {
                transform: scale(1.25);
                filter: drop-shadow(0 0 8px rgba(255, 223, 0, 0.95));
                color: #FFF2A8;
            }
        }

        .star-animated {
            display: inline-block;
            animation: starGlow 1.8s infinite ease-in-out;
        }

        .star-1 { animation-delay: 0.0s; }
        .star-2 { animation-delay: 0.2s; }
        .star-3 { animation-delay: 0.4s; }
        .star-4 { animation-delay: 0.6s; }
        .star-5 { animation-delay: 0.8s; }

        /* VIP Card Shimmer Effect */
        @keyframes vipShimmer {
            0% { background-position: -200% 0; }
            100% { background-position: 200% 0; }
        }

        .vip-shimmer-border {
            position: relative;
            background: #121110;
        }

        .vip-shimmer-border::before {
            content: '';
            position: absolute;
            top: -1px; left: -1px; right: -1px; bottom: -1px;
            background: linear-gradient(90deg, #AA771C, #FFDF00, #AA771C, #FFDF00);
            background-size: 300% 100%;
            border-radius: 1.25rem;
            z-index: 0;
            animation: vipShimmer 4s infinite linear;
            opacity: 0.85;
        }

        /* Glassmorphism Card Style */
        .glass-card {
            background: rgba(255, 255, 255, 0.78);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.9);
        }

        .glass-card:hover, .glass-card:active {
            background: rgba(255, 255, 255, 0.92);
        }

        /* Pulse aura for primary button */
        @keyframes auraPulse {
            0% { box-shadow: 0 0 0 0 rgba(212, 175, 55, 0.45); }
            70% { box-shadow: 0 0 0 12px rgba(212, 175, 55, 0); }
            100% { box-shadow: 0 0 0 0 rgba(212, 175, 55, 0); }
        }

        .pulse-aura {
            animation: auraPulse 2.2s infinite;
        }
    </style>
</head>
<body class="min-h-full flex flex-col items-center justify-between p-4 sm:p-6 select-none">

    <main class="w-full max-w-md mx-auto flex flex-col items-center space-y-6 pt-2 pb-8">
        
        <!-- HEADER SECTION: Exact Emblem Logo & Brand Title -->
        <header class="flex flex-col items-center text-center space-y-3 w-full">
            
            <!-- Logo Emblem SVG (Exact Geometric 8-Petal Rosette from image_1bffe3.png) -->
            <div class="relative flex items-center justify-center w-32 h-32 mb-0">
                <div class="absolute inset-0 rounded-full bg-amber-100/60 blur-xl"></div>
                <svg viewBox="0 0 200 200" class="w-32 h-32 relative z-10 drop-shadow-md" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <defs>
                        <linearGradient id="mksGoldGrad" x1="0%" y1="0%" x2="100%" y2="100%">
                            <stop offset="0%" stop-color="#7A5210" />
                            <stop offset="25%" stop-color="#C5A046" />
                            <stop offset="50%" stop-color="#FFF5B8" />
                            <stop offset="75%" stop-color="#D4AF37" />
                            <stop offset="100%" stop-color="#6B460B" />
                        </linearGradient>
                    </defs>
                    
                    <!-- 8 Interlocking Petal Capsule Loops + Central Diamond Core -->
                    <g stroke="url(#mksGoldGrad)" stroke-width="3.4" stroke-linecap="round" stroke-linejoin="round" fill="none">
                        <!-- Rotated Interlocking Capsule Petals at 0°, 45°, 90°, 135° -->
                        <rect x="84" y="38" width="32" height="124" rx="16" />
                        <rect x="84" y="38" width="32" height="124" rx="16" transform="rotate(45 100 100)" />
                        <rect x="84" y="38" width="32" height="124" rx="16" transform="rotate(90 100 100)" />
                        <rect x="84" y="38" width="32" height="124" rx="16" transform="rotate(135 100 100)" />
                        
                        <!-- Central Diamond Center -->
                        <polygon points="100,87 113,100 100,113 87,100" stroke-width="2.6" fill="rgba(255,245,184,0.15)" />
                    </g>
                </svg>
            </div>

            <!-- Title & Subtitle -->
            <div class="space-y-1">
                <h1 class="font-serif text-3xl sm:text-4xl font-semibold tracking-wide text-charcoal uppercase leading-tight">
                    MKS CLINIC
                </h1>
                <p class="font-sans text-xs tracking-[0.35em] text-amber-900/80 font-medium uppercase">
                    Estética Avançada
                </p>
            </div>

            <p class="text-xs sm:text-sm text-stone-700 max-w-[290px] font-light leading-relaxed pt-1">
                Sua beleza e bem-estar em mãos de especialistas.
            </p>
        </header>

        <!-- BUTTONS CONTAINER -->
        <section class="w-full space-y-4 pt-1">

            <!-- BUTTON 1: GOOGLE AVALIAÇÃO -->
            <a href="https://search.google.com/local/writereview?placeid=ChIJE_ibEQA9qwcRUgRdnS_KhgM" 
               target="_blank" 
               rel="noopener noreferrer"
               class="glass-card gold-button-border pulse-aura rounded-2xl p-4 flex items-center justify-between transition-all duration-300 transform active:scale-98 group block w-full relative overflow-hidden">
                
                <div class="absolute inset-0 bg-gradient-to-r from-amber-100/50 via-amber-50/20 to-transparent opacity-80 pointer-events-none"></div>
                
                <div class="flex items-center space-x-3.5 relative z-10">
                    <!-- Google Icon Wrapper -->
                    <div class="w-12 h-12 rounded-xl bg-white shadow-sm border border-amber-200/60 flex items-center justify-center shrink-0">
                        <svg class="w-6 h-6" viewBox="0 0 24 24">
                            <path fill="#4285F4" d="M22.56 12.25c0-.78-.07-1.53-.2-2.25H12v4.26h5.92c-.26 1.37-1.04 2.53-2.21 3.31v2.77h3.57c2.08-1.92 3.28-4.74 3.28-8.09z"/>
                            <path fill="#34A853" d="M12 23c2.97 0 5.46-.98 7.28-2.66l-3.57-2.77c-.98.66-2.23 1.06-3.71 1.06-2.86 0-5.29-1.93-6.16-4.53H2.18v2.84C3.99 20.53 7.7 23 12 23z"/>
                            <path fill="#FBBC05" d="M5.84 14.09c-.22-.66-.35-1.36-.35-2.09s.13-1.43.35-2.09V7.06H2.18C1.43 8.55 1 10.22 1 12s.43 3.45 1.18 4.94l2.85-2.22.81-.63z"/>
                            <path fill="#EA4335" d="M12 5.38c1.62 0 3.06.56 4.21 1.64l3.15-3.15C17.45 2.09 14.97 1 12 1 7.7 1 3.99 3.47 2.18 7.06l3.66 2.84c.87-2.6 3.3-4.52 6.16-4.52z"/>
                        </svg>
                    </div>

                    <!-- Button Label & Animated Stars -->
                    <div class="text-left">
                        <span class="text-xs font-semibold uppercase tracking-wider text-amber-900 block">
                            Avaliação Google
                        </span>
                        <h2 class="text-sm sm:text-base font-bold text-stone-900 font-sans leading-tight">
                            Deixe sua Avaliação 5 Estrelas
                        </h2>
                        
                        <!-- Animated 5 Stars -->
                        <div class="flex items-center space-x-1 mt-1 text-amber-500">
                            <i class="fa-solid fa-star text-xs star-animated star-1"></i>
                            <i class="fa-solid fa-star text-xs star-animated star-2"></i>
                            <i class="fa-solid fa-star text-xs star-animated star-3"></i>
                            <i class="fa-solid fa-star text-xs star-animated star-4"></i>
                            <i class="fa-solid fa-star text-xs star-animated star-5"></i>
                            <span class="text-[11px] font-medium text-amber-800 ml-1.5">(Clique para avaliar)</span>
                        </div>
                    </div>
                </div>

                <div class="w-8 h-8 rounded-full bg-amber-500/10 flex items-center justify-center shrink-0 relative z-10 text-amber-800 group-hover:translate-x-1 transition-transform">
                    <i class="fa-solid fa-chevron-right text-xs"></i>
                </div>
            </a>


            <!-- BUTTON 2: INSTAGRAM -->
            <a href="https://www.instagram.com/mks.clinic?stkn=MWJ4cW91NnM4MDQ4dg==" 
               target="_blank" 
               rel="noopener noreferrer"
               class="glass-card gold-button-border rounded-2xl p-4 flex items-center justify-between transition-all duration-300 transform active:scale-98 group block w-full">
                
                <div class="flex items-center space-x-3.5">
                    <div class="w-12 h-12 rounded-xl bg-gradient-to-tr from-amber-500 via-rose-500 to-purple-600 text-white shadow-sm flex items-center justify-center shrink-0">
                        <i class="fa-brands fa-instagram text-2xl"></i>
                    </div>

                    <div class="text-left">
                        <span class="text-xs font-semibold uppercase tracking-wider text-stone-500 block">
                            Instagram Oficial
                        </span>
                        <h2 class="text-sm sm:text-base font-bold text-stone-900 font-sans leading-tight">
                            Siga nosso Instagram
                        </h2>
                        <p class="text-xs text-amber-900 font-medium mt-0.5">
                            @mks.clinic
                        </p>
                    </div>
                </div>

                <div class="w-8 h-8 rounded-full bg-stone-100 flex items-center justify-center shrink-0 text-stone-600 group-hover:translate-x-1 transition-transform">
                    <i class="fa-solid fa-chevron-right text-xs"></i>
                </div>
            </a>


            <!-- BUTTON 3: WHATSAPP ATENDIMENTO -->
            <a href="https://wa.me/558197301987?text=Ol%C3%A1!%20Gostaria%20de%20agendar%20um%20atendimento%20na%20MKS%20Clinic." 
               target="_blank" 
               rel="noopener noreferrer"
               class="glass-card gold-button-border rounded-2xl p-4 flex items-center justify-between transition-all duration-300 transform active:scale-98 group block w-full">
                
                <div class="flex items-center space-x-3.5">
                    <div class="w-12 h-12 rounded-xl bg-emerald-600 text-white shadow-sm flex items-center justify-center shrink-0">
                        <i class="fa-brands fa-whatsapp text-2xl"></i>
                    </div>

                    <div class="text-left">
                        <span class="text-xs font-semibold uppercase tracking-wider text-emerald-800 block">
                            Atendimento & Agendamentos
                        </span>
                        <h2 class="text-sm sm:text-base font-bold text-stone-900 font-sans leading-tight">
                            Entre em Contato
                        </h2>
                        <p class="text-xs text-stone-600 font-medium mt-0.5">
                            Clique para conversar e agendar seu procedimento
                        </p>
                    </div>
                </div>

                <div class="w-8 h-8 rounded-full bg-emerald-50 flex items-center justify-center shrink-0 text-emerald-700 group-hover:translate-x-1 transition-transform">
                    <i class="fa-solid fa-chevron-right text-xs"></i>
                </div>
            </a>


            <!-- BUTTON 4: GRUPO VIP (Design Preto & Dourado de Luxo) -->
            <div class="vip-shimmer-border rounded-2xl p-[1.5px] shadow-xl w-full">
                <a href="https://chat.whatsapp.com/J373H4YQFpW2p8UOz6NJuk" 
                   target="_blank" 
                   rel="noopener noreferrer"
                   class="bg-stone-950 rounded-[1.15rem] p-4 flex items-center justify-between transition-all duration-300 transform active:scale-98 group block w-full relative overflow-hidden">
                    
                    <div class="absolute inset-0 bg-gradient-to-r from-amber-500/10 via-transparent to-amber-500/5 pointer-events-none"></div>

                    <div class="flex items-center space-x-3.5 relative z-10">
                        <div class="w-12 h-12 rounded-xl bg-gradient-to-br from-stone-800 to-stone-900 border border-amber-500/40 text-amber-400 shadow-md flex items-center justify-center shrink-0 relative">
                            <i class="fa-brands fa-whatsapp text-2xl"></i>
                            <i class="fa-solid fa-crown text-[10px] text-amber-300 absolute -top-1 -right-1 bg-black p-1 rounded-full border border-amber-400"></i>
                        </div>

                        <div class="text-left">
                            <div class="flex items-center space-x-1.5">
                                <span class="text-[10px] font-bold uppercase tracking-widest bg-amber-500/20 text-amber-300 px-2 py-0.5 rounded-full border border-amber-500/30">
                                    VIP EXCLUSIVO
                                </span>
                            </div>
                            <h2 class="text-sm sm:text-base font-bold text-amber-100 font-sans leading-tight mt-1">
                                Grupo VIP - Promoções
                            </h2>
                            <p class="text-xs text-stone-400 font-light mt-0.5">
                                Acompanhe nossas promoções
                            </p>
                        </div>
                    </div>

                    <div class="w-8 h-8 rounded-full bg-amber-500/20 border border-amber-500/40 flex items-center justify-center shrink-0 text-amber-300 group-hover:translate-x-1 transition-transform relative z-10">
                        <i class="fa-solid fa-chevron-right text-xs"></i>
                    </div>
                </a>
            </div>

        </section>

        <!-- FOOTER BRANDING -->
        <footer class="text-center pt-6 space-y-1">
            <p class="font-serif text-sm font-semibold text-stone-800 tracking-wider">
                MKS CLINIC ESTÉTICA AVANÇADA
            </p>
            <p class="text-[10px] text-stone-500 tracking-wider uppercase">
                Olinda - PE • Todos os direitos reservados
            </p>
        </footer>

    </main>

</body>
</html>
