---
toc: True
layout: post
title: Key Accomplishments List
description: A blog showing all of the things I've done in this class (CSSE 1) that I'm proud of.
author: Flora Segale
permalink: /key-accomplishments-list
kite-one: true
---

This trimester wasn’t just about coding.  
It was about learning how to think like an engineer, how to stay calm in the middle of code chaos, and how to find joy in the little things — even if it means there’s just one less error in an ocean.

---

## 1. Debugging 🥲

***This*** is the reason I have a combined total of… <mark class="hl">4 days, 17 hours, 35 minutes</mark> (or 117 hours and 35 minutes) on VSCode since the start of trimester 2 (from 11/25/25 to 2/10/26). Debugging took up most of my time, and it was a rollercoaster of emotions. I had moments where I felt like I was making progress, only to be hit with another error that sent me back to square one. This took years off of my life, but it taught me resilience and problem-solving skills, and lengthened my patience and attention span by a lot.

- My Makefile wouldn’t run (MULTIPLE TIMES)
- On several occasions, random notebooks were pointing to nowhere and killed the terminal when I tried to run them
- My deployment pipeline was sending my site to the wrong URL  
- The site WOULD. NOT. DEPLOY.  
- And every time I thought I had fixed it, something else would break. It was like playing whack-a-mole with bugs.

But instead of giving up, I learned how to trace problems back to their roots. I realized that the error messages conveniently stated what the problem was, so with the help of Copilot, I started reading the error messages and working backwards — peeling back each layer of the onion until I got to where I needed to be.

And when it finally worked, it felt like a boss battle victory. (Like the epic one I *thought* we could create for N@M)

---

## 2. Rebuilding My Workflow

Near the halfway point of CSSE 1, I was creating a new repository, and I realized my virtual environment was a half-fetched mess — and that didn’t sit right with me. So I took it apart and built it back up again. I…

- Cleaned up all of the files and directories in my repo (I learned lot of wsl terminal commands)
- Normalized ALL of my notebooks (it took way longer than intended)
- Re-initialized Git so it finally reflected *my* work and not someone else’s (my initialization was of the wrong directory, so I had to work backwards to change the ownership of the files)
- Figured out why my terminal was pulling the wrong modules  
- Finally got “make” to run (and felt invincible) [Until it broke again]

It was like doing a full system reset on myself!

### Click the arrows below to scroll through some of the screenshots of the errors I encountered during this process!
(I wish I had taken more screenshots, but I was too busy trying to fix the errors to remember to take them)

<!-- markdownlint-disable MD033 MD013 -->
<style>
/* Simple horizontal carousel: scrollable, snap, and arrow buttons */
.carousel-wrapper { position: relative; }
.image-gallery {
  display: flex;
  align-items: center;
  gap: 12px;
  overflow-x: auto;
  scroll-snap-type: x mandatory;
  -webkit-overflow-scrolling: touch;
  padding: 8px 4px;
}
.image-gallery img {
  /* show full image without cropping */
  height: auto;
  max-height: 200px;
  width: auto;
  max-width: 90%;
  flex: 0 0 auto;
  border-radius: 10px;
  scroll-snap-align: start;
  object-fit: contain;
}
.image-gallery::-webkit-scrollbar { height: 10px; }
.carousel-btn {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  background: rgba(0,0,0,0.45);
  color: #fff;
  border: none;
  width: 36px;
  height: 36px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 50%;
  cursor: pointer;
}
.carousel-btn.left { left: 8px; }
.carousel-btn.right { right: 8px; }
.carousel-btn:focus { outline: 2px solid rgba(255,255,255,0.8); }
</style>

<div class="carousel-wrapper">
  <button class="carousel-btn left" aria-label="Scroll left">◑</button>
  <div class="image-gallery" id="imageGallery">
    <img src="{{site.baseurl}}/images/FINAL/convert-notebook.png" alt="Convert notebook screenshot">
    <img src="{{site.baseurl}}/images/FINAL/required-file-not-found.png" alt="Required file not found screenshot">
    <img src="{{site.baseurl}}/images/FINAL/unable-to-locate-python.png" alt="Unable to locate python screenshot">
    <img src="{{site.baseurl}}/images/FINAL/create-fork.png" alt="permission to create fork screenshot">
  </div>
  <button class="carousel-btn right" aria-label="Scroll right">◐</button>
</div>

