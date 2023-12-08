<template>
  <div class="d-flex">
    <GoogleMap api-key="AIzaSyB1GhrKvPtal9CuIvyQYEC7hCeV9Vvq56E" style="margin: 10% 0 20% 0; width: 900px; height: 400px"
               :center="center" :zoom="6">
      <Marker :options="{ position: center }"/>
    </GoogleMap>
    <div style="margin: 80px 0 0 10% ">
      <h1 class="mt-5" style="color: green">Contact Us</h1>
      <a href="#" style="font-size: 20px">Link our managers</a>
      <p style="color: green;" class="mt-3">Our numbers</p>
      <div class="d-flex justify-content-between">
        <p style="color: green;">Kievstar:</p><a style="white-space: nowrap" href="#" class="ml-1">+380 98 883 46 52</a>
        <p style="color: green; margin-left: 10px;" class="ml-5">Life:</p><a style="white-space: nowrap" href="#" class="ml-1">+380 55 555 46 52</a>
      </div>
      <p style="font-size: 30px;color: green">Our address:</p>
      <p style="color: green;"><a href="#" style="font-size: 23px">Captain Canuck Bureau</a></p>

    </div>
  </div>
</template>

<script>
import {defineComponent} from "vue";
import {GoogleMap, Marker} from "vue3-google-map";
export default defineComponent({
  components: {GoogleMap, Marker},
  setup() {
    const center = {lat: 43.594342,  lng: -79.313294};

    return {center};
  },
});
</script>

<style scoped>

</style>