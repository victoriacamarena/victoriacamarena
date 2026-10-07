<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Helloooo, I am Victoria | Portfolio</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts: Montserrat, Quicksand, Caveat (handwritten) -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Caveat:wght@600&family=Montserrat:ital,wght@0,300;0,400;0,500;0,600;0,700;1,400&family=Quicksand:wght@400;500;600;700&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        brand: {
                            navy: '#1A3B5C',
                            blue: '#0F2C59',
                            sky: '#DDF0FF',
                            softBlue: '#CBE5FF',
                            pill: '#CDE5F7',
                            pillDark: '#2C537A',
                            text: '#223843',
                            subtext: '#4A6B82',
                            tagBg: '#D6ECFA',
                            tagText: '#3B729E'
                        }
                    },
                    fontFamily: {
                        sans: ['Quicksand', 'Montserrat', 'sans-serif'],
                        heading: ['Montserrat', 'sans-serif'],
                        handwritten: ['Caveat', 'cursive']
                    }
                }
            }
        }
    </script>

    <style>
        body {
            background-color: #F8FBFE;
            color: #223843;
            font-family: 'Quicksand', sans-serif;
            overflow-x: hidden;
        }

        .heading-font {
            font-family: 'Montserrat', sans-serif;
        }

        .handwritten-font {
            font-family: 'Caveat', cursive;
        }

        /* Sparkle float animation */
        @keyframes sparkle-float {
            0%, 100% { transform: translateY(0px) rotate(0deg); opacity: 0.8; }
            50% { transform: translateY(-4px) rotate(8deg); opacity: 1; }
        }

        .sparkle-anim {
            display: inline-block;
            animation: sparkle-float 3s ease-in-out infinite;
        }

        /* Hero text glow */
        .hero-glow {
            text-shadow: 0 0 15px rgba(255, 255, 255, 0.4), 0 0 30px rgba(100, 200, 255, 0.3);
        }

        /* Soft card shadow */
        .soft-card-shadow {
            box-shadow: 0 10px 30px -5px rgba(160, 195, 225, 0.25);
        }

        /* Custom scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #f1f5f9;
        }
        ::-webkit-scrollbar-thumb {
            background: #93c5fd;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #60a5fa;
        }
    </style>
</head>
<body class="min-h-screen flex flex-col items-center justify-start pb-12 antialiased">

    <!-- Top Action Bar for GitHub Markdown Export & Interactivity -->
    <div class="w-full bg-white/80 backdrop-blur-md border-b border-sky-100 sticky top-0 z-50 py-3 px-4 shadow-sm">
        <div class="max-w-4xl mx-auto flex flex-wrap items-center justify-between gap-3 text-xs sm:text-sm">
            <div class="flex items-center gap-2 font-medium text-slate-600">
                <i class="fa-brands fa-github text-lg text-slate-800"></i>
                <span>Victoria's Profile Readme Webview</span>
            </div>
            <div class="flex items-center gap-2">
                <button onclick="openExportModal()" class="flex items-center gap-1.5 px-3 py-1.5 bg-sky-500 hover:bg-sky-600 text-white rounded-full font-medium transition shadow-sm hover:shadow active:scale-95">
                    <i class="fa-regular fa-copy"></i>
                    <span>Get README Markdown</span>
                </button>
            </div>
        </div>
    </div>

    <!-- Main Container styled to emulate the graphic aesthetic precisely -->
    <div class="w-full max-w-4xl bg-white shadow-2xl my-0 sm:my-6 rounded-none sm:rounded-3xl overflow-hidden border border-slate-100 relative">

        <!-- ================= HERO SECTION ================= -->
        <header class="relative w-full h-[380px] sm:h-[460px] md:h-[500px] overflow-hidden bg-slate-900 select-none">
            <!-- Background Image with Northern Lights Aurora & Reflective Water -->
            <img 
                src="https://thehoneymoonboutiquemx.com/wp-content/uploads/2024/09/1-experience-northern-lights.webp" 
                alt="Northern Lights Aurora Borealis Over Snowy Mountains" 
                class="w-full h-full object-cover object-center scale-105 transform hover:scale-100 transition-transform duration-1000 ease-out"
                onerror="this.onerror=null; this.src='https://images.unsplash.com/photo-1531366936337-7c912a4589a7?q=80&w=1600&auto=format&fit=crop';"
            />
            
            <!-- Atmospheric Gradient Overlays for contrast and color depth -->
            <div class="absolute inset-0 bg-gradient-to-b from-sky-900/30 via-transparent to-slate-900/60"></div>
            
            <!-- Decorative SVG Stars/Sparkles overlay -->
            <svg class="absolute top-8 left-12 w-6 h-6 opacity-80 text-cyan-200 sparkle-anim" viewBox="0 0 24 24" fill="currentColor">
                <path d="M12 0L14.59 9.41L24 12L14.59 14.59L12 24L9.41 14.59L0 12L9.41 9.41L12 0Z"/>
            </svg>
            <svg class="absolute top-24 right-16 w-8 h-8 opacity-90 text-sky-100 sparkle-anim" style="animation-delay: 1s;" viewBox="0 0 24 24" fill="currentColor">
                <path d="M12 0L14.59 9.41L24 12L14.59 14.59L12 24L9.41 14.59L0 12L9.41 9.41L12 0Z"/>
            </svg>

            <!-- Centered Header Text Content -->
            <div class="absolute inset-0 flex flex-col items-center justify-start pt-12 sm:pt-16 md:pt-20 text-center px-4 z-10 text-white">
                <h1 class="heading-font text-3xl sm:text-5xl md:text-6xl font-normal tracking-wide hero-glow mb-1 drop-shadow-lg">
                    Helloooo,
                </h1>
                
                <div class="flex items-center justify-center gap-2 mt-1 sm:mt-2">
                    <span class="text-lg sm:text-2xl font-light opacity-90 tracking-wide italic">I am</span>
                    <span class="heading-font text-4xl sm:text-6xl md:text-7xl font-bold tracking-tight text-white drop-shadow-xl ml-1">
                        Victoria
                    </span>
                    <!-- Sparkle next to Victoria -->
                    <svg class="w-5 h-5 sm:w-7 sm:h-7 text-white sparkle-anim ml-1" viewBox="0 0 24 24" fill="currentColor">
                        <path d="M12 0L14.59 9.41L24 12L14.59 14.59L12 24L9.41 14.59L0 12L9.41 9.41L12 0Z"/>
                    </svg>
                </div>

                <!-- Curved swoosh line SVG beneath Victoria -->
                <svg class="w-48 sm:w-72 h-4 my-2 opacity-80" viewBox="0 0 250 20" fill="none" stroke="white" stroke-width="1.5">
                    <path d="M 5 12 Q 125 -5 245 12" stroke-linecap="round"/>
                </svg>

                <p class="text-xs sm:text-sm md:text-base font-light tracking-widest text-sky-100 opacity-95 uppercase mt-1">
                    a little corner of my creativity
                </p>
            </div>
        </header>

        <!-- ================= MAIN CONTENT WRAPPER ================= -->
        <main class="px-6 sm:px-12 md:px-16 py-10 bg-[#FAFDFE] space-y-12">

            <!-- 1. ABOUT ME SECTION -->
            <section class="grid grid-cols-1 md:grid-cols-12 gap-8 items-center pt-2">
                <!-- Left Column Text -->
                <div class="md:col-span-7 space-y-4">
                    <div class="flex items-center gap-3">
                        <h2 class="heading-font text-2xl sm:text-3xl font-bold text-[#1A3B5C]">
                            About me
                        </h2>
                        <div class="h-[1.5px] w-12 bg-[#9AC5E8]"></div>
                        <svg class="w-4 h-4 text-[#79B4E2] sparkle-anim" viewBox="0 0 24 24" fill="currentColor">
                            <path d="M12 0L14.59 9.41L24 12L14.59 14.59L12 24L9.41 14.59L0 12L9.41 9.41L12 0Z"/>
                        </svg>
                    </div>

                    <p class="text-slate-600 leading-relaxed text-sm sm:text-base font-medium pr-0 md:pr-4">
                        I’m Victoria, a creative and curious student. I love reading, adventures and makeup, and I enjoy turning ideas into projects that have a purpose.
                    </p>
                </div>

                <!-- Right Column Stacked Aesthetic Image & Sticky Note -->
                <div class="md:col-span-5 relative flex justify-center md:justify-end mt-4 md:mt-0">
                    <div class="relative group">
                        <!-- Main Stacked Books Image -->
                        <div class="w-64 sm:w-72 rounded-2xl overflow-hidden shadow-lg border-4 border-white transform transition duration-500 hover:scale-[1.02]">
                            <img 
                                src="https://images.unsplash.com/photo-1544716278-ca5e3f4abd8c?q=80&w=800&auto=format&fit=crop" 
                                alt="Stack of books and coffee cup" 
                                class="w-full h-56 object-cover"
                                onerror="this.onerror=null; this.src='https://images.unsplash.com/photo-1512820790803-83ca734da794?q=80&w=800&auto=format&fit=crop';"
                            />
                            <!-- Overlay book text effect matching reference -->
                            <div class="absolute inset-0 bg-gradient-to-t from-slate-900/60 via-transparent to-transparent flex flex-col justify-end p-3 text-white text-xs font-medium space-y-0.5">
                                <span class="bg-white/20 backdrop-blur-xs px-2 py-0.5 rounded text-[11px] w-max">Better Things Ahead</span>
                                <span class="bg-white/20 backdrop-blur-xs px-2 py-0.5 rounded text-[11px] w-max">Good Energy</span>
                                <span class="bg-white/20 backdrop-blur-xs px-2 py-0.5 rounded text-[11px] w-max">For a kinder tomorrow ♡</span>
                            </div>
                        </div>

                        <!-- Sticky Note Overlay -->
                        <div class="absolute -bottom-6 -right-4 sm:-right-6 bg-[#EBF4FA] border border-sky-200/60 p-4 rounded-xl shadow-md w-36 transform rotate-6 transition duration-300 hover:rotate-0 hover:scale-105 z-10">
                            <!-- Blue tape on top -->
                            <div class="absolute -top-2.5 left-1/2 -translate-x-1/2 w-10 h-3 bg-[#89BCE6]/70 rounded-xs"></div>
                            <p class="handwritten-font text-xl text-[#2B5278] text-center leading-tight pt-1">
                                same girl<br>bigger<br>dreams<br>
                                <span class="text-lg">♡</span>
                            </p>
                        </div>

                        <!-- Decorative floating sparkles around picture -->
                        <svg class="absolute -top-4 -left-6 w-5 h-5 text-sky-400 sparkle-anim" viewBox="0 0 24 24" fill="currentColor">
                            <path d="M12 0L14.59 9.41L24 12L14.59 14.59L12 24L9.41 14.59L0 12L9.41 9.41L12 0Z"/>
                        </svg>
                        <svg class="absolute top-1/2 -left-8 w-4 h-4 text-sky-300 sparkle-anim" style="animation-delay: 1.5s;" viewBox="0 0 24 24" fill="currentColor">
                            <path d="M12 0L14.59 9.41L24 12L14.59 14.59L12 24L9.41 14.59L0 12L9.41 9.41L12 0Z"/>
                        </svg>
                    </div>
                </div>
            </section>


            <!-- 2. SKILLS SECTION -->
            <section class="space-y-4 pt-4">
                <div class="flex items-center gap-3">
                    <h2 class="heading-font text-2xl sm:text-3xl font-bold text-[#1A3B5C]">
                        Skills
                    </h2>
                    <div class="h-[1.5px] w-12 bg-[#9AC5E8]"></div>
                    <svg class="w-4 h-4 text-[#79B4E2] sparkle-anim" viewBox="0 0 24 24" fill="currentColor">
                        <path d="M12 0L14.59 9.41L24 12L14.59 14.59L12 24L9.41 14.59L0 12L9.41 9.41L12 0Z"/>
                    </svg>
                </div>

                <!-- Line Doodle Left Side -->
                <div class="relative flex flex-wrap items-center gap-4 pt-2">
                    <!-- Left Doodle Accent -->
                    <div class="hidden lg:block absolute -left-12 top-1/2 -translate-y-1/2 text-sky-300 opacity-80">
                        <svg class="w-8 h-8" viewBox="0 0 50 50" fill="none" stroke="currentColor" stroke-width="2">
                            <path d="M 10 25 C 20 10, 30 40, 40 25"/>
                            <path d="M 35 20 C 40 25, 40 30, 35 30 C 30 30, 30 20, 35 20"/>
                        </svg>
                    </div>

                    <!-- Skill 1: Python -->
                    <div class="flex items-center gap-3 bg-[#DDF0FF] hover:bg-[#D2E9FD] transition-all px-5 py-3 rounded-2xl w-full sm:w-auto min-w-[200px] shadow-sm hover:shadow border border-sky-100 cursor-pointer group">
                        <div class="w-10 h-10 rounded-xl bg-white/80 flex items-center justify-center text-sky-600 text-2xl group-hover:scale-110 transition-transform">
                            <i class="fa-brands fa-python text-[#3776AB]"></i>
                        </div>
                        <div class="text-left">
                            <p class="font-bold text-[#1D3E60] text-sm leading-tight">Python</p>
                            <p class="text-xs text-[#4B7095] font-medium">Essential 1</p>
                        </div>
                    </div>

                    <!-- Skill 2: Excel -->
                    <div class="flex items-center gap-3 bg-[#DDF0FF] hover:bg-[#D2E9FD] transition-all px-5 py-3 rounded-2xl w-full sm:w-auto min-w-[180px] shadow-sm hover:shadow border border-sky-100 cursor-pointer group">
                        <div class="w-10 h-10 rounded-xl bg-white/80 flex items-center justify-center text-emerald-600 text-2xl group-hover:scale-110 transition-transform">
                            <i class="fa-regular fa-file-excel text-[#1D6F42]"></i>
                        </div>
                        <div class="text-left">
                            <p class="font-bold text-[#1D3E60] text-sm leading-tight">Excel</p>
                        </div>
                    </div>

                    <!-- Skill 3: Excel Expert -->
                    <div class="flex items-center gap-3 bg-[#DDF0FF] hover:bg-[#D2E9FD] transition-all px-5 py-3 rounded-2xl w-full sm:w-auto min-w-[180px] shadow-sm hover:shadow border border-sky-100 cursor-pointer group">
                        <div class="w-10 h-10 rounded-xl bg-white/80 flex items-center justify-center text-emerald-600 text-2xl group-hover:scale-110 transition-transform">
                            <i class="fa-solid fa-file-excel text-[#1D6F42]"></i>
                        </div>
                        <div class="text-left">
                            <p class="font-bold text-[#1D3E60] text-sm leading-tight">Excel</p>
                            <p class="text-xs text-[#4B7095] font-medium">Expert</p>
                        </div>
                    </div>

                    <!-- Right Doodle Accent -->
                    <div class="hidden lg:block absolute right-0 top-1/2 -translate-y-1/2 text-sky-300 opacity-80">
                        <svg class="w-10 h-10" viewBox="0 0 50 50" fill="none" stroke="currentColor" stroke-width="2">
                            <path d="M 5 35 C 20 10, 30 40, 45 15"/>
                            <path d="M 38 10 C 45 15, 45 22, 38 20"/>
                        </svg>
                    </div>
                </div>
            </section>


            <!-- 3. PROJECTS SECTION -->
            <section class="space-y-6 pt-2">
                <div class="flex items-center gap-3">
                    <h2 class="heading-font text-2xl sm:text-3xl font-bold text-[#1A3B5C]">
                        Projects
                    </h2>
                    <div class="h-[1.5px] w-12 bg-[#9AC5E8]"></div>
                    <svg class="w-4 h-4 text-[#79B4E2] sparkle-anim" viewBox="0 0 24 24" fill="currentColor">
                        <path d="M12 0L14.59 9.41L24 12L14.59 14.59L12 24L9.41 14.59L0 12L9.41 9.41L12 0Z"/>
                    </svg>
                </div>

                <!-- Projects Two Column Grid -->
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8 relative">
                    
                    <!-- Vertical Divider Line for Desktop -->
                    <div class="hidden md:block absolute left-1/2 top-2 bottom-2 w-[1.5px] bg-sky-200 -translate-x-1/2"></div>

                    <!-- Project 1: Flora Papel -->
                    <div class="space-y-3 pr-0 md:pr-4 group cursor-pointer" onclick="showProjectDetails('Flora Papel', 'Handmade paper embedded with wildflowers and native seeds that can be planted after use to grow flowers.')">
                        <h3 class="heading-font text-xl font-bold text-[#1D3E60] group-hover:text-sky-600 transition-colors flex items-center gap-2">
                            Flora Papel
                            <i class="fa-solid fa-arrow-up-right-from-square text-xs opacity-0 group-hover:opacity-100 transition-opacity"></i>
                        </h3>
                        <p class="text-slate-600 text-sm font-medium">
                            Handmade paper with seeds.
                        </p>
                        
                        <!-- Tags -->
                        <div class="flex flex-wrap gap-2 pt-1">
                            <span class="bg-[#D6ECFA] text-[#3B729E] text-xs font-semibold px-3 py-1 rounded-full border border-sky-100">
                                Sustainability
                            </span>
                            <span class="bg-[#D6ECFA] text-[#3B729E] text-xs font-semibold px-3 py-1 rounded-full border border-sky-100">
                                Nature
                            </span>
                            <span class="bg-[#D6ECFA] text-[#3B729E] text-xs font-semibold px-3 py-1 rounded-full border border-sky-100">
                                Creativity
                            </span>
                        </div>
                    </div>

                    <!-- Project 2: Panaroot -->
                    <div class="space-y-3 pl-0 md:pl-6 group cursor-pointer" onclick="showProjectDetails('Panaroot', 'A high-impact photography & design showcase highlighting the rich culture, natural reserves, and vibrant tourism spots of Panama.')">
                        <h3 class="heading-font text-xl font-bold text-[#1D3E60] group-hover:text-sky-600 transition-colors flex items-center gap-2">
                            Panaroot
                            <i class="fa-solid fa-arrow-up-right-from-square text-xs opacity-0 group-hover:opacity-100 transition-opacity"></i>
                        </h3>
                        <p class="text-slate-600 text-sm font-medium">
                            A visual project that showcases Panama.
                        </p>
                        
                        <!-- Tags -->
                        <div class="flex flex-wrap gap-2 pt-1">
                            <span class="bg-[#D6ECFA] text-[#3B729E] text-xs font-semibold px-3 py-1 rounded-full border border-sky-100">
                                Tourism
                            </span>
                            <span class="bg-[#D6ECFA] text-[#3B729E] text-xs font-semibold px-3 py-1 rounded-full border border-sky-100">
                                Culture
                            </span>
                            <span class="bg-[#D6ECFA] text-[#3B729E] text-xs font-semibold px-3 py-1 rounded-full border border-sky-100">
                                Design
                            </span>
                        </div>
                    </div>

                </div>
            </section>


            <!-- 4. THINGS I LOVE SECTION -->
            <section class="space-y-6 pt-4">
                <div class="flex items-center gap-3">
                    <h2 class="heading-font text-2xl sm:text-3xl font-bold text-[#1A3B5C]">
                        Things I love
                    </h2>
                    <div class="h-[1.5px] w-12 bg-[#9AC5E8]"></div>
                    <svg class="w-4 h-4 text-[#79B4E2] sparkle-anim" viewBox="0 0 24 24" fill="currentColor">
                        <path d="M12 0L14.59 9.41L24 12L14.59 14.59L12 24L9.41 14.59L0 12L9.41 9.41L12 0Z"/>
                    </svg>
                </div>

                <!-- 4 Thumbnails Side by Side Grid -->
                <div class="grid grid-cols-2 sm:grid-cols-4 gap-4 sm:gap-5">
                    
                    <!-- Love Item 1: READING -->
                    <div class="space-y-2 group text-center cursor-pointer">
                        <div class="h-36 sm:h-40 rounded-2xl overflow-hidden border-2 border-white shadow-md group-hover:shadow-xl transition-all duration-300 transform group-hover:-translate-y-1">
                            <img 
                                src="https://images.unsplash.com/photo-1512820790803-83ca734da794?q=80&w=500&auto=format&fit=crop" 
                                alt="Reading open book" 
                                class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500"
                            />
                        </div>
                        <p class="heading-font text-xs sm:text-sm font-bold tracking-widest text-[#23476E] uppercase pt-1">
                            READING
                        </p>
                    </div>

                    <!-- Love Item 2: ADVENTURES -->
                    <div class="space-y-2 group text-center cursor-pointer">
                        <div class="h-36 sm:h-40 rounded-2xl overflow-hidden border-2 border-white shadow-md group-hover:shadow-xl transition-all duration-300 transform group-hover:-translate-y-1">
                            <img 
                                src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e?q=80&w=500&auto=format&fit=crop" 
                                alt="Adventures ocean view" 
                                class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500"
                            />
                        </div>
                        <p class="heading-font text-xs sm:text-sm font-bold tracking-widest text-[#23476E] uppercase pt-1">
                            ADVENTURES
                        </p>
                    </div>

                    <!-- Love Item 3: MAKEUP -->
                    <div class="space-y-2 group text-center cursor-pointer">
                        <div class="h-36 sm:h-40 rounded-2xl overflow-hidden border-2 border-white shadow-md group-hover:shadow-xl transition-all duration-300 transform group-hover:-translate-y-1">
                            <img 
                                src="https://images.unsplash.com/photo-1522337360788-8b13dee7a37e?q=80&w=500&auto=format&fit=crop" 
                                alt="Makeup brushes and palettes" 
                                class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500"
                            />
                        </div>
                        <p class="heading-font text-xs sm:text-sm font-bold tracking-widest text-[#23476E] uppercase pt-1">
                            MAKEUP
                        </p>
                    </div>

                    <!-- Love Item 4: CREATIVITY -->
                    <div class="space-y-2 group text-center cursor-pointer">
                        <div class="h-36 sm:h-40 rounded-2xl overflow-hidden border-2 border-white shadow-md group-hover:shadow-xl transition-all duration-300 transform group-hover:-translate-y-1">
                            <img 
                                src="https://images.unsplash.com/photo-1513364776144-60967b0f800f?q=80&w=500&auto=format&fit=crop" 
                                alt="Creativity sketchbook" 
                                class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500"
                            />
                        </div>
                        <p class="heading-font text-xs sm:text-sm font-bold tracking-widest text-[#23476E] uppercase pt-1">
                            CREATIVITY
                        </p>
                    </div>

                </div>
            </section>

        </main>

        <!-- ================= FOOTER SECTION ================= -->
        <footer class="relative bg-gradient-to-b from-[#FAFDFE] to-[#E3F2FC] pt-8 pb-12 px-6 text-center overflow-hidden border-t border-sky-100">
            
            <!-- Bottom Wavy Decorative Motif -->
            <div class="max-w-md mx-auto flex items-center justify-center gap-4 text-[#396F99] mb-4">
                <svg class="w-16 h-4 opacity-70" viewBox="0 0 100 20" fill="none" stroke="currentColor" stroke-width="1.5">
                    <path d="M 0 10 Q 25 0, 50 10 T 100 10" stroke-linecap="round"/>
                </svg>
                <svg class="w-4 h-4 text-sky-400 sparkle-anim" viewBox="0 0 24 24" fill="currentColor">
                    <path d="M12 0L14.59 9.41L24 12L14.59 14.59L12 24L9.41 14.59L0 12L9.41 9.41L12 0Z"/>
                </svg>
                
                <p class="heading-font text-xs sm:text-sm font-bold tracking-widest uppercase text-[#2B5780]">
                    CREATE &bull; DREAM &bull; DISCOVER
                </p>

                <svg class="w-4 h-4 text-sky-400 sparkle-anim" style="animation-delay: 1s;" viewBox="0 0 24 24" fill="currentColor">
                    <path d="M12 0L14.59 9.41L24 12L14.59 14.59L12 24L9.41 9.41L12 0Z"/>
                </svg>
                <svg class="w-16 h-4 opacity-70" viewBox="0 0 100 20" fill="none" stroke="currentColor" stroke-width="1.5">
                    <path d="M 0 10 Q 25 20, 50 10 T 100 10" stroke-linecap="round"/>
                </svg>
            </div>

            <!-- Hand-drawn Flower Doodle Overlay right corner -->
            <div class="absolute right-6 bottom-4 text-sky-400 opacity-60 hidden sm:block">
                <svg class="w-12 h-16" viewBox="0 0 60 80" fill="none" stroke="currentColor" stroke-width="1.5">
                    <path d="M 30 75 C 30 50, 30 40, 30 25"/>
                    <circle cx="30" cy="20" r="5" fill="currentColor"/>
                    <circle cx="30" cy="12" r="4"/>
                    <circle cx="38" cy="20" r="4"/>
                    <circle cx="30" cy="28" r="4"/>
                    <circle cx="22" cy="20" r="4"/>
                    <path d="M 30 50 C 40 45, 45 40, 42 35 C 35 35, 30 45, 30 50"/>
                </svg>
            </div>

            <p class="text-xs text-slate-400 font-medium mt-2">
                Designed with ♡ for Victoria's GitHub Profile README
            </p>
        </footer>

    </div>

    <!-- Modal for GitHub README Markdown Export -->
    <div id="exportModal" class="fixed inset-0 bg-slate-900/60 backdrop-blur-sm z-50 flex items-center justify-center p-4 opacity-0 pointer-events-none transition-opacity duration-300">
        <div class="bg-white rounded-2xl max-w-2xl w-full p-6 shadow-2xl border border-sky-100 transform scale-95 transition-transform duration-300 space-y-4" id="exportModalBox">
            <div class="flex items-center justify-between border-b border-slate-100 pb-3">
                <div class="flex items-center gap-2 text-slate-800 font-bold">
                    <i class="fa-brands fa-markdown text-sky-500 text-xl"></i>
                    <span>GitHub README.md Source Code</span>
                </div>
                <button onclick="closeExportModal()" class="text-slate-400 hover:text-slate-600 p-1">
                    <i class="fa-solid fa-xmark text-lg"></i>
                </button>
            </div>

            <p class="text-xs text-slate-500">
                Copy this Markdown code directly into your GitHub repository's <code class="bg-slate-100 text-sky-600 px-1 py-0.5 rounded">README.md</code> file to embed this graphic portfolio layout:
            </p>

            <textarea id="markdownCode" readonly class="w-full h-64 p-3 bg-slate-900 text-emerald-400 font-mono text-xs rounded-xl focus:outline-none resize-none border border-slate-800 leading-relaxed"></textarea>

            <div class="flex items-center justify-end gap-3 pt-2">
                <button onclick="closeExportModal()" class="px-4 py-2 text-xs font-semibold text-slate-600 hover:bg-slate-100 rounded-lg transition">
                    Close
                </button>
                <button onclick="copyMarkdownToClipboard()" class="px-5 py-2 text-xs font-semibold bg-sky-500 hover:bg-sky-600 text-white rounded-lg transition flex items-center gap-1.5 shadow-sm active:scale-95">
                    <i class="fa-regular fa-copy"></i>
                    <span id="copyBtnText">Copy Markdown</span>
                </button>
            </div>
        </div>
    </div>

    <!-- Notification Toast -->
    <div id="toast" class="fixed bottom-6 right-6 bg-slate-900 text-white text-xs px-4 py-3 rounded-xl shadow-xl flex items-center gap-2 transform translate-y-20 opacity-0 transition-all duration-300 z-50">
        <i class="fa-solid fa-circle-check text-emerald-400 text-base"></i>
        <span id="toastMsg">Code copied to clipboard!</span>
    </div>

    <!-- Interactive JavaScript Logic -->
    <script>
        // Generated Markdown content tailored for GitHub Profile
        const readmeMarkdown = `<div align="center">

  <!-- Header Banner -->
  <img src="https://thehoneymoonboutiquemx.com/wp-content/uploads/2024/09/1-experience-northern-lights.webp" width="100%" alt="Victoria Header Banner" style="border-radius: 12px;"/>

  # Helloooo, I am **Victoria** ✨
  *a little corner of my creativity*

</div>

---

### ✦ About me
I’m **Victoria**, a creative and curious student. I love reading, adventures and makeup, and I enjoy turning ideas into projects that have a purpose.

---

### ✦ Skills
- 🐍 **Python** - Essential 1
- 📊 **Microsoft Excel** - Intermediate
- 📈 **Microsoft Excel** - Expert

---

### ✦ Projects

| Project | Description | Tags |
| :--- | :--- | :--- |
| **Flora Papel** | Handmade paper with seeds embedded inside | \`Sustainability\` \`Nature\` \`Creativity\` |
| **Panaroot** | A visual photographic project that showcases Panama | \`Tourism\` \`Culture\` \`Design\` |

---

### ✦ Things I love
- 📖 **Reading**
- 🏔️ **Adventures**
- 💄 **Makeup**
- 🎨 **Creativity**

<br>

<div align="center">
  <sub>✦ CREATE · DREAM · DISCOVER ✦</sub>
</div>`;

        // Fill modal textarea on startup
        document.getElementById('markdownCode').value = readmeMarkdown;

        function openExportModal() {
            const modal = document.getElementById('exportModal');
            const modalBox = document.getElementById('exportModalBox');
            modal.classList.remove('opacity-0', 'pointer-events-none');
            modalBox.classList.remove('scale-95');
            modalBox.classList.add('scale-100');
        }

        function closeExportModal() {
            const modal = document.getElementById('exportModal');
            const modalBox = document.getElementById('exportModalBox');
            modal.classList.add('opacity-0', 'pointer-events-none');
            modalBox.classList.remove('scale-100');
            modalBox.classList.add('scale-95');
        }

        function copyMarkdownToClipboard() {
            const textarea = document.getElementById('markdownCode');
            textarea.select();
            document.execCommand('copy');

            const copyBtnText = document.getElementById('copyBtnText');
            copyBtnText.innerText = 'Copied!';
            
            showToast('GitHub Markdown copied to clipboard!');

            setTimeout(() => {
                copyBtnText.innerText = 'Copy Markdown';
            }, 2500);
        }

        function showProjectDetails(title, description) {
            showToast(`${title}: ${description}`);
        }

        function showToast(message) {
            const toast = document.getElementById('toast');
            const toastMsg = document.getElementById('toastMsg');
            toastMsg.innerText = message;
            
            toast.classList.remove('translate-y-20', 'opacity-0');
            
            setTimeout(() => {
                toast.classList.add('translate-y-20', 'opacity-0');
            }, 3500);
        }
    </script>
</body>
</html>
