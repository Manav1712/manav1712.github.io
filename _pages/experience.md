---
layout: page
title: experience
permalink: /experience/
nav: true
---

Over the past few years, I’ve bounced between labs, startups, and dev teams — writing code, shipping features, and learning *a ton*. For more information about my internships, check out my cv!

* At **Rose Lab @ UCSD**, I wrangled epidemic simulations, built a FastAPI service, and got dangerously good at debugging GCP configs.
* **Princeton's Research Computing** taught me how to write clean, scalable code that actually gets used (yes, those Jupyter tutorials are official now!).
* At **NanoMood**, I dove deep into ML ops — designing pipelines, deploying on the cloud, and visualizing healthcare data with knowledge graphs.
* At **Intellect Design**, I turned GPT-3.5 into a résumé reviewer — learned prompt engineering *and* how to handle 1K+ users without breaking a sweat.
* And at **Chapter Apps**, I cut my front-end teeth on Angular + Tailwind, cleaned up onboarding flows, and made sure everything looked good while loading faster.

p.s I made sure I got the best possible coffee at every location

---

<div style="text-align: center; margin-top: 40px; padding: 20px;">
  <div style="display: flex; justify-content: center; align-items: center; gap: 40px; flex-wrap: wrap;">
    <div style="text-align: center;">
      <img src="{{ site.baseurl }}/assets/img/princeton-logo.png" 
           alt="Princeton University Logo" 
           class="logo-hover" 
           style="height: 60px; width: auto; max-width: 120px; border-radius: 12px; transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275); filter: drop-shadow(0 2px 4px rgba(0,0,0,0.1)); cursor: pointer;">
    </div>
    
    <div style="text-align: center;">
      <img src="{{ site.baseurl }}/assets/img/ucsd-logo.png" 
           alt="UC San Diego Logo" 
           class="logo-hover" 
           style="height: 60px; width: auto; max-width: 120px; border-radius: 12px; transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275); filter: drop-shadow(0 2px 4px rgba(0,0,0,0.1)); cursor: pointer;">
    </div>
    
    <div style="text-align: center;">
      <img src="{{ site.baseurl }}/assets/img/nanomood_logo.png" 
           alt="NanoMood Logo" 
           class="logo-hover" 
           style="height: 60px; width: auto; max-width: 120px; border-radius: 12px; transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275); filter: drop-shadow(0 2px 4px rgba(0,0,0,0.1)); cursor: pointer;">
    </div>
    
    <div style="text-align: center;">
      <img src="{{ site.baseurl }}/assets/img/intellect-logo.png" 
           alt="Intellect Design Logo" 
           class="logo-hover" 
           style="height: 60px; width: auto; max-width: 120px; border-radius: 12px; transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275); filter: drop-shadow(0 2px 4px rgba(0,0,0,0.1)); cursor: pointer;">
    </div>
    
    <div style="text-align: center;">
      <img src="{{ site.baseurl }}/assets/img/chapter-logo.png" 
           alt="Chapter Apps Logo" 
           class="logo-hover" 
           style="height: 60px; width: auto; max-width: 120px; border-radius: 12px; transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275); filter: drop-shadow(0 2px 4px rgba(0,0,0,0.1)); cursor: pointer;">
    </div>
  </div>
</div>

<style>
.logo-hover {
  position: relative;
  overflow: hidden;
}

.logo-hover::before {
  content: '';
  position: absolute;
  top: 0;
  left: -100%;
  width: 100%;
  height: 100%;
  background: linear-gradient(90deg, transparent, rgba(255,255,255,0.4), transparent);
  transition: left 0.5s;
}

.logo-hover:hover {
  transform: scale(1.1) rotate(2deg);
  filter: drop-shadow(0 8px 16px rgba(0,0,0,0.2)) brightness(1.1);
  box-shadow: 0 8px 25px rgba(0,0,0,0.15);
}

.logo-hover:hover::before {
  left: 100%;
}

.logo-hover:active {
  transform: scale(1.05) rotate(1deg);
  transition: all 0.1s ease;
}
</style>

