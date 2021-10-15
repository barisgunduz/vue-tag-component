<template>
    <div class="container">
      <app-tags v-model="tags" color="primary"></app-tags>
      {{tags}}
      <hr>
      <app-tags v-model="tags2" ></app-tags>
      {{tags2}}
      <hr>
    </div>
</template>

<script>
import Tags from "./components/Tags"
export default {
    components : {
      appTags : Tags
    },
    data(){
      return {
        tags: "deneme, test, barış",
        tags2: "deneme2, test2, barış2"
      }
    }
};
</script>

<style>
body {
    font-family: sans-serif;
}
</style>
