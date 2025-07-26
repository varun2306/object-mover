<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Object Mover - Visual Object Masking</title>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 40px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
        }
        
        .container {
            max-width: 800px;
            margin: 0 auto;
            background: white;
            border-radius: 15px;
            padding: 40px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.15);
        }
        
        .header {
            text-align: center;
            margin-bottom: 40px;
        }
        
        .emoji {
            font-size: 2rem;
            margin-right: 10px;
        }
        
        h1 {
            color: #2c3e50;
            font-size: 2.5rem;
            margin: 20px 0;
            text-align: center;
        }
        
        h2 {
            color: #34495e;
            font-size: 1.5rem;
            margin: 30px 0 20px 0;
            border-bottom: 3px solid #3498db;
            padding-bottom: 10px;
            display: flex;
            align-items: center;
        }
        
        .description {
            background: linear-gradient(135deg, #f8f9fa, #e9ecef);
            padding: 25px;
            border-radius: 10px;
            margin: 25px 0;
            border-left: 5px solid #3498db;
            font-size: 1.1rem;
            color: #2c3e50;
        }
        
        .steps {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 10px;
            margin: 20px 0;
        }
        
        .steps ul {
            list-style: none;
            padding: 0;
        }
        
        .steps li {
            background: white;
            margin: 10px 0;
            padding: 15px;
            border-radius: 8px;
            border-left: 4px solid #e74c3c;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
            transition: transform 0.2s ease;
        }
        
        .steps li:hover {
            transform: translateX(5px);
        }
        
        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
            gap: 15px;
            margin: 20px 0;
        }
        
        .tech-item {
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            padding: 15px;
            text-align: center;
            border-radius: 10px;
            font-weight: bold;
            box-shadow: 0 5px 15px rgba(102, 126, 234, 0.3);
            transition: transform 0.3s ease;
        }
        
        .tech-item:hover {
            transform: translateY(-5px);
        }
        
        .highlight {
            background: linear-gradient(135deg, #ff6b6b, #feca57);
            background-clip: text;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1><span class="emoji">🧠</span>Object Mover: Visual Object Masking in Images</h1>
        </div>
        
        <div class="description">
            This is a fun little Colab experiment where I built a basic pipeline that lets you highlight and visualize specific areas in an image — like the first step you'd take before moving objects using generative AI.
            <br><br>
            No deep training here — just some OpenCV and NumPy logic to mask parts of an image in red using defined coordinates. Later, this kind of setup could be used for <span class="highlight">object relocation</span> or <span class="highlight">AI-based scene editing</span>.
        </div>
        
        <h2><span class="emoji">🔧</span>How it works</h2>
        <div class="steps">
            <ul>
                <li>Load multiple images</li>
                <li>Define mask areas manually (for now)</li>
                <li>Overlay a red mask on each image</li>
                <li>Show both original and masked images side-by-side</li>
            </ul>
        </div>
        
        <h2><span class="emoji">🛠</span>Tech Used</h2>
        <div class="tech-grid">
            <div class="tech-item">Python</div>
            <div class="tech-item">OpenCV</div>
            <div class="tech-item">NumPy</div>
            <div class="tech-item">Matplotlib</div>
            <div class="tech-item">Google Colab</div>
        </div>
    </div>
</body>
</html>
