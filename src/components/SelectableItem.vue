<template>
  <div id="SelectableItem">
    <p align="center">{{ name }}</p>
    <img :src="url" alt="Arduino image" width="50" />
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
