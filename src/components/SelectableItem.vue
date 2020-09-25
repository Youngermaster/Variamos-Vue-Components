<template>
  <div id="SelectableItem">
    <p align="center">{{ name }}</p>
    <!-- <img :src="url" alt="Arduino Uno image" width="50" /> -->
    <img
      v-bind:src="'https://cdn.pixabay.com/photo/2017/03/23/12/32/' + url"
      alt="Arduino Uno image"
      width="50"
    />
  </div>
</template>

<script>
export default {
  name: "SelectableItem",
  props: {
    name: String,
    url: String,
  },
};
</script>
