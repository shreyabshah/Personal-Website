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
    font-size: 6rem;
    white-space: nowrap;
    clip-path: inset(0 100% 0 0);
    animation: reveal-handwriting 2s ease-out 0.3s forwards;
  }
  @keyframes reveal-handwriting {
    to { clip-path: inset(0 0% 0 0); }
  }
</style>

Hello, this is my site.
