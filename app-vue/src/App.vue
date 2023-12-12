<template>
  <div class="counter-app-container">
    <h1 class="counter-heading">Counter</h1>
    <h1 id="counter">{{ count }}</h1>
    <div class="button-container">
      <button id="decrease" aria-label="decrease button" @click="decreaseCount">
        {{ decrease }}
      </button>
      <button id="increase" aria-label="increase button" @click="increaseCount">
        {{ increase }}
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Vue Counter App",
  data() {
    return {
      count: 0,
      increase: "Increase Count",
      decrease: "Decrease Count",
    };
  },
  methods: {
    increaseCount() {
      this.count++;
    },
    decreaseCount() {
      this.count--;
    },
  },
};
</script>

<style>

</style>