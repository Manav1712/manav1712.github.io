---
layout: page
title: outside work
permalink: /outside-work/
nav: true
---

<!-- Quick links -->
<div class="quick-links" style="margin: 0 0 1rem 0; font-size: 0.95rem;">
  <a href="#reading" style="margin-right: 1rem;">Reading</a>
  <a href="#listening" style="margin-right: 1rem;">Listening</a>
  <a href="#photos">Photos</a>
  
</div>

<style>
/* Scoped hover effects for outside-work page */
.quick-links a {
  position: relative;
  color: inherit;
  text-decoration: none;
  padding: 0.2rem 0.35rem;
  border-radius: 6px;
  transition: color 200ms ease, background-color 200ms ease, transform 200ms ease;
}
.quick-links a::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: -2px;
  width: 100%;
  height: 2px;
  background: linear-gradient(90deg,#FF6B6B,#4ECDC4,#45B7D1);
  transform: scaleX(0);
  transform-origin: left;
  transition: transform 250ms ease;
}
.quick-links a:hover {
  background: rgba(0,0,0,0.04);
  transform: translateY(-1px);
}
.quick-links a:hover::after {
  transform: scaleX(1);
}

#content-wrap figure img {
  border-radius: 12px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.06);
  transition: transform 250ms ease, box-shadow 250ms ease, filter 250ms ease;
}
#content-wrap figure:hover img {
  transform: scale(1.02);
  box-shadow: 0 12px 28px rgba(0,0,0,0.14);
  filter: saturate(1.05);
}

#content-wrap iframe {
  box-shadow: 0 6px 20px rgba(0,0,0,0.08);
  transition: transform 250ms ease, box-shadow 250ms ease, filter 250ms ease;
}
#content-wrap iframe:hover {
  transform: translateY(-2px);
  box-shadow: 0 12px 28px rgba(0,0,0,0.14);
}

@media (prefers-reduced-motion: reduce) {
  .quick-links a::after,
  #content-wrap figure img,
  #content-wrap iframe {
    transition: none !important;
  }
}
</style>

<!-- Particles.js CDN -->
<script src="https://cdn.jsdelivr.net/particles.js/2.0.0/particles.min.js"></script>

<!-- Particles container -->
<div id="particles-js" style="position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1;"></div>

<div id="content-wrap" style="max-width: 820px; margin: 0 auto; padding: 0 1rem;">

this is what i enjoy doing in my day to day!

## <span id="reading"></span> reading

- add your reading notes or a short list of favorites here

## <span id="listening"></span> listening

<iframe title="Spotify playlist" style="border-radius:12px" src="https://open.spotify.com/embed/playlist/5c371NuyisQkbKiIkadrri?utm_source=generator" width="100%" height="352" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>

## <span id="photos"></span> 📸 photos

{% include figure.liquid path="/assets/img/spotify.png" alt="A placeholder image" caption="Sample image caption" max-width="700px" %}

this page will keep growing as I find new things to share!

<div id="thanks-typing" style="font-family: 'Courier New', monospace; font-size: 20px; color: #333; margin: 30px 0; min-height: 40px; text-align: center; font-weight: bold;"></div>

<script>
// Thanks typing animation
const thanksTexts = [
  "Thanks for stopping by! 👾",
  "Hope you enjoyed your visit! ✨",
  "Come back soon! 🚀",
  "Have a great day! 🌟"
];

let thanksTextIndex = 0;
let thanksCharIndex = 0;
let thanksIsDeleting = false;

function thanksTypeWriter() {
  const currentText = thanksTexts[thanksTextIndex];
  const typingElement = document.getElementById('thanks-typing');
  
  if (thanksIsDeleting) {
    typingElement.textContent = currentText.substring(0, thanksCharIndex - 1);
    thanksCharIndex--;
  } else {
    typingElement.textContent = currentText.substring(0, thanksCharIndex + 1);
    thanksCharIndex++;
  }
  
  let typeSpeed = thanksIsDeleting ? 80 : 120;
  
  if (!thanksIsDeleting && thanksCharIndex === currentText.length) {
    typeSpeed = 3000; // Longer pause at end
    thanksIsDeleting = true;
  } else if (thanksIsDeleting && thanksCharIndex === 0) {
    thanksIsDeleting = false;
    thanksTextIndex = (thanksTextIndex + 1) % thanksTexts.length;
    typeSpeed = 800; // Pause before next word
  }
  
  setTimeout(thanksTypeWriter, typeSpeed);
}

// Start thanks typing animation when page loads
window.addEventListener('load', thanksTypeWriter);

// Particles.js Configuration - Nyan Cat Theme
function initParticles() {
  particlesJS('particles-js', {
  particles: {
    number: {
      value: 80,
      density: {
        enable: true,
        value_area: 800
      }
    },
    color: {
      value: ['#FF6B6B', '#4ECDC4', '#45B7D1', '#96CEB4', '#FFEAA7', '#DDA0DD', '#98D8C8']
    },
    shape: {
      type: 'circle',
      stroke: {
        width: 0,
        color: '#000000'
      }
    },
    opacity: {
      value: 0.5,
      random: false,
      anim: {
        enable: false,
        speed: 1,
        opacity_min: 0.1,
        sync: false
      }
    },
    size: {
      value: 3,
      random: true,
      anim: {
        enable: false,
        speed: 40,
        size_min: 0.1,
        sync: false
      }
    },
    line_linked: {
      enable: true,
      distance: 150,
      color: '#FF6B6B',
      opacity: 0.4,
      width: 1
    },
    move: {
      enable: true,
      speed: 6,
      direction: 'none',
      random: false,
      straight: false,
      out_mode: 'out',
      bounce: false,
      attract: {
        enable: false,
        rotateX: 600,
        rotateY: 1200
      }
    }
  },
  interactivity: {
    detect_on: 'canvas',
    events: {
      onhover: {
        enable: true,
        mode: 'repulse'
      },
      onclick: {
        enable: true,
        mode: 'push'
      },
      resize: true
    },
    modes: {
      grab: {
        distance: 400,
        line_linked: {
          opacity: 1
        }
      },
      bubble: {
        distance: 400,
        size: 40,
        duration: 2,
        opacity: 8,
        speed: 3
      },
      repulse: {
        distance: 200,
        duration: 0.4
      },
      push: {
        particles_nb: 4
      },
      remove: {
        particles_nb: 2
      }
    }
  },
  retina_detect: true
  });
}

const prefersReducedMotion = window.matchMedia('(prefers-reduced-motion: reduce)');

function shouldDisableParticles() {
  return prefersReducedMotion.matches || window.innerWidth < 768;
}

function maybeStartOrStopParticles() {
  const canvas = document.querySelector('#particles-js canvas');
  if (shouldDisableParticles()) {
    if (window.pJSDom && window.pJSDom.length) {
      window.pJSDom.forEach((p) => p.pJS && p.pJS.fn.vendors.destroypJS());
      window.pJSDom = [];
    }
    if (canvas) canvas.remove();
  } else if (!window.pJSDom || !window.pJSDom.length) {
    initParticles();
  }
}

window.addEventListener('load', maybeStartOrStopParticles);
window.addEventListener('resize', maybeStartOrStopParticles);
prefersReducedMotion.addEventListener('change', maybeStartOrStopParticles);
</script>

</div>
