<script>
import Accordion from "./components/Accordion.vue";

export default {
  components: {
    Accordion,
  },
  data() {
    return {
      accordionItems: [
        {
          id: 1,
          headingMessage: "Wanna see something cool?",
          bodyMessage: "something cool",
        },
        {
          id: 2,
          headingMessage: "Wanna see it again?",
          bodyMessage: "it again",
        },
        {
          id: 3,
          headingMessage: "Haha..",
          bodyMessage: "got ya",
        },
      ],
      accordionItems2: [
        {
          id: 1,
          headingMessage: "test 1",
          bodyMessage: "answer 1",
        },
        {
          id: 2,
          headingMessage: "test 2",
          bodyMessage: "answer 2",
        },
      ],
    };
  },
};
</script>

<template>
  <Accordion :accordionItems="accordionItems"></Accordion>
  <Accordion :accordionItems="accordionItems2"></Accordion>
</template>
