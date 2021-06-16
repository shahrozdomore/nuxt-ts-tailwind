<template>
  <div class="bg-red-200">
    <h1>Counter : {{ count }}</h1>
    <button @click="increment()" class="mr-5 px-6 bg-gray-200">+</button>
    <button @click="decrement()" class="ml-5 px-6 bg-gray-200">-</button>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "nuxt-property-decorator";

@Component({})
export default class Counter extends Vue {
  // Local state
  count: number = 0;

  // Methods
  increment(): void {
    this.count++;
  }
  decrement(): void {
    this.count--;
  }
}
</script>

<style scoped lang="scss"></style>
