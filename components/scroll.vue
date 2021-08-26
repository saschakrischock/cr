
<template>
<div class="all">
<div class="logo">Logo</div>

<div class="text">
  <p class="trigger-logo">Campbell-Rey is an award-winning design studio founded by Duncan Campbell and Charlotte Rey.</p>

<p class="trigger-one">Working fluently between residential and commercial interior design, furniture and product design, their world is a celebration of conviviality, colour and exceptional craftsmanship.</p>

<p>With a love of historical architecture, traditional decorative techniques and an ability to create surprising dialogues between styles, periods and objects, their work is imbued with a playful, irreverent spirit and a desire to make magic.</p>

<p class="trigger-two">To see a selection of their interiors, objects and inspiration, find Campbell-Rey on Instagram</p>

<p>Campbell-Rey’s furniture is sold exclusively through 
The Invisible Collection, and their glassware and home accessories can be found on Matches Fashion, Svenskt Tenn and 1stDibs</p>

  <p>If you would like to discuss a commission or request a portfolio, please get in touch</p>
</div>

<div class="image background-image__one">
    <nuxt-img
    provider="static"
    src="/1.jpg"
  />
</div>

<div class="image background-image__two">
     <nuxt-img
    provider="static"
    src="/2.jpg"
  
  />
</div>

<div class="image background-image__three">
    <nuxt-img
    provider="static"
    src="/3.jpg"
    
  />
</div>
</div>
</template>




<style lang="scss">
.text {
  width: calc(68vw - 1rem);
  margin-left: 32vw;
  z-index: 100;
  position: relative;
  
  p {
    color: #fff;
    font-size: 5vw;
    font-family: serif;
    line-height: 4.8vw;
  }
}

.image {
  position: fixed;
  width: 100vw;
  height: 100vh;
  top:0;
  z-index: -1;
  left: 0;
  
  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
}

.background-image {
  &__one {
    z-index: 1;
  }
  &__two {
    z-index: 2;
        opacity:0;
  }
  &__three {
    opacity:0;
      z-index: 3;
  }
}

.logo {
  position: fixed;
  top: 0;
  left: 0;
  z-index: 100;
  font-size: 8vw;
  color: #fff;
  padding: 1rem;
  transform-origin: 0 0;
}

.trigger-logo {
  margin-top: 0;
  padding-top: 5rem;
}
</style>

