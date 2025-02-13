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
            overscroll-behavior-y: none;
        }
        
         /* Landing */
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
        
        /* Google scholar */
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
        
        /* Research areas */
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
            text-align: center;
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

        /* Updates */
        .latest-updates {
          margin: 2rem 0;
          padding: 1rem;
        }

        .updates-container {
          max-width: 800px;
          margin: 0 auto;
        }

        .update-card {
          display: flex;
          margin-bottom: 1.5rem;
          padding: 1rem;
          border-radius: 8px;
          background-color: #e1e6eb;
          transition: transform 0.2s ease;
        }

        .update-card:hover {
          transform: translateY(-2px);
          box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        .update-date {
          min-width: 200px;
          font-weight: 500;
          color: #666;
        }

        .update-content {
          flex: 1;
        }

        .update-content h3 {
          margin: 0 0 0.5rem 0;
          font-size: 1.1rem;
        }

        .update-content a {
          color: #1a73e8;
          text-decoration: none;
        }

        .update-content a:hover {
          text-decoration: underline;
        }

        .update-content p {
          margin: 0;
          color: #444;
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

    <br>
    <h2 class="section-title">Latest Updates</h2>
    <div class="updates-container">
    {% for update in site.data.updates limit:5 %}
      <div class="update-card">
        <div class="update-date">
          {{ update.date | date: "%B %d, %Y" }}
        </div>
        <div class="update-content">
          <h3>
            {% if update.link %}
              <a href="{{ update.link }}" target="_blank">{{ update.title }}</a>
            {% else %}
              {{ update.title }}
            {% endif %}
          </h3>
          <p>{{ update.description }}</p>
        </div>
      </div>
    {% endfor %}
  </div>
</body>
</html>