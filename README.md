<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio</title>
    
    <link rel="manifest" href="manifest.json">
    <meta name="theme-color" content="#3b82f6">

    <!-- External Resources -->
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">

    <style>
        .timeline-item {
            position: relative;
            padding-left: 2rem;
            border-left: 2px solid #3b82f6;
            margin-bottom: 2rem;
        }
        .timeline-item:before {
            content: '';
            position: absolute;
            left: -9px;
            top: 0;
            width: 16px;
            height: 16px;
            border-radius: 50%;
            background: #3b82f6;
        }
        .skill-bar {
            transition: width 1s ease-in-out;
        }
    </style>
</head>
<script>
if ("serviceWorker" in navigator) {
  navigator.serviceWorker.register("service-worker.js")
    .then(() => console.log("Service Worker Registered"))
    .catch(err => console.error(err));
}
</script>

<body class="bg-gray-50 text-gray-800">
    <!-- Navigation -->
    <nav class="bg-white shadow-lg fixed w-full z-10">
        <div class="max-w-6xl mx-auto px-4">
            <div class="flex justify-between items-center h-16">
                <div class="text-xl font-bold text-blue-600">Portfolio</div>
                <div class="hidden md:flex space-x-8">
                    <a href="#home" class="hover:text-blue-600 transition">Home</a>
                    <a href="#skills" class="hover:text-blue-600 transition">Skills</a>
                    <a href="#experience" class="hover:text-blue-600 transition">Experience</a>
                    <a href="#education" class="hover:text-blue-600 transition">Education</a>
                    <a href="#contact" class="hover:text-blue-600 transition">Contact</a>
                </div>
                <div class="md:hidden">
                    <button class="mobile-menu-button">
                        <i class="fas fa-bars text-xl"></i>
                    </button>
                </div>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="min-h-screen flex items-center justify-center bg-gradient-to-r from-blue-500 to-indigo-600 text-white pt-16">
        <div class="text-center max-w-4xl px-4">
            <h1 class="text-5xl md:text-6xl font-bold mb-6">Hi, I'm <span class="text-yellow-300">Snehal Yadav</span></h1>
            <p class="text-xl md:text-2xl mb-8">B.Tech AIML Student | Future Web Developer</p>
            <div class="space-x-4">
                <a href="#contact" class="bg-white text-blue-600 px-6 py-3 rounded-full font-semibold hover:bg-gray-100 transition">
                    Contact Me
                </a>
                <a href="#skills" class="bg-transparent border-2 border-white text-white px-6 py-3 rounded-full font-semibold hover:bg-white hover:text-blue-600 transition">
                    View My Work
                </a>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="py-20 bg-white">
        <div class="max-w-6xl mx-auto px-4">
            <h2 class="text-4xl font-bold text-center mb-16">My <span class="text-blue-600">Skills</span></h2>
            
            <div class="grid md:grid-cols-2 gap-8">
                <!-- Technical Skills -->
                <div>
                    <h3 class="text-2xl font-semibold mb-6">Technical Skills</h3>
                    <div class="space-y-6">
                        <div>
                            <div class="flex justify-between mb-2">
                                <span>HTML & CSS</span>
                                <span>90%</span>
                            </div>
                           <div class="h-2 bg-gray-200 rounded-full overflow-hidden">
                                <div class="h-full bg-blue-600 rounded-full skill-bar"
                                    style="width: 0%"
                                    data-width="90%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span>JavaScript</span>
                                <span>50%</span>
                            </div>
                            <div class="h-2 bg-gray-200 rounded-full">
                                <div class="h-full bg-blue-600 rounded-full skill-bar" style="width: 0%" data-width="85%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span>Python</span>
                                <span>50%</span>
                            </div>
                            <div class="h-2 bg-gray-200 rounded-full">
                                <div class="h-full bg-blue-500 rounded-full skill-bar" style="width: 0%" data-width="50%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span>C++</span>
                                <span>75%</span>
                            </div>
                            <div class="h-2 bg-gray-200 rounded-full">
                                <div class="h-full bg-blue-600 rounded-full skill-bar" style="width: 0%" data-width="75%"></div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Professional Skills -->
                <div>
                    <h3 class="text-2xl font-semibold mb-6">Professional Skills</h3>
                    <div class="space-y-6">
                        <div>
                            <div class="flex justify-between mb-2">
                                <span>Problem Solving</span>
                                <span>95%</span>
                            </div>
                            <div class="h-2 bg-gray-200 rounded-full">
                                <div class="h-full bg-blue-600 rounded-full skill-bar" style="width: 0%" data-width="95%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span>Teamwork</span>
                                <span>90%</span>
                            </div>
                            <div class="h-2 bg-gray-200 rounded-full">
                                <div class="h-full bg-blue-600 rounded-full skill-bar" style="width: 0%" data-width="90%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span>Communication</span>
                                <span>85%</span>
                            </div>
                            <div class="h-2 bg-gray-200 rounded-full">
                                <div class="h-full bg-blue-600 rounded-full skill-bar" style="width: 0%" data-width="85%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span>Project Management</span>
                                <span>80%</span>
                            </div>
                            <div class="h-2 bg-gray-200 rounded-full">
                                <div class="h-full bg-blue-600 rounded-full skill-bar" style="width: 0%" data-width="80%"></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Experience Section -->
    <section id="experience" class="py-20 bg-gray-50">
        <div class="max-w-4xl mx-auto px-4">
            <h2 class="text-4xl font-bold text-center mb-16">Work <span class="text-blue-600">Experience</span></h2>
            
            <div class="space-y-12">
                <!-- Experience Item 1 -->
                <div class="timeline-item">
                    <div class="bg-white p-6 rounded-lg shadow-md hover:shadow-xl transition">
                        <div class="flex flex-col md:flex-row md:justify-between md:items-center mb-4">
                            <h3 class="text-2xl font-semibold">DelXN Technologies Pvt Ltd</h3>
                            <span class="text-blue-600 font-medium">2024 - 2025</span>
                        </div>
                        <h4 class="text-lg text-gray-600 mb-4">Intern </h4>
                        <p class="text-gray-700">
                            <li>Worked in team to build scalable web applications using modern technologies.</li>
                            <li>Worked fully on frontend development.</li>
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Education Section -->
    <section id="education" class="py-20 bg-white">
        <div class="max-w-4xl mx-auto px-4">
            <h2 class="text-4xl font-bold text-center mb-16">My <span class="text-blue-600">Education</span></h2>
            
            <div class="space-y-12">
                <!-- Education Item 1 -->
                <div class="timeline-item">
                    <div class="bg-white p-6 rounded-lg shadow-md hover:shadow-xl transition">
                        <div class="flex flex-col md:flex-row md:justify-between md:items-center mb-4">
                            <h3 class="text-2xl font-semibold">B.Tech AI & ML </h3>
                            <span class="text-blue-600 font-medium">2024 - present</span>
                        </div>
                        <h4 class="text-lg text-gray-600 mb-4">Zeal College of Engineering and Research</h4>
                        <p class="text-gray-700">
                            F.Y  CGPA: 8.73
                         
                        </p>
                    </div>
                </div>

                <!-- Education Item 2 -->
                <div class="timeline-item">
                    <div class="bg-white p-6 rounded-lg shadow-md hover:shadow-xl transition">
                        <div class="flex flex-col md:flex-row md:justify-between md:items-center mb-4">
                            <h3 class="text-2xl font-semibold">12th </h3>
                            <span class="text-blue-600 font-medium">2022 - 2023</span>
                        </div>
                        <h4 class="text-lg text-gray-600 mb-4">Sarhad JR College of Science,Commerce and Arts</h4>
                        <p class="text-gray-700">
                            Percentage: 64.67%
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-gray-50">
        <div class="max-w-4xl mx-auto px-4">
            <h2 class="text-4xl font-bold text-center mb-16">Get In <span class="text-blue-600">Touch</span></h2>
            
            <div class="bg-white rounded-lg shadow-lg p-8">
                <form id="contactForm" class="space-y-6">
                    <div class="grid md:grid-cols-2 gap-6">
                        <div>
                            <label for="name" class="block text-gray-700 font-medium mb-2">Your Name</label>
                            <input type="text" id="name" class="w-full px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500" required>
                        </div>
                        <div>
                            <label for="email" class="block text-gray-700 font-medium mb-2">Your Email</label>
                            <input type="email" id="email" class="w-full px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500" required>
                        </div>
                    </div>
                    <div>
                        <label for="subject" class="block text-gray-700 font-medium mb-2">Subject</label>
                        <input type="text" id="subject" class="w-full px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500" required>
                    </div>
                    <div>
                        <label for="message" class="block text-gray-700 font-medium mb-2">Your Message</label>
                        <textarea id="message" rows="5" class="w-full px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500" required></textarea>
                    </div>
                    <div>
                        <button type="submit" class="bg-blue-600 text-white px-6 py-3 rounded-md font-semibold hover:bg-blue-700 transition w-full md:w-auto">
                            Send Message
                        </button>
                    </div>
                </form>
                
                <div class="mt-12 grid grid-cols-1 md:grid-cols-3 gap-6 text-center">
                    <div class="p-6 bg-blue-50 rounded-lg">
                        <div class="w-12 h-12 bg-blue-100 rounded-full flex items-center justify-center mx-auto mb-4">
                            <i class="fas fa-envelope text-blue-600 text-xl"></i>
                        </div>
                        <h4 class="font-semibold">Email Me</h4>
                        <p class="text-gray-600">snehalryadav29@gmail.com</p>
                    </div>
                    <div class="p-6 bg-blue-50 rounded-lg">
                        <div class="w-12 h-12 bg-blue-100 rounded-full flex items-center justify-center mx-auto mb-4">
                            <i class="fas fa-phone-alt text-blue-600 text-xl"></i>
                        </div>
                        <h4 class="font-semibold">Call Me</h4>
                        <p class="text-gray-600">7600796321</p>
                    </div>
                    <div class="p-6 bg-blue-50 rounded-lg">
                        <div class="w-12 h-12 bg-blue-100 rounded-full flex items-center justify-center mx-auto mb-4">
                            <i class="fas fa-map-marker-alt text-blue-600 text-xl"></i>
                        </div>
                        <h4 class="font-semibold">Location</h4>
                        <p class="text-gray-600">Pune, India</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <script>
        // Mobile menu toggle
        const mobileMenuButton = document.querySelector('.mobile-menu-button');
        const navLinks = document.querySelector('nav .hidden.md\:flex');
        
        mobileMenuButton.addEventListener('click', () => {
            navLinks.classList.toggle('hidden');
            navLinks.classList.toggle('flex');
            navLinks.classList.toggle('flex-col');
            navLinks.classList.toggle('absolute');
            navLinks.classList.toggle('top-16');
            navLinks.classList.toggle('left-0');
            navLinks.classList.toggle('w-full');
            navLinks.classList.toggle('bg-white');
            navLinks.classList.toggle('p-4');
            navLinks.classList.toggle('space-y-4');
            navLinks.classList.toggle('shadow-lg');
        });

        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    window.scrollTo({
                        top: target.offsetTop - 80,
                        behavior: 'smooth'
                    });
                    
                    // Close mobile menu if open
                    if (!navLinks.classList.contains('hidden')) {
                        mobileMenuButton.click();
                    }
                }
            });
        });

        // Animate skill bars on scroll
        function animateSkills() {
            const skillBars = document.querySelectorAll('.skill-bar');
            skillBars.forEach(bar => {
                const width = bar.getAttribute('data-width');
                if (isInViewport(bar) && !bar.style.width) {
                    bar.style.width = width;
                }
            });
        }
        

        function isInViewport(element) {
            const rect = element.getBoundingClientRect();
            return (
                rect.top >= 0 &&
                rect.left >= 0 &&
                rect.bottom <= (window.innerHeight || document.documentElement.clientHeight) &&
                rect.right <= (window.innerWidth || document.documentElement.clientWidth)
            );
        }

        // Form submission
        const contactForm = document.getElementById('contactForm');
        if (contactForm) {
            contactForm.addEventListener('submit', function(e) {
                e.preventDefault();
                // Here you would typically send the form data to a server
                alert('Thank you for your message! I will get back to you soon.');
                contactForm.reset();
            });
        }

        // Run animations on page load and scroll
        window.addEventListener('load', animateSkills);
        window.addEventListener('scroll', animateSkills);
    </script>
    <script>
  if ("serviceWorker" in navigator) {
    window.addEventListener("load", () => {
      navigator.serviceWorker
        .register("service-worker.js")
        .then(reg => console.log("Service Worker registered"))
        .catch(err => console.error("Service Worker error:", err));
    });
  }
</script>
</body>
</html>
