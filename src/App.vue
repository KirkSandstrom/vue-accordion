<script>
import AccordionItem from "./components/AccordionItem.vue";

export default {
  components: {
    AccordionItem,
  },
  data() {
    return {
      message: "Hello world!",
    };
  },
};
</script>

<template>
  <h1>{{ message }}</h1>
  <div class="accordion">
    <AccordionItem></AccordionItem>
  </div>
</template>
