---
layout: page
title: outside work
permalink: /outside-work/
nav: true
---

this is what i enjoy doing outside work!


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
</script>

