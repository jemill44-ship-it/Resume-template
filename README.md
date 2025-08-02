# Resume-template
Gulf Coast Industrial Resume
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gulf Coast Industrial Resume Template</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.4;
            color: #2c3e50;
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            padding: 20px;
        }
        
        .resume-container {
            max-width: 800px;
            margin: 0 auto;
            background: white;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            border-radius: 8px;
            overflow: hidden;
        }
        
        .header {
            background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
            color: white;
            padding: 30px;
            position: relative;
        }
        
        .header::before {
            content: '';
            position: absolute;
            top: 0;
            right: 0;
            width: 100px;
            height: 100px;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><circle cx="50" cy="50" r="40" fill="none" stroke="rgba(255,255,255,0.1)" stroke-width="2"/><path d="M30 50h40M50 30v40" stroke="rgba(255,255,255,0.2)" stroke-width="3"/></svg>') no-repeat center;
            opacity: 0.3;
        }
        
        .name {
            font-size: 2.5em;
            font-weight: bold;
            margin-bottom: 5px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }
        
        .title {
            font-size: 1.3em;
            margin-bottom: 15px;
            color: #ecf0f1;
            font-weight: 300;
        }
        
        .contact-info {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 15px;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            gap: 8px;
            font-size: 0.95em;
        }
        
        .safety-banner {
            background: linear-gradient(90deg, #27ae60, #2ecc71);
            color: white;
            padding: 15px 30px;
            text-align: center;
            font-weight: bold;
            font-size: 1.1em;
            position: relative;
        }
        
        .safety-banner::before {
            content: '🛡️';
            margin-right: 10px;
            font-size: 1.2em;
        }
        
        .content {
            padding: 30px;
        }
        
        .section {
            margin-bottom: 30px;
        }
        
        .section-title {
            font-size: 1.4em;
            color: #1e3c72;
            border-bottom: 3px solid #3498db;
            padding-bottom: 8px;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .certs-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
            margin-bottom: 20px;
        }
        
        .cert-item {
            background: linear-gradient(135deg, #74b9ff, #0984e3);
            color: white;
            padding: 12px 15px;
            border-radius: 6px;
            text-align: center;
            font-weight: bold;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }
        
        .experience-item {
            border-left: 4px solid #3498db;
            padding-left: 20px;
            margin-bottom: 25px;
            position: relative;
        }
        
        .experience-item::before {
            content: '';
            position: absolute;
            left: -8px;
            top: 0;
            width: 12px;
            height: 12px;
            background: #3498db;
            border-radius: 50%;
        }
        
        .job-title {
            font-size: 1.2em;
            font-weight: bold;
            color: #1e3c72;
        }
        
        .company-info {
            color: #7f8c8d;
            margin: 5px 0 10px 0;
            font-style: italic;
        }
        
        .achievement {
            background: #f8f9fa;
            border-left: 4px solid #27ae60;
            padding: 10px 15px;
            margin: 8px 0;
            border-radius: 0 4px 4px 0;
        }
        
        .achievement::before {
            content: '✓';
            color: #27ae60;
            font-weight: bold;
            margin-right: 10px;
        }
        
        .skills-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }
        
        .skill-category {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 8px;
            border-top: 4px solid #e74c3c;
        }
        
        .skill-category h4 {
            color: #e74c3c;
            margin-bottom: 12px;
            font-size: 1.1em;
        }
        
        .skill-list {
            list-style: none;
        }
        
        .skill-list li {
            padding: 4px 0;
            position: relative;
            padding-left: 20px;
        }
        
        .skill-list li::before {
            content: '⚙️';
            position: absolute;
            left: 0;
            font-size: 0.8em;
        }
        
        .jeremy-tip {
            background: linear-gradient(135deg, #ff7675, #fd79a8);
            color: white;
            padding: 20px;
            border-radius: 8px;
            margin: 20px 0;
            position: relative;
            font-style: italic;
        }
        
        .jeremy-tip::before {
            content: '💡 Jeremy\'s Pro Tip:';
            font-weight: bold;
            display: block;
            margin-bottom: 8px;
            font-style: normal;
        }
        
        .download-btn {
            background: linear-gradient(135deg, #1e3c72, #2a5298);
            color: white;
            padding: 15px 30px;
            border: none;
            border-radius: 25px;
            font-size: 1.1em;
            font-weight: bold;
            cursor: pointer;
            display: block;
            margin: 30px auto;
            box-shadow: 0 4px 15px rgba(30, 60, 114, 0.3);
            transition: all 0.3s ease;
        }
        
        .download-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(30, 60, 114, 0.4);
        }
        
        .fillable {
            background: rgba(255, 255, 255, 0.8);
            border: 2px dashed #3498db;
            padding: 8px 12px;
            border-radius: 4px;
            display: inline-block;
            min-width: 150px;
            margin: 2px;
        }
        
        .placeholder {
            color: #7f8c8d;
            font-style: italic;
        }
        
        @media (max-width: 768px) {
            .contact-info {
                flex-direction: column;
                gap: 10px;
            }
            
            .name {
                font-size: 2em;
            }
            
            .content {
                padding: 20px;
            }
            
            .certs-grid {
                grid-template-columns: 1fr;
            }
        }
        
        @media print {
            body {
                padding: 0;
                background: white;
            }
            
            .resume-container {
                box-shadow: none;
                max-width: none;
            }
            
            .download-btn {
                display: none;
            }
        }
    </style>
</head>
<body>
    <div class="resume-container">
        <!-- Header Section -->
        <div class="header">
            <div class="name"><span class="fillable placeholder">YOUR NAME HERE</span></div>
            <div class="title"><span class="fillable placeholder">Your Industrial Specialty Title</span></div>
            <div class="contact-info">
                <div class="contact-item">📱 <span class="fillable placeholder">(555) 123-4567</span></div>
                <div class="contact-item">📧 <span class="fillable placeholder">your.email@gmail.com</span></div>
                <div class="contact-item">📍 <span class="fillable placeholder">Lake Charles, LA</span></div>
                <div class="contact-item">🔗 <span class="fillable placeholder">LinkedIn Profile</span></div>
            </div>
        </div>

        <!-- Safety Banner -->
        <div class="safety-banner">
            <span class="fillable placeholder">X YEARS • ZERO RECORDABLE INCIDENTS • SAFETY LEADER</span>
        </div>

        <div class="content">
            <!-- Certifications Section -->
            <div class="section">
                <h2 class="section-title">🏆 CERTIFICATIONS & CREDENTIALS</h2>
                <div class="certs-grid">
                    <div class="cert-item">
                        <div><span class="fillable placeholder">OSHA 30</span></div>
                        <small>Exp: <span class="fillable placeholder">MM/YYYY</span></small>
                    </div>
                    <div class="cert-item">
                        <div><span class="fillable placeholder">AMPP Level 1</span></div>
                        <small>Exp: <span class="fillable placeholder">MM/YYYY</span></small>
                    </div>
                    <div class="cert-item">
                        <div><span class="fillable placeholder">AWS D1.1</span></div>
                        <small>Exp: <span class="fillable placeholder">MM/YYYY</span></small>
                    </div>
                    <div class="cert-item">
                        <div><span class="fillable placeholder">Your Certification</span></div>
                        <small>Exp: <span class="fillable placeholder">MM/YYYY</span></small>
                    </div>
                </div>
            </div>

            <!-- Professional Experience -->
            <div class="section">
                <h2 class="section-title">⚡ PROFESSIONAL EXPERIENCE</h2>
                
                <div class="experience-item">
                    <div class="job-title"><span class="fillable placeholder">Lead Painter / Foreman</span></div>
                    <div class="company-info"><span class="fillable placeholder">Company Name</span> • <span class="fillable placeholder">Location</span> • <span class="fillable placeholder">YYYY - Present</span></div>
                    
                    <div class="achievement">
                        Led <span class="fillable placeholder">#</span>-person crew on $<span class="fillable placeholder">X.X</span>M <span class="fillable placeholder">project type</span> projects, maintaining zero incidents over <span class="fillable placeholder">#</span> years
                    </div>
                    <div class="achievement">
                        Applied protective coatings per SSPC standards on <span class="fillable placeholder">facility types</span>, ensuring <span class="fillable placeholder">#</span>-year asset protection
                    </div>
                    <div class="achievement">
                        Reduced project completion time by <span class="fillable placeholder">#</span>% through improved crew coordination and quality control processes
                    </div>
                </div>

                <div class="experience-item">
                    <div class="job-title"><span class="fillable placeholder">Industrial Coating Specialist</span></div>
                    <div class="company-info"><span class="fillable placeholder">Previous Company</span> • <span class="fillable placeholder">Location</span> • <span class="fillable placeholder">YYYY - YYYY</span></div>
                    
                    <div class="achievement">
                        Executed surface preparation and coating applications on <span class="fillable placeholder">equipment types</span> across <span class="fillable placeholder">#</span> major facilities
                    </div>
                    <div class="achievement">
                        Maintained <span class="fillable placeholder">#</span>% quality rating through strict adherence to NACE and SSPC specifications
                    </div>
                </div>
            </div>

            <!-- Jeremy's Pro Tip -->
            <div class="jeremy-tip">
                Make every bullet point show IMPACT with numbers! Hiring managers scan for results, not just duties. "$2M project" beats "painted equipment" every time.
            </div>

            <!-- Technical Skills -->
            <div class="section">
                <h2 class="section-title">🔧 TECHNICAL EXPERTISE</h2>
                <div class="skills-container">
                    <div class="skill-category">
                        <h4>Safety & Compliance</h4>
                        <ul class="skill-list">
                            <li>OSHA 30-Hour Construction</li>
                            <li>Confined Space Entry</li>
                            <li>Fall Protection Systems</li>
                            <li>JSA Development</li>
                            <li><span class="fillable placeholder">Your Safety Skill</span></li>
                        </ul>
                    </div>
                    
                    <div class="skill-category">
                        <h4>Coating Systems</h4>
                        <ul class="skill-list">
                            <li>SSPC Surface Preparation</li>
                            <li>Multi-coat System Application</li>
                            <li>Spray Gun Operations</li>
                            <li>Quality Control Inspection</li>
                            <li><span class="fillable placeholder">Your Technical Skill</span></li>
                        </ul>
                    </div>
                    
                    <div class="skill-category">
                        <h4>Equipment & Tools</h4>
                        <ul class="skill-list">
                            <li>Airless Spray Systems</li>
                            <li>Abrasive Blasting Equipment</li>
                            <li>Power Tools & Hand Tools</li>
                            <li>Measuring Instruments</li>
                            <li><span class="fillable placeholder">Your Equipment Skill</span></li>
                        </ul>
                    </div>
                    
                    <div class="skill-category">
                        <h4>Project Management</h4>
                        <ul class="skill-list">
                            <li>Crew Leadership (<span class="fillable placeholder">#</span>+ personnel)</li>
                            <li>Schedule Coordination</li>
                            <li>Quality Assurance</li>
                            <li>Client Communication</li>
                            <li><span class="fillable placeholder">Your Leadership Skill</span></li>
                        </ul>
                    </div>
                </div>
            </div>

            <!-- Education & Training -->
            <div class="section">
                <h2 class="section-title">📚 EDUCATION & TRAINING</h2>
                <div class="experience-item">
                    <div class="job-title"><span class="fillable placeholder">Your Education/Training</span></div>
                    <div class="company-info"><span class="fillable placeholder">Institution Name</span> • <span class="fillable placeholder">Year</span></div>
                </div>
                
                <div class="achievement">
                    Completed <span class="fillable placeholder">#</span>+ hours of specialized industrial training in <span class="fillable placeholder">areas</span>
                </div>
                <div class="achievement">
                    Ongoing professional development through <span class="fillable placeholder">organizations/programs</span>
                </div>
            </div>

            <!-- Download Button -->
            <button class="download-btn" onclick="window.print()">📄 DOWNLOAD/PRINT RESUME</button>
        </div>
    </div>

    <script>
        // Make fillable fields editable
        document.addEventListener('DOMContentLoaded', function() {
            const fillableElements = document.querySelectorAll('.fillable');
            
            fillableElements.forEach(element => {
                element.addEventListener('click', function() {
                    if (this.classList.contains('placeholder')) {
                        this.textContent = '';
                        this.classList.remove('placeholder');
                        this.style.color = '#2c3e50';
                    }
                });
                
                element.addEventListener('blur', function() {
                    if (this.textContent.trim() === '') {
                        this.classList.add('placeholder');
                        this.style.color = '#7f8c8d';
                    }
                });
                
                element.setAttribute('contenteditable', 'true');
            });
        });
    </script>
</body>
</html>
