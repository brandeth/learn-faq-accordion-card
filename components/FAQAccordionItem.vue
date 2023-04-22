<script lang="ts" setup>
// define props in TypeScript

defineProps<{
  faq: {
    question: string;
    answer: string;
  };
}>();
</script>

<template>
  <div class="FAQAccordionCard-item">
    <div class="FAQAccordionCard-accordionHeader">
      <h3>{{ faq.question }}</h3>
      <img src="/icon-arrow-down.svg" alt="Arrow Down" />
    </div>
    <div class="FAQAccordionCard-accordionBody">
      <p>
        {{ faq.answer }}
      </p>
    </div>
  </div>
</template>
