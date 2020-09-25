<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Item selector Variamos" />

    <div class="container">
      <div class="row">
        <div class="col">1 of 3</div>
        <div class="col-2">2 of 3 (wider)</div>
        <div class="col">3 of 3</div>
      </div>
      <div class="row">
        <div class="col">1 of 3</div>
        <div class="col-5">
          <div class="container">
            <div class="row">
              <div class="col">1 of 3</div>
              <div class="col-5">2 of 3 (wider)</div>
              <div class="col">3 of 3</div>
            </div>
            <div class="row">
              <div class="col">1 of 3</div>
              <div class="col-5">2 of 3 (wider)</div>
              <div class="col">3 of 3</div>
            </div>
          </div>
        </div>

        <!-- <div class="col">
          <SelectableItem :name="item.name" :url="item.url" />
        </div>

        <div class="col">
          <SelectableItem :name="item.name" :url="item.url" />
        </div> -->

        <div class="col">
          <div class="row">
            <div class="col-6">
              <SelectableItem :name="item.name" :url="item.url" />
            </div>
            <div class="col-6">
              <SelectableItem :name="item.name" :url="item.url" />
            </div>
            <div class="col-6">
              <SelectableItem :name="SecondItem.name" :url="SecondItem.url" />
            </div>
            <div class="col-6">
              <SelectableItem :name="SecondItem.name" :url="SecondItem.url" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import SelectableItem from "./components/SelectableItem.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    SelectableItem,
  },
  data() {
    return {
      item: {
        name: "Arduino UNO",
        url:
          "https://cdn.pixabay.com/photo/2017/03/23/12/32/arduino-2168193_1280.png",
      },
      SecondItem: {
        name: "Arduino MEGA",
        url:
          "https://www.pngkey.com/png/full/207-2079814_bustedtheory-servo-motor-arduino-mega.png",
      },
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.row div {
  border: 1px solid #34495e;
  background-color: #41b883;
}
</style>
