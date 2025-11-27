<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Name | GitHub Profile</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdn.jsdelivr.net/npm/font-awesome@4.7.0/css/font-awesome.min.css" rel="stylesheet">
    <script>
        // 配置 Tailwind 自定义主题
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#2563eb', // GitHub 风格蓝色
                        secondary: '#1f2937',
                        accent: '#6366f1',
                        light: '#f9fafb',
                        dark: '#111827'
                    },
                    fontFamily: {
                        sans: ['Inter', 'system-ui', 'sans-serif'],
                    },
                }
            }
        }
    </script>
    <style type="text/tailwindcss">
        @layer utilities {
            .text-shadow {
                text-shadow: 0 2px 4px rgba(0,0,0,0.1);
            }
            .bg-gradient {
                background: linear-gradient(135deg, #2563eb 0%, #6366f1 100%);
            }
            .transition-custom {
                transition: all 0.3s ease;
            }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
</head>
<body class="bg-light text-secondary font-sans">
    <!-- 导航栏 -->
    <nav id="navbar" class="fixed w-full bg-white/90 backdrop-blur-sm shadow-sm z-50 transition-custom">
        <div class="container mx-auto px-4 py-3 flex justify-between items-center">
            <a href="#" class="text-xl font-bold text-primary flex items-center">
                <i class="fa fa-github mr-2"></i>
                <span>YourUsername</span>
            </a>
            <div class="hidden md:flex space-x-8">
                <a href="#about" class="font-medium hover:text-primary transition-custom">About</a>
                <a href="#skills" class="font-medium hover:text-primary transition-custom">Skills</a>
                <a href="#projects" class="font-medium hover:text-primary transition-custom">Projects</a>
                <a href="#contact" class="font-medium hover:text-primary transition-custom">Contact</a>
            </div>
            <button class="md:hidden text-secondary text-xl" id="menu-toggle">
                <i class="fa fa-bars"></i>
            </button>
        </div>
        <!-- 移动端菜单 -->
        <div id="mobile-menu" class="hidden md:hidden bg-white shadow-lg absolute w-full">
            <div class="container mx-auto px-4 py-3 flex flex-col space-y-4">
                <a href="#about" class="font-medium hover:text-primary transition-custom py-2">About</a>
                <a href="#skills" class="font-medium hover:text-primary transition-custom py-2">Skills</a>
                <a href="#projects" class="font-medium hover:text-primary transition-custom py-2">Projects</a>
                <a href="#contact" class="font-medium hover:text-primary transition-custom py-2">Contact</a>
            </div>
        </div>
    </nav>

    <!-- 英雄区域 -->
    <header class="pt-32 pb-20 md:pt-40 md:pb-28 bg-gradient text-white">
        <div class="container mx-auto px-4 text-center">
            <img 
                src="https://github.com/yourusername.png" 
                alt="Profile Picture" 
                class="w-32 h-32 md:w-40 md:h-40 rounded-full mx-auto border-4 border-white/30 mb-6 shadow-lg"
            >
            <h1 class="text-3xl md:text-4xl lg:text-5xl font-bold mb-4 text-shadow">Hi, I'm [Your Name]</h1>
            <p class="text-xl md:text-2xl opacity-90 max-w-2xl mx-auto mb-8">
                [Your Title, e.g., Full-Stack Developer | UI/UX Designer | Data Scientist]
            </p>
            <p class="text-base md:text-lg opacity-80 max-w-2xl mx-auto mb-10">
                [Brief intro: Passionate about building amazing products, open source contributor, 
                tech enthusiast, etc.]
            </p>
            <div class="flex flex-wrap justify-center gap-4">
                <a href="https://github.com/yourusername" class="bg-white text-primary px-6 py-3 rounded-lg font-medium hover:bg-opacity-90 transition-custom flex items-center">
                    <i class="fa fa-github mr-2"></i> GitHub
                </a>
                <a href="https://linkedin.com/in/yourusername" class="bg-transparent border-2 border-white text-white px-6 py-3 rounded-lg font-medium hover:bg-white/10 transition-custom flex items-center">
                    <i class="fa fa-linkedin mr-2"></i> LinkedIn
                </a>
                <a href="mailto:your.email@example.com" class="bg-transparent border-2 border-white text-white px-6 py-3 rounded-lg font-medium hover:bg-white/10 transition-custom flex items-center">
                    <i class="fa fa-envelope mr-2"></i> Email
                </a>
            </div>
        </div>
    </header>

    <!-- 关于我 -->
    <section id="about" class="py-16 md:py-24 bg-white">
        <div class="container mx-auto px-4">
            <div class="max-w-3xl mx-auto">
                <h2 class="text-2xl md:text-3xl font-bold mb-8 text-center text-secondary">About Me</h2>
                <div class="prose prose-lg max-w-none">
                    <p class="mb-4 text-gray-700">
                        Hello! I'm [Your Name], a [Your Profession] with [X years] of experience in [relevant field]. 
                        I specialize in [key expertise, e.g., building scalable web applications, designing intuitive user interfaces, 
                        analyzing complex data sets].
                    </p>
                    <p class="mb-4 text-gray-700">
                        I'm passionate about [your passion, e.g., open source, clean code, user-centered design, 
                        continuous learning]. I believe in [your values, e.g., creating technology that makes a difference, 
                        collaboration, writing maintainable software].
                    </p>
                    <p class="mb-6 text-gray-700">
                        When I'm not coding/designing/analyzing, you can find me [hobbies, e.g., contributing to open source projects, 
                        hiking, reading tech blogs, playing guitar].
                    </p>
                    <div class="flex flex-wrap gap-3 mt-8">
                        <span class="bg-primary/10 text-primary px-4 py-2 rounded-full text-sm font-medium">Open Source</span>
                        <span class="bg-primary/10 text-primary px-4 py-2 rounded-full text-sm font-medium">Tech Enthusiast</span>
                        <span class="bg-primary/10 text-primary px-4 py-2 rounded-full text-sm font-medium">Lifelong Learner</span>
                        <span class="bg-primary/10 text-primary px-4 py-2 rounded-full text-sm font-medium">Collaborative</span>
                        <span class="bg-primary/10 text-primary px-4 py-2 rounded-full text-sm font-medium">[Your Trait]</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 技能 -->
    <section id="skills" class="py-16 md:py-24 bg-gray-50">
        <div class="container mx-auto px-4">
            <h2 class="text-2xl md:text-3xl font-bold mb-12 text-center text-secondary">My Skills</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- 技能卡片 1 -->
                <div class="bg-white p-6 rounded-xl shadow-sm hover:shadow-md transition-custom">
                    <div class="w-12 h-12 bg-primary/10 rounded-lg flex items-center justify-center mb-4">
                        <i class="fa fa-code text-primary text-xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold mb-3">Development</h3>
                    <ul class="space-y-2 text-gray-700">
                        <li class="flex items-center">
                            <i class="fa fa-check text-green-500 mr-2"></i>
                            <span>JavaScript (ES6+), TypeScript</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fa fa-check text-green-500 mr-2"></i>
                            <span>React, Vue.js, Next.js</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fa fa-check text-green-500 mr-2"></i>
                            <span>Node.js, Express, NestJS</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fa fa-check text-green-500 mr-2"></i>
                            <span>HTML5, CSS3, Tailwind CSS</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fa fa-check text-green-500 mr-2"></i>
                            <span>SQL, MongoDB</span>
                        </li>
                    </ul>
                </div>

                <!-- 技能卡片 2 -->
                <div class="bg-white p-6 rounded-xl shadow-sm hover:shadow-md transition-custom">
                    <div class="w-12 h-12 bg-accent/10 rounded-lg flex items-center justify-center mb-4">
                        <i class="fa fa-paint-brush text-accent text-xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold mb-3">Design</h3>
                    <ul class="space-y-2 text-gray-700">
                        <li class="flex items-center">
                            <i class="fa fa-check text-green-500 mr-2"></i>
                            <span>UI/UX Design</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fa fa-check text-green-500 mr-2"></i>
                            <span>Figma, Adobe XD</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fa fa-check text-green-500 mr-2"></i>
                            <span>Responsive Design</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fa fa-check text-green-500 mr-2"></i>
                            <span>Typography & Color Theory</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fa fa-check text-green-500 mr-2"></i>
                            <span>Prototyping</span>
                        </li>
                    </ul>
                </div>

                <!-- 技能卡片 3 -->
                <div class="bg-white p-6 rounded-xl shadow-sm hover:shadow-md transition-custom">
                    <div class="w-12 h-12 bg-secondary/10 rounded-lg flex items-center justify-center mb-4">
                        <i class="fa fa-cogs text-secondary text-xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold mb-3">Tools & Workflow</h3>
                    <ul class="space-y-2 text-gray-700">
                        <li class="flex items-center">
                            <i class="fa fa-check text-green-500 mr-2"></i>
                            <span>Git, GitHub, GitLab</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fa fa-check text-green-500 mr-2"></i>
                            <span>Docker, Kubernetes</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fa fa-check text-green-500 mr-2"></i>
                            <span>CI/CD (GitHub Actions, Jenkins)</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fa fa-check text-green-500 mr-2"></i>
                            <span>VS Code, WebStorm</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fa fa-check text-green-500 mr-2"></i>
                            <span>Agile, Scrum</span>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- 项目展示 -->
    <section id="projects" class="py-16 md:py-24 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-2xl md:text-3xl font-bold mb-12 text-center text-secondary">Featured Projects</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <!-- 项目卡片 1 -->
                <div class="bg-gray-50 rounded-xl overflow-hidden shadow-sm hover:shadow-md transition-custom">
                    <img 
                        src="https://picsum.photos/id/0/800/400" 
                        alt="Project Screenshot" 
                        class="w-full h-48 object-cover"
                    >
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">Project Name 1</h3>
                        <p class="text-gray-700 mb-4">
                            Brief description of your project. What it does, the technologies used, and any key features.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-primary/10 text-primary px-3 py-1 rounded-full text-xs font-medium">React</span>
                            <span class="bg-primary/10 text-primary px-3 py-1 rounded-full text-xs font-medium">Node.js</span>
                            <span class="bg-primary/10 text-primary px-3 py-1 rounded-full text-xs font-medium">MongoDB</span>
                        </div>
                        <div class="flex space-x-4">
                            <a href="https://github.com/yourusername/project1" class="text-primary hover:text-primary/80 transition-custom flex items-center">
                                <i class="fa fa-github mr-1"></i> Code
                            </a>
                            <a href="https://project1-demo.com" class="text-accent hover:text-accent/80 transition-custom flex items-center">
                                <i class="fa fa-external-link mr-1"></i> Demo
                            </a>
                        </div>
                    </div>
                </div>

                <!-- 项目卡片 2 -->
                <div class="bg-gray-50 rounded-xl overflow-hidden shadow-sm hover:shadow-md transition-custom">
                    <img 
                        src="https://picsum.photos/id/180/800/400" 
                        alt="Project Screenshot" 
                        class="w-full h-48 object-cover"
                    >
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">Project Name 2</h3>
                        <p class="text-gray-700 mb-4">
                            Brief description of your project. What it does, the technologies used, and any key features.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-primary/10 text-primary px-3 py-1 rounded-full text-xs font-medium">Vue.js</span>
                            <span class="bg-primary/10 text-primary px-3 py-1 rounded-full text-xs font-medium">Tailwind CSS</span>
                            <span class="bg-primary/10 text-primary px-3 py-1 rounded-full text-xs font-medium">Firebase</span>
                        </div>
                        <div class="flex space-x-4">
                            <a href="https://github.com/yourusername/project2" class="text-primary hover:text-primary/80 transition-custom flex items-center">
                                <i class="fa fa-github mr-1"></i> Code
                            </a>
                            <a href="https://project2-demo.com" class="text-accent hover:text-accent/80 transition-custom flex items-center">
                                <i class="fa fa-external-link mr-1"></i> Demo
                            </a>
                        </div>
                    </div>
                </div>

                <!-- 项目卡片 3 -->
                <div class="bg-gray-50 rounded-xl overflow-hidden shadow-sm hover:shadow-md transition-custom">
                    <img 
                        src="https://picsum.photos/id/20/800/400" 
                        alt="Project Screenshot" 
                        class="w-full h-48 object-cover"
                    >
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">Project Name 3</h3>
                        <p class="text-gray-700 mb-4">
                            Brief description of your project. What it does, the technologies used, and any key features.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-primary/10 text-primary px-3 py-1 rounded-full text-xs font-medium">TypeScript</span>
                            <span class="bg-primary/10 text-primary px-3 py-1 rounded-full text-xs font-medium">Next.js</span>
                            <span class="bg-primary/10 text-primary px-3 py-1 rounded-full text-xs font-medium">PostgreSQL</span>
                        </div>
                        <div class="flex space-x-4">
                            <a href="https://github.com/yourusername/project3" class="text-primary hover:text-primary/80 transition-custom flex items-center">
                                <i class="fa fa-github mr-1"></i> Code
                            </a>
                            <a href="https://project3-demo.com" class="text-accent hover:text-accent/80 transition-custom flex items-center">
                                <i class="fa fa-external-link mr-1"></i> Demo
                            </a>
                        </div>
                    </div>
                </div>

                <!-- 项目卡片 4 -->
                <div class="bg-gray-50 rounded-xl overflow-hidden shadow-sm hover:shadow-md transition-custom">
                    <img 
                        src="https://picsum.photos/id/42/800/400" 
                        alt="Project Screenshot" 
                        class="w-full h-48 object-cover"
                    >
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">Project Name 4</h3>
                        <p class="text-gray-700 mb-4">
                            Brief description of your project. What it does, the technologies used, and any key features.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="bg-primary/10 text-primary px-3 py-1 rounded-full text-xs font-medium">Python</span>
                            <span class="bg-primary/10 text-primary px-3 py-1 rounded-full text-xs font-medium">Django</span>
                            <span class="bg-primary/10 text-primary px-3 py-1 rounded-full text-xs font-medium">Docker</span>
                        </div>
                        <div class="flex space-x-4">
                            <a href="https://github.com/yourusername/project4" class="text-primary hover:text-primary/80 transition-custom flex items-center">
                                <i class="fa fa-github mr-1"></i> Code
                            </a>
                            <a href="https://project4-demo.com" class="text-accent hover:text-accent/80 transition-custom flex items-center">
                                <i class="fa fa-external-link mr-1"></i> Demo
                            </a>
                        </div>
                    </div>
                </div>
            </div>

            <div class="text-center mt-10">
                <a href="https://github.com/yourusername?tab=repositories" class="inline-flex items-center text-primary font-medium hover:text-primary/80 transition-custom">
                    View All Projects <i class="fa fa-arrow-right ml-2"></i>
                </a>
            </div>
        </div>
    </section>

    <!-- 联系方式 -->
    <section id="contact" class="py-16 md:py-24 bg-gray-50">
        <div class="container mx-auto px-4">
            <h2 class="text-2xl md:text-3xl font-bold mb-12 text-center text-secondary">Get In Touch</h2>
            
            <div class="max-w-2xl mx-auto bg-white p-8 rounded-xl shadow-sm">
                <p class="text-gray-700 mb-8 text-center">
                    Have a project in mind or want to collaborate? Feel free to reach out!
                </p>
                
                <form class="space-y-6">
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                        <div>
                            <label for="name" class="block text-gray-700 mb-2">Your Name</label>
                            <input 
                                type="text" 
                                id="name" 
                                class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary focus:border-primary transition-custom"
                                placeholder="John Doe"
                            >
                        </div>
                        <div>
                            <label for="email" class="block text-gray-700 mb-2">Your Email</label>
                            <input 
                                type="email" 
                                id="email" 
                                class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary focus:border-primary transition-custom"
                                placeholder="john@example.com"
                            >
                        </div>
                    </div>
                    <div>
                        <label for="subject" class="block text-gray-700 mb-2">Subject</label>
                        <input 
                            type="text" 
                            id="subject" 
                            class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary focus:border-primary transition-custom"
                            placeholder="Project Inquiry"
                        >
                    </div>
                    <div>
                        <label for="message" class="block text-gray-700 mb-2">Message</label>
                        <textarea 
                            id="message" 
                            rows="5" 
                            class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary focus:border-primary transition-custom"
                            placeholder="Your message here..."
                        ></textarea>
                    </div>
                    <button 
                        type="submit" 
                        class="w-full bg-primary text-white px-6 py-3 rounded-lg font-medium hover:bg-primary/90 transition-custom flex items-center justify-center"
                    >
                        <i class="fa fa-paper-plane mr-2"></i> Send Message
                    </button>
                </form>
                
                <div class="mt-10 pt-6 border-t border-gray-200">
                    <h3 class="text-lg font-semibold mb-4 text-center">Or connect with me directly</h3>
                    <div class="flex justify-center space-x-6">
                        <a href="https://github.com/yourusername" class="text-gray-600 hover:text-primary transition-custom text-xl">
                            <i class="fa fa-github"></i>
                        </a>
                        <a href="https://linkedin.com/in/yourusername" class="text-gray-600 hover:text-primary transition-custom text-xl">
                            <i class="fa fa-linkedin"></i>
                        </a>
                        <a href="https://twitter.com/yourusername" class="text-gray-600 hover:text-primary transition-custom text-xl">
                            <i class="fa fa-twitter"></i>
                        </a>
                        <a href="https://dev.to/yourusername" class="text-gray-600 hover:text-primary transition-custom text-xl">
                            <i class="fa fa-dev"></i>
                        </a>
                        <a href="mailto:your.email@example.com" class="text-gray-600 hover:text-primary transition-custom text-xl">
                            <i class="fa fa-envelope"></i>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 页脚 -->
    <footer class="bg-secondary text-white py-10">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="mb-6 md:mb-0">
                    <a href="#" class="text-xl font-bold flex items-center">
                        <i class="fa fa-github mr-2"></i>
                        <span>YourUsername</span>
                    </a>
                    <p class="text-gray-400 mt-2">
                        [Your Tagline, e.g., Building amazing things with code]
                    </p>
                </div>
                <div class="flex space-x-6">
                    <a href="https://github.com/yourusername" class="text-gray-400 hover:text-white transition-custom">
                        <i class="fa fa-github text-xl"></i>
                    </a>
                    <a href="https://linkedin.com/in/yourusername" class="text-gray-400 hover:text-white transition-custom">
                        <i class="fa fa-linkedin text-xl"></i>
                    </a>
                    <a href="https://twitter.com/yourusername" class="text-gray-400 hover:text-white transition-custom">
                        <i class="fa fa-twitter text-xl"></i>
                    </a>
                    <a href="mailto:your.email@example.com" class="text-gray-400 hover:text-white transition-custom">
                        <i class="fa fa-envelope text-xl"></i>
                    </a>
                </div>
            </div>
            <div class="mt-8 pt-6 border-t border-gray-700 text-center text-gray-400">
                <p>&copy; 2024 [Your Name]. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <!-- 回到顶部按钮 -->
    <button id="back-to-top" class="fixed bottom-6 right-6 bg-primary text-white w-12 h-12 rounded-full flex items-center justify-center shadow-lg opacity-0 invisible transition-custom hover:bg-primary/90">
        <i class="fa fa-arrow-up"></i>
    </button>

    <script>
        // 移动端菜单切换
        const menuToggle = document.getElementById('menu-toggle');
        const mobileMenu = document.getElementById('mobile-menu');
        
        menuToggle.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // 导航栏滚动效果
        const navbar = document.getElementById('navbar');
        window.addEventListener('scroll', () => {
            if (window.scrollY > 50) {
                navbar.classList.add('py-2', 'shadow');
                navbar.classList.remove('py-3');
            } else {
                navbar.classList.add('py-3');
                navbar.classList.remove('py-2', 'shadow');
            }
        });

        // 回到顶部按钮
        const backToTopButton = document.getElementById('back-to-top');
        
        window.addEventListener('scroll', () => {
            if (window.scrollY > 300) {
                backToTopButton.classList.remove('opacity-0', 'invisible');
                backToTopButton.classList.add('opacity-100', 'visible');
            } else {
                backToTopButton.classList.add('opacity-0', 'invisible');
                backToTopButton.classList.remove('opacity-100', 'visible');
            }
        });
        
        backToTopButton.addEventListener('click', () => {
            window.scrollTo({
                top: 0,
                behavior: 'smooth'
            });
        });

        // 平滑滚动
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                // 关闭移动端菜单
                if (!mobileMenu.classList.contains('hidden')) {
                    mobileMenu.classList.add('hidden');
                }
                
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    const navbarHeight = navbar.offsetHeight;
                    const targetPosition = targetElement.getBoundingClientRect().top + window.pageYOffset - navbarHeight;
                    
                    window.scrollTo({
                        top: targetPosition,
                        behavior: 'smooth'
                    });
                }
            });
        });
    </script>
</body>
</html>
