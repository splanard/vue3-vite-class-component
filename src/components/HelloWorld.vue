<template>
  <main>
    <h1>{{ message }}</h1>
  </main>
</template>

<script lang="ts">
import Vue from "vue-class-component";

export default class HomePage extends Vue {
  message = "Hello world!";
}
</script>
