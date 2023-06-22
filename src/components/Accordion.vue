<script>
import AccordionItem from "./AccordionItem.vue";

export default {
  components: {
    AccordionItem,
  },
  props: ["accordionItems"],
  data() {
    return {};
  },
};
</script>

<template>
  <div class="accordion">
    <AccordionItem
      v-for="item in accordionItems"
      :key="item.id"
      :headingMessage="item.headingMessage"
      :bodyMessage="item.bodyMessage"
    ></AccordionItem>
  </div>
</template>
