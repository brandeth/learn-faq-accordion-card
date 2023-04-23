<script lang="ts" setup>
defineProps<{
  faqs: {
    question: string;
    answer: string;
  }[];
}>();
</script>

<template>
  <div class="FAQAccordionCard-content">
    <div class="FAQAccordionCard-title">
      <h2>FAQ</h2>
    </div>
    <div class="FAQAccordionCard-accordion">
      <FAQAccordionItem v-for="faq in faqs" :key="faq.question" :faq="faq" />
    </div>
  </div>
</template>
