# tejjolly.github.io
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Tej Jolly – Engineering Portfolio</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="description" content="Portfolio of Tej Jolly – mechanical engineer working at the intersection of CFD, biomechanics, and machine learning.">
  <style>
    :root {
      --bg: #f8f7f9;
      --bg-alt: #ffffff;
      --accent: #a50021;
      --accent-soft: #fdebed;
      --text: #222222;
      --muted: #666666;
      --border: #dddddd;
      --shadow: 0 8px 20px rgba(0, 0, 0, 0.06);
      --radius: 16px;
      --max-width: 960px;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      background: var(--bg);
      color: var(--text);
      line-height: 1.6;
    }

    a {
      color: var(--accent);
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    header {
      background: var(--bg-alt);
      border-bottom: 1px solid var(--border);
      position: sticky;
      top: 0;
      z-index: 10;
    }

    .nav-inner {
      max-width: var(--max-width);
      margin: 0 auto;
      padding: 0.75rem 1.25rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 1rem;
    }

    .brand {
      font-weight: 700;
      letter-spacing: 0.03em;
      font-size: 0.95rem;
      text-transform: uppercase;
      color: var(--accent);
    }

    nav ul {
      list-style: none;
      display: flex;
      gap: 1rem;
      margin: 0;
      padding: 0;
      font-size: 0.9rem;
    }

    nav a {
      padding: 0.25rem 0.5rem;
      border-radius: 999px;
    }

    nav a:hover {
      background: var(--accent-soft);
      text-decoration: none;
    }

    main {
      max-width: var(--max-width);
      margin: 0 auto;
      padding: 1.5rem 1.25rem 3rem;
    }

    .hero {
      display: grid;
      grid-template-columns: minmax(0, 3fr) minmax(0, 2fr);
      gap: 2rem;
      align-items: center;
      margin-top: 1.5rem;
      margin-bottom: 2rem;
    }

    .hero-text h1 {
      margin-top: 0;
      font-size: 2rem;
      line-height: 1.2;
    }

    .hero-text p.lead {
      font-size: 1.05rem;
      color: var(--muted);
      margin-bottom: 1rem;
    }

    .hero-tags {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
      margin-bottom: 1.5rem;
    }

    .tag {
      font-size: 0.75rem;
      padding: 0.15rem 0.65rem;
      border-radius: 999px;
      border: 1px solid var(--border);
      background: var(--bg-alt);
      color: var(--muted);
      text-transform: uppercase;
      letter-spacing: 0.05em;
    }

    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 0.75rem;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      padding: 0.6rem 1.1rem;
      border-radius: 999px;
      font-size: 0.9rem;
      font-weight: 500;
      border: 1px solid transparent;
      cursor: pointer;
      transition: transform 0.04s ease, box-shadow 0.04s ease, background 0.1s ease;
    }

    .btn-primary {
      background: var(--accent);
      color: #ffffff;
      box-shadow: var(--shadow);
    }

    .btn-primary:hover {
      transform: translateY(-1px);
      box-shadow: 0 10px 24px rgba(0, 0, 0, 0.14);
      text-decoration: none;
    }

    .btn-ghost {
      background: transparent;
      color: var(--accent);
      border-color: var(--accent-soft);
    }

    .btn-ghost:hover {
      background: var(--accent-soft);
      text-decoration: none;
    }

    .hero-aside {
      background: var(--bg-alt);
      padding: 1.2rem 1.3rem;
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      border: 1px solid var(--border);
      font-size: 0.9rem;
    }

    .hero-aside h2 {
      margin-top: 0;
      font-size: 1rem;
      margin-bottom: 0.5rem;
    }

    .hero-aside ul {
      margin: 0.25rem 0 0.25rem 1.1rem;
      padding: 0;
    }

    section {
      margin-top: 2.5rem;
    }

    section h2 {
      font-size: 1.4rem;
      margin-bottom: 0.5rem;
    }

    section > p.section-intro {
      margin-top: 0;
      color: var(--muted);
      font-size: 0.95rem;
      max-width: 44rem;
    }

    .project-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 1.5rem;
      margin-top: 1.25rem;
    }

    .project-card {
      background: var(--bg-alt);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      padding: 1.1rem 1.2rem 1.2rem;
      border: 1px solid var(--border);
      display: flex;
      flex-direction: column;
      gap: 0.4rem;
      position: relative;
      overflow: hidden;
    }

    .project-label {
      font-size: 0.75rem;
      text-transform: uppercase;
      color: var(--muted);
      letter-spacing: 0.08em;
    }

    .project-card h3 {
      margin: 0.1rem 0 0.2rem;
      font-size: 1.05rem;
    }

    .project-meta {
      font-size: 0.8rem;
      color: var(--muted);
    }

    .project-description {
      font-size: 0.9rem;
      margin-top: 0.2rem;
    }

    .project-skills {
      font-size: 0.8rem;
      color: var(--muted);
      margin-top: 0.4rem;
    }

    .resume-card {
      background: var(--bg-alt);
      padding: 1.2rem 1.3rem;
      border-radius: var(--radius);
      border: 1px solid var(--border);
      box-shadow: var(--shadow);
      max-width: 520px;
    }

    .resume-card p {
      margin-top: 0.2rem;
      font-size: 0.9rem;
      color: var(--muted);
    }

    @media (max-width: 768px) {
      .hero {
        grid-template-columns: 1fr;
      }
      .hero-aside {
        order: -1;
      }
      .nav-inner {
        flex-direction: column;
        align-items: flex-start;
      }
      nav ul {
        flex-wrap: wrap;
      }
    }
  </style>
