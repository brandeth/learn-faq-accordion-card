<template>
  <div class="FAQAccordionCard-imageContainer">
    <div class="WomanAndBox-container">
      <img
        srcset="
          illustration-woman-online-mobile.svg  278w,
          illustration-woman-online-desktop.svg 472w
        "
        sizes="(max-width: 768px) 278px,
             472px"
        src="illustration-woman-online-desktop.svg"
        alt="Woman Online"
        class="Image-womanOnline"
      />
      <img class="Image-box" src="illustration-box-desktop.svg" alt="Box" />
    </div>
    <div class="Pattern-container">
      <img
        class="Image-pattern"
        srcset="bg-pattern-mobile.svg 240w, bg-pattern-desktop.svg 966w"
        sizes="(max-width: 768px) 240px,
             966px"
        src="bg-pattern-mobile.svg"
        alt="Pattern"
      />
    </div>
  </div>
</template>
