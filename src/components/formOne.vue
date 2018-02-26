<template>
<div>
  <form-helper>
    <div slot="form-header">
      <h2>Form-One: Login here!</h2>
      <p>Please provide your login details here...</p>
    </div>

    <div slot="form-field">
      <input type="text" placeholder="Name" required>
      <input type="password" placeholder="password" required>
    </div>

    <div slot='form-controls'>
      <button v-on:click='handleSubmit'>Login</button>
    </div>
  </form-helper>
</div>
</template>

<script>
import formHelper from './formHelper';

export default {
  
  components: {
    'form-helper': formHelper,
  },
  data() {
    return {};
  },
  methods: {
    handleSubmit: function() {
      alert("thanks for submitting form one & contacting us");
    }
  }
};
</script>

<style>
body {
  margin: 0;
  font-family: "Nunito SemiBold";
}
</style>