<script>
/* Small helper: buttons scroll the gallery by ~70% of its width */
(function(){
  var gallery = document.getElementById('imageGallery');
  if(!gallery) return;
  var left = gallery.parentElement.querySelector('.carousel-btn.left');
  var right = gallery.parentElement.querySelector('.carousel-btn.right');
  function scrollAmount() { return Math.round(gallery.offsetWidth * 0.7); }
  left && left.addEventListener('click', function(){ gallery.scrollBy({ left: -scrollAmount(), behavior: 'smooth' }); });
  right && right.addEventListener('click', function(){ gallery.scrollBy({ left: scrollAmount(), behavior: 'smooth' }); });
})();
</script>
<!-- markdownlint-enable MD033 MD013 -->
---

## 3. Deploying My Site

I didn’t just write blogs — I learned how to manually publish them. I dug into how Jekyll builds my site, how GitHub Actions deploys it, and how to troubleshoot when things go wrong. I learned:

- How to read the GitHub Actions logs (and why they were yelling at me)  
- Why my site was publishing to the wrong URL  
- How to change the YAML file to ***fix*** the URL (AND WHY I NEEDED TO DO THAT)
- And most importantly: how to keep my cool when the site wouldn’t load

It was the first time I felt like I understood the *whole* pipeline — not just the parts I could see. I read every line of code in several files until I understood what part of the code was giving me errors.

---

## 4. Getting the Class to Night at the Museum

During the game-building unit, I found strength in myself by slowly stepping into a leadership role. I love to organize, and this role gave me a lot of opportunities.

I made:

- A base *[level requirements](https://docs.google.com/document/d/1qnGFbed-_j16Z0g5eUKDnKD-Fy6SLytzvBmvFRa2v8A/edit?tab=t.0#heading=h.sbpg7njbydck)* template  
- A clear system for level design  
- A workflow that made our project feel more like a team effort and less like a group chat (because the group chat method [slack] proved useless)

It was the first time I saw my organization skills turn into something that helped other people, not just me. Richab, Chet, and I worked tirelessly to float around the room, helping everyone stay on track and making sure we were all on the same page. It was a lot of work, but it was also rewarding to see our project come together - even if the N@M game didn’t turn out the way we wanted it to.

<!-- markdownlint-disable MD033 MD013 -->
<style>
/* Simple horizontal carousel (second instance): show full images */
.carousel-wrapper { position: relative; }
.image-gallery {
  display: flex;
  align-items: center;
  gap: 12px;
  overflow-x: auto;
  scroll-snap-type: x mandatory;
  -webkit-overflow-scrolling: touch;
  padding: 8px 4px;
}
.image-gallery img {
  /* show full image without cropping */
  height: auto;
  max-height: 200px;
  width: auto;
  max-width: 90%;
  flex: 0 0 auto;
  border-radius: 10px;
  scroll-snap-align: start;
  object-fit: contain;
}
.image-gallery::-webkit-scrollbar { height: 10px; }
.carousel-btn {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  background: rgba(0,0,0,0.45);
  color: #fff;
  border: none;
  width: 36px;
  height: 36px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 50%;
  cursor: pointer;
}
.carousel-btn.left { left: 8px; }
.carousel-btn.right { right: 8px; }
.carousel-btn:focus { outline: 2px solid rgba(255,255,255,0.8); }
</style>

<div class="carousel-wrapper">
  <button class="carousel-btn left" aria-label="Scroll left">◀</button>
  <div class="image-gallery" id="imageGallery2">
    <img src="{{site.baseurl}}/images/FINAL/theme-poll.png" alt="screenshot of the poll we made to decide on a theme for our game">
    <img src="{{site.baseurl}}/images/FINAL/level-base.png" alt="screenshot of the level base template I made for our game">
  </div>
  <button class="carousel-btn right" aria-label="Scroll right">▶</button>
</div>

<script>
/* Small helper: buttons scroll the gallery by ~70% of its width (second instance) */
(function(){
  var gallery = document.getElementById('imageGallery2');
  if(!gallery) return;
  var left = gallery.parentElement.querySelector('.carousel-btn.left');
  var right = gallery.parentElement.querySelector('.carousel-btn.right');
  function scrollAmount() { return Math.round(gallery.offsetWidth * 0.7); }
  left && left.addEventListener('click', function(){ gallery.scrollBy({ left: -scrollAmount(), behavior: 'smooth' }); });
  right && right.addEventListener('click', function(){ gallery.scrollBy({ left: scrollAmount(), behavior: 'smooth' }); });
})();
</script>
<!-- markdownlint-enable MD033 MD013 -->
---
