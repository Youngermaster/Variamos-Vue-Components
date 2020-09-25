<template>
  <div id="SelectableItem">
    <p align="center">{{ name }}</p>
    <img :src="url" alt="Arduino image" :width="imgWidth" />
  </div>
</template>

<script>
export default {
  name: "SelectableItem",
  props: {
    name: String,
    url: String,
    imgWidth: Number,
  },
};
</script>
