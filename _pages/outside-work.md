---
layout: page
title: outside work
permalink: /outside-work/
nav: true
---

<!-- Particles.js CDN -->
<script src="https://cdn.jsdelivr.net/particles.js/2.0.0/particles.min.js"></script>

<!-- Particles container -->
<div id="particles-js" style="position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1;"></div>

this is what i enjoy doing in my day to day!


## currently listening to - 
<iframe style="border-radius:12px" src="https://open.spotify.com/embed/playlist/5c371NuyisQkbKiIkadrri?utm_source=generator" width="100%" height="352" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>

## 📸 Photos
- Drop in some fun or memorable photos from travels, events, or daily life.


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
      value: 10,
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
</script>

