<script>
export default {
  data() {
    return {
      headingMessage: "Click this to see something cool",
      bodyMessage: "Something cool",
      bodyDisplayed: false,
    };
  },
  methods: {
    toggleBodyDisplay() {
      this.bodyDisplayed
        ? (this.bodyDisplayed = false)
        : (this.bodyDisplayed = true);
    },
  },
};
</script>

<template>
  <div class="accordion__heading" @click="toggleBodyDisplay">
    <h2>{{ headingMessage }}</h2>
  </div>
  <Transition name="accordion-body-slide">
    <div v-show="bodyDisplayed" class="accordion__body">
      <p>{{ bodyMessage }}</p>
    </div>
  </Transition>
</template>
