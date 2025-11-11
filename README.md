# InfinitePurpose_PassionRecipe-<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>From Passion to Purpose: Finding Your Infinite Purpose</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            padding: 20px;
        }
        
        .container {
            max-width: 900px;
            margin: 0 auto;
            background: white;
            border-radius: 20px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.3);
            overflow: hidden;
        }
        
        header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 40px;
            text-align: center;
        }
        
        h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }
        
        .subtitle {
            font-size: 1.2em;
            opacity: 0.95;
        }
        
        .content {
            padding: 40px;
        }
        
        .page {
            display: none;
            animation: fadeIn 0.5s;
        }
        
        .page.active {
            display: block;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        h2 {
            color: #667eea;
            margin-bottom: 20px;
            font-size: 1.8em;
            border-bottom: 3px solid #667eea;
            padding-bottom: 10px;
        }
        
        h3 {
            color: #764ba2;
            margin-top: 25px;
            margin-bottom: 15px;
            font-size: 1.3em;
        }
        
        .flow-diagram {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            border-radius: 15px;
            padding: 30px 20px;
            margin: 20px 0;
            text-align: center;
            overflow-x: auto;
        }
        
        .flow-line {
            display: flex;
            align-items: center;
            justify-content: center;
            flex-wrap: wrap;
            gap: 10px;
            margin: 10px 0;
        }
        
        .flow-step {
            display: inline-block;
            background: white;
            padding: 8px 16px;
            border-radius: 20px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            font-weight: 600;
            font-size: 0.95em;
            white-space: nowrap;
        }
        
        .flow-step.primary {
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
        }
        
        .flow-step.secondary {
            background: #667eea;
            color: white;
        }
        
        .flow-step.tertiary {
            background: #764ba2;
            color: white;
        }
        
        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.05); }
        }
        
        .flow-step:nth-child(odd) {
            animation: pulse 3s infinite;
            animation-delay: 0s;
        }
        
        .flow-step:nth-child(even) {
            animation: pulse 3s infinite;
            animation-delay: 1.5s;
        }
        
        .arrow {
            color: #764ba2;
            font-size: 1.2em;
            font-weight: bold;
        }
        
        .problem-method {
            background: #f9f9ff;
            border-left: 5px solid #667eea;
            padding: 20px;
            margin: 20px 0;
            border-radius: 5px;
        }
        
        .problem-method li {
            margin: 10px 0;
            margin-left: 20px;
        }
        
        .fuel-page {
            background: #f9f9ff;
            border-radius: 15px;
            padding: 30px;
            margin: 20px 0;
        }
        
        .positive-fuel {
            border-top: 5px solid #4ade80;
        }
        
        .negative-fuel {
            border-top: 5px solid #f87171;
        }
        
        .fuel-title {
            font-size: 1.5em;
            font-weight: bold;
            margin-bottom: 20px;
            text-align: center;
        }
        
        .positive-fuel .fuel-title {
            color: #16a34a;
        }
        
        .negative-fuel .fuel-title {
            color: #dc2626;
        }
        
        .bridge-section {
            background: linear-gradient(135deg, #fef3c7, #fbbf24);
            border-radius: 15px;
            padding: 30px;
            margin: 20px 0;
        }
        
        .connection-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            margin: 20px 0;
        }
        
        .connection-box {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }
        
        input[type="text"], textarea {
            width: 100%;
            padding: 10px;
            margin: 5px 0;
            border: 2px solid #e0e0e0;
            border-radius: 8px;
            font-size: 1em;
            transition: all 0.3s;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        input[type="text"]:focus, textarea:focus {
            outline: none;
            border-color: #667eea;
            box-shadow: 0 0 0 3px rgba(102, 126, 234, 0.1);
        }
        
        textarea {
            resize: vertical;
            min-height: 80px;
            overflow-y: hidden;
            line-height: 1.5;
        }
        
        /* For PDF export - ensure all content is visible */
        .pdf-ready textarea {
            height: auto !important;
            overflow-y: visible !important;
        }
        
        .mtp-builder {
            background: linear-gradient(135deg, #ffecd2 0%, #fcb69f 100%);
            border-radius: 15px;
            padding: 30px;
            margin-top: 20px;
        }
        
        .mtp-template {
            background: white;
            padding: 25px;
            border-radius: 10px;
            margin-top: 20px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .mtp-result {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 20px;
            border-radius: 10px;
            margin-top: 20px;
            font-size: 1.2em;
            font-weight: 600;
            text-align: center;
            min-height: 80px;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }
        
        .navigation {
            display: flex;
            justify-content: space-between;
            margin-top: 30px;
            padding-top: 20px;
            border-top: 2px solid #e0e0e0;
        }
        
        button {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            border: none;
            padding: 12px 30px;
            border-radius: 25px;
            font-size: 1.1em;
            font-weight: 600;
            cursor: pointer;
            margin: 5px;
            transition: all 0.3s;
            box-shadow: 0 4px 15px rgba(0,0,0,0.2);
        }
        
        button:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(0,0,0,0.3);
        }
        
        button:disabled {
            opacity: 0.5;
            cursor: not-allowed;
        }
        
        .page-indicator {
            text-align: center;
            margin-top: 20px;
            color: #667eea;
            font-weight: 600;
        }
        
        .info-box {
            background: #e0f2fe;
            border-left: 4px solid #0284c7;
            padding: 15px;
            margin: 20px 0;
            border-radius: 5px;
        }
        
        .example {
            background: #fef3c7;
            border-left: 4px solid #f59e0b;
            padding: 15px;
            margin: 15px 0;
            border-radius: 5px;
            font-style: italic;
        }
        
        .save-section {
            text-align: center;
            margin-top: 30px;
            padding: 20px;
            background: #f9f9ff;
            border-radius: 15px;
        }
        
        @media print {
            body {
                background: white;
                padding: 0;
            }
            
            .container {
                box-shadow: none;
                max-width: 100%;
            }
            
            button, .navigation {
                display: none !important;
            }
            
            .page {
                display: block !important;
                page-break-after: always;
                animation: none !important;
            }
            
            .page-indicator {
                display: none;
            }
            
            textarea, input[type="text"] {
                border: 1px solid #666 !important;
                height: auto !important;
                overflow: visible !important;
                page-break-inside: avoid;
            }
            
            .flow-step {
                animation: none !important;
            }
            
            /* Ensure text areas expand to show all content */
            .pdf-ready textarea {
                height: auto !important;
                min-height: fit-content !important;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>🚀 From Passion to Purpose</h1>
            <p class="subtitle">Discovering Your Infinite Purpose Through Connected Interests and Real Problems</p>
        </header>
        
        <div class="content">
            <!-- Page 1: Introduction and Flow -->
            <div class="page active" id="page1">
                <h2>The Neurobiological Architecture of Passion</h2>
                
                <p>Now that we've explored moonshots and Massive Transformative Purpose (MTP), let's dive deeper into connecting your passion to real-world problems. Your <strong>Infinite Purpose</strong> emerges when you use your passion to solve problems that matter to others.</p>
                
                <h3>How Passion Works in Your Brain</h3>
                
                <p>Passion isn't just a feeling—it's a neurobiological process that creates a powerful, self-reinforcing feedback loop:</p>
                
                <div class="flow-diagram">
                    <div class="flow-line">
                        <span class="flow-step primary">Intersecting Interests</span>
                        <span class="arrow">→</span>
                        <span class="flow-step secondary">Pattern Recognition</span>
                        <span class="arrow">→</span>
                        <span class="flow-step tertiary">Dopamine</span>
                        <span class="arrow">→</span>
                        <span class="flow-step primary">Focus</span>
                        <span class="arrow">→</span>
                        <span class="flow-step secondary">Flow</span>
                        <span class="arrow">→</span>
                        <span class="flow-step tertiary">Dopamine</span>
                    </div>
                    <div class="flow-line">
                        <span class="flow-step tertiary">Dopamine</span>
                        <span class="arrow">→</span>
                        <span class="flow-step primary">Pattern Recognition</span>
                        <span class="arrow">→</span>
                        <span class="flow-step secondary">Dopamine</span>
                        <span class="arrow">→</span>
                        <span class="flow-step tertiary">Focus</span>
                        <span class="arrow">→</span>
                        <span class="flow-step primary">Flow</span>
                        <span class="arrow">→</span>
                        <span class="flow-step secondary">Dopamine</span>
                    </div>
                    <div class="flow-line">
                        <span class="flow-step secondary">Dopamine</span>
                        <span class="arrow">→</span>
                        <span class="flow-step tertiary">Pattern Recognition</span>
                        <span class="arrow">→</span>
                        <span class="flow-step primary">Intersecting Interests</span>
                        <span class="arrow">→</span>
                        <span class="flow-step secondary">Pattern Recognition</span>
                        <span class="arrow">→</span>
                        <span class="flow-step tertiary">Dopamine</span>
                        <span class="arrow">↻</span>
                    </div>
                </div>
                
                <div class="info-box">
                    <strong>Key Insight:</strong> Your passion is fueled by combinations of interests. As you master different areas, you'll naturally begin to see connections. These connections aren't forced—they emerge through study and exploration. The pattern recognition gives you dopamine, which gives you more focus, which puts you into a flow state, which gives you more dopamine!
                </div>
                
                <div class="example">
                    <strong>Example:</strong> If you're interested in baseball and insects, you might discover that insects could serve as a protein source to enhance athletic performance. Or if you love creativity and AI, you might explore how artificial intelligence can be creative. These unexpected connections are where innovation happens!
                </div>
                
                <h3>Finding Your Problem: The Purpose Method</h3>
                
                <p><strong>Following your passion alone isn't enough.</strong> We need to use it to solve problems in the world. We need a purpose.</p>
                
                <div class="problem-method">
                    <p>To find your infinite purpose, connect your passion to a real problem using this method:</p>
                    <ul>
                        <li><strong>Keep a journal:</strong> Write down 5 things each day that bother or frustrate you. This helps you track potential problems to tackle.</li>
                        <li><strong>Validate with others:</strong> Ask people around you if they also experience these problems. This confirms the problem truly exists.</li>
                        <li><strong>Assess the scale:</strong> Figure out how big the problem is and whether people are hungry for a solution.</li>
                    </ul>
                </div>
                
                <div class="navigation">
                    <button disabled>Previous</button>
                    <button onclick="navigateTo(2)">Next: Positive Fuel →</button>
                </div>
                <div class="page-indicator">Page 1 of 5</div>
            </div>
            
            <!-- Page 2: Positive Fuel -->
            <div class="page" id="page2">
                <h2>✨ Positive Fuel: Your Interests and Passions</h2>
                
                <div class="fuel-page positive-fuel">
                    <div class="fuel-title">Things that fill you with enthusiasm, energy, and wonder</div>
                    
                    <h3>Your Individual Interests</h3>
                    <p>List 10 interests that energize and excite you:</p>
                    
                    <input type="text" placeholder="Interest 1" class="interest-input">
                    <input type="text" placeholder="Interest 2" class="interest-input">
                    <input type="text" placeholder="Interest 3" class="interest-input">
                    <input type="text" placeholder="Interest 4" class="interest-input">
                    <input type="text" placeholder="Interest 5" class="interest-input">
                    <input type="text" placeholder="Interest 6" class="interest-input">
                    <input type="text" placeholder="Interest 7" class="interest-input">
                    <input type="text" placeholder="Interest 8" class="interest-input">
                    <input type="text" placeholder="Interest 9" class="interest-input">
                    <input type="text" placeholder="Interest 10" class="interest-input">
                    
                    <h3 style="margin-top: 30px;">Connecting Interests</h3>
                    <p>Can you see connections between your interests? If yes, describe them. If not yet, that's okay—they'll emerge with time and mastery!</p>
                    
                    <textarea placeholder="Connection 1: How do two or more of your interests intersect?" class="connection-input"></textarea>
                    <textarea placeholder="Connection 2" class="connection-input"></textarea>
                    <textarea placeholder="Connection 3" class="connection-input"></textarea>
                    <textarea placeholder="Connection 4" class="connection-input"></textarea>
                    <textarea placeholder="Connection 5" class="connection-input"></textarea>
                </div>
                
                <div class="navigation">
                    <button onclick="navigateTo(1)">← Previous</button>
                    <button onclick="navigateTo(3)">Next: Negative Fuel →</button>
                </div>
                <div class="page-indicator">Page 2 of 5</div>
            </div>
            
            <!-- Page 3: Negative Fuel -->
            <div class="page" id="page3">
                <h2>🔥 Negative Fuel: Problems That Energize You</h2>
                
                <div class="fuel-page negative-fuel">
                    <div class="fuel-title">Problems that frustrate you and energize you to create change</div>
                    
                    <p>List problems from your journaling that genuinely agitate you—not generic issues, but situations that you personally find disheartening and want to solve:</p>
                    
                    <input type="text" placeholder="Problem 1: A specific issue that bothers you" class="problem-input">
                    <input type="text" placeholder="Problem 2" class="problem-input">
                    <input type="text" placeholder="Problem 3" class="problem-input">
                    <input type="text" placeholder="Problem 4" class="problem-input">
                    <input type="text" placeholder="Problem 5" class="problem-input">
                    <input type="text" placeholder="Problem 6" class="problem-input">
                    <input type="text" placeholder="Problem 7" class="problem-input">
                    <input type="text" placeholder="Problem 8" class="problem-input">
                    <input type="text" placeholder="Problem 9" class="problem-input">
                    <input type="text" placeholder="Problem 10" class="problem-input">
                    
                    <div class="info-box" style="margin-top: 20px;">
                        <strong>Remember:</strong> These should be problems that get you energized to act, not just abstract issues. They should be situations in the world that you find personally disagreeable and that you'd genuinely like to see solved.
                    </div>
                </div>
                
                <div class="navigation">
                    <button onclick="navigateTo(2)">← Previous</button>
                    <button onclick="navigateTo(4)">Next: Connect Passion to Problem →</button>
                </div>
                <div class="page-indicator">Page 3 of 5</div>
            </div>
            
            <!-- Page 4: Bridging -->
            <div class="page" id="page4">
                <h2>🌉 Connecting Your Passion to a Problem</h2>
                
                <div class="bridge-section">
                    <h3 style="text-align: center; color: #764ba2;">Now comes the crucial step: Bridge your positive and negative fuel!</h3>
                    
                    <p style="text-align: center; font-size: 1.1em; margin: 20px 0;">Look at your interests and passions (positive fuel) and your problems (negative fuel). Which passions do you think you could use to deal with one of the problems you raised?</p>
                    
                    <div class="connection-grid">
                        <div class="connection-box">
                            <h4>Selected Passion(s):</h4>
                            <textarea id="bridge-passion" placeholder="Which interest(s) or connecting interests from Page 2 could you use?" style="min-height: 120px;"></textarea>
                        </div>
                        
                        <div class="connection-box">
                            <h4>Target Problem:</h4>
                            <textarea id="bridge-problem" placeholder="Which problem from Page 3 do you want to solve?" style="min-height: 120px;"></textarea>
                        </div>
                    </div>
                    
                    <div style="background: white; padding: 20px; border-radius: 10px; margin-top: 20px;">
                        <h4>How they connect:</h4>
                        <textarea placeholder="Explain how you could use your passion to solve this problem..." style="min-height: 150px;"></textarea>
                    </div>
                    
                    <div class="example">
                        <strong>Example:</strong> "I could use my passion for AI and creativity to solve the problem of students feeling disconnected from learning by creating adaptive educational tools that make learning feel more like creative play."
                    </div>
                </div>
                
                <div class="navigation">
                    <button onclick="navigateTo(3)">← Previous</button>
                    <button onclick="navigateTo(5)">Next: Create Your MTP →</button>
                </div>
                <div class="page-indicator">Page 4 of 5</div>
            </div>
            
            <!-- Page 5: MTP Creation -->
            <div class="page" id="page5">
                <h2>🎯 Crafting Your Infinite Purpose Statement</h2>
                
                <div class="mtp-builder">
                    <h3 style="color: #764ba2; text-align: center;">The MTP Template</h3>
                    
                    <div class="mtp-template">
                        <p style="margin-bottom: 20px; font-size: 1.1em;">Fill in the template below to create your Infinite Purpose statement:</p>
                        
                        <p style="font-size: 1.2em; margin: 20px 0;">
                            <strong>My infinite purpose is to use</strong>
                        </p>
                        
                        <textarea id="passion-field" placeholder="[Insert your passion, primary interest, or connecting interests here]" style="margin: 15px 0; min-height: 100px;"></textarea>
                        
                        <p style="font-size: 1.2em; margin: 20px 0;">
                            <strong>to solve</strong>
                        </p>
                        
                        <textarea id="problem-field" placeholder="[Insert the problem you want to solve here]" style="margin: 15px 0; min-height: 100px;"></textarea>
                        
                        <button onclick="generateMTP()">Generate My Infinite Purpose</button>
                    </div>
                    
                    <div id="mtp-result" class="mtp-result" style="display: none;">
                        <!-- MTP will appear here -->
                    </div>
                </div>
                
                <div class="save-section">
                    <h3>Save Your Work</h3>
                    <p>Save your worksheet locally or download as PDF to submit</p>
                    <button onclick="saveWorksheet()">💾 Save Worksheet Locally</button>
                    <button onclick="downloadAsPDF()">📥 Download as PDF</button>
                </div>
                
                <div class="navigation">
                    <button onclick="navigateTo(4)">← Previous</button>
                    <button onclick="navigateTo(1)">Start Over</button>
                </div>
                <div class="page-indicator">Page 5 of 5</div>
            </div>
        </div>
    </div>
    
    <script>
        let currentPage = 1;
        
        // Auto-expand textareas as user types
        function autoExpand(textarea) {
            textarea.style.height = 'auto';
            textarea.style.height = textarea.scrollHeight + 'px';
        }
        
        // Initialize auto-expand for all textareas
        function initializeAutoExpand() {
            document.querySelectorAll('textarea').forEach(textarea => {
                // Set initial height
                autoExpand(textarea);
                
                // Add event listeners for auto-expansion
                textarea.addEventListener('input', function() {
                    autoExpand(this);
                });
                
                // Also expand on focus to show all content
                textarea.addEventListener('focus', function() {
                    autoExpand(this);
                });
            });
        }
        
        // Navigation function
        function navigateTo(pageNum) {
            // Hide all pages
            document.querySelectorAll('.page').forEach(page => {
                page.classList.remove('active');
            });
            
            // Show selected page
            document.getElementById('page' + pageNum).classList.add('active');
            currentPage = pageNum;
            
            // Scroll to top
            window.scrollTo(0, 0);
            
            // Auto-populate MTP fields if on page 5
            if (pageNum === 5) {
                const bridgePassion = document.getElementById('bridge-passion').value;
                const bridgeProblem = document.getElementById('bridge-problem').value;
                
                if (bridgePassion && !document.getElementById('passion-field').value) {
                    document.getElementById('passion-field').value = bridgePassion;
                }
                if (bridgeProblem && !document.getElementById('problem-field').value) {
                    document.getElementById('problem-field').value = bridgeProblem;
                }
            }
            
            // Re-initialize auto-expand for the new page
            setTimeout(initializeAutoExpand, 100);
        }
        
        // Generate MTP Statement
        function generateMTP() {
            const passion = document.getElementById('passion-field').value;
            const problem = document.getElementById('problem-field').value;
            const resultDiv = document.getElementById('mtp-result');
            
            if (passion.trim() && problem.trim()) {
                resultDiv.innerHTML = `My infinite purpose is to use <strong>${passion}</strong> to solve <strong>${problem}</strong>`;
                resultDiv.style.display = 'flex';
                
                // Animate the result
                resultDiv.style.animation = 'none';
                setTimeout(() => {
                    resultDiv.style.animation = 'pulse 1s ease-in-out';
                }, 10);
            } else {
                alert('Please fill in both your passion and the problem you want to solve!');
            }
        }
        
        // Save worksheet data to localStorage
        function saveWorksheet() {
            const data = {
                interests: [],
                connections: [],
                problems: [],
                bridgePassion: document.getElementById('bridge-passion').value,
                bridgeProblem: document.getElementById('bridge-problem').value,
                passion: document.getElementById('passion-field').value,
                problem: document.getElementById('problem-field').value,
                savedDate: new Date().toISOString()
            };
            
            // Collect interests
            document.querySelectorAll('.interest-input').forEach(input => {
                if (input.value) data.interests.push(input.value);
            });
            
            // Collect connections
            document.querySelectorAll('.connection-input').forEach(input => {
                if (input.value) data.connections.push(input.value);
            });
            
            // Collect problems
            document.querySelectorAll('.problem-input').forEach(input => {
                if (input.value) data.problems.push(input.value);
            });
            
            localStorage.setItem('infinitePurposeWorksheet', JSON.stringify(data));
            alert('Worksheet saved locally! Your responses will be here when you return.');
        }
        
        // Download as PDF function
        function downloadAsPDF() {
            // First, expand all textareas to show full content
            document.querySelectorAll('textarea').forEach(textarea => {
                autoExpand(textarea);
            });
            
            // Make all pages visible for printing
            document.querySelectorAll('.page').forEach(page => {
                page.style.display = 'block';
                page.style.pageBreakAfter = 'always';
            });
            
            // Add PDF-ready class to ensure all content is visible
            document.body.classList.add('pdf-ready');
            
            // Give browser time to render changes, then trigger print
            setTimeout(() => {
                window.print();
                
                // After printing, restore normal view
                setTimeout(() => {
                    document.body.classList.remove('pdf-ready');
                    document.querySelectorAll('.page').forEach(page => {
                        page.style.display = '';
                        page.style.pageBreakAfter = '';
                    });
                    navigateTo(currentPage);
                }, 1000);
            }, 100);
        }
        
        // Load saved data on page load
        window.addEventListener('load', function() {
            const saved = localStorage.getItem('infinitePurposeWorksheet');
            if (saved) {
                const data = JSON.parse(saved);
                
                // Load interests
                const interestInputs = document.querySelectorAll('.interest-input');
                data.interests.forEach((interest, i) => {
                    if (interestInputs[i]) interestInputs[i].value = interest;
                });
                
                // Load connections
                const connectionInputs = document.querySelectorAll('.connection-input');
                data.connections.forEach((connection, i) => {
                    if (connectionInputs[i]) connectionInputs[i].value = connection;
                });
                
                // Load problems
                const problemInputs = document.querySelectorAll('.problem-input');
                data.problems.forEach((problem, i) => {
                    if (problemInputs[i]) problemInputs[i].value = problem;
                });
                
                // Load bridge fields
                if (data.bridgePassion) document.getElementById('bridge-passion').value = data.bridgePassion;
                if (data.bridgeProblem) document.getElementById('bridge-problem').value = data.bridgeProblem;
                
                // Load MTP fields
                if (data.passion) document.getElementById('passion-field').value = data.passion;
                if (data.problem) document.getElementById('problem-field').value = data.problem;
            }
            
            // Initialize auto-expand after loading
            initializeAutoExpand();
        });
        
        // Export data as text (keeping this function even though button is removed, in case needed)
        function exportData() {
            let text = "MY INFINITE PURPOSE WORKSHEET\n";
            text += "Generated: " + new Date().toLocaleString() + "\n\n";
            
            text += "=" + "=".repeat(50) + "\n";
            text += "POSITIVE FUEL - INTERESTS:\n";
            text += "=" + "=".repeat(50) + "\n";
            document.querySelectorAll('.interest-input').forEach((input, i) => {
                if (input.value) text += `${i + 1}. ${input.value}\n`;
            });
            
            text += "\n" + "=".repeat(50) + "\n";
            text += "CONNECTING INTERESTS:\n";
            text += "=" + "=".repeat(50) + "\n";
            document.querySelectorAll('.connection-input').forEach((input, i) => {
                if (input.value) text += `${i + 1}. ${input.value}\n`;
            });
            
            text += "\n" + "=".repeat(50) + "\n";
            text += "NEGATIVE FUEL - PROBLEMS:\n";
            text += "=" + "=".repeat(50) + "\n";
            document.querySelectorAll('.problem-input').forEach((input, i) => {
                if (input.value) text += `${i + 1}. ${input.value}\n`;
            });
            
            text += "\n" + "=".repeat(50) + "\n";
            text += "BRIDGING PASSION TO PROBLEM:\n";
            text += "=" + "=".repeat(50) + "\n";
            const bridgePassion = document.getElementById('bridge-passion').value;
            const bridgeProblem = document.getElementById('bridge-problem').value;
            if (bridgePassion) text += `Selected Passion: ${bridgePassion}\n`;
            if (bridgeProblem) text += `Target Problem: ${bridgeProblem}\n`;
            
            const passion = document.getElementById('passion-field').value;
            const problem = document.getElementById('problem-field').value;
            
            text += "\n" + "=".repeat(50) + "\n";
            text += "MY INFINITE PURPOSE:\n";
            text += "=" + "=".repeat(50) + "\n";
            if (passion && problem) {
                text += `My infinite purpose is to use ${passion} to solve ${problem}\n`;
            } else {
                text += "[Complete the worksheet to generate your infinite purpose]\n";
            }
            
            // Create download
            const blob = new Blob([text], { type: 'text/plain' });
            const url = window.URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.href = url;
            a.download = 'my-infinite-purpose.txt';
            document.body.appendChild(a);
            a.click();
            document.body.removeChild(a);
            window.URL.revokeObjectURL(url);
        }
    </script>
</body>
</html>
