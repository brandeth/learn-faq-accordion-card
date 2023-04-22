<script lang="ts" setup>
// define props in TypeScript

defineProps<{
  faq: {
    question: string;
    answer: string;
  };
}>();

const isActive = ref(false);

const toggleAccordion = () => {
  isActive.value = !isActive.value;
};
</script>

<template>
  <div @click="toggleAccordion" :class="{
    'is-open': isActive,
  }" class="FAQAccordionCard-item">
    <div class="FAQAccordionCard-accordionHeader">
      <h3>{{ faq.question }}</h3>
      <img class="FAQAccordionCard-icon" src="/icon-arrow-down.svg" alt="Arrow Down" />
    </div>
    <div class="FAQAccordionCard-accordionBody">
      <p>
        {{ faq.answer }}
      </p>
    </div>
  </div>
</template>
