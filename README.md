<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>KOTTU KADE | Sri Lanka's Ultimate Cheese Kottu</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        brand: {
                            orange: '#FF5722',
                            yellow: '#FFC107',
                            dark: '#0F172A',
                            card: '#1E293B',
                            accent: '#F59E0B'
                        }
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        heading: ['Poppins', 'sans-serif']
                    }
                }
            }
        }
    </script>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&family=Poppins:wght@700;800;900&display=swap" rel="stylesheet">
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- AOS Animation Library -->
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <!-- Canvas Confetti -->
    <script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.5.1/dist/confetti.browser.min.js"></script>
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #0B0F17;
            color: #F8FAFC;
        }
        .font-heading {
            font-family: 'Poppins', sans-serif;
        }
        .glow-effect {
            box-shadow: 0 0 25px rgba(255, 87, 34, 0.4);
        }
        .glow-yellow {
            box-shadow: 0 0 25px rgba(255, 193, 7, 0.3);
        }
        .glass-panel {
            background: rgba(30, 41, 59, 0.7);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        /* Custom scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #0B0F17;
        }
        ::-webkit-scrollbar-thumb {
            background: #FF5722;
            border-radius: 4px;
        }
    </style>
</head>
<body class="bg-[#0B0F17] text-gray-100 min-h-screen flex flex-col justify-between selection:bg-brand-orange selection:text-white">

    <!-- Navigation Bar -->
    <nav class="fixed top-0 left-0 right-0 z-50 glass-panel border-b border-gray-800 transition-all duration-300" id="navbar">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-20">
                <!-- Logo -->
                <a href="#" class="flex items-center gap-3 group">
                    <div class="w-12 h-12 rounded-2xl bg-gradient-to-tr from-brand-orange to-brand-yellow flex items-center justify-center text-white font-black text-2xl shadow-lg transform group-hover:rotate-6 transition-transform">
                        <i class="fa-solid fa-fire-flame-curved"></i>
                    </div>
                    <div>
                        <span class="font-heading font-black text-2xl tracking-wider text-white">KOTTU <span class="text-brand-orange">KADE</span></span>
                        <span class="block text-xs text-brand-yellow tracking-widest uppercase font-semibold">Extra Cheese Heaven</span>
                    </div>
                </a>

                <!-- Desktop Links -->
                <div class="hidden md:flex items-center space-x-8 font-semibold">
                    <a href="#hero" class="text-gray-300 hover:text-brand-orange transition-colors">Home</a>
                    <a href="#menu" class="text-gray-300 hover:text-brand-orange transition-colors">Special Kottu Menu</a>
                    <a href="#about" class="text-gray-300 hover:text-brand-orange transition-colors">Why Us</a>
                    <a href="#reviews" class="text-gray-300 hover:text-brand-orange transition-colors">Reviews</a>
                </div>

                <!-- Action Button & Cart -->
                <div class="flex items-center gap-4">
                    <button onclick="toggleCartDrawer()" class="relative p-3 bg-gray-800 hover:bg-gray-700 rounded-xl transition-colors border border-gray-700">
                        <i class="fa-solid fa-basket-shopping text-xl text-brand-yellow"></i>
                        <span id="cartBadge" class="absolute -top-2 -right-2 bg-brand-orange text-white text-xs font-bold w-6 h-6 rounded-full flex items-center justify-center hidden scale-0 transition-transform">0</span>
                    </button>
                    <a href="#menu" class="hidden sm:inline-flex items-center justify-center px-6 py-3 rounded-xl font-bold bg-gradient-to-r from-brand-orange to-amber-500 hover:opacity-90 transition-all shadow-lg glow-effect text-white">
                        Order Now <i class="fa-solid fa-arrow-right ml-2"></i>
                    </a>
                </div>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="hero" class="relative pt-32 pb-20 md:pt-40 md:pb-28 overflow-hidden">
        <!-- Background Accents -->
        <div class="absolute top-1/4 left-1/2 -translate-x-1/2 -translate-y-1/2 w-96 h-96 bg-brand-orange/20 rounded-full blur-3xl pointer-events-none"></div>
        <div class="absolute top-1/3 right-10 w-72 h-72 bg-brand-yellow/15 rounded-full blur-3xl pointer-events-none"></div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                <!-- Left Content -->
                <div data-aos="fade-right" data-aos-duration="1000">
                    <div class="inline-flex items-center gap-2 px-4 py-2 rounded-full bg-brand-orange/10 border border-brand-orange/30 text-brand-orange font-semibold text-sm mb-6">
                        <i class="fa-solid fa-pepper-hot"></i> 100% Authentic Melty Cheese Kottu
                    </div>
                    <h1 class="font-heading text-4xl sm:text-6xl font-extrabold leading-tight tracking-tight mb-6">
                        Lankan Street Flavour <br>
                        <span class="bg-gradient-to-r from-brand-orange via-amber-400 to-yellow-300 bg-clip-text text-transparent">Drowned in Cheese!</span>
                    </h1>
                    <p class="text-gray-400 text-lg mb-8 max-w-xl leading-relaxed">
                        Welcome to <strong class="text-white">KOTTU KADE</strong>! Machan, api langa thiyenne Sri Lankawe supirima, thadi molten cheese layer ekak ekka hadana signature kottu 3k witarai. Hot, Fresh & Unmatched Taste!
                    </p>
                    
                    <div class="flex flex-col sm:flex-row gap-4 mb-10">
                        <a href="#menu" class="inline-flex justify-center items-center px-8 py-4 rounded-xl font-extrabold text-lg bg-gradient-to-r from-brand-orange to-amber-500 text-white hover:shadow-2xl hover:scale-105 transition-all duration-300 glow-effect">
                            <i class="fa-solid fa-utensils mr-3"></i> View Specialty Menu
                        </a>
                        <a href="tel:+94771234567" class="inline-flex justify-center items-center px-8 py-4 rounded-xl font-bold text-lg bg-gray-800 border border-gray-700 text-gray-200 hover:bg-gray-700 transition-all">
                            <i class="fa-solid fa-phone text-brand-yellow mr-3"></i> Quick Call
                        </a>
                    </div>

                    <!-- Quick Highlights -->
                    <div class="grid grid-cols-3 gap-4 border-t border-gray-800 pt-8">
                        <div>
                            <span class="block font-heading text-2xl font-black text-brand-yellow">100%</span>
                            <span class="text-xs text-gray-400 font-medium uppercase tracking-wider">Real Cheese</span>
                        </div>
                        <div>
                            <span class="block font-heading text-2xl font-black text-brand-orange">Hot & Fresh</span>
                            <span class="text-xs text-gray-400 font-medium uppercase tracking-wider">Made Live</span>
                        </div>
                        <div>
                            <span class="block font-heading text-2xl font-black text-amber-400">Fast</span>
                            <span class="text-xs text-gray-400 font-medium uppercase tracking-wider">WhatsApp Order</span>
                        </div>
                    </div>
                </div>

                <!-- Right Hero Image Stack -->
                <div class="relative flex justify-center" data-aos="zoom-in" data-aos-duration="1000">
                    <div class="relative w-full max-w-md aspect-square rounded-3xl bg-gradient-to-tr from-brand-orange/30 to-brand-yellow/20 p-2 border border-white/10 glow-yellow">
                        <img src="https://images.unsplash.com/photo-1585238342024-78d387f4a707?auto=format&fit=crop&w=800&q=80" 
                             alt="Hot Cheese Kottu" 
                             class="w-full h-full object-cover rounded-2xl shadow-2xl">
                        
                        <!-- Floating Badge 1 -->
                        <div class="absolute -bottom-6 -left-6 glass-panel p-4 rounded-2xl shadow-xl flex items-center gap-3 border border-brand-orange/40 animate-bounce">
                            <div class="w-10 h-10 rounded-xl bg-brand-orange/20 flex items-center justify-center text-brand-orange font-bold text-xl">
                                🔥
                            </div>
                            <div>
                                <p class="text-xs text-gray-400 font-medium">Customer Favorite</p>
                                <p class="text-sm font-bold text-white">Triple Cheese Chicken</p>
                            </div>
                        </div>

                        <!-- Floating Badge 2 -->
                        <div class="absolute -top-6 -right-6 glass-panel p-4 rounded-2xl shadow-xl flex items-center gap-3 border border-brand-yellow/40">
                            <div class="w-10 h-10 rounded-xl bg-brand-yellow/20 flex items-center justify-center text-brand-yellow font-bold text-xl">
                                🧀
                            </div>
                            <div>
                                <p class="text-xs text-gray-400 font-medium">Extra Gooey</p>
                                <p class="text-sm font-bold text-white">Mozzarella Loaded</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Kottu Specialty Menu -->
    <section id="menu" class="py-20 bg-slate-950/60 relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-2xl mx-auto mb-16" data-aos="fade-up">
                <span class="text-brand-orange font-bold text-sm tracking-widest uppercase mb-2 block">Exclusive Dishes</span>
                <h2 class="font-heading text-3xl sm:text-5xl font-black text-white">OUR 3 SPECIALTY KOTTUS</h2>
                <div class="w-20 h-1.5 bg-gradient-to-r from-brand-orange to-brand-yellow rounded-full mx-auto mt-4"></div>
                <p class="text-gray-400 mt-4">Ape specialized recipes 3 vitarai! Quality, quantity saha cheese pull eka 100% guaranteed!</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8" id="menuItemsContainer">
                <!-- Javascript will populate or static load below -->
            </div>
        </div>
    </section>

    <!-- Customizer Promo Banner -->
    <section class="py-16 relative overflow-hidden bg-gradient-to-r from-slate-900 via-brand-dark to-slate-900 border-y border-gray-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="glass-panel rounded-3xl p-8 sm:p-12 relative overflow-hidden flex flex-col lg:flex-row items-center justify-between gap-8 border border-brand-orange/30">
                <div class="max-w-xl z-10" data-aos="fade-right">
                    <span class="bg-amber-500/20 text-amber-400 font-bold text-xs uppercase tracking-wider px-3 py-1 rounded-full border border-amber-500/30">Machan Choice</span>
                    <h3 class="font-heading text-3xl sm:text-4xl font-extrabold text-white mt-3">Spice Level & Extra Cheese Options</h3>
                    <p class="text-gray-300 mt-3 leading-relaxed">
                        Normal spicy da, pissu hadena nai miris kottu ekakda ඕන? Order eka karaddi cheese level ekai spicy level ekai ketiwenma customize karala illanna puluwan!
                    </p>
                </div>
                <div class="z-10 flex flex-wrap gap-4" data-aos="fade-left">
                    <div class="text-center bg-gray-900/80 p-4 rounded-2xl border border-gray-700 min-w-[120px]">
                        <span class="text-3xl">🌶️</span>
                        <p class="text-xs text-gray-400 font-bold mt-2">Nai Miris Extra</p>
                    </div>
                    <div class="text-center bg-gray-900/80 p-4 rounded-2xl border border-gray-700 min-w-[120px]">
                        <span class="text-3xl">🧀</span>
                        <p class="text-xs text-gray-400 font-bold mt-2">Double Cheese</p>
                    </div>
                    <div class="text-center bg-gray-900/80 p-4 rounded-2xl border border-gray-700 min-w-[120px]">
                        <span class="text-3xl">🥚</span>
                        <p class="text-xs text-gray-400 font-bold mt-2">Extra Fried Egg</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Why Choose Us -->
    <section id="about" class="py-20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div class="glass-panel p-8 rounded-3xl hover:border-brand-orange/50 transition-all duration-300" data-aos="fade-up" data-aos-delay="100">
                    <div class="w-14 h-14 bg-brand-orange/20 rounded-2xl flex items-center justify-center text-brand-orange text-2xl font-bold mb-6">
                        <i class="fa-solid fa-cheese"></i>
                    </div>
                    <h4 class="font-heading text-xl font-bold text-white mb-3">100% Dairy Mozzarella</h4>
                    <p class="text-gray-400 leading-relaxed text-sm">
                        Cheap blend cheese aithikaralama ne. Real gooey Mozzarella & Cheddar combinations with melted creaminess.
                    </p>
                </div>

                <div class="glass-panel p-8 rounded-3xl hover:border-brand-yellow/50 transition-all duration-300" data-aos="fade-up" data-aos-delay="200">
                    <div class="w-14 h-14 bg-brand-yellow/20 rounded-2xl flex items-center justify-center text-brand-yellow text-2xl font-bold mb-6">
                        <i class="fa-solid fa-drumstick-bite"></i>
                    </div>
                    <h4 class="font-heading text-xl font-bold text-white mb-3">Freshly Prepared Ingredients</h4>
                    <p class="text-gray-400 leading-relaxed text-sm">
                        Dawasa gane aluth chicken, fish and fresh vegetables. Stale ingredients naha, high hygiene guaranteed!
                    </p>
                </div>

                <div class="glass-panel p-8 rounded-3xl hover:border-amber-500/50 transition-all duration-300" data-aos="fade-up" data-aos-delay="300">
                    <div class="w-14 h-14 bg-amber-500/20 rounded-2xl flex items-center justify-center text-amber-500 text-2xl font-bold mb-6">
                        <i class="fa-solid fa-bolt"></i>
                    </div>
                    <h4 class="font-heading text-xl font-bold text-white mb-3">Instant Direct Delivery</h4>
                    <p class="text-gray-400 leading-relaxed text-sm">
                        WhatsApp ekata ewelema message eka yanawa. Kadeiyin eka sarata rasatama hadala minute ganen delivery eka enawa.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Reviews Section -->
    <section id="reviews" class="py-20 bg-slate-950/40">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-2xl mx-auto mb-16" data-aos="fade-up">
                <span class="text-brand-yellow font-bold text-sm tracking-widest uppercase mb-2 block">Customer Love</span>
                <h2 class="font-heading text-3xl sm:text-5xl font-black text-white">WHAT MACHANS SAY</h2>
                <div class="w-20 h-1.5 bg-brand-yellow rounded-full mx-auto mt-4"></div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Review 1 -->
                <div class="glass-panel p-6 rounded-2xl border border-gray-800" data-aos="fade-up">
                    <div class="flex items-center gap-1 text-brand-yellow mb-4 text-sm">
                        <i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i>
                    </div>
                    <p class="text-gray-300 italic text-sm mb-6">"Cheese Chicken Kottu eka nam superma machan! Cheese volume eka niyamai, chicken portion ekath godak vadi. Best spot in town!"</p>
                    <div class="flex items-center gap-3">
                        <div class="w-10 h-10 rounded-full bg-gradient-to-tr from-brand-orange to-red-500 flex items-center justify-center font-bold text-white">
                            S
                        </div>
                        <div>
                            <p class="text-sm font-bold text-white">Sahan Perera</p>
                            <p class="text-xs text-gray-500">Verified Customer</p>
                        </div>
                    </div>
                </div>

                <!-- Review 2 -->
                <div class="glass-panel p-6 rounded-2xl border border-gray-800" data-aos="fade-up" data-aos-delay="100">
                    <div class="flex items-center gap-1 text-brand-yellow mb-4 text-sm">
                        <i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i>
                    </div>
                    <p class="text-gray-300 italic text-sm mb-6">"Cheese Fish Kottu eka try kare mulawathawata. Puduuma taste ekak, fish eka fried & spicy. Cheese ekka perfect blend eka!"</p>
                    <div class="flex items-center gap-3">
                        <div class="w-10 h-10 rounded-full bg-gradient-to-tr from-brand-yellow to-amber-600 flex items-center justify-center font-bold text-white">
                            K
                        </div>
                        <div>
                            <p class="text-sm font-bold text-white">Kasun Jayasinghe</p>
                            <p class="text-xs text-gray-500">Regular Diner</p>
                        </div>
                    </div>
                </div>

                <!-- Review 3 -->
                <div class="glass-panel p-6 rounded-2xl border border-gray-800" data-aos="fade-up" data-aos-delay="200">
                    <div class="flex items-center gap-1 text-brand-yellow mb-4 text-sm">
                        <i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i>
                    </div>
                    <p class="text-gray-300 italic text-sm mb-6">"Veg Cheese kottu ekata mecharama cheese godak danawa kiyala hithuwe naha. Value for money machan, ekenma highly recommended!"</p>
                    <div class="flex items-center gap-3">
                        <div class="w-10 h-10 rounded-full bg-gradient-to-tr from-emerald-500 to-teal-700 flex items-center justify-center font-bold text-white">
                            N
                        </div>
                        <div>
                            <p class="text-sm font-bold text-white">Nimesha Fernando</p>
                            <p class="text-xs text-gray-500">Food Blogger</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer Section -->
    <footer class="bg-black border-t border-gray-800 pt-16 pb-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-10 mb-12">
                <!-- Brand Info -->
                <div class="md:col-span-2">
                    <div class="flex items-center gap-3 mb-4">
                        <div class="w-10 h-10 rounded-xl bg-brand-orange flex items-center justify-center text-white font-black text-xl">
                            <i class="fa-solid fa-fire-flame-curved"></i>
                        </div>
                        <span class="font-heading font-black text-2xl text-white">KOTTU <span class="text-brand-orange">KADE</span></span>
                    </div>
                    <p class="text-gray-400 text-sm leading-relaxed max-w-sm mb-6">
                        Sri Lanka's premier destination for ultra-cheesy, fresh and authentic street food. Specializing in Chicken, Fish, and Veg Cheese Kottus.
                    </p>
                    <div class="flex space-x-4 text-gray-400">
                        <a href="#" class="w-10 h-10 rounded-xl bg-gray-900 border border-gray-800 flex items-center justify-center hover:bg-brand-orange hover:text-white transition-colors"><i class="fa-brands fa-facebook-f"></i></a>
                        <a href="#" class="w-10 h-10 rounded-xl bg-gray-900 border border-gray-800 flex items-center justify-center hover:bg-brand-orange hover:text-white transition-colors"><i class="fa-brands fa-instagram"></i></a>
                        <a href="#" class="w-10 h-10 rounded-xl bg-gray-900 border border-gray-800 flex items-center justify-center hover:bg-brand-orange hover:text-white transition-colors"><i class="fa-brands fa-whatsapp"></i></a>
                    </div>
                </div>

                <!-- Quick Links -->
                <div>
                    <h5 class="font-heading font-bold text-white mb-4">Quick Links</h5>
                    <ul class="space-y-2 text-sm text-gray-400">
                        <li><a href="#hero" class="hover:text-brand-orange transition-colors">Home</a></li>
                        <li><a href="#menu" class="hover:text-brand-orange transition-colors">Special Kottu Items</a></li>
                        <li><a href="#about" class="hover:text-brand-orange transition-colors">Why Choose Us</a></li>
                        <li><a href="#reviews" class="hover:text-brand-orange transition-colors">Reviews</a></li>
                    </ul>
                </div>

                <!-- Opening Hours -->
                <div>
                    <h5 class="font-heading font-bold text-white mb-4">Opening Hours</h5>
                    <ul class="space-y-2 text-sm text-gray-400">
                        <li>Monday - Sunday:</li>
                        <li class="font-bold text-brand-yellow">4:00 PM - 12:00 Midnight</li>
                        <li class="pt-2 text-xs text-gray-500"><i class="fa-solid fa-location-dot text-brand-orange mr-1"></i> Colombo & Suburbs Delivery Available</li>
                    </ul>
                </div>
            </div>

            <div class="border-t border-gray-900 pt-8 flex flex-col sm:flex-row justify-between items-center text-xs text-gray-500 gap-4">
                <p>&copy; 2026 KOTTU KADE. All Rights Reserved. Designed for ultimate Kottu lovers.</p>
                <p>Machan's Speciality Spot 🇱🇰</p>
            </div>
        </div>
    </footer>

    <!-- Slide-over Cart Drawer -->
    <div id="cartDrawer" class="fixed inset-0 z-50 overflow-hidden hidden" aria-labelledby="slide-over-title" role="dialog" aria-modal="true">
        <!-- Overlay -->
        <div class="fixed inset-0 bg-black/70 backdrop-blur-sm transition-opacity" onclick="toggleCartDrawer()"></div>

        <div class="fixed inset-y-0 right-0 pl-10 max-w-full flex">
            <div class="w-screen max-w-md bg-slate-900 border-l border-gray-800 text-white flex flex-col shadow-2xl">
                <!-- Header -->
                <div class="p-6 bg-slate-950 border-b border-gray-800 flex items-center justify-between">
                    <div class="flex items-center gap-3">
                        <i class="fa-solid fa-basket-shopping text-brand-yellow text-xl"></i>
                        <h3 class="font-heading font-bold text-xl">Your Kottu Basket</h3>
                    </div>
                    <button onclick="toggleCartDrawer()" class="text-gray-400 hover:text-white p-2">
                        <i class="fa-solid fa-xmark text-2xl"></i>
                    </button>
                </div>

                <!-- Cart Items Container -->
                <div class="flex-1 overflow-y-auto p-6 space-y-4" id="cartItemsList">
                    <!-- Populated dynamically via Javascript -->
                </div>

                <!-- Footer Summary & Action -->
                <div class="p-6 bg-slate-950 border-t border-gray-800 space-y-4">
                    <div class="flex justify-between items-center text-gray-300">
                        <span>Total Items</span>
                        <span id="totalItemsCount" class="font-bold text-white">0</span>
                    </div>
                    <div class="flex justify-between items-center text-lg font-bold text-white">
                        <span>Total Price</span>
                        <span id="totalPrice" class="text-brand-yellow font-black text-xl">Rs. 0</span>
                    </div>

                    <!-- Customer Info Inputs -->
                    <div class="space-y-3 pt-2">
                        <input type="text" id="custName" placeholder="Your Name (Nama)" class="w-full bg-gray-800 border border-gray-700 rounded-xl px-4 py-2 text-sm text-white focus:outline-none focus:border-brand-orange">
                        <input type="text" id="custAddress" placeholder="Delivery Address / Landmark" class="w-full bg-gray-800 border border-gray-700 rounded-xl px-4 py-2 text-sm text-white focus:outline-none focus:border-brand-orange">
                    </div>

                    <button onclick="sendWhatsAppOrder()" class="w-full py-4 rounded-xl bg-emerald-600 hover:bg-emerald-500 font-extrabold text-white text-base shadow-lg transition-all flex items-center justify-center gap-2">
                        <i class="fa-brands fa-whatsapp text-2xl"></i> Order via WhatsApp
                    </button>
                </div>
            </div>
        </div>
    </div>

    <!-- Item Customizer Modal -->
    <div id="customizeModal" class="fixed inset-0 z-50 overflow-y-auto hidden">
        <div class="flex items-center justify-center min-h-screen px-4 pt-4 pb-20 text-center sm:block sm:p-0">
            <div class="fixed inset-0 bg-black/80 backdrop-blur-sm transition-opacity" onclick="closeModal()"></div>

            <span class="hidden sm:inline-block sm:align-middle sm:h-screen" aria-hidden="true">&#8203;</span>

            <div class="inline-block align-bottom bg-slate-900 border border-gray-800 rounded-3xl text-left overflow-hidden shadow-2xl transform transition-all sm:my-8 sm:align-middle sm:max-w-lg sm:w-full">
                <div class="p-6" id="modalContent">
                    <!-- Populated dynamically -->
                </div>
            </div>
        </div>
    </div>

    <!-- AOS Animation Library JS -->
    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        // Initialize AOS animations
        AOS.init({
            duration: 800,
            once: true
        });

        // KOTTU KADE Menu Data (Strictly 3 Specified Items)
        const menuProducts = [
            {
                id: 'c1',
                name: 'Cheese Chicken Kottu',
                sinhalaName: 'චීස් චිකන් කොත්තු',
                price: 1650,
                rating: 4.9,
                badge: 'BESTSELLER',
                badgeColor: 'bg-brand-orange',
                image: 'https://images.unsplash.com/photo-1585238342024-78d387f4a707?auto=format&fit=crop&w=600&q=80',
                description: 'Tender seasoned chicken cubes mixed with fresh shredded roti, veggies & drowned in rich creamy melting mozzarella cheese.',
                ingredients: ['Crispy Roti', 'Spicy Chicken', 'Double Mozzarella', 'Secret Gravy']
            },
            {
                id: 'c2',
                name: 'Cheese Fish Kottu',
                sinhalaName: 'චීස් ෆිෂ් කොත්තු',
                price: 1550,
                rating: 4.8,
                badge: 'CHEF SPECIAL',
                badgeColor: 'bg-brand-yellow text-slate-950',
                image: 'https://images.unsplash.com/photo-1534422298391-e4f8c172dddb?auto=format&fit=crop&w=600&q=80',
                description: 'Deep-fried spicy fish pieces chopped live on the hot griddle with scrambled eggs, melted cheese & fiery Lankan spices.',
                ingredients: ['Fried Spicy Fish', 'Melted Cheese', 'Eggs & Onions', 'Hot Gravy']
            },
            {
                id: 'c3',
                name: 'Cheese Vegetable Kottu',
                sinhalaName: 'චීස් වෙජිටබල් කොත්තු',
                price: 1250,
                rating: 4.7,
                badge: 'HEALTHY & CHEESY',
                badgeColor: 'bg-emerald-500',
                image: 'https://images.unsplash.com/photo-1540420773420-3366772f4999?auto=format&fit=crop&w=600&q=80',
                description: 'Loaded with fresh carrots, leeks, cabbage, sweetcorn & extra heavy cheese layer. A vegetarian dream come true!',
                ingredients: ['Fresh Veggies', 'Sweetcorn', 'Creamy Cheese', 'Mild Spice']
            }
        ];

        // Shopping Cart State
        let cart = [];
        let activeModalItem = null;

        // Render Menu Items
        function renderMenu() {
            const container = document.getElementById('menuItemsContainer');
            container.innerHTML = menuProducts.map(item => `
                <div class="glass-panel rounded-3xl overflow-hidden border border-gray-800 hover:border-brand-orange/60 transition-all duration-300 flex flex-col justify-between group" data-aos="fade-up">
                    <div>
                        <!-- Image Container -->
                        <div class="relative h-56 overflow-hidden">
                            <img src="${item.image}" alt="${item.name}" class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                            <span class="absolute top-4 left-4 ${item.badgeColor} text-white font-extrabold text-xs px-3 py-1.5 rounded-full uppercase tracking-wider shadow-md">
                                ${item.badge}
                            </span>
                            <div class="absolute bottom-3 right-3 bg-slate-950/80 backdrop-blur-md px-3 py-1 rounded-xl border border-gray-700 text-brand-yellow text-xs font-bold flex items-center gap-1">
                                <i class="fa-solid fa-star"></i> ${item.rating}
                            </div>
                        </div>

                        <!-- Details -->
                        <div class="p-6">
                            <div class="flex justify-between items-start mb-2">
                                <div>
                                    <h3 class="font-heading font-extrabold text-xl text-white group-hover:text-brand-orange transition-colors">${item.name}</h3>
                                    <p class="text-xs text-brand-yellow font-semibold">${item.sinhalaName}</p>
                                </div>
                            </div>
                            <p class="text-gray-400 text-sm mb-4 leading-relaxed">${item.description}</p>
                            
                            <!-- Tags -->
                            <div class="flex flex-wrap gap-1.5 mb-6">
                                ${item.ingredients.map(ing => `
                                    <span class="bg-gray-800 text-gray-300 text-xs px-2.5 py-1 rounded-lg border border-gray-700/50">${ing}</span>
                                `).join('')}
                            </div>
                        </div>
                    </div>

                    <!-- Price & Action -->
                    <div class="p-6 pt-0 flex items-center justify-between border-t border-gray-800/60 mt-auto">
                        <div>
                            <span class="text-xs text-gray-400 block">Price</span>
                            <span class="font-heading font-black text-2xl text-white">Rs. ${item.price}</span>
                        </div>
                        <button onclick="openCustomizeModal('${item.id}')" class="px-5 py-3 rounded-xl bg-gradient-to-r from-brand-orange to-amber-500 text-white font-bold text-sm hover:opacity-90 transition-all shadow-md flex items-center gap-2 glow-effect">
                            <i class="fa-solid fa-plus"></i> Order
                        </button>
                    </div>
                </div>
            `).join('');
        }

        // Open Customization Modal
        function openCustomizeModal(itemId) {
            const item = menuProducts.find(p => p.id === itemId);
            if (!item) return;

            activeModalItem = item;
            const modalContent = document.getElementById('modalContent');

            modalContent.innerHTML = `
                <div class="flex justify-between items-start mb-4">
                    <div>
                        <h3 class="font-heading font-black text-2xl text-white">${item.name}</h3>
                        <p class="text-brand-yellow text-sm font-semibold">${item.sinhalaName}</p>
                    </div>
                    <button onclick="closeModal()" class="text-gray-400 hover:text-white text-xl p-1">
                        <i class="fa-solid fa-xmark"></i>
                    </button>
                </div>

                <div class="space-y-5 my-6">
                    <!-- Spice Level Selection -->
                    <div>
                        <label class="block text-sm font-bold text-gray-300 mb-2"><i class="fa-solid fa-pepper-hot text-brand-orange mr-1"></i> Spice Level (මිරිස් ප්‍රමාණය)</label>
                        <div class="grid grid-cols-3 gap-2">
                            <button type="button" onclick="selectOption('spice', 'Normal')" class="spice-btn bg-brand-orange text-white border-brand-orange p-2.5 rounded-xl border text-xs font-bold transition-all text-center">Normal</button>
                            <button type="button" onclick="selectOption('spice', 'Extra Spicy')" class="spice-btn bg-gray-800 text-gray-300 border-gray-700 p-2.5 rounded-xl border text-xs font-bold transition-all text-center">Extra Spicy 🌶️</button>
                            <button type="button" onclick="selectOption('spice', 'Nai Miris Hot')" class="spice-btn bg-gray-800 text-gray-300 border-gray-700 p-2.5 rounded-xl border text-xs font-bold transition-all text-center">Nai Miris 🔥</button>
                        </div>
                    </div>

                    <!-- Cheese Level Option -->
                    <div>
                        <label class="block text-sm font-bold text-gray-300 mb-2"><i class="fa-solid fa-cheese text-brand-yellow mr-1"></i> Extra Cheese Option</label>
                        <div class="grid grid-cols-2 gap-2">
                            <button type="button" onclick="selectOption('cheese', 'Standard Cheese')" class="cheese-btn bg-brand-orange text-white border-brand-orange p-2.5 rounded-xl border text-xs font-bold transition-all text-center">Standard Cheese</button>
                            <button type="button" onclick="selectOption('cheese', 'Double Cheese Layer (+Rs.300)')" class="cheese-btn bg-gray-800 text-gray-300 border-gray-700 p-2.5 rounded-xl border text-xs font-bold transition-all text-center">Double Cheese (+Rs.300)</button>
                        </div>
                    </div>

                    <!-- Extra Notes -->
                    <div>
                        <label class="block text-sm font-bold text-gray-300 mb-2">Special Instructions (වෙනත් ඉල්ලීම්)</label>
                        <input type="text" id="modalNotes" placeholder="eg: Gravy separate danna / Less salt..." class="w-full bg-gray-800 border border-gray-700 rounded-xl p-3 text-sm text-white focus:outline-none focus:border-brand-orange">
                    </div>
                </div>

                <div class="flex items-center justify-between border-t border-gray-800 pt-4 mt-6">
                    <div>
                        <span class="text-xs text-gray-400 block">Unit Price</span>
                        <span class="font-heading font-black text-xl text-brand-yellow">Rs. ${item.price}</span>
                    </div>
                    <button onclick="confirmAddToCart()" class="px-6 py-3 rounded-xl bg-gradient-to-r from-brand-orange to-amber-500 text-white font-extrabold text-sm hover:opacity-90 transition-all shadow-lg glow-effect">
                        Add To Cart
                    </button>
                </div>
            `;

            // Set temporary selection states
            window.selectedOptions = {
                spice: 'Normal',
                cheese: 'Standard Cheese'
            };

            document.getElementById('customizeModal').classList.remove('hidden');
        }

        // Handle customizer selection buttons UI
        function selectOption(type, value) {
            window.selectedOptions[type] = value;
            const buttons = document.querySelectorAll(`.${type}-btn`);
            buttons.forEach(btn => {
                if(btn.innerText.includes(value.split(' ')[0])) {
                    btn.className = `${type}-btn bg-brand-orange text-white border-brand-orange p-2.5 rounded-xl border text-xs font-bold transition-all text-center`;
                } else {
                    btn.className = `${type}-btn bg-gray-800 text-gray-300 border-gray-700 p-2.5 rounded-xl border text-xs font-bold transition-all text-center`;
                }
            });
        }

        function closeModal() {
            document.getElementById('customizeModal').classList.add('hidden');
        }

        // Add Customized Item to Cart
        function confirmAddToCart() {
            if (!activeModalItem) return;

            const notes = document.getElementById('modalNotes').value;
            let finalPrice = activeModalItem.price;

            if (window.selectedOptions.cheese.includes('+Rs.300')) {
                finalPrice += 300;
            }

            const cartItem = {
                cartId: Date.now(),
                id: activeModalItem.id,
                name: activeModalItem.name,
                basePrice: activeModalItem.price,
                price: finalPrice,
                spice: window.selectedOptions.spice,
                cheese: window.selectedOptions.cheese,
                notes: notes,
                qty: 1
            };

            cart.push(cartItem);
            updateCartUI();
            closeModal();

            // Trigger Confetti Effect
            confetti({
                particleCount: 50,
                spread: 60,
                origin: { y: 0.8 }
            });

            // Auto Open Cart Drawer
            toggleCartDrawer(true);
        }

        // Toggle Cart Drawer Visibility
        function toggleCartDrawer(forceOpen = false) {
            const drawer = document.getElementById('cartDrawer');
            if (forceOpen) {
                drawer.classList.remove('hidden');
            } else {
                drawer.classList.toggle('hidden');
            }
        }

        // Update Cart Interface
        function updateCartUI() {
            const list = document.getElementById('cartItemsList');
            const badge = document.getElementById('cartBadge');
            const totalItemsCount = document.getElementById('totalItemsCount');
            const totalPrice = document.getElementById('totalPrice');

            const totalQty = cart.reduce((acc, item) => acc + item.qty, 0);
            const totalAmount = cart.reduce((acc, item) => acc + (item.price * item.qty), 0);

            // Badge counter
            if (totalQty > 0) {
                badge.innerText = totalQty;
                badge.classList.remove('hidden', 'scale-0');
                badge.classList.add('scale-100');
            } else {
                badge.classList.add('hidden', 'scale-0');
            }

            totalItemsCount.innerText = totalQty;
            totalPrice.innerText = `Rs. ${totalAmount}`;

            if (cart.length === 0) {
                list.innerHTML = `
                    <div class="text-center py-12 text-gray-500">
                        <i class="fa-solid fa-basket-shopping text-5xl mb-4 text-gray-700"></i>
                        <p class="font-semibold text-gray-400">Your basket is empty, machan!</p>
                        <p class="text-xs mt-1">Select a cheese kottu from the menu to start ordering.</p>
                    </div>
                `;
                return;
            }

            list.innerHTML = cart.map(item => `
                <div class="p-4 bg-gray-800/80 rounded-2xl border border-gray-700/60 flex flex-col justify-between gap-3">
                    <div class="flex justify-between items-start">
                        <div>
                            <h4 class="font-bold text-white text-base">${item.name}</h4>
                            <div class="text-xs text-brand-yellow font-medium mt-0.5">
                                ${item.spice} | ${item.cheese}
                            </div>
                            ${item.notes ? `<p class="text-xs text-gray-400 italic mt-1">"${item.notes}"</p>` : ''}
                        </div>
                        <button onclick="removeFromCart(${item.cartId})" class="text-gray-500 hover:text-red-400 transition-colors p-1">
                            <i class="fa-solid fa-trash-can"></i>
                        </button>
                    </div>

                    <div class="flex justify-between items-center border-t border-gray-700/50 pt-3 mt-1">
                        <div class="flex items-center gap-3 bg-gray-900 px-3 py-1 rounded-xl border border-gray-700">
                            <button onclick="changeQty(${item.cartId}, -1)" class="text-gray-400 hover:text-white font-bold text-lg">-</button>
                            <span class="text-sm font-bold text-white">${item.qty}</span>
                            <button onclick="changeQty(${item.cartId}, 1)" class="text-gray-400 hover:text-white font-bold text-lg">+</button>
                        </div>
                        <span class="font-heading font-black text-brand-yellow">Rs. ${item.price * item.qty}</span>
                    </div>
                </div>
            `).join('');
        }

        function changeQty(cartId, delta) {
            const item = cart.find(i => i.cartId === cartId);
            if (!item) return;

            item.qty += delta;
            if (item.qty <= 0) {
                cart = cart.filter(i => i.cartId !== cartId);
            }
            updateCartUI();
        }

        function removeFromCart(cartId) {
            cart = cart.filter(i => i.cartId !== cartId);
            updateCartUI();
        }

        // Send Order Direct to Owner WhatsApp
        function sendWhatsAppOrder() {
            if (cart.length === 0) {
                alert('Machan, basket eka empty! Kotiuk item ekak select karala inna.');
                return;
            }

            const name = document.getElementById('custName').value.trim();
            const address = document.getElementById('custAddress').value.trim();

            if (!name || !address) {
                alert('Karunakarala oyage Nama saha Delivery Address eka fill karanna, machan!');
                return;
            }

            // KOTTU KADE Phone Number (Replace with owner real number)
            const phoneNumber = '94771234567'; 

            let message = `*NEW ORDER - KOTTU KADE* 🧀🔥\n\n`;
            message += `*Customer Name:* ${name}\n`;
            message += `*Address:* ${address}\n\n`;
            message += `*ORDER ITEMS:*\n`;

            let grandTotal = 0;
            cart.forEach((item, index) => {
                const itemTotal = item.price * item.qty;
                grandTotal += itemTotal;
                message += `${index + 1}. *${item.name}* x ${item.qty}\n`;
                message += `   • Option: ${item.spice}, ${item.cheese}\n`;
                if(item.notes) message += `   • Note: ${item.notes}\n`;
                message += `   • Subtotal: Rs. ${itemTotal}\n\n`;
            });

            message += `*GRAND TOTAL:* Rs. ${grandTotal}\n\n`;
            message += `Please confirm my Kottu order machan!`;

            const encodedURL = `https://wa.me/${phoneNumber}?text=${encodeURIComponent(message)}`;
            window.open(encodedURL, '_blank');
        }

        // Initialize script execution on DOM Ready
        window.addEventListener('DOMContentLoaded', () => {
            renderMenu();
        });
    </script>
</body>
</html>
