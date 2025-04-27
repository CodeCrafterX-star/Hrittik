<!DOCTYPE html>
<html lang="en" style="scroll-behavior: smooth;">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Futuristic Portfolio</title>
  <!-- Note: cdn.tailwindcss.com is used here for development. For production, install Tailwind CSS as a PostCSS plugin or use the Tailwind CLI: https://tailwindcss.com/docs/installation -->
  <script src="https://cdn.tailwindcss.com"></script>
  <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Inter', sans-serif;
      margin: 0;
      padding: 0;
    }
    #webgl-bg {
      position: absolute;
      inset: 0;
      z-index: -1;
      width: 100%;
      height: 100%;
      overflow: hidden;
    }
    .glass {
      background: rgba(255, 255, 255, 0.08);
      backdrop-filter: blur(15px);
      border: 1px solid rgba(255, 255, 255, 0.15);
      box-shadow: 0 8px 32px rgba(0, 0, 0, 0.3);
      transition: transform 0.7s ease-in-out, box-shadow 0.7s ease-in-out, scale 0.5s ease-in-out; /* Smoother transitions */
      transform: perspective(1000px) rotateX(0deg) rotateY(0deg);
      border-radius: 0;
      /* Updated animations with smoother timing */
      animation: scaleFadeIn 1.2s ease-in-out forwards, pulse 2s ease-in-out 1s forwards, float 4s ease-in-out infinite;
    }
    .glass:hover {
      transform: perspective(1000px) rotateX(2deg) rotateY(2deg) translateY(-8px) scale(1.05) rotateZ(5deg);
      box-shadow: 0 15px 40px rgba(0, 0, 0, 0.5);
    }
    /* Smoother animations */
    @keyframes scaleFadeIn {
      0% {
        transform: scale(0.85); /* Slightly larger starting scale for smoother effect */
        opacity: 0;
      }
      100% {
        transform: scale(1);
        opacity: 1;
      }
    }
    @keyframes pulse {
      0%, 100% {
        transform: scale(1);
      }
      50% {
        transform: scale(1.03); /* Reduced scale for smoother pulse */
      }
    }
    @keyframes float {
      0%, 100% {
        transform: translateY(0);
      }
      50% {
        transform: translateY(-8px); /* Slightly reduced float distance */
      }
    }
    .input-field {
      transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
    }
    .input-field:focus + .input-label,
    .input-field:not(:placeholder-shown) + .input-label {
      transform: translateY(-1.75rem);
      font-size: 0.8rem;
      color: #a78bfa;
    }
    .input-field:invalid:not(:placeholder-shown) {
      border-color: #f87171;
    }
    section {
      opacity: 0;
      transform: translateY(30px);
      transition: opacity 0.8s cubic-bezier(0.4, 0, 0.2, 1), transform 0.8s cubic-bezier(0.4, 0, 0.2, 1);
      will-change: opacity, transform;
    }
    section.visible {
      opacity: 1;
      transform: translateY(0);
    }
    .ripple {
      position: relative;
      overflow: hidden;
    }
    .ripple::after {
      content: '';
      position: absolute;
      width: 100px;
      height: 100px;
      background: rgba(255, 255, 250, 0.3);
      border-radius: 50%;
      transform: scale(0);
      opacity: 0;
      top: 50%;
      left: 50%;
      pointer-events: none;
      transition: transform 0.6s cubic-bezier(0.4, 0, 0.2, 1), opacity 0.6s cubic-bezier(0.4, 0, 0.2, 1);
    }
    .ripple:active::after {
      transform: scale(2);
      opacity: 1;
      transition: transform 0.3s cubic-bezier(0.4, 0, 0.2, 1), opacity 0.3s cubic-bezier(0.4, 0, 0.2, 1);
    }
    .loading::before {
      content: '';
      display: inline-block;
      width: 16px;
      height: 16px;
      border: 2px solid #fff;
      border-top-color: transparent;
      border-radius: 50%;
      animation: spin 1s linear infinite;
      margin-right: 8px;
    }
    @keyframes spin {
      to { transform: rotate(360deg); }
    }
    .nav-link {
      position: relative;
    }
    .nav-link::after {
      content: '';
      position: absolute;
      width: 0;
      height: 2px;
      bottom: -4px;
      left: 0;
      background: #a78bfa;
      transition: width 0.3s cubic-bezier(0.4, 0, 0.2, 1);
    }
    .nav-link:hover::after {
      width: 100%;
    }
    .cursor-trail {
      position: fixed;
      width: 12px;
      height: 12px;
      background: radial-gradient(circle, #a78bfa 0%, transparent 70%);
      border-radius: 50%;
      pointer-events: none;
      z-index: 9999;
      transition: transform 0.2s cubic-bezier(0.4, 0, 0.2, 1);
      transform: translate(-50%, -50%) scale(1);
    }
    .cursor-trail.active {
      transform: translate(-50%, -50%) scale(1.5);
    }
    #menu-toggle {
      display: none;
    }
    #menu-toggle:checked ~ .nav-actions #menu {
      display: flex;
    }
    .nav-container {
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: relative;
    }
    .nav-actions {
      display: flex;
      align-items: center;
      gap: 1rem;
    }
    #menu {
      display: flex;
      flex-direction: row;
      align-items: center;
      gap: 1.5rem;
    }
    #menu li {
      margin: 0;
    }
    #menu a {
      font-size: 0.9rem;
    }
    .fullscreen-btn {
      background: transparent;
      border: none;
      color: #a78bfa;
      font-size: 1.2rem;
      cursor: pointer;
      padding: 0.5rem;
      transition: color 0.3s ease;
    }
    .fullscreen-btn:hover {
      color: #d8b4fe;
    }
    .hero-button, .contact-button {
      display: block;
      margin-left: auto;
      margin-right: auto;
      width: fit-content;
    }
    .profile-pic {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      object-fit: cover;
      border: 3px solid #a78bfa;
      box-shadow: 0 4px 20px rgba(167, 139, 250, 0.5);
      margin: 0 auto 1rem auto;
      display: block;
    }
    @media (max-width: 768px) {
      .nav-actions {
        width: auto;
        justify-content: flex-end;
        padding-right: 0;
      }
      #menu {
        display: none;
        position: absolute;
        top: 100%;
        left: 0;
        right: 0;
        background: rgba(17, 24, 39, 0.95);
        backdrop-filter: blur(10px);
        padding: 0.5rem;
        flex-direction: row;
        justify-content: center;
        align-items: center;
      }
      #menu-toggle:checked ~ .nav-actions #menu {
        display: flex;
      }
      #menu a, .fullscreen-btn {
        font-size: 0.8rem;
      }
      .hero-button, .contact-button {
        width: 100%;
        max-width: 200px;
      }
      .menu-icon {
        display: block;
        cursor: pointer;
        margin-left: auto;
      }
      .menu-icon span {
        display: block;
        width: 24px;
        height: 3px;
        background: #fff;
        margin: 5px 0;
        transition: all 0.3s ease;
      }
      #menu-toggle:checked + .menu-icon span:nth-child(1) {
        transform: rotate(45deg) translate(5px, 5px);
      }
      #menu-toggle:checked + .menu-icon span:nth-child(2) {
        opacity: 0;
      }
      #menu-toggle:checked + .menu-icon span:nth-child(3) {
        transform: rotate(-45deg) translate(7px, -7px);
      }
      .fullscreen-btn-nav {
        display: none;
      }
      .profile-pic {
        width: 100px;
        height: 100px;
      }
    }
    @media (min-width: 769px) {
      .menu-icon {
        display: none;
      }
      #menu {
        display: flex !important;
      }
      #menu a {
        font-size: 1rem;
      }
      .hero-button, .contact-button {
        width: auto;
      }
      .fullscreen-btn-nav {
        display: block;
      }
    }
  </style>
