<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Coder-o-cloud | Full Stack Developer</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        dark: '#0f172a',
                        primary: '#3b82f6',
                        secondary: '#8b5cf6',
                        accent: '#06b6d4'
                    },
                    animation: {
                        'blob': 'blob 7s infinite',
                        'fade-in': 'fadeIn 1s ease-out',
                        'slide-up': 'slideUp 0.8s ease-out',
                    },
                    keyframes: {
                        blob: {
                            '0%': { transform: 'translate(0px, 0px) scale(1)' },
                            '33%': { transform: 'translate(30px, -50px) scale(1.1)' },
                            '66%': { transform: 'translate(-20px, 20px) scale(0.9)' },
                            '100%': { transform: 'translate(0px, 0px) scale(1)' },
                        },
                        fadeIn: {
                            '0%': { opacity: '0' },
                            '100%': { opacity: '1' },
                        },
                        slideUp: {
                            '0%': { transform: 'translateY(20px)', opacity: '0' },
                            '100%': { transform: 'translateY(0)', opacity: '1' },
                        }
                    }
                }
            }
        }
    </script>
    <style>
        .glass {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        .text-gradient {
            background: linear-gradient(to right, #3b82f6, #8b5cf6, #06b6d4);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        /* Hide scrollbar for clean look */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #0f172a;
        }
        ::-webkit-scrollbar-thumb {
            background: #334155;
            border-radius: 4px;
        }
    </style>
</head>
<body class="bg-dark text-slate-200 font-sans antialiased selection:bg-primary selection:text-white overflow-x-hidden">

    <!-- Background Effects -->
    <div class="fixed inset-0 z-0 pointer-events-none overflow-hidden">
        <div class="absolute top-0 left-1/4 w-96 h-96 bg-primary/20 rounded-full mix-blend-screen filter blur-3xl opacity-30 animate-blob"></div>
        <div class="absolute top-0 right-1/4 w-96 h-96 bg-secondary/20 rounded-full mix-blend-screen filter blur-3xl opacity-30 animate-blob animation-delay-2000"></div>
        <div class="absolute -bottom-32 left-1/3 w-96 h-96 bg-accent/20 rounded-full mix-blend-screen filter blur-3xl opacity-30 animate-blob animation-delay-4000"></div>
    </div>

    <!-- Navigation -->
    <nav class="fixed w-full z-50 glass border-b border-white/10">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-16">
                <div class="flex items-center">
                    <span class="text-2xl font-bold text-gradient cursor-pointer" onclick="window.scrollTo(0,0)">
                        &lt;Coder-o-cloud/&gt;
                    </span>
                </div>
                <div class="hidden md:block">
                    <div class="ml-10 flex items-baseline space-x-4">
                        <a href="#about" class="hover:text-primary px-3 py-2 rounded-md text-sm font-medium transition-colors">About</a>
                        <a href="#stack" class="hover:text-primary px-3 py-2 rounded-md text-sm font-medium transition-colors">Tech Stack</a>
                        <a href="#projects" class="hover:text-primary px-3 py-2 rounded-md text-sm font-medium transition-colors">Projects</a>
                        <a href="#contact" class="bg-primary/20 hover:bg-primary/40 text-primary border border-primary/50 px-4 py-2 rounded-full text-sm font-medium transition-all">
                            Contact Me
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="about" class="relative z-10 min-h-screen flex items-center justify-center pt-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col md:flex-row items-center">
            <div class="md:w-1/2 text-center md:text-left mb-10 md:mb-0 animate-slide-up">
                <h2 class="text-accent font-semibold tracking-wide uppercase text-sm mb-2">Welcome to my universe</h2>
                <h1 class="text-5xl md:text-7xl font-bold mb-6">
                    Hi, I'm <span class="text-gradient">Coder-o-cloud</span>
                </h1>
                <p class="text-xl text-slate-400 mb-8 max-w-lg mx-auto md:mx-0">
                    A passionate <span class="text-white font-semibold">Frontend & Full Stack Developer</span> exploring the frontier where Web Development meets Artificial Intelligence.
                </p>
                <div class="flex flex-col sm:flex-row gap-4 justify-center md:justify-start">
                    <a href="#projects" class="px-8 py-3 bg-gradient-to-r from-primary to-secondary rounded-full font-semibold hover:shadow-lg hover:shadow-primary/50 transition-all transform hover:-translate-y-1 text-white">
                        View Projects
                    </a>
                    <a href="https://github.com/Coder-o-cloud" target="_blank" class="px-8 py-3 glass rounded-full font-semibold hover:bg-white/10 transition-all flex items-center justify-center gap-2">
                        <i class="fab fa-github"></i> GitHub Profile
                    </a>
                </div>
            </div>
            <div class="md:w-1/2 flex justify-center animate-fade-in">
                <div class="relative">
                    <div class="absolute -inset-1 bg-gradient-to-r from-primary to-secondary rounded-2xl blur opacity-30"></div>
                    <div class="relative glass p-8 rounded-2xl border border-white/10 max-w-sm w-full">
                        <div class="flex items-center space-x-4 mb-4">
                            <div class="w-3 h-3 rounded-full bg-red-500"></div>
                            <div class="w-3 h-3 rounded-full bg-yellow-500"></div>
                            <div class="w-3 h-3 rounded-full bg-green-500"></div>
                        </div>
                        <div class="font-mono text-sm text-slate-300">
                            <p><span class="text-purple-400">const</span> developer = {</p>
                            <p class="pl-4">name: <span class="text-green-400">'Coder-o-cloud'</span>,</p>
                            <p class="pl-4">role: <span class="text-green-400">'Full Stack Dev'</span>,</p>
                            <p class="pl-4">passion: <span class="text-green-400">'AI & MERN'</span>,</p>
                            <p class="pl-4">hardWorker: <span class="text-blue-400">true</span>,</p>
                            <p class="pl-4">hireable: <span class="text-blue-400">true</span></p>
                            <p>}</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Tech Stack -->
    <section id="stack" class="relative z-10 py-20 bg-black/20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <h2 class="text-3xl font-bold text-center mb-16"><span class="border-b-4 border-primary pb-2">My Tech Stack</span></h2>
            
            <div class="grid grid-cols-2 md:grid-cols-4 gap-8 text-center">
                <!-- MERN -->
                <div class="group p-6 glass rounded-xl hover:bg-white/5 transition-all">
                    <i class="fab fa-react text-5xl text-[#61DAFB] mb-4 group-hover:scale-110 transition-transform"></i>
                    <h3 class="font-semibold">React.js</h3>
                </div>
                <div class="group p-6 glass rounded-xl hover:bg-white/5 transition-all">
                    <i class="fab fa-node text-5xl text-[#43853D] mb-4 group-hover:scale-110 transition-transform"></i>
                    <h3 class="font-semibold">Node.js</h3>
                </div>
                <div class="group p-6 glass rounded-xl hover:bg-white/5 transition-all">
                    <i class="fas fa-database text-5xl text-[#4ea94b] mb-4 group-hover:scale-110 transition-transform"></i>
                    <h3 class="font-semibold">MongoDB</h3>
                </div>
                <div class="group p-6 glass rounded-xl hover:bg-white/5 transition-all">
                    <i class="fas fa-server text-5xl text-gray-400 mb-4 group-hover:scale-110 transition-transform"></i>
                    <h3 class="font-semibold">Express</h3>
                </div>

                <!-- Languages & AI -->
                <div class="group p-6 glass rounded-xl hover:bg-white/5 transition-all">
                    <i class="fab fa-js text-5xl text-[#F7DF1E] mb-4 group-hover:scale-110 transition-transform"></i>
                    <h3 class="font-semibold">JavaScript</h3>
                </div>
                <div class="group p-6 glass rounded-xl hover:bg-white/5 transition-all">
                    <i class="fab fa-python text-5xl text-[#3776AB] mb-4 group-hover:scale-110 transition-transform"></i>
                    <h3 class="font-semibold">Python</h3>
                </div>
                <div class="group p-6 glass rounded-xl hover:bg-white/5 transition-all">
                    <i class="fas fa-brain text-5xl text-[#FF6F00] mb-4 group-hover:scale-110 transition-transform"></i>
                    <h3 class="font-semibold">TensorFlow</h3>
                </div>
                <div class="group p-6 glass rounded-xl hover:bg-white/5 transition-all">
                    <i class="fab fa-html5 text-5xl text-[#E34F26] mb-4 group-hover:scale-110 transition-transform"></i>
                    <h3 class="font-semibold">HTML/CSS</h3>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="relative z-10 py-20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <h2 class="text-3xl font-bold text-center mb-16"><span class="border-b-4 border-secondary pb-2">Featured Projects</span></h2>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                
                <!-- Project 1 -->
                <div class="glass rounded-2xl overflow-hidden hover:transform hover:-translate-y-2 transition-all duration-300 group">
                    <div class="h-48 bg-gradient-to-br from-gray-800 to-black flex items-center justify-center relative overflow-hidden">
                        <i class="fas fa-users text-6xl text-slate-600 group-hover:text-primary transition-colors"></i>
                        <div class="absolute inset-0 bg-primary/10 opacity-0 group-hover:opacity-100 transition-opacity"></div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2">CollabVerse</h3>
                        <p class="text-sm text-primary mb-4">MERN Stack • Team Building</p>
                        <p class="text-slate-400 text-sm mb-6 h-20 overflow-hidden">
                            A platform for students to find teammates for hackathons and projects. Features real-time collaboration and user matching.
                        </p>
                        <a href="https://github.com/Coder-o-cloud/CollabVerse" target="_blank" class="inline-flex items-center text-white hover:text-primary transition-colors">
                            View Code <i class="fas fa-arrow-right ml-2 text-sm"></i>
                        </a>
                    </div>
                </div>

                <!-- Project 2 -->
                <div class="glass rounded-2xl overflow-hidden hover:transform hover:-translate-y-2 transition-all duration-300 group">
                    <div class="h-48 bg-gradient-to-br from-gray-800 to-black flex items-center justify-center relative overflow-hidden">
                        <i class="fas fa-apple-alt text-6xl text-slate-600 group-hover:text-red-500 transition-colors"></i>
                        <div class="absolute inset-0 bg-red-500/10 opacity-0 group-hover:opacity-100 transition-opacity"></div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2">Fruit Classification</h3>
                        <p class="text-sm text-secondary mb-4">Python • Deep Learning</p>
                        <p class="text-slate-400 text-sm mb-6 h-20 overflow-hidden">
                            AI system utilizing deep learning to classify fruits by texture, shape, and color. Improves agricultural sorting efficiency.
                        </p>
                        <a href="https://github.com/Coder-o-cloud/Fruit_Classification_System" target="_blank" class="inline-flex items-center text-white hover:text-secondary transition-colors">
                            View Code <i class="fas fa-arrow-right ml-2 text-sm"></i>
                        </a>
                    </div>
                </div>

                <!-- Project 3 -->
                <div class="glass rounded-2xl overflow-hidden hover:transform hover:-translate-y-2 transition-all duration-300 group">
                    <div class="h-48 bg-gradient-to-br from-gray-800 to-black flex items-center justify-center relative overflow-hidden">
                        <i class="fas fa-film text-6xl text-slate-600 group-hover:text-accent transition-colors"></i>
                        <div class="absolute inset-0 bg-accent/10 opacity-0 group-hover:opacity-100 transition-opacity"></div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2">Movie Recommender</h3>
                        <p class="text-sm text-accent mb-4">Python • Machine Learning</p>
                        <p class="text-slate-400 text-sm mb-6 h-20 overflow-hidden">
                            Smart recommendation engine fetching real-time data to suggest movies based on user preferences and popularity metrics.
                        </p>
                        <a href="https://github.com/Coder-o-cloud/Movie_recommender_tool" target="_blank" class="inline-flex items-center text-white hover:text-accent transition-colors">
                            View Code <i class="fas fa-arrow-right ml-2 text-sm"></i>
                        </a>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- Footer / Contact -->
    <footer id="contact" class="relative z-10 bg-black/40 border-t border-white/5 py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h2 class="text-2xl font-bold mb-8">Let's Build Something Amazing</h2>
            <div class="flex justify-center gap-6 mb-8">
                <a href="https://github.com/Coder-o-cloud" target="_blank" class="w-12 h-12 rounded-full glass flex items-center justify-center hover:bg-white/10 transition-colors text-2xl">
                    <i class="fab fa-github"></i>
                </a>
                <a href="#" class="w-12 h-12 rounded-full glass flex items-center justify-center hover:bg-white/10 transition-colors text-2xl">
                    <i class="fab fa-linkedin-in"></i>
                </a>
                <a href="mailto:your-email@example.com" class="w-12 h-12 rounded-full glass flex items-center justify-center hover:bg-white/10 transition-colors text-2xl">
                    <i class="fas fa-envelope"></i>
                </a>
            </div>
            <p class="text-slate-500 text-sm">
                © 2026 Coder-o-cloud. All rights reserved. <br>
                <span class="text-xs">Built with Tailwind CSS & HTML5</span>
            </p>
        </div>
    </footer>

</body>
</html>
