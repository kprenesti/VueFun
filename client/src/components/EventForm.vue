<template>
  <div>
    <div class="interests">
      <label for="interests">Interests</label>
      <input
        type="text"
        v-model="interests"
        name="interests"
        id="interests"
        placeholder="Ex: JavaScript, HTML, CSS"
      >
    </div>
    <div class="zip">
      <label for="zip">Zipcode</label>
      <input type="text" name="zip" v-model="zip" id="zip" placeholder="Ex: 30062">
    </div>
    <div class="radius">
      <label for="radius">Radius (in miles)</label>
      <input type="text" v-model="radius" name="radius" id="radius" placeholder="Ex: 10">
    </div>
    <button type="submit" @click.stop.prevent="handleSubmit">Submit</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      input: {
        interests: "",
        zip: "",
        radius: ""
      }
    };
  },
  methods: {
    handleSubmit(event) {}
  }
};
</script>

<style scoped>
</style>