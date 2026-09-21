---
layout: default
title: CV
---

.spacer {
  height: 20rem;
}


<div class="cv-download">
  <a href="{{ '/ShreyaShahCV.pdf' | relative_url }}" download class="cv-download">Download my CV (PDF)</a>
</div>


<section class="cv-section">
  <h2>Education</h2>

  <div class="cv-entry">
    <div class="cv-logo-box"><img src="{{ '/logos/ImperialLogo.jpg' | relative_url }}" alt="Imperial College London" class="cv-logo"></div>
    <div>
      <h3>Imperial College London — BSc (Hons) Bioengineering</h3>
      <p class="cv-dates">2024 – 2027</p>
      <p>Programming, Mathematics, Probability &amp; Statistics, Data Analysis, Finance &amp; Financial Management, Business Economics, Entrepreneurship &amp; Innovation</p>
    </div>
  </div>

  <div class="cv-entry">
    <div class="cv-logo-box"><img src="{{ '/logos/IBLogo.webp' | relative_url }}" alt="International Baccalaureate" class="cv-logo"></div>
    <div>
      <h3>North London Collegiate School — International Baccalaureate, 42/45</h3>
      <p class="cv-dates">2022 – 2024</p>
      <p>Higher Level: Mathematics, Biology, Chemistry. Standard Level: English, French, Politics</p>
    </div>
  </div>
</section>

<section class="cv-section">
  <h2>Experience</h2>

  <div class="cv-entry">
    <div class="cv-logo-box"><img src="{{ '/logos/aberdeenLogo.jpg' | relative_url }}" alt="Aberdeen Group PLC" class="cv-logo"></div>
    <div>
      <h3>Aberdeen Group PLC — Investments Intern</h3>
      <p class="cv-dates">Jun – Aug 2026</p>
      <ul>
        <li>Designed and shipped an end-to-end automation tool (Power Apps / Power Automate) that re-engineered a manual governance process, cutting turnaround by 3 hours per request with full traceability.</li>
        <li>Owned a new investment product from concept to launch: structured it, selected constituents via quantitative analysis, and built the go-to-market strategy.</li>
        <li>Ran a cross-market process review, translating regulatory requirements into a practical, compliant framework.</li>
      </ul>
    </div>
  </div>

  <div class="cv-entry">
    <div class="cv-logo-box"><img src="{{ '/logos/30TLogo.jpeg' | relative_url }}" alt="3O Technology" class="cv-logo"></div>
    <div>
      <h3>3O Technology — Operations Intern</h3>
      <p class="cv-dates">Aug – Sept 2025</p>
      <ul>
        <li>Diagnosed regulatory and supply chain bottlenecks limiting a startup's ability to scale.</li>
        <li>Authored a data-backed report that directly shaped the company's funding strategy.</li>
      </ul>
    </div>
  </div>

  <div class="cv-entry">
    <div class="cv-logo-box"><img src="{{ '/logos/occuityLogo.png' | relative_url }}" alt="Occuity" class="cv-logo"></div>
    <div>
      <h3>Occuity — Product &amp; Research Assistant</h3>
      <p class="cv-dates">Aug 2023</p>
      <ul>
        <li>Bridged R&amp;D and commercial teams, turning user needs into concrete product decisions.</li>
        <li>Applied quantitative modelling to evaluate and de-risk design trade-offs.</li>
      </ul>
    </div>
  </div>

  <div class="cv-entry">
    <div class="cv-logo-box"><img src="{{ '/logos/centralvisionlogo.jpeg' | relative_url }}" alt="Central Vision Opticians" class="cv-logo"></div>
    <div>
      <h3>Central Vision Opticians — Finance, Operations and Marketing Assistant</h3>
      <p class="cv-dates">2020 – 2024</p>
      <ul>
        <li>Accounting support for the practice to understand key performance metrics to support growth.</li>
        <li>Developed marketing campaigns to provide useful content and insights to patients.</li>
      </ul>
    </div>
  </div>

  <div class="cv-entry">
    <div class="cv-logo-box"><img src="{{ '/logos/NHSLogo.webp' | relative_url }}" alt="NHS" class="cv-logo"></div>
    <div>
      <h3>Attenborough Surgery (NHS) — Clinic Administration Assistant</h3>
      <p class="cv-dates">2020 – 2024</p>
      <ul>
        <li>Managed sensitive data in a regulated environment through the COVID-19 vaccination programme, building rigor under pressure.</li>
      </ul>
    </div>
  </div>
