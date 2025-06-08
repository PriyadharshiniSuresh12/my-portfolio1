<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Priyadharshini S - Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f3f4f6; /* Light gray background */
            color: #333;
        }
        .section-heading {
            position: relative;
            display: inline-block;
            margin-bottom: 2rem;
            font-size: 2.25rem; /* text-4xl */
            font-weight: 700; /* font-bold */
            color: #1a202c; /* darker text */
        }
        .section-heading::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: -8px;
            width: 70%;
            height: 4px;
            background-color: #6366f1; /* Indigo 500 */
            border-radius: 9999px; /* rounded-full */
        }
        .card {
            background-color: white;
            padding: 1.5rem;
            border-radius: 0.75rem; /* rounded-xl */
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); /* shadow-md */
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px rgba(0, 0, 0, 0.15); /* shadow-lg */
        }
        .btn-primary {
            background-color: #6366f1; /* Indigo 500 */
            color: rgb(255, 255, 255);
            padding: 0.75rem 1.5rem;
            border-radius: 0.5rem; /* rounded-lg */
            transition: background-color 0.3s ease;
        }
        .btn-primary:hover {
            background-color: #4682b4; /* Indigo 600 */
        }
        .social-icon {      
            font-size: 1.8rem;
            color: #6366f1;
            transition: color 0.3s ease;
        }
        .social-icon:hover {
            color: #4f46e5;
        }
        /* Fade-in animation for sections */
        .fade-in-section {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.6s ease-out, transform 0.6s ease-out;
        }
        .fade-in-section.is-visible {
            opacity: 1;
            transform: translateY(0);
        }
        .delay-100 { transition-delay: 0.1s; }
        .delay-200 { transition-delay: 0.2s; }
        .delay-300 { transition-delay: 0.3s; }
        .delay-400 { transition-delay: 0.4s; }
    </style>
