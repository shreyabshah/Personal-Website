---
layout: default
title: Home
---

<header class="hero">
  <div class="curtain-overlay">
    <div class="curtain-panel curtain-left"></div>
    <div class="curtain-panel curtain-right"></div>
    <h1 class="curtain-text">Welcome to Shreya's Website</h1>
  </div>
</header>

<style>
  .hero {
    position: relative;
    height: 100vh;
    background-image: url('{{ "/curtains-homepage.jpg" | relative_url }}');
    background-size: cover;
    background-position: center;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .curtain-overlay {
    position: absolute;
    inset: 0;
    z-index: 999;
    display: flex;
    align-items: center;
    justify-content: center;
    pointer-events: none;
  }

  .curtain-panel {
    position: absolute;
    top: 0;
    height: 100%;
    width: 50%;
    background: linear-gradient(90deg, #4a0000, #8b0000, #4a0000);
  }
  .curtain-left { left: 0; }
  .curtain-right { right: 0; }

  .curtain-left  { animation: slide-left  1.5s ease-in-out 2.5s forwards; }
  .curtain-right { animation: slide-right 1.5s ease-in-out 2.5s forwards; }
  @keyframes slide-left  { to { transform: translateX(-100%); } }
  @keyframes slide-right { to { transform: translateX(100%);  } }

  .curtain-text {
  display: inline-block;
  color: #f5e6c8;
  font-family: 'Dancing Script', cursive;
  font-weight: 700;
  font-size: 3rem;
  white-space: nowrap;
  clip-path: inset(0 100% 0 0);
  animation: reveal-handwriting 2s ease-out 0.3s forwards;
  }
  
  @keyframes reveal-handwriting {
    to { clip-path: inset(0 0% 0 0); }
  }
  
  @media (max-width: 600px) {
    .curtain-text {
      font-size: 1.6rem;
      white-space: normal;
      text-align: center;
      padding: 0 1rem;
    }
  }
  
  @keyframes reveal-handwriting {
    to { clip-path: inset(0 0% 0 0); }
  }
</style>

<section class="about-section">
  <div class="about-grid">
    <img src="{{ '/images/about-portrait.jpg' | relative_url }}" alt="Shreya" class="about-photo">
    <div class="about-text">
      <h2>Hi, I'm Shreya</h2>
      <p>I've always been the person who wants to take things apart to see how they actually work, these days that means a soldering iron and CAD as often as a textbook. I'm a Bioengineering student at Imperial College London, and what pulls me in isn't the subject itself so much as the puzzle underneath it, the kind of problem that doesn't have an obvious fix yet.</p>
      <p>
        <img src="{{ '/images/about-cheer.jpg' | relative_url }}" alt="Cheerleading stunt" class="about-inline-photo">
        Outside of that, I stunt and base for my university's competitive cheer squad, which has taught me more about trust and timing than most lectures have.
      </p>
    </div>
  </div>
</section>

<style>
  .about-section {
    max-width: 900px;
    margin: 4rem auto;
    padding: 0 1.5rem;
  }

  /* Two columns on wide screens: fixed-width photo, flexible text.
     "grid-template-columns: 280px 1fr" means the first column is
     exactly 280px, the second takes up whatever space is left. */
  .about-grid {
    display: grid;
    grid-template-columns: 280px 1fr;
    gap: 2rem;
    align-items: start;
  }

  .about-photo {
    width: 100%;
    border-radius: 8px;
    object-fit: cover;
  }

  .about-text h2 {
    margin-top: 0;
  }

  .about-text p {
    line-height: 1.6;
    margin-bottom: 1.2rem;
  }

  /* Small inline photo that floats beside the cheerleading text
     rather than taking a full column, since it's a secondary
     detail, not equal billing with the main portrait. */
  .about-inline-photo {
    float: left;
    width: 120px;
    border-radius: 6px;
    margin: 0 1rem 0.5rem 0;
  }

  /* Stack to a single column on narrow screens, same reasoning
     as the nav media query earlier: a 280px fixed column plus
     body text has no room to breathe on a phone. */
  @media (max-width: 700px) {
    .about-grid {
      grid-template-columns: 1fr;
    }
    .about-inline-photo {
      float: none;
      width: 100%;
      margin: 0 0 1rem 0;
    }
  }
</style>
