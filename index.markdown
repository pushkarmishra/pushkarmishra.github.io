---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
# title: Pushkar Mishra
---

<html lang="en">
<title>Pushkar Mishra | Google DeepMind</title>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, sans-serif;
            margin: 0 auto;
            color: #333;
        }
        
        .header {
            display: grid;
            grid-template-columns: 2fr 1fr;
            gap: 25px;
            margin-bottom: 40px;
        }
        
        .profile-info h1 {
            font-size: 2.5em;
            margin: 0;
            color: #2d3748;
        }
        
        .profile-info .subtitle {
            color: #718096;
            font-size: 1.1em;
            margin: 10px 0 20px 0;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }
        
        .profile-image {
            max-width: 100%;
            height: auto;
            border-radius: 4px;
        }
        
        .google-scholar {
            display: inline-flex;
            align-items: center;
            padding: 12px 24px;
            background: #fff;
            border: 1px solid #e2e8f0;
            border-radius: 8px;
            text-decoration: none;
            color: #2d3748;
            font-weight: 500;
            margin-bottom: 40px;
        }
        
        .google-scholar svg {
            margin-left: 8px;
        }
        
        .section-title {
            color: #718096;
            font-size: 1.5em;
            margin: 30px 0 20px 0;
        }
        
        .research-areas {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
            margin-bottom: 40px;
        }
        
        .research-area {
            padding: 20px;
            color: white;
            border-radius: 8px;
            font-weight: 500;
        }
        
        .generative-ai {
            background: #1a1b3b;
        }
        
        .core-ml {
            background: #582f1c;
        }
        
        .nlp {
            background: #1f3937;
        }
    </style>
</head>
<body>
    <div class="header">
        <div class="profile-info">
            <h1>Pushkar Mishra</h1>
            <div class="subtitle">Lead AI Researcher | Google DeepMind</div>
            <p>Pushkar Mishra is a Lead AI researcher at Google DeepMind. His research interests include Generative AI, Core Machine Learning, and Natural Language Processing.</p>
        </div>
        <img src="assets/Pushkar_Mishra.jpg" alt="Pushkar Mishra" class="profile-image">
    </div>

    <a href="https://scholar.google.com/citations?user=bVcZ1qkAAAAJ" class="google-scholar" target="_blank">
        Google Scholar
        <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M5 10H15M15 10L10 5M15 10L10 15" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
        </svg>
    </a>

    <h2 class="section-title">Research Areas</h2>
    <div class="research-areas">
        <div class="research-area generative-ai">Generative AI</div>
        <div class="research-area core-ml">Core Machine Learning</div>
        <div class="research-area nlp">Natural Language Processing (NLP)</div>
    </div>
</body>
</html>