<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Item selector Variamos" />

    <AccountInfo :username="user.username" />

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

        <div class="col">
          <p align="center">Arduino UNO</p>
          <img
            src="./assets/arduino-uno.png"
            alt="Arduino Uno image"
            width="50"
          />
        </div>

        <div class="col">
          <div class="row">
            <div class="col-6">
              <SelectableItem :name="item.name" :url="item.url" />
            </div>
            <div class="col-6">
              <p align="center">Arduino MEGA</p>
              <img
                src="./assets/arduino-uno.png"
                alt="Arduino Uno image"
                width="50"
              />
            </div>
          </div>
        </div>
      </div>
      <p>Test</p>
    </div>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import AccountInfo from "./components/AccountInfo.vue";
import SelectableItem from "./components/SelectableItem.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    AccountInfo,
    SelectableItem,
  },
  data() {
    return {
      user: {
        username: "Juan",
      },
      item: {
        name: "Arduino UNO",
        url: "arduino-2168193_1280.png",
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
  /* border: 1px solid #34495E;
  background-color: #41B883; */
}
</style>
