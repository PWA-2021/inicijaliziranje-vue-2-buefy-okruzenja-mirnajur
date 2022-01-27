<template>
  <div class="container" id="prvigrid">
    <div class="row align-items-center">
      <div class="col">
        <img src="@/assets/slika2.jpg" />
      </div>
      <div class="col" id="title">
        <h1>WELCOME TO eBEAUTY</h1>
        <p>Book your makeup appointment now!</p>
      </div>
    </div>

    <b-datepicker
      v-model="time"
      placeholder="Click to select..."
      icon="calendar-today"
      trap-focus
    >
    </b-datepicker>

    <b-field label="Select time">
      <b-timepicker v-model="time" placeholder="Click to select...">
        <b-button
          label="Now"
          type="is-primary"
          icon-left="clock"
          @click="time = new Date()"
        />
        <b-button
          label="Clear"
          type="is-danger"
          icon-left="close"
          outlined
          @click="time = null"
        />
      </b-timepicker>
    </b-field>
  </div>
</template>

<script>
export default {
  data() {
    return {
      time: new Date(),
    };
  },
};
</script>

<style scoped>
</style>
