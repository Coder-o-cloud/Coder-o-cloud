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
                        dark: '#0d1117', /* GitHub Dark Dimmed */
                        primary: '#58a6ff', /* GitHub Blue */
                        secondary: '#bc8cff', /* GitHub Purple */
                        accent: '#3fb950', /* GitHub Green */
                        card: '#161b22',
                        border: '#30363d'
                    },
                    animation: {
                        'blob': 'blob 7s infinite',
                        'fade-in': 'fadeIn 1s ease-out',
                        'slide-up': 'slideUp 0.8s ease-out',
                        'typing': 'typing 3.5s steps(40, end)',
                        'blink-caret': 'blink-caret .75s step-end infinite',
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
                        },
                        typing: {
                            'from': { width: '0' },
                            'to': { width: '100%' }
                        },
                        'blink-caret': {
                            'from, to': { borderColor: 'transparent' },
                            '50%': { borderColor: '#58a6ff' }
                        }
                    }
                }
            }
        }
    </script>
    <style>
        .glass {
            background: rgba(22, 27, 34, 0.8);
            backdrop-filter: blur(10px);
            border: 1px solid #30363d;
        }
        .text-gradient {
            background: linear-gradient(to right, #58a6ff, #bc8cff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        /* Custom Typewriter Class */
        .typewriter h1 {
            overflow: hidden;
            border-right: .15em solid #58a6ff; 
            white-space: nowrap; 
            letter-spacing: .15em;
            animation: 
                typing 3.5s steps(40, end),
                blink-caret .75s step-end infinite;
        }
        
        /* Hide scrollbar for clean look */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #0d1117;
        }
        ::-webkit-scrollbar-thumb {
            background: #30363d;
            border-radius: 4px;
        }
    </style>
</head>
<body class="bg-dark text-slate-300 font-sans antialiased selection:bg-primary selection:text-white overflow-x-hidden">

    <!-- Background Effects -->
    <div class="fixed inset-0 z-0 pointer-events-none overflow-hidden">
        <div class="absolute top-0 left-1/4 w-96 h-96 bg-primary/10 rounded-full mix-blend-screen filter blur-3xl opacity-20 animate-blob"></div>
        <div class="absolute top-0 right-1/4 w-96 h-96 bg-secondary/10 rounded-full mix-blend-screen filter blur-3xl opacity-20 animate-blob animation-delay-2000"></div>
        <div class="absolute -bottom-32 left-1/3 w-96 h-96 bg-accent/10 rounded-full mix-blend-screen filter blur-3xl opacity-20 animate-blob animation-delay-4000"></div>
    </div>

    <!-- Navigation -->
    <nav class="fixed w-full z-50 glass border-b border-border">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-16">
                <div class="flex items-center gap-2">
                    <i class="fab fa-github text-3xl text-white"></i>
                    <span class="text-xl font-bold text-white cursor-pointer" onclick="window.scrollTo(0,0)">
                        Coder-o-cloud
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

    <!-- Hero Section (Readme Style) -->
    <section id="about" class="relative z-10 min-h-screen flex items-center justify-center pt-24 pb-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 w-full">
            <div class="flex flex-col lg:flex-row gap-12 items-start">
                
                <!-- Left Column: Intro -->
                <div class="lg:w-7/12 animate-slide-up">
                    <div class="inline-block px-3 py-1 mb-4 text-xs font-semibold tracking-wider text-accent uppercase bg-accent/10 rounded-full">
                        Available for hire
                    </div>
                    <div class="typewriter mb-4">
                        <h1 class="text-4xl md:text-6xl font-bold text-white">Hi there, I'm <span class="text-primary">Coder-o-cloud</span> 👋</h1>
                    </div>
                    <h2 class="text-2xl text-slate-400 mb-8 font-light">
                        Frontend + Full Stack Developer | AI Enthusiast
                    </h2>
                    
                    <!-- Profile Readme Style List -->
                    <div class="glass p-6 rounded-xl border-l-4 border-primary mb-8 bg-card/50">
                        <ul class="space-y-4 text-lg">
                            <li class="flex items-start gap-3">
                                <span class="text-2xl">🔭</span>
                                <span>I’m currently working on <strong class="text-white">CollabVerse & AI Systems</strong></span>
                            </li>
                            <li class="flex items-start gap-3">
                                <span class="text-2xl">🌱</span>
                                <span>I’m currently learning <strong class="text-white">Advanced Deep Learning & MLOps</strong></span>
                            </li>
                            <li class="flex items-start gap-3">
                                <span class="text-2xl">👯</span>
                                <span>I’m looking to collaborate on <strong class="text-white">Open Source MERN Projects</strong></span>
                            </li>
                            <li class="flex items-start gap-3">
                                <span class="text-2xl">💬</span>
                                <span>Ask me about <strong class="text-white">React, Node.js, or Python</strong></span>
                            </li>
                            <li class="flex items-start gap-3">
                                <span class="text-2xl">⚡</span>
                                <span>Fun fact: <span class="italic text-slate-400">I can debug code in my sleep (literally).</span></span>
                            </li>
                        </ul>
                    </div>

                    <div class="flex flex-wrap gap-4">
                        <a href="#projects" class="px-6 py-3 bg-primary hover:bg-blue-600 text-white font-semibold rounded-md transition-all shadow-lg shadow-primary/25">
                            <i class="fas fa-code mr-2"></i> View My Work
                        </a>
                        <a href="https://github.com/Coder-o-cloud" target="_blank" class="px-6 py-3 glass hover:bg-white/5 text-white font-semibold rounded-md transition-all border border-border">
                            <i class="fab fa-github mr-2"></i> GitHub
                        </a>
                        <a href="#" class="px-6 py-3 glass hover:bg-white/5 text-white font-semibold rounded-md transition-all border border-border">
                            <i class="fab fa-linkedin mr-2"></i> LinkedIn
                        </a>
                    </div>
                </div>

                <!-- Right Column: Code Snippet / Visual -->
                <div class="lg:w-5/12 w-full animate-fade-in lg:mt-10">
                    <div class="relative group">
                        <div class="absolute -inset-1 bg-gradient-to-r from-primary to-secondary rounded-xl blur opacity-25 group-hover:opacity-50 transition duration-1000 group-hover:duration-200"></div>
                        <div class="relative glass rounded-xl overflow-hidden bg-[#0d1117] border border-border">
                            <!-- Window Controls -->
                            <div class="flex items-center px-4 py-3 bg-[#161b22] border-b border-border">
                                <div class="flex space-x-2">
                                    <div class="w-3 h-3 rounded-full bg-red-500"></div>
                                    <div class="w-3 h-3 rounded-full bg-yellow-500"></div>
                                    <div class="w-3 h-3 rounded-full bg-green-500"></div>
                                </div>
                                <div class="ml-4 text-xs text-slate-500 font-mono">profile.js</div>
                            </div>
                            <!-- Code -->
                            <div class="p-6 font-mono text-sm overflow-x-auto">
                                <div class="text-slate-300">
                                    <span class="text-secondary">const</span> <span class="text-primary">coder</span> = {<br>
                                    &nbsp;&nbsp;name: <span class="text-accent">'Coder-o-cloud'</span>,<br>
                                    &nbsp;&nbsp;skills: [<br>
                                    &nbsp;&nbsp;&nbsp;&nbsp;<span class="text-accent">'MERN Stack'</span>,<br>
                                    &nbsp;&nbsp;&nbsp;&nbsp;<span class="text-accent">'Python & AI'</span>,<br>
                                    &nbsp;&nbsp;&nbsp;&nbsp;<span class="text-accent">'Full Stack Dev'</span><br>
                                    &nbsp;&nbsp;],<br>
                                    &nbsp;&nbsp;hardWorker: <span class="text-secondary">true</span>,<br>
                                    &nbsp;&nbsp;problemSolver: <span class="text-secondary">true</span>,<br>
                                    &nbsp;&nbsp;hireable: <span class="text-secondary">function</span>() {<br>
                                    &nbsp;&nbsp;&nbsp;&nbsp;<span class="text-secondary">return</span> <span class="text-secondary">this</span>.hardWorker;<br>
                                    &nbsp;&nbsp;}<br>
                                    };
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Github Stats Image (Simulated) -->
                    <div class="mt-6 glass p-4 rounded-xl border border-border text-center">
                        <p class="text-xs text-slate-500 mb-2 uppercase tracking-widest">Contributions</p>
                        <div class="flex gap-1 justify-center items-end h-16">
                            <!-- Simulated contribution graph bars -->
                            <div class="w-2 bg-accent/20 h-4 rounded-sm"></div>
                            <div class="w-2 bg-accent/40 h-8 rounded-sm"></div>
                            <div class="w-2 bg-accent h-12 rounded-sm"></div>
                            <div class="w-2 bg-accent/60 h-6 rounded-sm"></div>
                            <div class="w-2 bg-accent h-10 rounded-sm"></div>
                            <div class="w-2 bg-accent/80 h-14 rounded-sm"></div>
                            <div class="w-2 bg-accent h-8 rounded-sm"></div>
                            <div class="w-2 bg-accent/20 h-4 rounded-sm"></div>
                        </div>
                        <p class="text-xs text-accent mt-2 font-mono">1,024 Contributions in the last year</p>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- Tech Stack -->
    <section id="stack" class="relative z-10 py-20 bg-[#161b22]">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <h2 class="text-3xl font-bold text-center mb-16 text-white"><span class="border-b-4 border-primary pb-2">Tools & Technologies</span></h2>
            
            <div class="grid grid-cols-2 md:grid-cols-4 gap-6 text-center">
                <!-- MERN -->
                <div class="group p-6 glass rounded-xl hover:border-primary/50 transition-all cursor-default">
                    <i class="fab fa-react text-5xl text-[#61DAFB] mb-4 group-hover:scale-110 transition-transform"></i>
                    <h3 class="font-semibold text-slate-200">React.js</h3>
                </div>
                <div class="group p-6 glass rounded-xl hover:border-primary/50 transition-all cursor-default">
                    <i class="fab fa-node text-5xl text-[#43853D] mb-4 group-hover:scale-110 transition-transform"></i>
                    <h3 class="font-semibold text-slate-200">Node.js</h3>
                </div>
                <div class="group p-6 glass rounded-xl hover:border-primary/50 transition-all cursor-default">
                    <i class="fas fa-database text-5xl text-[#4ea94b] mb-4 group-hover:scale-110 transition-transform"></i>
                    <h3 class="font-semibold text-slate-200">MongoDB</h3>
                </div>
                <div class="group p-6 glass rounded-xl hover:border-primary/50 transition-all cursor-default">
                    <i class="fas fa-server text-5xl text-gray-400 mb-4 group-hover:scale-110 transition-transform"></i>
                    <h3 class="font-semibold text-slate-200">Express</h3>
                </div>

                <!-- Languages & AI -->
                <div class="group p-6 glass rounded-xl hover:border-primary/50 transition-all cursor-default">
                    <i class="fab fa-js text-5xl text-[#F7DF1E] mb-4 group-hover:scale-110 transition-transform"></i>
                    <h3 class="font-semibold text-slate-200">JavaScript</h3>
                </div>
                <div class="group p-6 glass rounded-xl hover:border-primary/50 transition-all cursor-default">
                    <i class="fab fa-python text-5xl text-[#3776AB] mb-4 group-hover:scale-110 transition-transform"></i>
                    <h3 class="font-semibold text-slate-200">Python</h3>
                </div>
                <div class="group p-6 glass rounded-xl hover:border-primary/50 transition-all cursor-default">
                    <i class="fas fa-brain text-5xl text-[#FF6F00] mb-4 group-hover:scale-110 transition-transform"></i>
                    <h3 class="font-semibold text-slate-200">TensorFlow</h3>
                </div>
                <div class="group p-6 glass rounded-xl hover:border-primary/50 transition-all cursor-default">
                    <i class="fab fa-html5 text-5xl text-[#E34F26] mb-4 group-hover:scale-110 transition-transform"></i>
                    <h3 class="font-semibold text-slate-200">HTML/CSS</h3>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="relative z-10 py-20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <h2 class="text-3xl font-bold text-center mb-16 text-white"><span class="border-b-4 border-secondary pb-2">Featured Projects</span></h2>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                
                <!-- Project 1 -->
                <div class="glass rounded-xl overflow-hidden hover:border-primary transition-all duration-300 group flex flex-col h-full">
                    <div class="h-48 bg-[#0d1117] border-b border-border flex items-center justify-center relative overflow-hidden">
                        <i class="fas fa-users text-6xl text-slate-700 group-hover:text-primary transition-colors"></i>
                        <div class="absolute top-2 right-2 bg-card px-2 py-1 text-xs rounded border border-border">Public</div>
                    </div>
                    <div class="p-6 flex-1 flex flex-col">
                        <h3 class="text-xl font-bold mb-2 text-primary group-hover:underline">CollabVerse</h3>
                        <p class="text-sm text-slate-400 mb-4 flex-1">
                            A platform for students to find teammates for hackathons and projects. Features real-time collaboration and user matching.
                        </p>
                        <div class="flex gap-2 mb-4 text-xs">
                            <span class="flex items-center gap-1"><div class="w-3 h-3 rounded-full bg-[#f1e05a]"></div> JavaScript</span>
                            <span class="flex items-center gap-1"><div class="w-3 h-3 rounded-full bg-[#4F5D95]"></div> PHP</span>
                        </div>
                        <a href="https://github.com/Coder-o-cloud/CollabVerse" target="_blank" class="w-full text-center py-2 bg-card hover:bg-[#30363d] border border-border rounded-md transition-colors text-sm font-medium">
                            <i class="far fa-star mr-1"></i> Star on GitHub
                        </a>
                    </div>
                </div>

                <!-- Project 2 -->
                <div class="glass rounded-xl overflow-hidden hover:border-secondary transition-all duration-300 group flex flex-col h-full">
                    <div class="h-48 bg-[#0d1117] border-b border-border flex items-center justify-center relative overflow-hidden">
                        <i class="fas fa-apple-alt text-6xl text-slate-700 group-hover:text-secondary transition-colors"></i>
                        <div class="absolute top-2 right-2 bg-card px-2 py-1 text-xs rounded border border-border">Public</div>
                    </div>
                    <div class="p-6 flex-1 flex flex-col">
                        <h3 class="text-xl font-bold mb-2 text-secondary group-hover:underline">Fruit Classification</h3>
                        <p class="text-sm text-slate-400 mb-4 flex-1">
                            AI system utilizing deep learning to classify fruits by texture, shape, and color. Improves agricultural sorting efficiency.
                        </p>
                        <div class="flex gap-2 mb-4 text-xs">
                            <span class="flex items-center gap-1"><div class="w-3 h-3 rounded-full bg-[#3572A5]"></div> Python</span>
                            <span class="flex items-center gap-1"><div class="w-3 h-3 rounded-full bg-[#FF6F00]"></div> Jupyter</span>
                        </div>
                        <a href="https://github.com/Coder-o-cloud/Fruit_Classification_System" target="_blank" class="w-full text-center py-2 bg-card hover:bg-[#30363d] border border-border rounded-md transition-colors text-sm font-medium">
                            <i class="far fa-star mr-1"></i> Star on GitHub
                        </a>
                    </div>
                </div>

                <!-- Project 3 -->
                <div class="glass rounded-xl overflow-hidden hover:border-accent transition-all duration-300 group flex flex-col h-full">
                    <div class="h-48 bg-[#0d1117] border-b border-border flex items-center justify-center relative overflow-hidden">
                        <i class="fas fa-film text-6xl text-slate-700 group-hover:text-accent transition-colors"></i>
                        <div class="absolute top-2 right-2 bg-card px-2 py-1 text-xs rounded border border-border">Public</div>
                    </div>
                    <div class="p-6 flex-1 flex flex-col">
                        <h3 class="text-xl font-bold mb-2 text-accent group-hover:underline">Movie Recommender</h3>
                        <p class="text-sm text-slate-400 mb-4 flex-1">
                            Smart recommendation engine fetching real-time data to suggest movies based on user preferences and popularity metrics.
                        </p>
                        <div class="flex gap-2 mb-4 text-xs">
                            <span class="flex items-center gap-1"><div class="w-3 h-3 rounded-full bg-[#3572A5]"></div> Python</span>
                            <span class="flex items-center gap-1"><div class="w-3 h-3 rounded-full bg-[#e34c26]"></div> HTML</span>
                        </div>
                        <a href="https://github.com/Coder-o-cloud/Movie_recommender_tool" target="_blank" class="w-full text-center py-2 bg-card hover:bg-[#30363d] border border-border rounded-md transition-colors text-sm font-medium">
                            <i class="far fa-star mr-1"></i> Star on GitHub
                        </a>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- Footer / Contact -->
    <footer id="contact" class="relative z-10 bg-[#0d1117] border-t border-border py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h2 class="text-2xl font-bold mb-8 text-white">Let's Connect</h2>
            <div class="flex justify-center gap-6 mb-8">
                <a href="https://github.com/Coder-o-cloud" target="_blank" class="w-12 h-12 rounded-full glass flex items-center justify-center hover:bg-white/10 transition-colors text-2xl text-white">
                    <i class="fab fa-github"></i>
                </a>
                <a href="#" class="w-12 h-12 rounded-full glass flex items-center justify-center hover:bg-white/10 transition-colors text-2xl text-[#0077B5]">
                    <i class="fab fa-linkedin-in"></i>
                </a>
                <a href="mailto:your-email@example.com" class="w-12 h-12 rounded-full glass flex items-center justify-center hover:bg-white/10 transition-colors text-2xl text-[#EA4335]">
                    <i class="fas fa-envelope"></i>
                </a>
            </div>
            <p class="text-slate-500 text-sm">
                Designed & Built by Coder-o-cloud <br>
                <span class="text-xs">Inspired by GitHub Profile READMEs</span>
            </p>
        </div>
    </footer>

</body>
</html>