</head>
<body class="bg-gray-950 text-gray-100">
  <!-- Navigation -->
  <nav class="fixed w-full top-0 z-30 backdrop-blur-xl bg-gray-900/10 border-b border-gray-800/20">
    <div class="container mx-auto px-4 sm:px-6 py-4 nav-container">
      <h1 class="text-2xl sm:text-3xl font-extrabold text-white tracking-tighter">Portfolio</h1>
      <input type="checkbox" id="menu-toggle" class="hidden">
      <label for="menu-toggle" class="menu-icon">
        <span></span>
        <span></span>
        <span></span>
      </label>
      <div class="nav-actions">
        <ul id="menu" class="flex">
          <li data-aos="fade-up" data-aos-duration="1000" data-aos-delay="100"><a href="#home" class="nav-link text-gray-200 hover:text-purple-400 font-medium transition duration-300">Home</a></li>
          <li data-aos="fade-up" data-aos-duration="1000" data-aos-delay="300"><a href="#about" class="nav-link text-gray-200 hover:text-purple-400 font-medium transition duration-300">About</a></li>
          <li data-aos="fade-up" data-aos-duration="1000" data-aos-delay="500"><a href="#contact" class="nav-link text-gray-200 hover:text-purple-400 font-medium transition duration-300">Contact</a></li>
          <li class="fullscreen-btn-menu"><button id="fullscreen-btn-menu" class="fullscreen-btn" title="Toggle Fullscreen"><span>⬜</span></button></li>
        </ul>
        <button id="fullscreen-btn-nav" class="fullscreen-btn fullscreen-btn-nav" title="Toggle Fullscreen">
          <span>⬜</span>
        </button>
      </div>
    </div>
  </nav>

  <!-- Hero Section -->
  <section id="home" class="min-h-screen flex items-center justify-center bg-gradient-to-br from-gray-900 to-blue-950 relative overflow-hidden z-10">
    <canvas id="webgl-bg"></canvas>
    <div class="container mx-auto px-4 sm:px-6 text-center relative z-20" data-aos="zoom-in" data-aos-duration="1400">
      <h2 class="text-4xl sm:text-5xl md:text-7xl font-extrabold mb-6 bg-clip-text text-transparent bg-gradient-to-r from-purple-400 to-pink-500">Next-Gen Web Architect</h2>
      <p class="text-lg sm:text-xl md:text-2xl mb-8 max-w-3xl mx-auto text-gray-200" data-aos="fade-up" data-aos-delay="300" data-aos-duration="1200">
        Crafting immersive, high-performance digital realms with visionary tech.
      </p>
      <a href="#contact" class="hero-button inline-block bg-gradient-to-r from-purple-400 to-pink-500 text-white px-6 sm:px-10 py-3 sm:py-4 rounded-full font-semibold glass ripple transition duration-300" data-aos="fade-up" data-aos-delay="600" data-aos-duration="1200">Launch a Project</a>
    </div>
  </section>

  <!-- About Section -->
  <section id="about" class="py-20 sm:py-28 bg-gray-950">
    <div class="container mx-auto px-4 sm:px-6">
      <h2 class="text-4xl sm:text-5xl font-bold text-center mb-12 sm:mb-16 text-white" data-aos="fade-up" data-aos-duration="1000">About Me</h2>
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8 sm:gap-12 max-w-5xl mx-auto">
        <div class="glass p-8 sm:p-12" data-aos="fade-right" data-aos-duration="800" data-aos-delay="200">
          <img src="https://i.ibb.co/fGdrVG5H/IMG-20250226-192236-2.jpg" alt="Profile Picture" class="profile-pic">
          <h3 class="text-2xl sm:text-3xl font-semibold mb-4 text-center text-white">Who I Am</h3>
          <p class="text-gray-200 text-center">
            A creative visionary building seamless, futuristic web experiences.
          </p>
        </div>
        <div class="glass p-8 sm:p-12" data-aos="fade-left" data-aos-duration="800" data-aos-delay="400">
          <h3 class="text-2xl sm:text-3xl font-semibold mb-4 text-center text-white">My Expertise</h3>
          <p class="text-gray-200 text-center">
            Master of JavaScript, React, Tailwind CSS, and Node.js, delivering next-level solutions.
          </p>
        </div>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="py-20 sm:py-28 bg-gradient-to-b from-gray-950 to-gray-900">
    <div class="container mx-auto px-4 sm:px-6">
      <h2 class="text-4xl sm:text-5xl font-bold text-center mb-12 sm:mb-16 text-white" data-aos="fade-up" data-aos-duration="1000">Connect With Me</h2>
      <div class="max-w-lg mx-auto" data-aos="fade-up" data-aos-duration="1200" data-aos-delay="200">
        <div class="space-y-8">
          <div class="relative">
            <input type="text" id="name" class="input-field w-full px-5 py-4 bg-transparent border-b-2 border-gray-500 focus:border-purple-400 outline-none text-white" placeholder="Your Name" required>
            <label for="name" class="input-label absolute left-5 top-4 text-gray-300 transition-all duration-300">Your Name</label>
          </div>
          <div class="relative">
            <input type="email" id="email" class="input-field w-full px-5 py-4 bg-transparent border-b-2 border-gray-500 focus:border-purple-400 outline-none text-white" placeholder="Your Email" required>
            <label for="email" class="input-label absolute left-5 top-4 text-gray-300 transition-all duration-300">Your Email</label>
          </div>
          <div class="relative">
            <textarea id="message" class="input-field w-full px-5 py-4 bg-transparent border-b-2 border-gray-500 focus:border-purple-400 outline-none text-white" rows="5" placeholder="Your Message" required></textarea>
            <label for="message" class="input-label absolute left-5 top-4 text-gray-300 transition-all duration-300">Your Message</label>
          </div>
          <button id="submit-btn" class="contact-button w-full bg-gradient-to-r from-purple-400 to-pink-500 text-white px-8 py-4 rounded-full font-semibold glass ripple transition duration-300" onclick="submitForm()">Send Message</button>
          <div id="success-animation" class="hidden w-24 h-24 mx-auto"></div>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-gray-950 py-10 sm:py-12">
    <div class="container mx-auto px-4 sm:px-6 text-center">
      <p class="text-gray-400 text-sm">© 2025 Futuristic Portfolio. All rights reserved.</p>
    </div>
  </footer>

  <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r134/three.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/bodymovin/5.9.6/lottie.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js"></script>
  <script>
    // Initialize AOS
    AOS.init({
      once: true,
      offset: 120,
      easing: 'cubic-bezier(0.4, 0, 0.2, 1)',
      duration: 1200,
    });

    // Initialize EmailJS with your provided Public Key
    (function() {
      emailjs.init("yIIS7mX-ioJAShWBN");
    })();

    // WebGL Background (Three.js)
    const initWebGL = () => {
      const canvas = document.getElementById('webgl-bg');
      if (!canvas) return;
      const scene = new THREE.Scene();
      const camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
      const renderer = new THREE.WebGLRenderer({ canvas, alpha: true });
      renderer.setSize(window.innerWidth, window.innerHeight);
      renderer.setPixelRatio(Math.min(window.devicePixelRatio, 2));

      const count = window.innerWidth < 768 ? 300 : 500;
      const particlesGeometry = new THREE.BufferGeometry();
      const positions = new Float32Array(count * 3);
      for (let i = 0; i < count * 3; i++) {
        positions[i] = (Math.random() - 0.5) * 10;
      }
      particlesGeometry.setAttribute('position', new THREE.BufferAttribute(positions, 3));
      const particlesMaterial = new THREE.PointsMaterial({
        size: 0.02,
        sizeAttenuation: true,
        transparent: true,
        color: '#a78bfa',
      });
      const particles = new THREE.Points(particlesGeometry, particlesMaterial);
      scene.add(particles);
      camera.position.z = 5;

      const animate = () => {
        requestAnimationFrame(animate);
        particles.rotation.y += 0.002;
        renderer.render(scene, camera);
      };
      animate();

      window.addEventListener('resize', () => {
        camera.aspect = window.innerWidth / window.innerHeight;
        camera.updateProjectionMatrix();
        renderer.setSize(window.innerWidth, window.innerHeight);
      });
    };

    // Fallback if WebGL is not supported or fails
    const canvas = document.getElementById('webgl-bg');
    if (canvas && (canvas.getContext('webgl') || canvas.getContext('experimental-webgl'))) {
      window.addEventListener('load', initWebGL);
    } else {
      canvas.style.background = 'linear-gradient(135deg, #0f172a 0%, #1e3a8a 100%)';
      canvas.style.zIndex = '-1';
    }

    // Cursor trail effect (disable on mobile for performance)
    if (window.innerWidth > 768) {
      const cursorTrail = document.createElement('div');
      cursorTrail.classList.add('cursor-trail');
      document.body.appendChild(cursorTrail);
      let lastUpdate = 0;
      document.addEventListener('mousemove', (e) => {
        const now = performance.now();
        if (now - lastUpdate < 16) return;
        lastUpdate = now;
        cursorTrail.style.left = `${e.clientX}px`;
        cursorTrail.style.top = `${e.clientY}px`;
        cursorTrail.classList.add('active');
        setTimeout(() => cursorTrail.classList.remove('active'), 100);
      });
    }

    // Scroll-triggered section animations
    const sections = document.querySelectorAll('section');
    const observer = new IntersectionObserver(
      (entries) => {
        entries.forEach((entry) => {
          if (entry.isIntersecting) {
            entry.target.classList.add('visible');
            observer.unobserve(entry.target);
          }
        });
      },
      { threshold: 0.3 }
    );
    sections.forEach((section) => observer.observe(section));

    // Form submission with EmailJS
    let isSubmitting = false;
    async function submitForm() {
      if (isSubmitting) return;
      isSubmitting = true;

      const submitBtn = document.getElementById('submit-btn');
      const name = document.getElementById('name').value.trim();
      const email = document.getElementById('email').value.trim();
      const message = document.getElementById('message').value.trim();

      if (!name || !email || !message) {
        alert('Please complete all fields.');
        isSubmitting = false;
        return;
      }

      submitBtn.classList.add('loading');
      submitBtn.disabled = true;

      try {
        const response = await emailjs.send('service_jqyuztj', 'template_y1ipa5o', {
          from_name: name,
          from_email: email,
          message: message,
          title: "Portfolio Contact Form",
        });
        console.log('Email sent successfully:', response);
        submitBtn.classList.remove('loading');
        submitBtn.disabled = false;

        const successAnimation = document.getElementById('success-animation');
        successAnimation.classList.remove('hidden');
        lottie.loadAnimation({
          container: successAnimation,
          renderer: 'svg',
          loop: false,
          autoplay: true,
          path: 'https://assets.lottiefiles.com/packages/lf20_jbrw3hcz.json',
        });
        setTimeout(() => successAnimation.classList.add('hidden'), 2000);

        document.getElementById('name').value = '';
        document.getElementById('email').value = '';
        document.getElementById('message').value = '';
      } catch (error) {
        console.error('Email send failed:', error);
        alert('Failed to send message. Please try again later.');
        submitBtn.classList.remove('loading');
        submitBtn.disabled = false;
      } finally {
        isSubmitting = false;
      }
    }

    // Fullscreen toggle functionality for both buttons (nav and menu)
    const fullscreenBtnNav = document.getElementById('fullscreen-btn-nav');
    const fullscreenBtnMenu = document.getElementById('fullscreen-btn-menu');

    const toggleFullscreen = () => {
      if (!document.fullscreenElement) {
        document.documentElement.requestFullscreen().catch(err => {
          console.error('Error attempting to enable full-screen mode:', err);
        });
      } else {
        if (document.exitFullscreen) {
          document.exitFullscreen();
        }
      }
    };

    fullscreenBtnNav.addEventListener('click', toggleFullscreen);
    fullscreenBtnMenu.addEventListener('click', toggleFullscreen);
  </script>
</body>
</html>
