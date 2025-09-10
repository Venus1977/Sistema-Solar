<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>README - Solar System Explorer</title>
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
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
            overflow: hidden;
        }

        .header {
            background: linear-gradient(45deg, #4ecdc4, #45b7d1);
            color: white;
            padding: 40px;
            text-align: center;
        }

        .header h1 {
            font-size: 3em;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }

        .header p {
            font-size: 1.3em;
            opacity: 0.9;
        }

        .content {
            padding: 40px;
        }

        .section {
            margin-bottom: 40px;
        }

        .section h2 {
            color: #4ecdc4;
            font-size: 2em;
            margin-bottom: 20px;
            border-bottom: 3px solid #4ecdc4;
            padding-bottom: 10px;
        }

        .section h3 {
            color: #45b7d1;
            font-size: 1.5em;
            margin: 25px 0 15px 0;
        }

        .feature-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 20px 0;
        }

        .feature-card {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            padding: 25px;
            border-radius: 15px;
            border-left: 5px solid #4ecdc4;
            transition: transform 0.3s ease;
        }

        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }

        .feature-icon {
            font-size: 2.5em;
            margin-bottom: 15px;
            display: block;
        }

        .feature-title {
            font-size: 1.3em;
            font-weight: bold;
            color: #333;
            margin-bottom: 10px;
        }

        .feature-description {
            color: #666;
        }

        .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            margin: 20px 0;
        }

        .tech-badge {
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
            color: white;
            padding: 8px 16px;
            border-radius: 20px;
            font-weight: bold;
            font-size: 0.9em;
        }

        .code-block {
            background: #2d3748;
            color: #e2e8f0;
            padding: 20px;
            border-radius: 10px;
            font-family: 'Courier New', monospace;
            margin: 15px 0;
            overflow-x: auto;
        }

        .installation-steps {
            background: #f8f9fa;
            border-radius: 15px;
            padding: 25px;
            margin: 20px 0;
        }

        .step {
            display: flex;
            align-items: flex-start;
            margin-bottom: 20px;
            padding: 15px;
            background: white;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
        }

        .step-number {
            background: #4ecdc4;
            color: white;
            width: 30px;
            height: 30px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            margin-right: 15px;
            flex-shrink: 0;
        }

        .step-content {
            flex: 1;
        }

        .step-title {
            font-weight: bold;
            margin-bottom: 5px;
            color: #333;
        }

        .controls-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 15px;
            margin: 20px 0;
        }

        .control-item {
            background: #f8f9fa;
            padding: 15px;
            border-radius: 10px;
            border-left: 4px solid #4ecdc4;
        }

        .control-key {
            background: #333;
            color: white;
            padding: 4px 8px;
            border-radius: 5px;
            font-family: monospace;
            font-weight: bold;
        }

        .mission-list {
            list-style: none;
            margin: 20px 0;
        }

        .mission-item {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 20px;
            margin-bottom: 15px;
            border-radius: 15px;
            display: flex;
            align-items: center;
        }

        .mission-icon {
            font-size: 2em;
            margin-right: 20px;
        }

        .mission-details h4 {
            font-size: 1.2em;
            margin-bottom: 5px;
        }

        .mission-details p {
            opacity: 0.9;
        }

        .footer {
            background: #2d3748;
            color: white;
            padding: 30px;
            text-align: center;
        }

        .footer a {
            color: #4ecdc4;
            text-decoration: none;
        }

        .footer a:hover {
            text-decoration: underline;
        }

        @media (max-width: 768px) {
            .header h1 {
                font-size: 2em;
            }
            
            .content {
                padding: 20px;
            }
            
            .feature-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="readme-container">
        <div class="header">
            <h1>🪐 Solar System Explorer</h1>
            <p>An Interactive Educational Space Game</p>
        </div>

        <div class="content">
            <!-- Overview Section -->
            <div class="section">
                <h2>🌟 Overview</h2>
                <p>Solar System Explorer is an engaging, educational web-based game designed to teach users about our solar system through interactive exploration, missions, and quizzes. Built with modern web technologies, it provides an immersive learning experience suitable for students, educators, and space enthusiasts of all ages.</p>
            </div>

            <!-- Features Section -->
            <div class="section">
                <h2>✨ Features</h2>
                <div class="feature-grid">
                    <div class="feature-card">
                        <span class="feature-icon">🪐</span>
                        <div class="feature-title">Interactive Planet Explorer</div>
                        <div class="feature-description">Click on planets to discover detailed information, facts, and characteristics of each celestial body in our solar system.</div>
                    </div>
                    
                    <div class="feature-card">
                        <span class="feature-icon">🚀</span>
                        <div class="feature-title">Space Missions</div>
                        <div class="feature-description">Complete 5 unique missions including Apollo moon landing, Mars exploration, Voyager navigation, Jupiter orbit, and Saturn rings traversal.</div>
                    </div>
                    
                    <div class="feature-card">
                        <span class="feature-icon">📏</span>
                        <div class="feature-title">Scientific Tools</div>
                        <div class="feature-description">Use distance calculators, planet comparisons, and weight calculators to understand space science concepts.</div>
                    </div>
                    
                    <div class="feature-card">
                        <span class="feature-icon">🧠</span>
                        <div class="feature-title">Educational Quiz</div>
                        <div class="feature-description">Test your knowledge with 10 comprehensive questions about the solar system with detailed explanations.</div>
                    </div>
                    
                    <div class="feature-card">
                        <span class="feature-icon">🏆</span>
                        <div class="feature-title">Achievement System</div>
                        <div class="feature-description">Unlock 8 different achievements by completing missions, answering quiz questions, and exploring planets.</div>
                    </div>
                    
                    <div class="feature-card">
                        <span class="feature-icon">📱</span>
                        <div class="feature-title">Responsive Design</div>
                        <div class="feature-description">Fully responsive interface that works seamlessly on desktop, tablet, and mobile devices.</div>
                    </div>
                </div>
            </div>

            <!-- Technology Stack -->
            <div class="section">
                <h2>🛠️ Technology Stack</h2>
                <div class="tech-stack">
                    <span class="tech-badge">HTML5</span>
                    <span class="tech-badge">CSS3</span>
                    <span class="tech-badge">JavaScript (ES6+)</span>
                    <span class="tech-badge">Tailwind CSS</span>
                    <span class="tech-badge">CSS Grid & Flexbox</span>
                    <span class="tech-badge">CSS Animations</span>
                    <span class="tech-badge">Responsive Design</span>
                </div>
            </div>

            <!-- Installation -->
            <div class="section">
                <h2>🚀 Getting Started</h2>
                <div class="installation-steps">
                    <div class="step">
                        <div class="step-number">1</div>
                        <div class="step-content">
                            <div class="step-title">Download the File</div>
                            <div>Save the HTML file to your computer as <code>solar-system-explorer.html</code></div>
                        </div>
                    </div>
                    
                    <div class="step">
                        <div class="step-number">2</div>
                        <div class="step-content">
                            <div class="step-title">Open in Browser</div>
                            <div>Double-click the file or right-click and select "Open with" your preferred web browser</div>
                        </div>
                    </div>
                    
                    <div class="step">
                        <div class="step-number">3</div>
                        <div class="step-content">
                            <div class="step-title">Start Exploring</div>
                            <div>Begin your space adventure by clicking on planets or starting your first mission!</div>
                        </div>
                    </div>
                </div>

                <h3>📋 System Requirements</h3>
                <ul>
                    <li>Modern web browser (Chrome 70+, Firefox 65+, Safari 12+, Edge 79+)</li>
                    <li>JavaScript enabled</li>
                    <li>Screen resolution: 1024x768 or higher (recommended)</li>
                    <li>Internet connection not required (fully offline capable)</li>
                </ul>
            </div>

            <!-- How to Play -->
            <div class="section">
                <h2>🎮 How to Play</h2>
                
                <h3>🪐 Planet Exploration</h3>
                <p>Click on any planet or the Sun to learn fascinating facts about celestial bodies. Each planet provides unique information about temperature, size, composition, and interesting characteristics.</p>
                
                <h3>🚀 Space Missions</h3>
                <ul class="mission-list">
                    <li class="mission-item">
                        <span class="mission-icon">🌙</span>
                        <div class="mission-details">
                            <h4>Apollo Mission</h4>
                            <p>Navigate your spacecraft to the lunar landing zone and successfully land on the Moon's surface.</p>
                        </div>
                    </li>
                    
                    <li class="mission-item">
                        <span class="mission-icon">🔴</span>
                        <div class="mission-details">
                            <h4>Mars Exploration</h4>
                            <p>Collect 3 soil samples from the Martian surface by navigating close to sample locations and clicking to collect.</p>
                        </div>
                    </li>
                    
                    <li class="mission-item">
                        <span class="mission-icon">🛰️</span>
                        <div class="mission-details">
                            <h4>Voyager Journey</h4>
                            <p>Follow the historic Voyager route by navigating through 5 sequential waypoints in the outer solar system.</p>
                        </div>
                    </li>
                    
                    <li class="mission-item">
                        <span class="mission-icon">🪐</span>
                        <div class="mission-details">
                            <h4>Jupiter Orbit</h4>
                            <p>Complete 3 full orbital rotations around Jupiter by following the orbital path indicated by the dashed circle.</p>
                        </div>
                    </li>
                    
                    <li class="mission-item">
                        <span class="mission-icon">💍</span>
                        <div class="mission-details">
                            <h4>Saturn's Rings</h4>
                            <p>Navigate through Saturn's ring system by crossing through the rings 4 times to study their composition.</p>
                        </div>
                    </li>
                </ul>

                <h3>🎯 Controls</h3>
                <div class="controls-grid">
                    <div class="control-item">
                        <strong>Movement:</strong> <span class="control-key">↑↓←→</span> or <span class="control-key">WASD</span>
                    </div>
                    <div class="control-item">
                        <strong>Complete Mission:</strong> <span class="control-key">SPACE</span> or Complete Button
                    </div>
                    <div class="control-item">
                        <strong>Planet Info:</strong> Click on planets
                    </div>
                    <div class="control-item">
                        <strong>Navigation:</strong> Tab buttons at top
                    </div>
                </div>
            </div>

            <!-- Educational Content -->
            <div class="section">
                <h2>📚 Educational Content</h2>
                
                <h3>🌍 Planet Information</h3>
                <p>Each planet provides comprehensive information including:</p>
                <ul>
                    <li>Surface temperature ranges</li>
                    <li>Diameter and size comparisons</li>
                    <li>Unique characteristics and phenomena</li>
                    <li>Orbital properties and rotation periods</li>
                    <li>Atmospheric composition</li>
                    <li>Notable features and discoveries</li>
                </ul>

                <h3>🔬 Scientific Tools</h3>
                <ul>
                    <li><strong>Distance Calculator:</strong> Measure distances between planets</li>
                    <li><strong>Planet Comparator:</strong> Compare sizes and masses of different planets</li>
                    <li><strong>Weight Calculator:</strong> Calculate your weight on different celestial bodies</li>
                </ul>

                <h3>🧠 Quiz System</h3>
                <p>The quiz features 10 carefully crafted questions covering:</p>
                <ul>
                    <li>Planet identification and characteristics</li>
                    <li>Solar system structure and composition</li>
                    <li>Astronomical phenomena and discoveries</li>
                    <li>Comparative planetology</li>
                </ul>
            </div>

            <!-- Achievement System -->
            <div class="section">
                <h2>🏆 Achievement System</h2>
                <p>Unlock achievements by completing various activities:</p>
                <ul>
                    <li>🚀 <strong>First Flight:</strong> Complete your first mission</li>
                    <li>🌙 <strong>Lunar Explorer:</strong> Successfully complete the Apollo mission</li>
                    <li>🔴 <strong>Martian Pioneer:</strong> Complete Mars exploration mission</li>
                    <li>🧠 <strong>Space Genius:</strong> Answer 5 quiz questions correctly</li>
                    <li>🎓 <strong>Space Professor:</strong> Achieve perfect quiz score</li>
                    <li>🛰️ <strong>Space Commander:</strong> Complete all 5 missions</li>
                    <li>🔬 <strong>Space Scientist:</strong> Use all 3 scientific tools</li>
                    <li>🌟 <strong>Solar System Master:</strong> Explore all planets and the Sun</li>
                </ul>
            </div>

            <!-- Browser Compatibility -->
            <div class="section">
                <h2>🌐 Browser Compatibility</h2>
                <p>Solar System Explorer is compatible with all modern web browsers:</p>
                <ul>
                    <li>✅ Google Chrome 70+</li>
                    <li>✅ Mozilla Firefox 65+</li>
                    <li>✅ Safari 12+</li>
                    <li>✅ Microsoft Edge 79+</li>
                    <li>✅ Opera 57+</li>
                </ul>
                
                <h3>📱 Mobile Support</h3>
                <p>Fully responsive design optimized for:</p>
                <ul>
                    <li>📱 Smartphones (iOS Safari, Android Chrome)</li>
                    <li>📟 Tablets (iPad, Android tablets)</li>
                    <li>💻 Desktop computers</li>
                    <li>🖥️ Large displays and projectors</li>
                </ul>
            </div>

            <!-- Customization -->
            <div class="section">
                <h2>🎨 Customization</h2>
                <p>The game is built with modular CSS and JavaScript, making it easy to customize:</p>
                
                <h3>🎨 Visual Customization</h3>
                <ul>
                    <li>Modify color schemes by updating CSS custom properties</li>
                    <li>Adjust planet sizes and positions</li>
                    <li>Change animation speeds and effects</li>
                    <li>Update fonts and typography</li>
                </ul>

                <h3>📝 Content Customization</h3>
                <ul>
                    <li>Add new planets or celestial bodies</li>
                    <li>Create additional missions</li>
                    <li>Expand quiz questions</li>
                    <li>Add new achievements</li>
                </ul>

                <h3>🔧 Code Structure</h3>
                <div class="code-block">
// Main game state object
let gameState = {
    completedMissions: [],
    currentMission: null,
    quizScore: 0,
    planetsVisited: [],
    achievements: {}
};

// Planet data structure
const planetData = {
    earth: {
        name: "🌍 Earth",
        description: "Our home planet...",
        facts: [...]
    }
};
                </div>
            </div>

            <!-- Performance -->
            <div class="section">
                <h2>⚡ Performance</h2>
                <ul>
                    <li>🚀 <strong>Fast Loading:</strong> Single HTML file with inline CSS and JavaScript</li>
                    <li>💾 <strong>Lightweight:</strong> No external dependencies or frameworks</li>
                    <li>🔄 <strong>Smooth Animations:</strong> Hardware-accelerated CSS animations</li>
                    <li>📱 <strong>Mobile Optimized:</strong> Touch-friendly interface and responsive design</li>
                    <li>🌐 <strong>Offline Ready:</strong> Works without internet connection</li>
                </ul>
            </div>

            <!-- Educational Use -->
            <div class="section">
                <h2>🎓 Educational Use</h2>
                
                <h3>👨‍🏫 For Educators</h3>
                <ul>
                    <li>Perfect for astronomy and science classes</li>
                    <li>Interactive learning tool for students aged 8-18</li>
                    <li>Can be used on classroom computers or interactive whiteboards</li>
                    <li>No installation required - just open and play</li>
                    <li>Encourages exploration and discovery learning</li>
                </ul>

                <h3>👨‍🎓 For Students</h3>
                <ul>
                    <li>Learn through interactive gameplay</li>
                    <li>Visual and kinesthetic learning support</li>
                    <li>Self-paced exploration and learning</li>
                    <li>Achievement system provides motivation</li>
                    <li>Reinforces learning through quizzes and missions</li>
                </ul>

                <h3>🏠 For Home Use</h3>
                <ul>
                    <li>Family-friendly educational entertainment</li>
                    <li>Spark interest in astronomy and space science</li>
                    <li>Screen time that's both fun and educational</li>
                    <li>No ads or external content</li>
                </ul>
            </div>

            <!-- Troubleshooting -->
            <div class="section">
                <h2>🔧 Troubleshooting</h2>
                
                <h3>Common Issues</h3>
                <div class="installation-steps">
                    <div class="step">
                        <div class="step-number">?</div>
                        <div class="step-content">
                            <div class="step-title">Game doesn't load</div>
                            <div>Ensure JavaScript is enabled in your browser settings and try refreshing the page.</div>
                        </div>
                    </div>
                    
                    <div class="step">
                        <div class="step-number">?</div>
                        <div class="step-content">
                            <div class="step-title">Controls not working</div>
                            <div>Click inside the game area first, then try using keyboard controls or clicking the control buttons.</div>
                        </div>
                    </div>
                    
                    <div class="step">
                        <div class="step-number">?</div>
                        <div class="step-content">
                            <div class="step-title">Layout issues on mobile</div>
                            <div>Try rotating your device to landscape mode for the best experience on smaller screens.</div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- License -->
            <div class="section">
                <h2>📄 License & Credits</h2>
                <p>This project is created for educational purposes and is free to use, modify, and distribute for non-commercial educational use.</p>
                
                <h3>🙏 Acknowledgments</h3>
                <ul>
                    <li>NASA for planetary data and imagery inspiration</li>
                    <li>Educational astronomy resources and textbooks</li>
                    <li>Modern web development community for best practices</li>
                    <li>Accessibility guidelines for inclusive design</li>
                </ul>
            </div>
        </div>

        <div class="footer">
            <p>🌟 Made with ❤️ for space education and exploration</p>
            <p>🚀 Ready to explore the cosmos? <a href="#" onclick="alert('Open the solar-system-explorer.html file to start your space adventure!')">Start Your Space Adventure!</a></p>
        </div>
    </div>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'97cf034fb60ccc70',t:'MTc1NzUwODIyNi4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
