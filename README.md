<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ghufran Arain - AI Student</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
            color: #f0f0f0;
            line-height: 1.6;
            padding: 20px;
            min-height: 100vh;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        header {
            text-align: center;
            padding: 40px 0;
            position: relative;
            overflow: hidden;
        }
        
        .header-content {
            position: relative;
            z-index: 2;
        }
        
        h1 {
            font-size: 3.5rem;
            margin-bottom: 10px;
            background: linear-gradient(45deg, #4facfe, #00f2fe);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: fadeIn 1s ease-out;
        }
        
        h2 {
            font-size: 1.8rem;
            color: #a1c4fd;
            margin-bottom: 20px;
            animation: slideIn 1s ease-out;
        }
        
        h3 {
            font-size: 1.5rem;
            margin: 30px 0 20px;
            color: #4facfe;
            position: relative;
            display: inline-block;
        }
        
        h3:after {
            content: '';
            position: absolute;
            width: 100%;
            height: 3px;
            bottom: -5px;
            left: 0;
            background: linear-gradient(45deg, #4facfe, #00f2fe);
            border-radius: 3px;
        }
        
        p {
            margin-bottom: 15px;
            font-size: 1.1rem;
        }
        
        .stats {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 30px 0;
            flex-wrap: wrap;
        }
        
        .stat-item {
            background: rgba(255, 255, 255, 0.1);
            padding: 15px 25px;
            border-radius: 10px;
            text-align: center;
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: transform 0.3s, box-shadow 0.3s;
            animation: fadeInUp 1s ease-out;
        }
        
        .stat-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
        }
        
        .stat-item span {
            display: block;
            font-size: 2rem;
            font-weight: 700;
            color: #4facfe;
        }
        
        .about {
            background: rgba(255, 255, 255, 0.05);
            padding: 30px;
            border-radius: 15px;
            margin: 30px 0;
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            animation: fadeIn 1.5s ease-out;
        }
        
        .skills {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }
        
        .skill-category {
            background: rgba(255, 255, 255, 0.05);
            padding: 20px;
            border-radius: 15px;
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: transform 0.3s;
            animation: fadeInUp 1s ease-out;
        }
        
        .skill-category:hover {
            transform: translateY(-5px);
        }
        
        .skill-icons {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            margin-top: 15px;
        }
        
        .skill-icon {
            display: flex;
            flex-direction: column;
            align-items: center;
            transition: transform 0.3s;
        }
        
        .skill-icon:hover {
            transform: scale(1.2);
        }
        
        .skill-icon i {
            font-size: 2.5rem;
            margin-bottom: 5px;
            color: #4facfe;
        }
        
        .skill-icon span {
            font-size: 0.8rem;
            color: #a1c4fd;
        }
        
        .contact {
            text-align: center;
            margin: 40px 0;
            animation: fadeIn 2s ease-out;
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }
        
        .social-link {
            display: inline-block;
            width: 50px;
            height: 50px;
            background: linear-gradient(45deg, #4facfe, #00f2fe);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .social-link:hover {
            transform: translateY(-5px) rotate(10deg);
            box-shadow: 0 5px 15px rgba(79, 172, 254, 0.4);
        }
        
        .github-stats {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
            margin: 40px 0;
        }
        
        .stat-card {
            background: rgba(255, 255, 255, 0.05);
            padding: 20px;
            border-radius: 15px;
            min-width: 250px;
            text-align: center;
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            animation: fadeInUp 1.5s ease-out;
        }
        
        .trophy {
            display: flex;
            justify-content: center;
            margin: 30px 0;
            flex-wrap: wrap;
            gap: 10px;
        }
        
        .trophy-item {
            font-size: 2rem;
            color: #FFD700;
            animation: bounce 2s infinite;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        @keyframes fadeInUp {
            from { 
                opacity: 0;
                transform: translateY(20px);
            }
            to { 
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        @keyframes slideIn {
            from { 
                opacity: 0;
                transform: translateX(-30px);
            }
            to { 
                opacity: 1;
                transform: translateX(0);
            }
        }
        
        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }
        
        .floating {
            animation: float 6s ease-in-out infinite;
        }
        
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }
        
        @media (max-width: 768px) {
            h1 {
                font-size: 2.5rem;
            }
            
            h2 {
                font-size: 1.5rem;
            }
            
            .stats {
                flex-direction: column;
                align-items: center;
            }
            
            .github-stats {
                flex-direction: column;
                align-items: center;
            }
        }
        
        .particles {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: 1;
        }
        
        .particle {
            position: absolute;
            background: rgba(79, 172, 254, 0.5);
            border-radius: 50%;
            animation: float 10s infinite ease-in-out;
        }
        
        .typewriter {
            overflow: hidden;
            border-right: 0.15em solid #4facfe;
            white-space: nowrap;
            margin: 0 auto;
            letter-spacing: 0.15em;
            animation: typing 3.5s steps(40, end), blink-caret 0.75s step-end infinite;
        }
        
        @keyframes typing {
            from { width: 0 }
            to { width: 100% }
        }
        
        @keyframes blink-caret {
            from, to { border-color: transparent }
            50% { border-color: #4facfe }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="particles" id="particles"></div>
            <div class="header-content">
                <h1>Hi 👋, I'm Ghufran Arain</h1>
                <h2 class="typewriter">A Student of Artificial Intelligence</h2>
                
                <div class="stats">
                    <div class="stat-item floating">
                        <span>5+</span>
                        Projects Completed
                    </div>
                    <div class="stat-item floating" style="animation-delay: 0.2s;">
                        <span>10+</span>
                        Technologies Mastered
                    </div>
                    <div class="stat-item floating" style="animation-delay: 0.4s;">
                        <span>2+</span>
                        Years of Experience
                    </div>
                </div>
            </div>
        </header>
        
        <section class="about">
            <h3>About Me</h3>
            <p>I'm a passionate Artificial Intelligence student with a strong interest in machine learning and deep learning. I enjoy turning complex problems into simple, beautiful and intuitive solutions.</p>
            
            <p>🌱 <strong>Currently learning:</strong> Advanced AI and Machine Learning algorithms</p>
            <p>💬 <strong>Ask me about:</strong> Machine Learning and Deep Learning</p>
            <p>📫 <strong>How to reach me:</strong> ghufranarain55@gmail.com</p>
        </section>
        
        <section>
            <h3>Languages and Tools</h3>
            <div class="skills">
                <div class="skill-category">
                    <h4>AI & Data Science</h4>
                    <div class="skill-icons">
                        <div class="skill-icon">
                            <i class="fab fa-python"></i>
                            <span>Python</span>
                        </div>
                        <div class="skill-icon">
                            <i class="fas fa-brain"></i>
                            <span>TensorFlow</span>
                        </div>
                        <div class="skill-icon">
                            <i class="fas fa-project-diagram"></i>
                            <span>PyTorch</span>
                        </div>
                        <div class="skill-icon">
                            <i class="fas fa-chart-line"></i>
                            <span>Pandas</span>
                        </div>
                        <div class="skill-icon">
                            <i class="fas fa-chart-bar"></i>
                            <span>Seaborn</span>
                        </div>
                        <div class="skill-icon">
                            <i class="fas fa-cogs"></i>
                            <span>Scikit-learn</span>
                        </div>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h4>Web Development</h4>
                    <div class="skill-icons">
                        <div class="skill-icon">
                            <i class="fab fa-js"></i>
                            <span>JavaScript</span>
                        </div>
                        <div class="skill-icon">
                            <i class="fab fa-react"></i>
                            <span>React</span>
                        </div>
                        <div class="skill-icon">
                            <i class="fab fa-node-js"></i>
                            <span>Node.js</span>
                        </div>
                        <div class="skill-icon">
                            <i class="fab fa-css3-alt"></i>
                            <span>CSS3</span>
                        </div>
                        <div class="skill-icon">
                            <i class="fab fa-django"></i>
                            <span>Django</span>
                        </div>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h4>Databases & Tools</h4>
                    <div class="skill-icons">
                        <div class="skill-icon">
                            <i class="fas fa-database"></i>
                            <span>MySQL</span>
                        </div>
                        <div class="skill-icon">
                            <i class="fas fa-server"></i>
                            <span>MongoDB</span>
                        </div>
                        <div class="skill-icon">
                            <i class="fas fa-database"></i>
                            <span>SQLite</span>
                        </div>
                        <div class="skill-icon">
                            <i class="fab fa-git-alt"></i>
                            <span>Git</span>
                        </div>
                        <div class="skill-icon">
                            <i class="fab fa-linux"></i>
                            <span>Linux</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        
        <section class="contact">
            <h3>Connect with me</h3>
            <div class="social-links">
                <a href="https://linkedin.com/in/ghufran arain" target="_blank" class="social-link">
                    <i class="fab fa-linkedin-in"></i>
                </a>
                <a href="https://github.com/ghufran-arain55" target="_blank" class="social-link">
                    <i class="fab fa-github"></i>
                </a>
                <a href="mailto:ghufranarain55@gmail.com" class="social-link">
                    <i class="fas fa-envelope"></i>
                </a>
            </div>
        </section>
        
        <section>
            <h3>GitHub Stats</h3>
            <div class="github-stats">
                <div class="stat-card">
                    <i class="fas fa-eye"></i>
                    <h4>Profile Views</h4>
                    <p>1,200+</p>
                </div>
                <div class="stat-card">
                    <i class="fas fa-project-diagram"></i>
                    <h4>Public Repositories</h4>
                    <p>15+</p>
                </div>
                <div class="stat-card">
                    <i class="fas fa-code-branch"></i>
                    <h4>Contributions</h4>
                    <p>200+</p>
                </div>
            </div>
            
            <div class="trophy">
                <div class="trophy-item"><i class="fas fa-trophy"></i></div>
                <div class="trophy-item" style="animation-delay: 0.2s;"><i class="fas fa-trophy"></i></div>
                <div class="trophy-item" style="animation-delay: 0.4s;"><i class="fas fa-trophy"></i></div>
                <div class="trophy-item" style="animation-delay: 0.6s;"><i class="fas fa-trophy"></i></div>
                <div class="trophy-item" style="animation-delay: 0.8s;"><i class="fas fa-trophy"></i></div>
            </div>
        </section>
    </div>

    <script>
        // Create floating particles
        document.addEventListener('DOMContentLoaded', function() {
            const particlesContainer = document.getElementById('particles');
            const particleCount = 30;
            
            for (let i = 0; i < particleCount; i++) {
                const particle = document.createElement('div');
                particle.classList.add('particle');
                
                const size = Math.random() * 10 + 2;
                particle.style.width = `${size}px`;
                particle.style.height = `${size}px`;
                
                particle.style.left = `${Math.random() * 100}%`;
                particle.style.top = `${Math.random() * 100}%`;
                
                particle.style.animationDuration = `${Math.random() * 10 + 10}s`;
                particle.style.animationDelay = `${Math.random() * 5}s`;
                particle.style.opacity = Math.random() * 0.5 + 0.1;
                
                particlesContainer.appendChild(particle);
            }
            
            // Typewriter effect
            const typewriter = document.querySelector('.typewriter');
            setTimeout(() => {
                typewriter.style.borderRight = 'none';
            }, 3500);
        });
    </script>
</body>
</html>
