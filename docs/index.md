# Welcome to the Jujutsu Shenanigans Wiki
---

The ultimate wiki dedicated to the Roblox battlegrounds game, **[Jujutsu Shenanigans](https://www.roblox.com/games/9391468976/Jujutsu-Shenanigans)**, developed by **[Tze](https://www.patreon.com/MaybeTze)**.


<div class="wiki-carousel">
  <div class="carousel-slides">
    <img src="assets/banner1.png" class="slide active">
    <img src="assets/banner2.png" class="slide">
    <img src="assets/banner3.png" class="slide">
    <img src="assets/banner4.png" class="slide">
  </div>
  
  <button class="prev" onclick="changeSlide(-1)">&#10094;</button>
  <button class="next" onclick="changeSlide(1)">&#10095;</button>
</div>

<style>
.wiki-carousel {
  position: relative;
  width: 100%;
  max-width: 800px;
  margin: auto;
  overflow: hidden;
  border-radius: 10px;
  box-shadow: 0 4px 15px rgba(0,0,0,0.3);
}

.carousel-slides .slide {
  display: none;
  width: 100%;
  transition: opacity 0.5s ease-in-out; /* Quick transition */
}

.carousel-slides .active {
  display: block;
}

.prev, .next {
  cursor: pointer;
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  width: auto;
  padding: 16px;
  color: white;
  font-weight: bold;
  font-size: 20px;
  border: none;
  background: rgba(0,0,0,0.3);
  user-select: none;
  transition: 0.3s;
  z-index: 2;
}

.prev { 
  left: 0; 
  border-radius: 0 3px 3px 0; 
}

.next { 
  right: 0; 
  border-radius: 3px 0 0 3px; 
}

.prev:hover, .next:hover { 
  background: rgba(0,0,0,0.8); 
}
</style>

<script>
let slideIndex = 0;
let timer = setInterval(() => changeSlide(1), 7000); // 7 seconds wait

function changeSlide(n) {
  const slides = document.getElementsByClassName("slide");
  slides[slideIndex].classList.remove("active");
  
  slideIndex = (slideIndex + n + slides.length) % slides.length;
  
  slides[slideIndex].classList.add("active");
  
  clearInterval(timer);
  timer = setInterval(() => changeSlide(1), 7000);
}
</script>

---

<div style="
    border: 3px solid black; 
    padding: 10px; 
    margin-bottom: 20px; 
    box-shadow: 5px 5px 0px rgba(0,0,0,0.2); 
    text-align: center;
    font-family: 'Patrick Hand', cursive;
    font-size: 24px;
    font-weight: bold;">
    Navigation
</div>

| [![Chars](assets/heian.webp)](./characters.md) | [![Logs](assets/gambler_ult_icon.webp)](./update-logs.md) | [![Controls](assets/perfect_icon.webp)](./game-controls.md) | [![Discord](assets/discord_icon.webp)](https://discord.com/invite/bKaUchYTZK) |
| :---: | :---: | :---: | :---: |
| **Game Characters** | **Update Logs** | **Game Controls** | **Official Discord** |
