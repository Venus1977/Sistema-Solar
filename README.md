<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>🪐 Solar System Explorer - README</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #333;
            line-height: 1.6;
            padding: 20px;
        }

        .readme-container {
            max-width: 1000px;
            margin: 0 auto;
            background: white;
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
        }

        .header {
            text-align: center;
            margin-bottom: 40px;
            padding-bottom: 30px;
            border-bottom: 3px solid #4ecdc4;
        }

        .title {
            font-size: 3em;
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4, #45b7d1);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 10px;
        }

        .subtitle {
            font-size: 1.3em;
            color: #666;
            margin-bottom: 20px;
        }

        .badges {
            display: flex;
            justify-content: center;
            gap: 10px;
            flex-wrap: wrap;
        }

        .badge {
            background: linear-gradient(45deg, #4ecdc4, #2ecc71);
            color: white;
            padding: 8px 16px;
            border-radius: 20px;
            font-size: 0.9em;
            font-weight: bold;
        }

        .section {
            margin-bottom: 40px;
        }

        .section-title {
            font-size: 2em;
            color: #4ecdc4;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .section-content {
            background: #f8f9fa;
            padding: 25px;
            border-radius: 15px;
            border-left: 5px solid #4ecdc4;
        }

        .feature-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .feature-card {
            background: white;
            padding: 20px;
            border-radius: 10px;
            border: 2px solid #e9ecef;
            transition: all 0.3s ease;
        }

        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
            border-color: #4ecdc4;
        }

        .feature-icon {
            font-size: 2.5em;
            text-align: center;
            margin-bottom: 15px;
        }

        .feature-title {
            font-size: 1.2em;
            font-weight: bold;
            color: #333;
            margin-bottom: 10px;
            text-align: center;
        }

        .feature-description {
            color: #666;
            text-align: center;
        }

        .code-block {
            background: #2d3748;
            color: #e2e8f0;
            padding: 20px;
            border-radius: 10px;
            font-family: 'Courier New', monospace;
            overflow-x: auto;
            margin: 15px 0;
        }

        .installation-steps {
            counter-reset: step-counter;
        }

        .step {
            counter-increment: step-counter;
            background: white;
            padding: 20px;
            margin: 15px 0;
            border-radius: 10px;
            border-left: 5px solid #4ecdc4;
            position: relative;
        }

        .step::before {
            content: counter(step-counter);
            position: absolute;
            left: -15px;
            top: 20px;
            background: #4ecdc4;
            color: white;
            width: 30px;
            height: 30px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
        }

        .step-title {
            font-weight: bold;
            color: #333;
            margin-bottom: 10px;
        }

        .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            margin-top: 20px;
        }

        .tech-item {
            background: linear-gradient(45deg, #667eea, #764ba2);
            color: white;
            padding: 10px 20px;
            border-radius: 25px;
            font-weight: bold;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .screenshot-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .screenshot {
            background: linear-gradient(135deg, #667eea, #764ba2);
            height: 150px;
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 3em;
            transition: transform 0.3s ease;
        }

        .screenshot:hover {
            transform: scale(1.05);
        }

        .contact-info {
            background: linear-gradient(135deg, #4ecdc4, #2ecc71);
            color: white;
            padding: 30px;
            border-radius: 15px;
            text-align: center;
        }

        .contact-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
            flex-wrap: wrap;
        }

        .contact-link {
            background: rgba(255, 255, 255, 0.2);
            color: white;
            padding: 10px 20px;
            border-radius: 25px;
            text-decoration: none;
            transition: all 0.3s ease;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .contact-link:hover {
            background: rgba(255, 255, 255, 0.3);
            transform: translateY(-2px);
        }

        .toc {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 10px;
            margin-bottom: 30px;
        }

        .toc-title {
            font-size: 1.3em;
            font-weight: bold;
            margin-bottom: 15px;
            color: #333;
        }

        .toc-list {
            list-style: none;
            padding: 0;
        }

        .toc-item {
            margin: 8px 0;
        }

        .toc-link {
            color: #4ecdc4;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s ease;
        }

        .toc-link:hover {
            color: #2ecc71;
        }

        @media (max-width: 768px) {
            .readme-container {
                padding: 20px;
            }

            .title {
                font-size: 2em;
            }

            .section-title {
                font-size: 1.5em;
            }

            .badges {
                flex-direction: column;
                align-items: center;
            }

            .tech-stack {
                justify-content: center;
            }

            .contact-links {
                flex-direction: column;
                align-items: center;
            }
        }
    </style>
</head>
<body>
    <div class="readme-container">
        <!-- Header -->
        <div class="header">
            <div class="title">🪐 Solar System Explorer</div>
            <div class="subtitle">Interactive Educational Space Game</div>
            <div class="badges">
                <span class="badge">🎮 Educational Game</span>
                <span class="badge">🌟 Interactive</span>
                <span class="badge">📱 Responsive</span>
                <span class="badge">🚀 Space Theme</span>
            </div>
        </div>

        <!-- Table of Contents -->
        <div class="toc">
            <div class="toc-title">📋 Table of Contents</div>
            <ul class="toc-list">
                <li class="toc-item"><a href="#overview" class="toc-link">🌟 Overview</a></li>
                <li class="toc-item"><a href="#features" class="toc-link">✨ Features</a></li>
                <li class="toc-item"><a href="#installation" class="toc-link">🚀 Installation</a></li>
                <li class="toc-item"><a href="#usage" class="toc-link">🎮 How to Play</a></li>
                <li class="toc-item"><a href="#technology" class="toc-link">💻 Technology Stack</a></li>
                <li class="toc-item"><a href="#screenshots" class="toc-link">📸 Screenshots</a></li>
                <li class="toc-item"><a href="#contributing" class="toc-link">🤝 Contributing</a></li>
                <li class="toc-item"><a href="#contact" class="toc-link">📞 Contact</a></li>
            </ul>
        </div>

        <!-- Overview -->
        <div class="section" id="overview">
            <div class="section-title">🌟 Overview</div>
            <div class="section-content">
                <p><strong>Solar System Explorer</strong> is an interactive educational web game designed to teach players about our solar system in an engaging and fun way. The game combines beautiful 3D animations, interactive missions, educational quizzes, and scientific tools to create an immersive learning experience.</p>
                
                <p>Perfect for students, educators, and space enthusiasts of all ages, this game makes learning about astronomy exciting and accessible. Players can explore planets, complete space missions, test their knowledge with quizzes, and unlock achievements as they journey through our solar system.</p>
            </div>
        </div>

        <!-- Features -->
        <div class="section" id="features">
            <div class="section-title">✨ Features</div>
            <div class="section-content">
                <div class="feature-grid">
                    <div class="feature-card">
                        <div class="feature-icon">🪐</div>
                        <div class="feature-title">Interactive Solar System</div>
                        <div class="feature-description">3D animated solar system with clickable planets and detailed information</div>
                    </div>
                    
                    <div class="feature-card">
                        <div class="feature-icon">🚀</div>
                        <div class="feature-title">Space Missions</div>
                        <div class="feature-description">5 exciting missions including Apollo, Mars exploration, and Voyager journey</div>
                    </div>
                    
                    <div class="feature-card">
                        <div class="feature-icon">🧠</div>
                        <div class="feature-title">Educational Quiz</div>
                        <div class="feature-description">10 challenging questions about the solar system with detailed explanations</div>
                    </div>
                    
                    <div class="feature-card">
                        <div class="feature-icon">📏</div>
                        <div class="feature-title">Scientific Tools</div>
                        <div class="feature-description">Distance calculator, planet comparison tool, and space weight calculator</div>
                    </div>
                    
                    <div class="feature-card">
                        <div class="feature-icon">🏆</div>
                        <div class="feature-title">Achievement System</div>
                        <div class="feature-description">8 unlockable achievements to track progress and encourage exploration</div>
                    </div>
                    
                    <div class="feature-card">
                        <div class="feature-icon">📱</div>
                        <div class="feature-title">Responsive Design</div>
                        <div class="feature-description">Works perfectly on desktop, tablet, and mobile devices</div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Installation -->
        <div class="section" id="installation">
            <div class="section-title">🚀 Installation</div>
            <div class="section-content">
                <p>Getting started with Solar System Explorer is incredibly easy! No installation required - just download and open in your browser.</p>
                
                <div class="installation-steps">
                    <div class="step">
                        <div class="step-title">Download the Game</div>
                        <p>Download the HTML file to your computer or save the code as <code>solar-system-explorer.html</code></p>
                    </div>
                    
                    <div class="step">
                        <div class="step-title">Open in Browser</div>
                        <p>Double-click the HTML file or right-click and select "Open with" your preferred web browser</p>
                    </div>
                    
                    <div class="step">
                        <div class="step-title">Start Exploring!</div>
                        <p>The game will load automatically. No internet connection required after download!</p>
                    </div>
                </div>

                <h4>🌐 Supported Browsers:</h4>
                <ul>
                    <li>✅ Chrome (Recommended)</li>
                    <li>✅ Firefox</li>
                    <li>✅ Safari</li>
                    <li>✅ Edge</li>
                    <li>✅ Opera</li>
                </ul>
            </div>
        </div>

        <!-- Usage -->
        <div class="section" id="usage">
            <div class="section-title">🎮 How to Play</div>
            <div class="section-content">
                <h4>🪐 Exploring Planets:</h4>
                <ul>
                    <li>Click on any planet in the solar system to learn fascinating facts</li>
                    <li>Each planet has detailed information about temperature, size, and unique characteristics</li>
                    <li>Visit all 8 planets to unlock the "Solar System Master" achievement</li>
                </ul>

                <h4>🚀 Completing Missions:</h4>
                <ul>
                    <li>Choose from 5 different space missions</li>
                    <li>Use arrow keys or on-screen controls to navigate your spaceship</li>
                    <li>Reach the target to complete each mission</li>
                    <li>Complete all missions to become a Space Commander</li>
                </ul>

                <h4>🧠 Taking the Quiz:</h4>
                <ul>
                    <li>Answer 10 questions about the solar system</li>
                    <li>Get detailed explanations for each answer</li>
                    <li>Score 5+ correct answers to unlock "Space Genius"</li>
                    <li>Perfect score unlocks "Space Professor" achievement</li>
                </ul>

                <h4>📏 Using Scientific Tools:</h4>
                <ul>
                    <li><strong>Distance Measurer:</strong> Calculate distances between planets</li>
                    <li><strong>Planet Comparator:</strong> Compare sizes and masses of different planets</li>
                    <li><strong>Weight Calculator:</strong> Find out your weight on other planets</li>
                </ul>

                <h4>🏆 Unlocking Achievements:</h4>
                <ul>
                    <li>Complete missions to unlock flight-related achievements</li>
                    <li>Use all tools to become a "Space Scientist"</li>
                    <li>Explore all planets to master the solar system</li>
                    <li>Excel in the quiz to prove your space knowledge</li>
                </ul>
            </div>
        </div>

        <!-- Technology Stack -->
        <div class="section" id="technology">
            <div class="section-title">💻 Technology Stack</div>
            <div class="section-content">
                <p>Solar System Explorer is built using modern web technologies for optimal performance and compatibility:</p>
                
                <div class="tech-stack">
                    <div class="tech-item">
                        <span>🌐</span>
                        HTML5
                    </div>
                    <div class="tech-item">
                        <span>🎨</span>
                        CSS3
                    </div>
                    <div class="tech-item">
                        <span>⚡</span>
                        JavaScript ES6+
                    </div>
                    <div class="tech-item">
                        <span>🎭</span>
                        CSS Animations
                    </div>
                    <div class="tech-item">
                        <span>📱</span>
                        Responsive Design
                    </div>
                    <div class="tech-item">
                        <span>🎮</span>
                        Interactive Elements
                    </div>
                </div>

                <h4>🔧 Key Technical Features:</h4>
                <ul>
                    <li><strong>Self-contained:</strong> No external dependencies or libraries</li>
                    <li><strong>Responsive:</strong> Adapts to all screen sizes automatically</li>
                    <li><strong>Animated:</strong> Smooth CSS animations and transitions</li>
                    <li><strong>Interactive:</strong> Full keyboard and mouse support</li>
                    <li><strong>Accessible:</strong> Works offline after initial download</li>
                </ul>
            </div>
        </div>

        <!-- Screenshots -->
        <div class="section" id="screenshots">
            <div class="section-title">📸 Screenshots</div>
            <div class="section-content">
                <p>Experience the beautiful and engaging interface of Solar System Explorer:</p>
                
                <div class="screenshot-grid">
                    <div class="screenshot">🪐</div>
                    <div class="screenshot">🚀</div>
                    <div class="screenshot">🧠</div>
                    <div class="screenshot">📏</div>
                    <div class="screenshot">🏆</div>
                    <div class="screenshot">🌟</div>
                </div>
                
                <p style="margin-top: 20px; text-align: center; color: #666;">
                    <em>Interactive solar system, space missions, educational quiz, scientific tools, achievements, and more!</em>
                </p>
            </div>
        </div>

        <!-- Contributing -->
        <div class="section" id="contributing">
            <div class="section-title">🤝 Contributing</div>
            <div class="section-content">
                <p>We welcome contributions to make Solar System Explorer even better! Here's how you can help:</p>
                
                <h4>🌟 Ways to Contribute:</h4>
                <ul>
                    <li><strong>🐛 Bug Reports:</strong> Found a bug? Let us know!</li>
                    <li><strong>💡 Feature Requests:</strong> Have ideas for new features?</li>
                    <li><strong>📚 Educational Content:</strong> Suggest new facts or quiz questions</li>
                    <li><strong>🎨 Design Improvements:</strong> Help make the game even more beautiful</li>
                    <li><strong>🌍 Translations:</strong> Help translate the game to other languages</li>
                </ul>

                <h4>📋 Development Guidelines:</h4>
                <ul>
                    <li>Keep the game self-contained (no external dependencies)</li>
                    <li>Maintain educational value and accuracy</li>
                    <li>Ensure responsive design for all devices</li>
                    <li>Test thoroughly across different browsers</li>
                    <li>Follow the existing code style and structure</li>
                </ul>
            </div>
        </div>

        <!-- Contact -->
        <div class="section" id="contact">
            <div class="section-title">📞 Contact</div>
            <div class="contact-info">
                <h3>🚀 Get in Touch!</h3>
                <p>Have questions, suggestions, or just want to share your space exploration experience? We'd love to hear from you!</p>
                
                <div class="contact-links">
                    <a href="mailto:space@explorer.com" class="contact-link">
                        <span>📧</span>
                        Email Us
                    </a>
                    <a href="#" class="contact-link">
                        <span>🐙</span>
                        GitHub
                    </a>
                    <a href="#" class="contact-link">
                        <span>🐦</span>
                        Twitter
                    </a>
                    <a href="#" class="contact-link">
                        <span>💬</span>
                        Discord
                    </a>
                </div>
            </div>
        </div>

        <!-- Footer -->
        <div style="text-align: center; margin-top: 40px; padding-top: 30px; border-top: 2px solid #e9ecef; color: #666;">
            <p>🌟 Made with ❤️ for space enthusiasts everywhere</p>
            <p style="margin-top: 10px;">© 2024 Solar System Explorer - Educational Gaming Project</p>
        </div>
    </div>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'97cec33e44512186',t:'MTc1NzUwNTYwMi4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
