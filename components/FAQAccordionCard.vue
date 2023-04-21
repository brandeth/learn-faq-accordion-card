<script lang="ts" setup>
interface FAQ {
  question: string;
  answer: string;
}

const faqs: FAQ[] = [
  {
    question: "How many team members can I invite?",
    answer:
      "You can invite up to 2 additional users on the Free plan. There is no limit on team members for the Premium plan.",
  },
  {
    question: "What is the maximum file upload size?",
    answer:
      "No more than 2GB. All files in your account must fit your allotted storage space.",
  },
  {
    question: "How do I reset my password?",
    answer:
      "Click “Forgot password” from the login page or “Change password” from your profile page. A reset link will be emailed to you.",
  },
  {
    question: "Can I cancel my subscription?",
    answer:
      "Yes! Send us a message and we’ll process your request no questions asked.",
  },
  {
    question: "Do you provide additional support?",
    answer:
      "Chat and email support is available 24/7. Phone lines are open during normal business hours.",
  },
];
</script>

<template>
  <div class="FAQAccordionCard">
    <div class="FAQAccordionCard-container">
      <div class="FAQAccordionCard-imageContainer">
        <img
          srcset="
            illustration-woman-online-mobile.svg   375w,
            illustration-woman-online-desktop.svg 1440w
          "
          sizes="(max-width: 600px) 100%,
         100%"
          src="elva-fairy-800w.jpg"
          alt="Woman Online"
        />
      </div>
      <div class="FAQAccordionCard-content">
        <div class="FAQAccordionCard-title">
          <h2>FAQ</h2>
        </div>
        <div class="FAQAccordionCard-accordion">
          <FAQAccordionItem
            v-for="faq in faqs"
            :key="faq.question"
            :faq="faq"
          />
        </div>
      </div>
    </div>
  </div>
</template>
