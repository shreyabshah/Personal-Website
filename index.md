<div class="curtain-overlay">
  <div class="curtain-panel curtain-left"></div>
  <div class="curtain-panel curtain-right"></div>
  <h1 class="curtain-text">Welcome to Shreya's Website</h1>
</div>

<style>
  /* Fixed = stays pinned to the screen regardless of scroll,
     inset:0 is shorthand for top/right/bottom/left all 0, so this
     covers the entire viewport. z-index:999 puts it above
     everything else on the page. */
  .curtain-overlay {
    position: fixed;
    inset: 0;
    z-index: 999;
    display: flex;
    align-items: center;
    justify-content: center;
    pointer-events: none;
  }

  /* Each panel is half the screen, dark red, sitting side by side
     to fully cover the screen at the start. */
  .curtain-panel {
    position: absolute;
    top: 0;
    height: 100%;
    width: 50%;
    background: linear-gradient(90deg, #4a0000, #8b0000, #4a0000);
  }
  .curtain-left { left: 0; }
  .curtain-right { right: 0; }

  /* "animation-delay: 2.5s" means these don't start moving until
     2.5s in, giving the typewriter text time to finish first.
     "forwards" means the panel stays at its end position (fully
     off-screen) instead of snapping back once the animation ends. */
  .curtain-left  { animation: slide-left  1.5s ease-in-out 2.5s forwards; }
  .curtain-right { animation: slide-right 1.5s ease-in-out 2.5s forwards; }
  @keyframes slide-left  { to { transform: translateX(-100%); } }
  @keyframes slide-right { to { transform: translateX(100%);  } }

  /* The typewriter trick: the full text is already in the HTML.
     "overflow: hidden" + "width: 0" hides all of it. Animating
     width from 0 up to the text's full width, using "steps(27)"
     instead of a smooth transition, reveals it in 27 discrete
     jumps, one per character, which is what reads as "typing"
     rather than a smooth wipe. 27 is the character count of
     "Welcome to Shreya's Website" — if you change the text, this
     number and the "27ch" below both need to match the new length. */
  .curtain-text {
    position: relative;
    color: #f5e6c8;
    font-family: Georgia, serif;
    font-size: 2.5rem;
    white-space: nowrap;
    overflow: hidden;
    width: 0;
    border-right: 2px solid #f5e6c8;
    animation:
      typing 2s steps(27) forwards,
      blink-cursor 0.6s step-end infinite;
  }
  @keyframes typing { to { width: 27ch; } }
  @keyframes blink-cursor { 50% { border-color: transparent; } }
</style>

---
layout: default
title: Home
---
Hello, this is my site.