</section>

<section class="cv-section">
  <h2>Projects</h2>
  <ul class="cv-plain-list">
    <li><strong>Automated Cell Subculture System</strong> — designed and built a sensor-driven device with automated control logic (CAD, 3D printing, Arduino) to spec and budget.</li>
    <li><strong>Robotic Arm</strong> — engineered a working prototype with closed-loop, sensor-based feedback control.</li>
    <li><strong>Heart Rate Meter</strong> — built a custom PCB device applying signal processing to capture physiological data.</li>
  </ul>
</section>

<section class="cv-section">
  <h2>Skills</h2>
  <p><strong>Programming &amp; AI:</strong> Python, MATLAB, Arduino, LaTeX, AI agent building, Claude Code, Copilot</p>
  <p><strong>Automation &amp; Tools:</strong> Power Apps, Power Automate, Excel, CAD (SolidWorks)</p>
  <p><strong>Analysis:</strong> Quantitative &amp; statistical analysis, data-driven decision making</p>
</section>

<section class="cv-section">
  <h2>Extracurricular</h2>
  <ul class="cv-plain-list">
    <li><strong>Cheerleading:</strong> competitive athlete and coach, developing discipline and time management under a demanding schedule.</li>
    <li><strong>Tutor:</strong> taught students aged 11 through A-Level, distilling complex ideas into clear explanations.</li>
    <li>Manages a personal investment portfolio with an ESG and sustainability focus.</li>
  </ul>
</section>

<style>
  .cv-download {
    display: inline-block;
    margin-bottom: 2rem;
    padding: 0.6rem 1.4rem;
    border: 1px solid #ffffff;
    color: #ffffff;
    text-decoration: none;
    transition: background-color 0.2s ease, color 0.2s ease;
    text-align: center;
  }
  .cv-download:hover {
    background-color: #b30000;
    color: #000000;
  }

  .cv-section {
    max-width: 800px;
    margin: 0 auto 3rem auto;
    padding: 0 1rem;
  }
  .cv-section h2 {
    border-bottom: 1px solid #444;
    padding-bottom: 0.5rem;
  }

  /* The core new layout: logo box on the left, text block on the
     right, aligned to the top since text blocks vary in height. */
  .cv-entry {
    display: flex;
    align-items: flex-start;
    gap: 1rem;
    margin-bottom: 1.5rem;
  }

  /* Fixed-size box, regardless of each logo's actual dimensions,
     so a wide logo (Imperial) and a square one (Occuity) still
     occupy the same footprint and line up neatly down the page. */
  .cv-logo-box {
    flex-shrink: 0; /* stops the box being squashed by long text next to it */
    width: 70px;
    height: 70px;
    background-color: #ffffff;
    border-radius: 8px;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 6px;
  }

  /* object-fit: contain scales the image to fit fully inside its
     box without cropping or stretching, whatever its original
     aspect ratio. This is the key property making mismatched logo
     shapes behave consistently. */
  .cv-logo {
    max-width: 100%;
    max-height: 100%;
    object-fit: contain;
  }

  .cv-logo-placeholder {
    color: #000000;
    font-weight: 600;
    font-size: 0.8rem;
  }

  .cv-dates {
    color: #b3b3b3;
    font-style: italic;
    margin: 0.2rem 0 0.5rem 0;
  }

  .cv-plain-list {
    padding-left: 1.2rem;
  }
</style>