</head>
<body class="bg-gray-100 text-gray-800">

    <header class="bg-white shadow-md py-4 px-6 md:px-10 sticky top-0 z-50 rounded-b-xl">
        <nav class="container mx-auto flex justify-between items-center">
            <a href="#" class="text-3xl font-bold text-indigo-600 rounded-lg">Priyadharshini S</a>
            <div class="hidden md:flex space-x-6">
                <a href="#about" class="text-gray-700 hover:text-indigo-600 transition duration-300 rounded-lg p-2">About</a>
                <a href="#skills" class="text-gray-700 hover:text-indigo-600 transition duration-300 rounded-lg p-2">Skills</a>
                <a href="#projects" class="text-gray-700 hover:text-indigo-600 transition duration-300 rounded-lg p-2">Projects</a>
                <a href="#Internship" class="text-gray-700 hover:text-indigo-600 transition duration-300 rounded-lg p-2">Internship</a>
                <a href="#contact" class="text-gray-700 hover:text-indigo-600 transition duration-300 rounded-lg p-2">Contact</a>
            </div>
            <button id="mobile-menu-button" class="md:hidden text-gray-700 focus:outline-none rounded-lg p-2">
                <i class="fas fa-bars text-2xl"></i>
            </button>
        </nav>
        <div id="mobile-menu" class="hidden md:hidden absolute top-full left-0 w-full bg-white shadow-lg py-4 rounded-b-xl">
            <div class="flex flex-col items-center space-y-4">
                <a href="#about" class="text-gray-700 hover:text-indigo-600 transition duration-300 rounded-lg p-2 block w-full text-center" onclick="toggleMobileMenu()">About</a>
                <a href="#skills" class="text-gray-700 hover:text-indigo-600 transition duration-300 rounded-lg p-2 block w-full text-center" onclick="toggleMobileMenu()">Skills</a>
                <a href="#projects" class="text-gray-700 hover:text-indigo-600 transition duration-300 rounded-lg p-2 block w-full text-center" onclick="toggleMobileMenu()">Projects</a>
                <a href="#Internship" class="text-gray-700 hover:text-indigo-600 transition duration-300 rounded-lg p-2 block w-full text-center" onclick="toggleMobileMenu()">#Internship</a>
                <a href="#contact" class="text-gray-700 hover:text-indigo-600 transition duration-300 rounded-lg p-2 block w-full text-center" onclick="toggleMobileMenu()">Contact</a>
                
            </div>
        </div>
    </header>

    <main class="container mx-auto px-6 md:px-10 py-8">

        <section id="hero" class="flex flex-col md:flex-row items-center justify-center text-center md:text-left min-h-screen py-16 fade-in-section">
            <div class="WhatsApp Image 2025-06-08 at 17.20.51_f55ca86c.jpg">
                <h1 class="text-5xl md:text-6xl font-extrabold leading-tight text-gray-900 mb-4">
                    Hi, I'm <span class="text-indigo-600">Priyadharshini S</span>
                </h1>
                <p class="text-xl md:text-2xl text-gray-600 mb-6">
                    An Enthusiastic and Motivated <span class="font-semibold text-indigo-700">UI/UX Fresher</span>.
                </p>
                <p class="text-lg text-gray-500 mb-8 max-w-xl mx-auto md:mx-0">
                    Welcome to my portfolio! I'm seeking an entry-level position in the software industry, eager to learn and contribute to a dynamic team.I focus on designing user-friendly interfaces and enhancing user experiences for web and mobile applications. 
                </p>
                <div class="flex flex-col sm:flex-row space-y-4 sm:space-y-0 sm:space-x-4 justify-center md:justify-start">
                    <a href="#projects" class="btn-primary inline-block text-center rounded-lg shadow-md hover:shadow-lg">View My Work</a>
                    <a href="#contact" class="bg-gray-200 text-gray-800 py-3 px-6 rounded-lg shadow-md hover:bg-gray-300 hover:shadow-lg transition duration-300 inline-block text-center">Get in Touch</a>
                </div>
            </div>
            
        </section>

        <section id="about" class="py-16 bg-white rounded-xl shadow-lg mb-12 px-6 fade-in-section">
            <h2 class="section-heading text-center mx-auto mb-10">About Me</h2>
            <div class="flex flex-col md:flex-row items-center md:space-x-12 max-w-4xl mx-auto">
                <div class="md:w-1/2 text-center md:text-left">
                    <p class="text-lg text-gray-700 leading-relaxed mb-6">
                        As an enthusiastic and motivated UI/UX Fresher, I am dedicated to creating intuitive and efficient user experiences. My strong skills in Figma and Adobe XD enable me to design visually appealing and user-friendly interfaces for both web and mobile applications. 
                    </p>
                    <p class="text-lg text-gray-700 leading-relaxed">
                        I am eager to learn and contribute to a dynamic team, leveraging my foundational knowledge in HTML, CSS, and C to bridge design with development. I am committed to continuous growth and delivering high-quality results.
                    </p>
                    <a href="#contact" class="mt-6 inline-block btn-primary shadow-md hover:shadow-lg">Let's Connect</a>
                </div>
            </div>
        </section>

        <section id="skills" class="py-16 bg-gray-50 rounded-xl shadow-lg mb-12 px-6 fade-in-section">
            <h2 class="section-heading text-center mx-auto mb-10">My Skills</h2>
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8 max-w-5xl mx-auto">
                <div class="card flex items-center p-4">
                    <i class="fas fa-palette text-4xl text-pink-500 mr-4"></i>
                    <div>
                        <h3 class="text-xl font-bold mb-1">UI/UX Design</h3>
                        <p class="text-gray-600">Figma, Adobe XD</p>
                    </div>
                </div>
                <div class="card flex items-center p-4">
                    <i class="fas fa-code text-4xl text-blue-600 mr-4"></i>
                    <div>
                        <h3 class="text-xl font-bold mb-1">Programming Languages</h3>
                        <p class="text-gray-600">C,Python, HTML, CSS</p>
                    </div>
                </div>
                <div class="card flex items-center p-4">
                    <i class="fas fa-tools text-4xl text-gray-700 mr-4"></i>
                    <div>
                        <h3 class="text-xl font-bold mb-1">Development Tools</h3>
                        <p class="text-gray-600">Visual Studio Code</p>
                    </div>
                </div>
                <div class="card flex items-center p-4">
                    <i class="fas fa-file-alt text-4xl text-green-700 mr-4"></i>
                    <div>
                        <h3 class="text-xl font-bold mb-1">Office Applications</h3>
                        <p class="text-gray-600">Microsoft Word, Excel, PowerPoint</p>
                    </div>
                </div>
                 <div class="card flex items-center p-4">
                    <i class="fas fa-bezier-curve text-4xl text-purple-600 mr-4"></i>
                    <div>
                        <h3 class="text-xl font-bold mb-1">Design Concepts</h3>
                        <p class="text-gray-600">User Flows, Prototyping</p>
                    </div>
                </div>
                <div class="card flex items-center p-4">
                    <i class="fas fa-mobile-alt text-4xl text-indigo-600 mr-4"></i>
                    <div>
                        <h3 class="text-xl font-bold mb-1">Responsive Design</h3>
                        <p class="text-gray-600">Web & Mobile Optimization</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="projects" class="py-16 bg-white rounded-xl shadow-lg mb-12 px-6 fade-in-section">
            <h2 class="section-heading text-center mx-auto mb-10">My Projects</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-2 gap-8 max-w-4xl mx-auto">
                <div class="card">
                    <img src="https://placehold.co/600x400/E5E7EB/4F46E5?text=Web+AR+App" alt="Web based AR application" class="rounded-t-lg mb-4 object-cover w-full h-48">
                    <h3 class="text-2xl font-bold text-gray-900 mb-2">Web-based AR Application</h3>
                    <p class="text-gray-700 text-base mb-4">
                        [cite_start]Winner of a Hackathon at Arunai Engineering College (Feb 2025).Developed an interactive WebAR application using MindAR.js for image-based AR experiences. Designed and integrated 3D assets into the AR environment, ensuring seamless rendering and performance. Implemented dynamic 3D model loading and optimized real-time interaction with AR overlays. 
                    </p>
                    <div class="flex flex-wrap gap-2 mb-4">
                        <span class="bg-indigo-100 text-indigo-800 text-xs font-semibold px-2.5 py-0.5 rounded-full">WebAR</span>
                        <span class="bg-indigo-100 text-indigo-800 text-xs font-semibold px-2.5 py-0.5 rounded-full">MindAR.js</span>
                        <span class="bg-indigo-100 text-indigo-800 text-xs font-semibold px-2.5 py-0.5 rounded-full">3D Assets</span>
    
                    </div>
                </div>

                <div class="card">
                    <img src="https://placehold.co/600x400/E5E7EB/4F46E5?text=Food+App+Design" alt="Food Order App using Figma" class="rounded-t-lg mb-4 object-cover w-full h-48">
                    <h3 class="text-2xl font-bold text-gray-900 mb-2">Food Order App (Figma Design)</h3>
                    <p class="text-gray-700 text-base mb-4">
                        Designed a visually appealing food order application using Figma with high-quality images. Features include easy navigation and search functionality to find preferred cuisines or dishes, a streamlined ordering process with secure payment options, real-time order tracking and delivery updates, and a user-friendly interface with personalized recommendations and promotions.
                    </p>
                    <div class="flex flex-wrap gap-2 mb-4">
                        <span class="bg-indigo-100 text-indigo-800 text-xs font-semibold px-2.5 py-0.5 rounded-full">Figma</span>
                        <span class="bg-indigo-100 text-indigo-800 text-xs font-semibold px-2.5 py-0.5 rounded-full">UI/UX Design</span>
                        <span class="bg-indigo-100 text-indigo-800 text-xs font-semibold px-2.5 py-0.5 rounded-full">Prototyping</span>
                    </div>
                
                </div>

                <div class="card">
                    <img src="https://placehold.co/600x400/E5E7EB/4F46E5?text=Fuel+System" alt="Fuel Level Monitoring System" class="rounded-t-lg mb-4 object-cover w-full h-48">
                    <h3 class="text-2xl font-bold text-gray-900 mb-2">Fuel Level Monitoring System</h3>
                    <p class="text-gray-700 text-base mb-4">
                        Designed and implemented a real-time fuel monitoring system using IoT and embedded systems. The project reads analog values from a float sensor, processes them through ESP8266, and displays fuel levels using an LED bar graph. The system alerts users with a buzzer when fuel is low and optionally sends data to a web interface or cloud dashboard for remote monitoring.
                    </p>
                    <div class="flex flex-wrap gap-2 mb-4">
                        <span class="bg-indigo-100 text-indigo-800 text-xs font-semibold px-2.5 py-0.5 rounded-full">IoT</span>
                        <span class="bg-indigo-100 text-indigo-800 text-xs font-semibold px-2.5 py-0.5 rounded-full">ESP8266</span>
                        <span class="bg-indigo-100 text-indigo-800 text-xs font-semibold px-2.5 py-0.5 rounded-full">Arduino IDE</span>
                        <span class="bg-indigo-100 text-indigo-800 text-xs font-semibold px-2.5 py-0.5 rounded-full">Embedded Systems</span>
                    </div>
                
                </div>

                <div class="card">
                    <img src="https://placehold.co/600x400/E5E7EB/4F46E5?text=Smart+Bottle" alt="Smart Water Bottle" class="rounded-t-lg mb-4 object-cover w-full h-48">
                    <h3 class="text-2xl font-bold text-gray-900 mb-2">Smart Water Bottle</h3>
                    <p class="text-gray-700 text-base mb-4">
                        Developed a smart water bottle that monitors user hydration in real-time. The system tracks water intake, reminds the user to drink water, and syncs data to a web/mobile interface. The goal is to promote healthy hydration habits using smart technology. Key features include water level detection, temperature sensing, hydration reminders via buzzer/light, app/web dashboard syncing, and a battery-efficient, portable design.
                    </p>
                    <div class="flex flex-wrap gap-2 mb-4">
                        <span class="bg-indigo-100 text-indigo-800 text-xs font-semibold px-2.5 py-0.5 rounded-full">IoT</span>
                        <span class="bg-indigo-100 text-indigo-800 text-xs font-semibold px-2.5 py-0.5 rounded-full">ESP32/ESP8266</span>
                        <span class="bg-indigo-100 text-indigo-800 text-xs font-semibold px-2.5 py-0.5 rounded-full">Sensors</span>
                        <span class="bg-indigo-100 text-indigo-800 text-xs font-semibold px-2.5 py-0.5 rounded-full">Firebase</span>
                    </div>

            </div>
        </section>

        <section id="contact" class="py-16 bg-gray-50 rounded-xl shadow-lg px-6 fade-in-section">
            <h2 class="section-heading text-center mx-auto mb-10">Get in Touch</h2>
            <div class="max-w-xl mx-auto text-center">
                <p class="text-lg text-gray-700 mb-8">
                    Have a project in mind, a question, or just want to say hello? Feel free to reach out! I'm always open to new opportunities and collaborations.
                </p>
                <div class="flex flex-col space-y-6">
                    <a href="mailto:your.email@example.com" class="bg-indigo-600 text-white py-3 px-6 rounded-lg shadow-md hover:bg-indigo-700 transition duration-300 flex items-center justify-center text-lg">
                        <i class="fas fa-envelope mr-3"></i> sureshpriyatvm@gmail.com
                    </a>
                    <a href="tel:+919361423064" class="bg-gray-200 text-gray-800 py-3 px-6 rounded-lg shadow-md hover:bg-gray-300 transition duration-300 flex items-center justify-center text-lg">
                      <i class="fas fa-phone mr-3"></i> +91 9361423064
                    </a>
                </div>
                <div class="flex justify-center space-x-6 mt-10">
                    <a href="www.linkedin.com/in/priyadharshini-s-21438a258" target="_blank" class="social-icon hover:scale-110 transition-transform duration-300" aria-label="LinkedIn Profile">
                        <i class="fab fa-linkedin"></i>
                    </a>
                    <a href="PriyadharshiniSuresh12" target="_blank" class="social-icon hover:scale-110 transition-transform duration-300" aria-label="GitHub Profile">
                        <i class="fab fa-github"></i>
                    </a>
                </div>
            </div>
        </section>

    </main>



    <script>
        // JavaScript for mobile menu toggle
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');

        function toggleMobileMenu() {
            mobileMenu.classList.toggle('hidden');
        }

        mobileMenuButton.addEventListener('click', toggleMobileMenu);

        // Close mobile menu when clicking outside (optional, but good for UX)
        document.addEventListener('click', function(event) {
            const isClickInside = mobileMenu.contains(event.target) || mobileMenuButton.contains(event.target);
            if (!isClickInside && !mobileMenu.classList.contains('hidden')) {
                mobileMenu.classList.add('hidden');
            }
        });

        // Optional: Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();

                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Intersection Observer for fade-in animations
        document.addEventListener("DOMContentLoaded", function() {
            const sections = document.querySelectorAll(".fade-in-section");

            const observerOptions = {
                root: null, // relative to the viewport
                rootMargin: "0px",
                threshold: 0.1 // 10% of the section must be visible to trigger
            };

            const observer = new IntersectionObserver((entries, observer) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add("is-visible");
                        observer.unobserve(entry.target); // Stop observing once visible
                    }
                });
            }, observerOptions);

            sections.forEach(section => {
                observer.observe(section);
            });
        });
    </script>
</body>
</html>
