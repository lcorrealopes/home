---
layout: homepage
title: Miscellanea
---

## Miscellanea

## Nice places around the world (and a little bit of history)

<div style="margin-bottom: 50px;" markdown="1">

<img src="assets/historia/duomo.jpg" 
       alt="Duomo di Milano" 
       data-src="assets/historia/duomo.jpg" 
       data-caption="Duomo di Milano" 
       onclick="openLightbox(this)" 
       style="width: 100%; max-width: 800px; height: auto; border-radius: 12px; cursor: pointer; margin-bottom: 15px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">

  **Duomo di Milano:** The construction of the Duomo di Milano began around 1380. Built almost entirely of pink-veined Candoglia marble, it took nearly six centuries to complete. This is the largest church in Italy (and Italy really has a lot of churches), except for the Vatican. In the neighborhood of the Duomo you will find a lot of quite expensive coffee shops and souvenirs (you can also find the most expensive Aperol Spritz of your life in case you drink alcohol).

</div>

<div style="margin-bottom: 50px;" markdown="1">

<div style="display: flex; gap: 15px; margin-bottom: 15px;">
    
<img src="assets/historia/sforzesco.jpg" 
         alt="Castello Sforzesco" 
         data-src="assets/historia/sforzesco.jpg" 
         data-caption="Castello Sforzesco" 
         onclick="openLightbox(this)" 
         style="flex: 1; width: 100%; height: 250px; object-fit: cover; border-radius: 12px; cursor: pointer; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">

<img src="assets/historia/michelangelolast.jpg" 
         alt="Rondanini Pietà" 
         data-src="assets/historia/michelangelolast.jpg" 
         data-caption="Rondanini Pietà" 
         onclick="openLightbox(this)" 
         style="flex: 1; width: 100%; height: 250px; object-fit: cover; border-radius: 12px; cursor: pointer; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">

</div>

  **Castello Sforzesco:**  The Castello Sforzesco in Milan was built way back in the 1400s by Francesco Sforza. Inside you will find Michelangelo's final unfinished work, the Rondanini Pietà (probably the castle's most famous piece). He kept chiselling away at this Virgin mourning Christ right up until a few days before he died in 1564. Honestly, it's totally worth a visit, just 5 euros and you get to see a ton of different art (seriously, trust me).

</div>

<div style="margin-bottom: 50px;" markdown="1">

<img src="assets/historia/bernina.jpeg" 
       alt="Bernina Express train" 
       data-src="assets/historia/bernina.jpeg" 
       data-caption="Bernina Express train" 
       onclick="openLightbox(this)" 
       style="width: 100%; max-width: 800px; height: auto; border-radius: 12px; cursor: pointer; margin-bottom: 15px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">

  **Bernina Express train:** I must start by saying that this is not the Hogwarts train. The Bernina Express will give you a chill ride through the Swiss Alps. You will have an insanely beautiful view. Ah, and it’s a UNESCO World Heritage Site. It’s not the cheapest trip but you should grab a window seat and just enjoy the views.

</div>

<div style="margin-bottom: 50px;" markdown="1">

<img src="assets/historia/operaviena.jpg" 
       alt="Wiener Staatsoper" 
       data-src="assets/historia/operaviena.jpg" 
       data-caption="Wiener Staatsoper" 
       onclick="openLightbox(this)" 
       style="width: 100%; max-width: 800px; height: auto; border-radius: 12px; cursor: pointer; margin-bottom: 15px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">

 **Wiener Staatsoper:** One of the world’s most famous opera houses, set in a very beautiful building (this pic was taken from a little raised square right near the opera, keep that tip). If you don’t want to shell out a ton or couldn’t preorder a seat, head to the side of the building where you can grab way cheaper standing-room tickets and watch the whole thing on your feet.

</div>

<!-- ========================================== -->
<!-- ESTRUTURA DO LIGHTBOX -->
<!-- ========================================== -->
<div id="gallery-lightbox" class="lightbox" onclick="closeLightbox()">
  <span class="lightbox-close">&times;</span>
  <img class="lightbox-content" id="lightbox-img" onclick="event.stopPropagation()">
  <div id="lightbox-caption" class="lightbox-caption" onclick="event.stopPropagation()"></div>
</div>

<script>
function openLightbox(element) {
  const imgUrl = element.getAttribute('data-src');
  const captionHtmlFull = element.getAttribute('data-caption') || ''; 
  
  document.getElementById('lightbox-img').src = imgUrl;
  document.getElementById('lightbox-caption').innerHTML = captionHtmlFull;
  
  document.getElementById('gallery-lightbox').style.display = 'flex';
  document.body.style.overflow = 'hidden'; 
}

function closeLightbox() {
  document.getElementById('gallery-lightbox').style.display = 'none';
  document.body.style.overflow = 'auto'; 
}

document.addEventListener('keydown', function(e) {
  if (e.key === 'Escape') {
    closeLightbox();
  }
});
</script>
