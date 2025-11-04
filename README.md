<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Maurizio Farina - GitHub Portfolio</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    
    body {
      font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
      background: linear-gradient(135deg, #f5f7fa 0%, #e8ecf1 100%);
      color: #2a3442;
      line-height: 1.6;
      min-height: 100vh;
      padding: 2rem 1rem;
    }
    
    .container {
      max-width: 1200px;
      margin: 0 auto;
    }
    
    .header {
      text-align: center;
      margin-bottom: 3rem;
      padding: 2rem;
      background: white;
      border-radius: 1rem;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
    }
    
    .avatar {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      border: 4px solid #5a7aa8;
      margin: 0 auto 1.5rem;
      display: block;
    }
    
    .name {
      font-size: 2.25rem;
      font-weight: 700;
      color: #5a7aa8;
      margin-bottom: 0.5rem;
      letter-spacing: -0.02em;
    }
    
    .username {
      font-size: 1.25rem;
      color: #6b7785;
      font-family: 'JetBrains Mono', 'Courier New', monospace;
      margin-bottom: 1rem;
    }
    
    .bio {
      font-size: 1.125rem;
      color: #4a5568;
      max-width: 600px;
      margin: 0 auto 1.5rem;
    }
    
    .user-links {
      display: flex;
      gap: 1.5rem;
      justify-content: center;
      flex-wrap: wrap;
      margin-top: 1rem;
    }
    
    .user-link {
      color: #5a7aa8;
      text-decoration: none;
      font-weight: 500;
      transition: color 0.2s;
    }
    
    .user-link:hover {
      color: #d4924a;
    }
    
    .stats {
      display: flex;
      gap: 2rem;
      justify-content: center;
      margin-top: 1.5rem;
      padding-top: 1.5rem;
      border-top: 1px solid #e8ecf1;
    }
    
    .stat {
      text-align: center;
    }
    
    .stat-value {
      font-size: 1.5rem;
      font-weight: 700;
      color: #5a7aa8;
    }
    
    .stat-label {
      font-size: 0.875rem;
      color: #6b7785;
      text-transform: uppercase;
      letter-spacing: 0.05em;
    }
    
    .projects-header {
      text-align: center;
      margin-bottom: 2rem;
    }
    
    .projects-title {
      font-size: 2rem;
      font-weight: 600;
      color: #2a3442;
      margin-bottom: 0.5rem;
    }
    
    .projects-subtitle {
      color: #6b7785;
      font-size: 1rem;
    }
    
    .projects-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
      gap: 1.5rem;
      margin-bottom: 3rem;
    }
    
    .project-card {
      background: white;
      border-radius: 0.75rem;
      padding: 1.5rem;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.05);
      transition: all 0.3s ease;
      border: 1px solid #e8ecf1;
    }
    
    .project-card:hover {
      transform: translateY(-4px);
      box-shadow: 0 8px 16px rgba(90, 122, 168, 0.15);
      border-color: #5a7aa8;
    }
    
    .project-header {
      display: flex;
      justify-content: space-between;
      align-items: start;
      margin-bottom: 1rem;
      gap: 1rem;
    }
    
    .project-title {
      font-size: 1.25rem;
      font-weight: 600;
      flex: 1;
    }
    
    .project-title a {
      color: #2a3442;
      text-decoration: none;
      transition: color 0.2s;
    }
    
    .project-title a:hover {
      color: #5a7aa8;
    }
    
    .language-badge {
      background: #5a7aa8;
      color: white;
      padding: 0.25rem 0.75rem;
      border-radius: 1rem;
      font-size: 0.75rem;
      font-weight: 500;
      white-space: nowrap;
    }
    
    .project-description {
      color: #4a5568;
      margin-bottom: 1rem;
      line-height: 1.6;
    }
    
    .topics {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
      margin-bottom: 1rem;
    }
    
    .topic-tag {
      background: #f0f4f8;
      color: #5a7aa8;
      padding: 0.25rem 0.625rem;
      border-radius: 0.375rem;
      font-size: 0.75rem;
      font-weight: 500;
    }
    
    .project-stats {
      color: #6b7785;
      font-size: 0.875rem;
      padding-top: 1rem;
      border-top: 1px solid #f0f4f8;
    }
    
    .footer {
      text-align: center;
      padding: 2rem;
      color: #6b7785;
      font-size: 0.875rem;
    }
    
    .footer a {
      color: #5a7aa8;
      text-decoration: none;
      font-weight: 500;
    }
    
    .footer a:hover {
      color: #d4924a;
    }
    
    @media (max-width: 640px) {
      .projects-grid {
        grid-template-columns: 1fr;
      }
      
      .stats {
        gap: 1rem;
      }
      
      .name {
        font-size: 1.75rem;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <header class="header">
      <img src="https://avatars.githubusercontent.com/u/1065769?v=4" alt="Maurizio Farina" class="avatar">
      <h1 class="name">Maurizio Farina</h1>
      <div class="username">@mwzero</div>
      <p class="bio">//dev</p>
      
      <div class="user-links">
        <a href="https://github.com/mwzero" class="user-link" target="_blank" rel="noopener noreferrer">GitHub Profile</a>
        <a href="https://www.linkedin.com/in/farinamaurizio" class="user-link" target="_blank" rel="noopener noreferrer">Website</a>
        <span class="user-link">📍 Napoli</span>
      </div>
      
      <div class="stats">
        <div class="stat">
          <div class="stat-value">21</div>
          <div class="stat-label">Repositories</div>
        </div>
        <div class="stat">
          <div class="stat-value">6</div>
          <div class="stat-label">Followers</div>
        </div>
        <div class="stat">
          <div class="stat-value">8</div>
          <div class="stat-label">Following</div>
        </div>
      </div>
    </header>
    
    <div class="projects-header">
      <h2 class="projects-title">Projects</h2>
      <p class="projects-subtitle">21 public repositories</p>
    </div>
    
    <div class="projects-grid">
      
        <div class="project-card">
          <div class="project-header">
            <h3 class="project-title">
              <a href="https://github.com/mwzero/mwzero" target="_blank" rel="noopener noreferrer">
                mwzero
              </a>
            </h3>
            <span class="language-badge">HTML</span>
          </div>
          
          <p class="project-description">The "mwzero" repository showcases a collection of portfolio projects that highlight my skills and creativity as a developer. Primarily built with HTML, these projects reflect my dedication to crafting engaging and visually appealing web experiences. This repository serves as a testament to my ability to combine technical knowledge with artistic design, making it a valuable resource for potential employers and collaborators seeking innovative web solutions.</p>
          
          
          
          
        </div>
      
        <div class="project-card">
          <div class="project-header">
            <h3 class="project-title">
              <a href="https://github.com/mwzero/promptworks" target="_blank" rel="noopener noreferrer">
                promptworks
              </a>
            </h3>
            
          </div>
          
          <p class="project-description">**Promptworks** is a dynamic collection of prompt seeds designed to simplify the creation of ETL (Extract, Transform, Load) configurations for data management projects. By generating customizable ETL configurations with ease, this repository empowers developers to streamline their workflows and enhance data processing efficiency. Its innovative approach to prompt generation showcases a commitment to optimizing developer productivity, making it an attractive asset for teams focused on robust data solutions.</p>
          
          
          
          
        </div>
      
        <div class="project-card">
          <div class="project-header">
            <h3 class="project-title">
              <a href="https://github.com/mwzero/jui" target="_blank" rel="noopener noreferrer">
                jui
              </a>
            </h3>
            <span class="language-badge">Java</span>
          </div>
          
          <p class="project-description">JUI is an innovative framework designed to empower Java developers to effortlessly create interactive web applications without the need for HTML, CSS, or JavaScript. By simply writing Java code, users can build dynamic user interfaces and serve their applications via a built-in HTTP server, streamlining the development process. With its lightweight design and ease of use, JUI not only enhances productivity but also allows developers to focus on their ideas, making it an impressive addition to any software project.</p>
          
          
            <div class="topics">
              <span class="topic-tag">frontend</span><span class="topic-tag">java</span><span class="topic-tag">web</span>
            </div>
          
          
          <div class="project-stats">⭐ 5 · 🔀 1</div>
        </div>
      
        <div class="project-card">
          <div class="project-header">
            <h3 class="project-title">
              <a href="https://github.com/mwzero/AskCam" target="_blank" rel="noopener noreferrer">
                AskCam
              </a>
            </h3>
            
          </div>
          
          <p class="project-description">**AskCam** is an innovative voice-activated assistant that transforms your webcam into an intelligent query platform, allowing users to ask questions about their surroundings in real-time. By leveraging advanced vision-language integration through the LLaVA model, it intelligently interprets visual data and delivers informative spoken responses. This project showcases proficiency in Python and the use of cutting-edge tech, like OpenCV for live camera handling and Whisper for speech recognition, demonstrating a strong ability to create interactive and user-friendly applications.</p>
          
          
          
          
        </div>
      
        <div class="project-card">
          <div class="project-header">
            <h3 class="project-title">
              <a href="https://github.com/mwzero/system-prompts" target="_blank" rel="noopener noreferrer">
                system-prompts
              </a>
            </h3>
            
          </div>
          
          <p class="project-description">The **system-prompts** repository is a comprehensive collection of system prompts designed for large language models (LLMs), showcasing over 7000 lines of curated insights from various AI tools and agents. This project not only provides valuable prompts from well-known platforms like Manus, Replit, and VSCode but also aims to enhance AI interactions by streamlining how users engage with technology. By contributing to and organizing this resource, I demonstrate my commitment to advancing AI capabilities and fostering collaboration in the developer community, making it a standout addition to my portfolio.</p>
          
          
          
          
        </div>
      
        <div class="project-card">
          <div class="project-header">
            <h3 class="project-title">
              <a href="https://github.com/mwzero/hubbers" target="_blank" rel="noopener noreferrer">
                hubbers
              </a>
            </h3>
            <span class="language-badge">Java</span>
          </div>
          
          <p class="project-description">Hubbers is an innovative Java framework designed to facilitate collaboration among autonomous agents in multi-agent systems. By enabling seamless communication and coordination, Hubbers empowers developers to create complex systems where agents work together to achieve shared goals. With built-in tools for messaging, lifecycle management, and task coordination, this framework streamlines the development process and enhances the capabilities of your applications, making it an exciting resource for anyone looking to harness the power of agent-based technology.</p>
          
          
          
          
        </div>
      
        <div class="project-card">
          <div class="project-header">
            <h3 class="project-title">
              <a href="https://github.com/mwzero/screenshot-to-code" target="_blank" rel="noopener noreferrer">
                screenshot-to-code
              </a>
            </h3>
            
          </div>
          
          <p class="project-description">The **screenshot-to-code** project is an innovative tool that effortlessly transforms screenshots, mockups, and Figma designs into high-quality, responsive code, supporting various frameworks such as HTML, React, and Vue. Utilizing advanced AI models, including Claude Sonnet 3.5 and GPT-4o, it not only generates clean code but also experiments with converting screen recordings into functional prototypes. This versatile solution enhances productivity and streamlines the design-to-development workflow, making it a valuable asset for developers and teams aiming to accelerate project delivery.</p>
          
          
          
          
        </div>
      
        <div class="project-card">
          <div class="project-header">
            <h3 class="project-title">
              <a href="https://github.com/mwzero/maildiscoverer" target="_blank" rel="noopener noreferrer">
                maildiscoverer
              </a>
            </h3>
            <span class="language-badge">Python</span>
          </div>
          
          <p class="project-description">**Maildiscoverer** is a Python-based tool designed to streamline email discovery processes, helping users efficiently identify and retrieve email addresses from various sources. Its intuitive functionality caters to both personal and academic projects, making it a valuable asset for developers looking to enhance their email outreach strategies. By leveraging Python’s robust capabilities, this project not only showcases proficiency in coding but also reflects a commitment to creating practical solutions in the realm of communication and data collection.</p>
          
          
          
          
        </div>
      
        <div class="project-card">
          <div class="project-header">
            <h3 class="project-title">
              <a href="https://github.com/mwzero/ChatDev" target="_blank" rel="noopener noreferrer">
                ChatDev
              </a>
            </h3>
            
          </div>
          
          <p class="project-description">ChatDev is an innovative virtual software company that harnesses the power of intelligent agents to facilitate software development through natural language interactions. By utilizing advanced Large Language Model (LLM) technology, these collaborative agents assume various roles—like CEO, programmer, and designer—to streamline the creation of customized software solutions. This unique multi-agent approach not only simplifies the development process but also empowers users to transform ideas into functional software efficiently, making it an exciting tool for developers and organizations aiming to revolutionize their programming workflows.</p>
          
          
          
          
        </div>
      
        <div class="project-card">
          <div class="project-header">
            <h3 class="project-title">
              <a href="https://github.com/mwzero/ai-cookbook" target="_blank" rel="noopener noreferrer">
                ai-cookbook
              </a>
            </h3>
            
          </div>
          
          <p class="project-description">The **ai-cookbook** repository serves as a collaborative platform where users can share practical examples of utilizing Mistral models. It showcases a variety of interactive notebooks that demonstrate capabilities such as prompt design, retrieval-augmented generation, and embedding techniques, all optimized for Google Colab. By fostering community contributions and focusing on reproducibility, this project not only highlights innovative applications in AI but also offers valuable resources for developers and researchers looking to leverage Mistral technologies in their own work.</p>
          
          
          
          
        </div>
      
        <div class="project-card">
          <div class="project-header">
            <h3 class="project-title">
              <a href="https://github.com/mwzero/flowy" target="_blank" rel="noopener noreferrer">
                flowy
              </a>
            </h3>
            
          </div>
          
          <p class="project-description">Flowy is a minimal JavaScript library designed to simplify the creation of visually appealing flowcharts, making it easy for developers to integrate flowchart functionality into their web applications. With features like responsive drag-and-drop, automatic snapping, and mobile support, Flowy enables the rapid development of tools for automation, mind mapping, and programming without any dependencies. This project showcases not only the elegance of JavaScript but also the capability to enhance user interaction and experience, making it an impressive addition to any developer's portfolio.</p>
          
          
          
          
        </div>
      
        <div class="project-card">
          <div class="project-header">
            <h3 class="project-title">
              <a href="https://github.com/mwzero/Drawflow" target="_blank" rel="noopener noreferrer">
                Drawflow
              </a>
            </h3>
            
          </div>
          
          <p class="project-description">Drawflow is an intuitive library designed for creating dynamic data flow diagrams effortlessly. With just a few lines of code, developers can implement features like draggable nodes, customizable inputs and outputs, and seamless data synchronization—all without any dependencies. This lightweight solution is perfect for building visual applications, making it an impressive addition to any portfolio that showcases versatility in front-end development.</p>
          
          
          
          
        </div>
      
        <div class="project-card">
          <div class="project-header">
            <h3 class="project-title">
              <a href="https://github.com/mwzero/colab" target="_blank" rel="noopener noreferrer">
                colab
              </a>
            </h3>
            <span class="language-badge">Jupyter Notebook</span>
          </div>
          
          <p class="project-description">The **Colab** repository showcases a series of Jupyter Notebooks designed for interactive data analysis and exploration. One notable project within this collection demonstrates how to seamlessly utilize OpenAI's embeddings to query a Pinecone index, enabling efficient data retrieval and insight generation. This project not only highlights proficiency in integrating cutting-edge AI technologies but also illustrates a hands-on approach to solving real-world problems through innovative data solutions, making it a valuable asset for potential employers or collaborators in the tech industry.</p>
          
          
          
          
        </div>
      
        <div class="project-card">
          <div class="project-header">
            <h3 class="project-title">
              <a href="https://github.com/mwzero/Criteria" target="_blank" rel="noopener noreferrer">
                Criteria
              </a>
            </h3>
            <span class="language-badge">C</span>
          </div>
          
          <p class="project-description">The Criteria repository is a powerful workflow engine developed in C/C++, designed to streamline and automate complex processes efficiently. By leveraging the robust capabilities of these programming languages, it offers a flexible solution for managing workflows, enabling developers to build efficient systems tailored to various applications. This project not only showcases strong coding skills but also demonstrates a commitment to enhancing productivity through innovative technology, making it an impressive addition to any developer's portfolio.</p>
          
          
            <div class="topics">
              <span class="topic-tag">workflow</span><span class="topic-tag">workflow-engine</span>
            </div>
          
          
          
        </div>
      
        <div class="project-card">
          <div class="project-header">
            <h3 class="project-title">
              <a href="https://github.com/mwzero/pipeline-flow" target="_blank" rel="noopener noreferrer">
                pipeline-flow
              </a>
            </h3>
            
          </div>
          
          <p class="project-description">The "pipeline-flow" project demonstrates an innovative approach to streamlining data processes, likely focusing on efficient data manipulation and workflow automation. Leveraging state-of-the-art coding practices, this repository showcases how to create a seamless flow of data, making it easy to integrate and manage complex pipelines. Its elegant design and functionality not only enhance productivity but also illustrate a commitment to quality and user-friendly solutions, making it an impressive addition to any developer's portfolio for potential employers or collaborators seeking expertise in data workflows.</p>
          
          
          
          
        </div>
      
        <div class="project-card">
          <div class="project-header">
            <h3 class="project-title">
              <a href="https://github.com/mwzero/low-code" target="_blank" rel="noopener noreferrer">
                low-code
              </a>
            </h3>
            
          </div>
          
          <p class="project-description">The repository collects personal technical investigation about low-code programming</p>
          
          
          
          
        </div>
      
        <div class="project-card">
          <div class="project-header">
            <h3 class="project-title">
              <a href="https://github.com/mwzero/katacoda" target="_blank" rel="noopener noreferrer">
                katacoda
              </a>
            </h3>
            
          </div>
          
          <p class="project-description">A software project focused on katacoda.</p>
          
          
          
          
        </div>
      
        <div class="project-card">
          <div class="project-header">
            <h3 class="project-title">
              <a href="https://github.com/mwzero/bOS.NET" target="_blank" rel="noopener noreferrer">
                bOS.NET
              </a>
            </h3>
            <span class="language-badge">C#</span>
          </div>
          
          <p class="project-description">a common library for .net development</p>
          
          
          
          
        </div>
      
        <div class="project-card">
          <div class="project-header">
            <h3 class="project-title">
              <a href="https://github.com/mwzero/mkjava" target="_blank" rel="noopener noreferrer">
                mkjava
              </a>
            </h3>
            <span class="language-badge">Java</span>
          </div>
          
          <p class="project-description">Java code used by the tutorials and posts included in http://www.mkjava.com</p>
          
          
            <div class="topics">
              <span class="topic-tag">learning</span><span class="topic-tag">log4j</span><span class="topic-tag">opentracing</span>
            </div>
          
          
          
        </div>
      
        <div class="project-card">
          <div class="project-header">
            <h3 class="project-title">
              <a href="https://github.com/mwzero/Criteria.Web" target="_blank" rel="noopener noreferrer">
                Criteria.Web
              </a>
            </h3>
            <span class="language-badge">JavaScript</span>
          </div>
          
          <p class="project-description">Criteria Workflow Engine Web Console</p>
          
          
          
          
        </div>
      
        <div class="project-card">
          <div class="project-header">
            <h3 class="project-title">
              <a href="https://github.com/mwzero/passwd" target="_blank" rel="noopener noreferrer">
                passwd
              </a>
            </h3>
            <span class="language-badge">JavaScript</span>
          </div>
          
          <p class="project-description">a simple html mobile application to manage passwords</p>
          
          
          
          
        </div>
      
    </div>
    
    <footer class="footer">
      <p>Generated with <a href="https://github.com" target="_blank" rel="noopener noreferrer">GitHub Portfolio Generator</a></p>
      <p>Last updated: November 4, 2025</p>
    </footer>
  </div>
</body>
</html>