</head>
<body>

<header>
  <div class="nav-inner">
    <div class="brand">Tej Jolly</div>
    <nav>
      <ul>
        <li><a href="#intro">About</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#resume">Resume</a></li>
      </ul>
    </nav>
  </div>
</header>

<main>
  <section id="intro" class="hero">
    <div class="hero-text">
      <h1>Mechanical engineer working at the intersection of CFD, biomechanics, and machine learning.</h1>
      <p class="lead">
        I enjoy turning complex physical systems—blood flow, building ventilation, and real-time perception—into simulations and models that answer concrete questions for clinicians and engineers.
      </p>
      <div class="hero-tags">
        <span class="tag">Computational Fluid Dynamics</span>
        <span class="tag">Cardiovascular Biomechanics</span>
        <span class="tag">Machine Learning</span>
        <span class="tag">High-Performance Computing</span>
      </div>
      <div class="hero-actions">
        <a class="btn btn-primary" href="#projects">View projects</a>
        <a class="btn btn-ghost" href="#resume">Download resume</a>
      </div>
    </div>

    <aside class="hero-aside">
      <h2>About me</h2>
      <p>
        I am a mechanical engineering M.S. student at Carnegie Mellon University with a focus on computational fluid dynamics and cardiovascular biomechanics. In the BioSiMM Lab, I build and analyze coronary flow models to understand how vessel geometry and microvascular resistance shape the diagnostic indices clinicians rely on.
      </p>
      <p>
        My broader work spans decarbonization building simulations, sports analytics, and deep learning. I like projects where careful modeling, numerical methods, and clear communication come together to support better design and decision-making, whether the setting is a hospital, a city, or a research lab.
      </p>
    </aside>
  </section>

  <section id="projects">
    <h2>Selected Projects</h2>
    <p class="section-intro">
      These projects highlight how I use CFD, data analysis, and machine learning to study complex flows, design systems, and communicate results to both technical and non-technical audiences.
    </p>

    <div class="project-grid">
      <article class="project-card">
        <div class="project-label">Project 1 · Research</div>
        <h3>Microvascular Resistance and Coronary Diagnostic Indices</h3>
        <div class="project-meta">BioSiMM Lab, Carnegie Mellon · 2024–present</div>
        <p class="project-description">
          Coronary artery disease is often assessed with Fractional Flow Reserve (FFR) and Coronary Flow Reserve (CFR), yet many patients show conflicting results because these indices rarely account for downstream microvascular resistance. In this project, I build 3D coronary models and couple them to lumped-parameter networks to sweep hyperemic microvascular resistance in a controlled way. Using SimVascular, ParaView/VTK scripting, and high-performance computing, I run large CFD campaigns and compute FFR, CFR, and related indices to quantify how microvascular conditions alone can push identical lesions across clinical decision thresholds. The work shows that pressure- and flow-based metrics must be interpreted in the context of microvascular health if we want reliable, patient-specific diagnostics.
        </p>
        <p class="project-skills">
          Skills: Coronary CFD · Lumped-parameter modeling · ParaView/VTK scripting · Slurm/HPC · Python data analysis
        </p>
      </article>

      <article class="project-card">
        <div class="project-label">Project 2 · Course Project</div>
        <h3>Decarbonization Building CFD: Reducing Re-Entrained Exhaust</h3>
        <div class="project-meta">Computational Fluid Dynamics · Fall 2024</div>
        <p class="project-description">
          Direct-air-capture facilities pull ambient air through sorbent systems and exhaust carbon-depleted air, but under some wind conditions that cleaned exhaust can be swept back into the inlet, wasting energy and reducing CO₂ removal. Our team used 3D CFD to evaluate how building shape and intake/exhaust flow rates influence this re-entrainment. We defined a simplified atmospheric boundary-layer domain, tested candidate building geometries, and tracked a passive scalar representing processed exhaust air. By comparing the fraction of exhaust that reappeared at the inlet across cases, we identified geometric features and operating points that reduce wake recirculation and re-entrainment, offering design guidance for more efficient decarbonization buildings.
        </p>
        <p class="project-skills">
          Skills: External-flow CFD · Species transport · Parametric studies · Technical reporting
        </p>
      </article>

      <article class="project-card">
        <div class="project-label">Project 3 · Computer Vision</div>
        <h3>PlayerVision: Real-Time Player &amp; Ball Tracking for Sports</h3>
        <div class="project-meta">Computer Vision for Engineers · Fall 2024</div>
        <p class="project-description">
          Professional broadcasters still depend heavily on manual tagging of events and players. In PlayerVision, our team built an end-to-end pipeline that ingests soccer broadcast footage, detects players and the ball with a YOLO-based model, and tracks identities over time using DeepSORT. I implemented contrast enhancement and a jersey-color clustering module that masks out the pitch and assigns tracks to teams based on color distance to reference swatches. On top of that, I added proximity analysis between the ball and all players to highlight the current ball-carrier and nearest defender. The result is a prototype system that can overlay player IDs, team labels, and ball highlights in near real time.
        </p>
        <p class="project-skills">
          Skills: Python · OpenCV · YOLO · DeepSORT · K-means clustering · Real-time visualization
        </p>
      </article>

      <article class="project-card">
        <div class="project-label">Project 4 · Deep Learning</div>
        <h3>Modular Diffusion Model Framework for Image Synthesis</h3>
        <div class="project-meta">Deep Learning · Fall 2024</div>
        <p class="project-description">
          Diffusion models can generate impressive images but are often slow and memory-intensive when run directly in pixel space. For this project, our team built a modular diffusion toolkit from scratch: I implemented the core DDPM training loop and U-Net architecture with timestep conditioning, while teammates added DDIM sampling, a VAE-based latent diffusion stage, and classifier-free guidance. We layered in strategies such as Exponential Moving Average of weights and Karras noise schedules. Trained on a subset of ImageNet, our best configuration—latent DDIM with guidance—reduced Fréchet Inception Distance by over 40% relative to a baseline DDPM while requiring far fewer sampling steps, demonstrating a practical speed–quality tradeoff.
        </p>
        <p class="project-skills">
          Skills: PyTorch · U-Nets · DDPM/DDIM · Latent diffusion · Classifier-free guidance · Model evaluation (FID/IS)
        </p>
      </article>
    </div>
  </section>

  <section id="resume">
    <h2>Resume</h2>
    <p class="section-intro">
      A one-page resume summarizing my education, research, and experience is available here.
    </p>

    <div class="resume-card">
      <strong>Download my resume (PDF)</strong>
      <p>
        This resume highlights my work in coronary CFD, engineering communication, and applied machine learning.
      </p>
      <p>
        <a class="btn btn-primary" href="Resume_TJ.pdf" download>
          Download Resume
        </a>
      </p>
    </div>
  </section>
</main>

</body>
</html>
```
