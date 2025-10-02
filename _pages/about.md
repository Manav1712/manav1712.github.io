---
layout: about
title: about
permalink: /
profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>9500 Gilman Dr</p>
    <p>La Jolla, CA 92092</p>

news: true # includes a list of news items
social: false # includes social icons at the bottom of the page
---

<span id="typing-text" style="font-family: 'Fira Mono', 'Menlo', 'Monaco', 'Consolas', monospace; font-size: 2rem;"></span>

I recently completed my bachelor’s degree in Data Science at [UC San Diego](https://datascience.ucsd.edu/), where I worked with the [Rose Lab](https://roseyu.com/) on deploying epidemic simulators and AI models to production using FastAPI and GCP. I also spent time at [Princeton Research Computing](https://researchcomputing.princeton.edu/), where I contributed to algorithmic solvers for scientific research under Professor [Bartolomeo Stellato](https://stellato.io/). Currently, I'm working at [MathGPT.ai](https://mathgpt.ai/)!

My research interests lie at the intersection of **machine learning**, **operations research**, and **personalized decision-making systems**, with applications in **healthcare**, **finance**, and **policy**. I'm particularly excited about problems involving uncertainty, optimization, and human-AI interaction.

Recently, I completed a paper on Paid Family Leave and the gender wage gap, advised by Prof. Gordon B. Dahl, reflecting my growing interest in econometrics and data-driven policy research.

I’ve also held roles in applied ML and software engineering at NanoMood, Intellect Design Arena, and Chapter Apps, where I worked on everything from clinical knowledge graphs to LLM applications and front-end infrastructure.


Outside of work, I enjoy playing poker, long-distance running, and music festivals. I’m always on the lookout for interesting playlists—feel free to share yours on Spotify.

<script>
document.addEventListener('DOMContentLoaded', function() {
    const text = "Welcome!";
    const element = document.getElementById('typing-text');
    let index = 0;
    function typeWriter() {
        if (index < text.length) {
            element.innerHTML += text.charAt(index);
            index++;
            setTimeout(typeWriter, 100);
        }
    }
    typeWriter();
});
</script>